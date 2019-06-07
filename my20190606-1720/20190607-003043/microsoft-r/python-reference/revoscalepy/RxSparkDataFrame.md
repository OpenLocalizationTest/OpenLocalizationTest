---
title: 'RxSparkDataFrame: Class generator for Spark data frame objects (revoscalepy)'
description: Main generator for class RxSparkDataFrame, which extends RxSparkData.
keywords: datasource
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
ms.openlocfilehash: f327efc4843a26d58532e8a7596da4081d806cbd
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxsparkdataframe"></a>RxSparkDataFrame


 



```
revoscalepy.RxSparkDataFrame(data=None, column_info=None,
    write_factors_as_indexes: bool = False)
```





## <a name="description"></a>Description

Main generator for class RxSparkDataFrame, which extends RxSparkData.


## <a name="arguments"></a>Arguments


### <a name="data"></a>data

Spark data frame obj from pyspark.sql.DataFrame.


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


### <a name="writefactorsasindexes"></a>write_factors_as_indexes

Bool value, if True, when writing to an RxSparkDataFrame data source, underlying factor indexes will be written instead of the string representations.


## <a name="returns"></a>Returns

Object of class `RxSparkDataFrame`.


## <a name="example"></a>Example



```
import os
from revoscalepy import rx_data_step, RxSparkDataFrame
from pyspark.sql import SparkSession
spark = SparkSession.builder.getOrCreate()
df = spark.createDataFrame([('Monday',3012),('Friday',1354),('Sunday',5452)], ["DayOfWeek", "Sale"])
col_info = {"DayOfWeek": {"type":"factor"}}
ds = RxSparkDataFrame(df, column_info=col_info)
out_ds = RxSparkDataFrame(write_factors_as_indexes=True)
rx_data_step(ds, out_ds)
out_df = out_ds.spark_data_frame
out_df.take(2)
# [Row(DayOfWeek=0, Sale=3012), Row(DayOfWeek=2, Sale=1354)]
```

