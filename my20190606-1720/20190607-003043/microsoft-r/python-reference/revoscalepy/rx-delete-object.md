---
title: 'rx_delete_object: Manage objects in ODBC data sources (revoscalepy)'
description: Deletes an object from an ODBC data source. The APIs are modelled after a simple key value store.
keywords: delete, object
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
ms.openlocfilehash: 882ee420c86dc5fc3812ba52faad1f946b9b22ba
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxdeleteobject"></a>rx_delete_object


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_delete_object(src: revoscalepy.datasource.RxOdbcData.RxOdbcData,
    key: str = None, version: str = None,
    key_name: str = 'id', version_name: str = 'version',
    all: bool = False)
```





## <a name="description"></a>Description

Deletes an object from an ODBC data source. The APIs are modeled after a simple key value store.


## <a name="details"></a>Details

Deletes an object from the ODBC data source. If there are multiple objects identified by the key/version combination, all are deleted.

The key and the version column should be of some SQL character type (CHAR, VARCHAR, NVARCHAR, etc.) supported by the data source. The value column should be a binary type (VARBINARY for instance). Some conversions to other types might work, however, they are dependent on the ODBC driver and on the underlying package functions.


## <a name="arguments"></a>Arguments


### <a name="src"></a>src

The object being stored into the data source.


### <a name="key"></a>key

A character string identifying the object. The intended use is for the key+version to be unique.


### <a name="version"></a>version

None or a character string which carries the version of the object. Combined with key identifies the object.


### <a name="keyname"></a>key_name

Character string specifying the column name for the key in the underlying table.


### <a name="versionname"></a>version_name

Character string specifying the column name for the version in the underlying table.


### <a name="all"></a>all

Bool value. *True* to remove all objects from the data source.
If *True*, the ‘key’ parameter is ignored.


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

