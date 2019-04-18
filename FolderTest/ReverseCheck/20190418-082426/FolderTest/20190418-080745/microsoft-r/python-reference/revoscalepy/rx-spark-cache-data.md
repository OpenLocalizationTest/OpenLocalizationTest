---
title: 'rx_spark_cache_data: Set the Cache Flag in Spark compute context (revoscalepy)'
description: Use this function to set the cache flag to control whether data objects should be cached in Spark  memory system, applicable for RxXdfData, RxHiveData, RxParquetData, RxOrcData and RxSparkDataFrame.
keywords: spark, data, cache
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
ms.openlocfilehash: 816b8b960d55858cf2ecc5395eca8adefb8e520c
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="rxsparkcachedata"></a>rx_spark_cache_data


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_spark_cache_data(in_data: revoscalepy.datasource.RxDataSource.RxDataSource,
    cache: bool)
```





## <a name="description"></a>Description

Use this function to set the cache flag to control whether data objects should be cached in Spark memory system, applicable for RxXdfData, RxHiveData, RxParquetData, RxOrcData and RxSparkDataFrame.


## <a name="arguments"></a>Arguments


### <a name="indata"></a>in_data

A data source that can be RxXdfData, RxHiveData, RxParquetData, RxOrcData or RxSparkDataFrame.
RxTextData is currently not supported.


### <a name="cache"></a>cache

Bool value controlling whether the data should be cached or not. If TRUE the data will be cached in the Spark memory system after the first use for performance enhancement.


## <a name="returns"></a>Returns

Data object with new cache flag.


## <a name="example"></a>Example



```
from revoscalepy import RxHiveData, rx_spark_connect, rx_spark_cache_data
hive_data = RxHiveData(table = "mytable")

# The cache flag of hiveData is now set to TRUE.
hive_data = rx_spark_cache_data(hive_data, True)

# set cache value to False
hive_data = rx_spark_cache_data(hive_data, False)
```

