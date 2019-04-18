---
title: 'rx_read_object: Read an ODBC data source object (revoscalepy)'
description: Retrieves an ODBC data source object by its key value.
keywords: odbc
author: HeidiSteen
manager: cgronlun
ms.date: 01/26/2018
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ROBOTS: ''
audience: ''
ms.devlang: Python
ms.reviewer: ''
ms.suite: ''
ms.tgt_pltfrm: ''
ms.custom: ''
ms.openlocfilehash: ae43733d12cd15777eefb29f16bcd6e1280a218d
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="rxreadobject"></a>rx_read_object


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_read_object(src: revoscalepy.datasource.RxOdbcData.RxOdbcData,
    key: str = None, version: str = None,
    key_name: str = 'id', value_name: str = 'value',
    version_name: str = 'version', deserialize: bool = True,
    decompress: str = 'zip')
```





## <a name="description"></a>Description

Retrieves an ODBC data source object by its key value.


## <a name="details"></a>Details

Loads an object from the ODBC data source, decompressing and unserializing it (by default) in the process.
Returns the object. If the data source parameter defines a query, the key and the version parameters are ignored.

The key and the version should be of some SQL character type (CHAR, VARCHAR, NVARCHAR, etc.) supported by the data source. The value column should be a binary type (VARBINARY for instance). Some conversions to other types might work, however, they are dependent on the ODBC driver and on the underlying package functions.


## <a name="arguments"></a>Arguments


### <a name="src"></a>src

The object being stored into the data source.


### <a name="key"></a>key

A character string identifying the object. The intended use is for the key+version to be unique.


### <a name="version"></a>version

None or a character string which carries the version of the object. Combined with key identifies the object.


### <a name="keyname"></a>key_name

Character string specifying the column name for the key in the underlying table.


### <a name="valuename"></a>value_name

Character string specifying the column name for the objects in the underlying table.


### <a name="versionname"></a>version_name

Character string specifying the column name for the version in the underlying table.


### <a name="serialize"></a>serialize

Bool value. Dictates whether the object is to be serialized. Only raw values are supported if serialization is off.


### <a name="deserialize"></a>deserialize

logical value. Defines whether the object is to be de-serialized.


### <a name="decompress"></a>decompress

Character string defining the compression algorithm to use for memDecompress.


## <a name="returns"></a>Returns

rx_read_object returns an object. rx_write_object and rx_delete_object return bool, True on success. rx_list_keys returns a single column data frame containing strings.


## <a name="example"></a>Example



```
from pandas import DataFrame
from numpy import random
from revoscalepy import RxOdbcData, rx_write_object, rx_read_object, rx_list_keys, rx_delete_object

connection_string = 'Driver=SQL Server;Server=.;Database=RevoTestDb;Trusted_Connection=True;'
dest = RxOdbcData(connection_string, table = "dataframe")

df = DataFrame(random.randn(10, 5))

status = rx_write_object(dest, key = "myDf", value = df)

read_obj = rx_read_object(dest, key = "myDf")

keys = rx_list_keys(dest)

rx_delete_object(dest, key = "myDf")
```

