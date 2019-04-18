---
title: rxTeradataSql function (revoAnalytics) | Microsoft Docs
description: " Execute an arbitrary SQL statement that does not return data in a Teradata data base. "
keywords: (revoAnalytics), rxTeradataSql, rxTeradataTableExists, rxTeradataDropTable, file
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
ms.openlocfilehash: e2af4f974b2eb183373dd7809a2df04ac327d67e
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxteradatasql--rxteradatasql"></a>rxTeradataSql:  rxTeradataSql  
 ## <a name="description"></a>Description

Execute an arbitrary SQL statement that does not return data in a Teradata data base.


 ## <a name="usage"></a>Usage

```   
  rxTeradataSql(sqlStatement, connectionString = NULL, ...)
  rxTeradataTableExists(table, connectionString = NULL, ...)
  rxTeradataDropTable(table, connectionString = NULL, ...)

```


 ## <a name="arguments"></a>Arguments



 ### `sqlStatement`
  character string specifying valid SQL statement that does not return data  


 ### `table`
  One of the following:  
*   a character string specifying a table name, in the form `"tablename"` or`"database.tablename"`. (In Teradata, each user is a database; the user database can be specified as `"username.tablename"`.) 
*   an [RxTeradata](RxTeradata.md) data source that has the `table` specified 
*   an [RxOdbcData](RxOdbcData.md) data source that has the `table` specified. 




 ### `connectionString`
 `NULL` or character string specifying the connection string.  If `NULL`, the connection string from the currently  active compute context will be used if available.  



 ### ` ...`
  Additional arguments to be passed through.   




 ## <a name="details"></a>Details

An SQL query is passed to the Teradata ODBC driver.


 ## <a name="value"></a>Value

`rxTeradataSql` is executed for the side effects and returns `NULL` invisibly.
`rxTeradataTableExists` returns `TRUE` is the table exists, `FALSE` otherwise. The database searched for the table is determined as follows:


* 
 If the `table` argument is a character string and specifies a database, that is, if the `table` argument is specified as `"database.tablename"`, the specified database is searched for the table. If the containing database does not exist, an error is returned.

* 
 If the `table` argument is a character string and does not specify a database, that is, if the `table` argument is specified as `"tablename"`,the database specified in the `connectionString` is searched. If `connectionString` is missing, the connection string in the current compute context object is used. 

* 
 If the `table` argument is an [RxTeradata](RxTeradata.md) or [RxOdbcData](RxOdbcData.md) data source, the table name specified in the data source is searched for in the database specified in the data source.



`rxTeradataDropTable` returns `TRUE` is the table is successfully dropped, `FALSE` otherwise (for example, if the table did not exist).


 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)





 ## <a name="see-also"></a>See Also

[RxTeradata](RxTeradata.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# Copy a table
sqlStatement <- "CREATE TABLE YourDataBase.rxClaimsCopy AS YourDataBase.claims WITH DATA"
rxTeradataSql(sqlStatement = sqlStatement)

# Use the RxOdbcData data source and its sqlQuery argument to 
# get data back as a data frame:
rxTeradataQuery <- function(query, connectionString=NULL, maxRowsByCols=NULL)
{
    if (is.null(connectionString))
    {
        currentComputeContext <- rxGetComputeContext()
        if (.hasSlot(currentComputeContext, "connectionString"))
        {
            connectionString <- currentComputeContext@connectionString
        }
        else
        {
            stop("A 'connectionString' must be specified.")
        }
    }   
    internalDS <- RxOdbcData(sqlQuery=query, connectionString=connectionString)
    rxImport(internalDS, maxRowsByCols=maxRowsByCols)   
}
## Use the above to show the tables in database 'dbtest':
tableQuery <- paste("SELECT TableName FROM dbc.tables ",
                    "WHERE tablekind = 'T' and databasename='dbtest'", sep="")
rxTeradataQuery(query=tableQuery)
 ## End(Not run) 
```




