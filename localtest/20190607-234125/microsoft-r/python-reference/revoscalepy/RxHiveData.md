---
title: 'RxHiveData: Class generator for Hive data source objects (revoscalepy)'
description: Main generator for class RxHiveData, which extends RxSparkData.
keywords: datasource, hive
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
ms.openlocfilehash: 614e454a484c8de90d93e009d4e7ded82fa9900a
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxhivedata"></a>RxHiveData


 



```
revoscalepy.RxHiveData(query=None, table=None, save_as_temp_table=False,
    write_factors_as_indexes: bool = False, column_info=None)
```





## <a name="description"></a>Description

Main generator for class RxHiveData, which extends RxSparkData.


## <a name="arguments"></a>Arguments


### <a name="query"></a>query

Character string specifying a Hive query, e.g. “select * from >>sample_<< table”. Cannot be used with ‘table’.


### <a name="table"></a>table

Character string specifying the name of a Hive table, e.g. “sample_table”.
Cannot be used with ‘query’.


### <a name="columninfo"></a>column_info

List of named variable information lists. Each variable information list contains one or more of the named elements given below.
Currently available properties for a column information list are: type: Character string specifying the data type for the column.

    Supported types are:
        ”bool” (stored as uchar),
        “integer” (stored as int32),
        “int16” (alternative to integer for smaller storage space),
        “float32” (stored as FloatType),
        “numeric” (stored as float64),
        “character” (stored as string),
        “factor” (stored as uint32),
        “Date” (stored as Date, i.e. float64.)
        “POSIXct” (stored as POSIXct, i.e. float64.)

levels: List of strings containing the levels when type = “factor”. If the levels property is not provided, factor levels will be determined by the values in the source column. If levels are provided, any value that does not match a provided level will be converted to a missing value.


### <a name="saveastemptable"></a>save_as_temp_table

Bool value, only applicable when using as output with “table” parameter.
If “TRUE” register a temporary Hive table in Spark memory system otherwise generate a persistent Hive table. The temporary Hive table is always cached in Spark memory system.


### <a name="writefactorsasindexes"></a>write_factors_as_indexes

Bool value, If True, when writing to an RxHiveData data source, underlying factor indexes will be written instead of the string representations.


## <a name="returns"></a>Returns

object of class `RxHiveData`.


## <a name="example"></a>Example



```
import os
from revoscalepy import rx_data_step, RxOptions, RxHiveData
sample_data_path = RxOptions.get_option("sampleDataDir")
colInfo = {"DayOfWeek": {"type":"factor"}}
ds1 = RxHiveData(table = "AirlineDemo")
result = rx_data_step(ds1)
ds2 = RxHiveData(query = "select * from hivesampletable")
result = rx_data_step(ds2)
```

