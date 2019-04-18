---
title: rxWriteObject function (revoAnalytics) | Microsoft Docs
description: " Store/Retrieve R objects to/from ODBC data sources. The APIs are modelled after a simple key value store. These are generic APIs and if the ODBC data source isn't specified in the argument, the function does serialization or deserialization of the R object with the specified compression if any. "
keywords: (revoAnalytics), rxWriteObject, rxReadObject, rxDeleteObject, rxListKeys
author: heidisteen
manager: cgronlun
ms.date: 01/24/2018
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ROBOTS: ''
audience: ''
ms.devlang: ''
ms.reviewer: ''
ms.suite: ''
ms.tgt_pltfrm: ''
ms.custom: ''
ms.openlocfilehash: 828a621bcf069b0e4a08e5d3a0856c77abdc4af3
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxwriteobject--manage-r-objects-in-odbc-data-sources"></a>rxWriteObject:  Manage R objects in ODBC Data Sources  
 ## <a name="description"></a>Description

Store/Retrieve R objects to/from ODBC data sources. The APIs are modelled after a simple key value store. These are generic APIs and if the ODBC data source isn't specified in the argument, the function does serialization or deserialization of the R object with the specified compression if any.


 ## <a name="usage"></a>Usage

```   
 ## S3 method for class `RxOdbcData':
rxWriteObject  (odbcDestination, key, value, version = NULL, keyName = "id", valueName = "value", versionName = "version", serialize = TRUE, overwrite = FALSE, compress = "gzip")
 ## S3 method for class `default':
rxWriteObject  (value, serialize = TRUE, compress = "gzip")
 ## S3 method for class `RxOdbcData':
rxReadObject  (odbcSource, key, version = NULL, keyName = "id", versionName = "version", valueName = "value", deserialize = TRUE, decompress = "gzip")
 ## S3 method for class `raw':
rxReadObject  (rawSource, deserialize = TRUE, decompress = "gzip")
 ## S3 method for class `RxOdbcData':
rxDeleteObject  (odbcSource, key, version = NULL, keyName = "id", valueName = "value", versionName = "version", all = FALSE)
 ## S3 method for class `RxOdbcData':
rxListKeys  (odbcSource, key = NULL, version = NULL, keyName = "id", versionName = "version")

```


 ## <a name="arguments"></a>Arguments



 ### `odbcDestination`
  an RxOdbcData object identifying the destination to which the data is to be written.  


 ### `odbcSource`
  an RxOdbcData object identifying the source from which the data is to be read.  

  ..  
 ### `rawSource`
  a raw R object to be read from.  


 ### `key`
 a character string identifying the R object to be written or read. The intended use is  for the key+version to be unique.  


 ### `value`
 the R object being stored into the data source.  


 ### `version`
 `NULL` or a character string which carries the version of the object.  Combined with key identifies the object.  


 ### `keyName`
 character string specifying the column name for the key in the underlying table.   


 ### `valueName`
 character string specifying the column name for the objects in the underlying table.  


 ### `versionName`
 character string specifying the column name for the version in the underlying table.  



 ### `serialize`
 logical value. Dictates whether the object is to be serialized. Only raw values are supported if serialization is off.  



 ### `compress`
 character string defining the compression algorithm to use for memCompress.  



 ### `deserialize`
 logical value. Defines whether the object is to be de-serialized.  



 ### `decompress`
 character string defining the compression algorithm to use for memDecompress.  



 ### `overwrite`
 logical value. If `TRUE`, `rxWriteObject` first removes the key (or the key+version combination) before writing the new value. Even when `overwrite` is `FALSE`, `rxWriteObject` may still succeed if there is no database constraint (or index) enforcing uniqueness.  



 ### `all`
 logical value. `TRUE` to remove all objects from the data source. If `TRUE`, the 'key' parameter is ignored.  



 ## <a name="details"></a>Details

`rxWriteObject` stores an R object into the specified ODBC data destination.
The R object to be written is identified by a key, and optionally, by a version (key+version). By default, the object is serialized and compressed. Returns `TRUE` if successful.
If the ODBC data destination is not specified, the default implementation is dispatched which takes only the value of the R object with serialize and compress arguments.

`rxReadObject` loads an R object from the ODBC data source (or from a raw) decompressing and unserializing it (by default) in the process. Returns the R object. If the data source parameter defines a query, the `key` and the `version` parameters are ignored.

`rxDeleteObject` deletes an R object from the ODBC data source. If there are multiple objects identified by the key/version combination, all are deleted.

`rxListKeys` enumerates all keys or versions for a given key, depending on the parameters. When `key` is `NULL`, the function enumerates all unique keys in the table. Otherwise, it enumerates all versions for the given key.
Returns a single column data frame.

The `key` and the `version` column should be of some SQL character type (`CHAR`, `VARCHAR`, `NVARCHAR`, etc) supported by the data source.
The `value` column should be a binary type (`VARBINARY` for instance). Some conversions to other types might work, however, they are dependant on the ODBC driver and on the underlying package functions.


 ## <a name="value"></a>Value

`rxReadObject` returns an R object.
`rxWriteObject` and `rxDeleteObject` return logical, `TRUE` on success.
`rxListKeys` returns a single column data frame containing strings.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)




 ## <a name="see-also"></a>See Also


 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# Setup the connection string
conStr <- 'Driver={SQL Server};Server=localhost;Database=storedb;Trusted_Connection=true'

# Create the data source
ds <- RxOdbcData(table="robjects", connectionString=conStr)

# Re-create the table
if(rxSqlServerTableExists(ds@table, ds@connectionString)) {
  rxSqlServerDropTable(ds@table, ds@connectionString)
}

# An example table definition for SQL Server (no version)
ddl <- paste(" create table [", ds@table, "] (",
             "     [id] varchar(200) not null, ",
             "     [value] varbinary(max), ",
             "     constraint unique_id unique (id))",
             sep = "")
rxOpen(ds, "w")
rxExecuteSQLDDL(ds, ddl)
rxClose(ds)

# Fit a logit model
infertLogit <- rxLogit(case ~ age + parity + education + spontaneous + induced,
                       data = infert)

# Store the model in the database
rxWriteObject(ds, "logit.model", infertLogit)

# Load the model
infertLogit2 <- rxReadObject(ds, "logit.model")

all.equal(infertLogit, infertLogit2)
# TRUE

 ## End(Not run) 
```

