---
title: 'rx_write_object: Writes to an ODBC data source object (revoscalepy)'
description: Stores objects in an ODBC data source. The APIs are modelled after a simple key value store.
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
ms.openlocfilehash: df51619dfa9aa3ce4bab72be263a3a070276574e
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxwriteobject"></a>rx_write_object


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_write_object(dest: revoscalepy.datasource.RxOdbcData.RxOdbcData,
    key: str = None, value=None, version: str = None,
    key_name: str = 'id', value_name: str = 'value',
    version_name: str = 'version', serialize: bool = True,
    overwrite: bool = False, compress: str = 'zip')
```





## <a name="description"></a>Description

Stores objects in an ODBC data source. The APIs are modeled after a simple key value store.


## <a name="details"></a>Details

Stores an object into the ODBC data source. The object is identified by a key, and optionally, by a version (key+version). By default, the object is serialized and compressed. Returns True if successful.

The key and the version should be of some SQL character type (CHAR, VARCHAR, NVARCHAR, etc.) supported by the data source. The value column should be a binary type (VARBINARY for instance). Some conversions to other types might work, however, they are dependent on the ODBC driver and on the underlying package functions.


## <a name="arguments"></a>Arguments


### <a name="key"></a>key

A character string identifying the object. The intended use is for the key+version to be unique.


### <a name="value"></a>value

A python object serializable by dill.


### <a name="dest"></a>dest

The object being stored into the data source.


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


### <a name="compress"></a>compress

Character string defining the compression algorithm to use for memCompress.


### <a name="deserialize"></a>deserialize

Bool value. Defines whether the object is to be de-serialized.


### <a name="overwrite"></a>overwrite

Bool value. If True, rx_write_object first removes the key (or the key+version combination) before writing the new value. Even when overwrite is False, rx_write_object may still succeed if there is no database constraint (or index) enforcing uniqueness.


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

