---
title: 'rx_get_pyspark_connection: Get pyspark spark_context connection from Spark compute context (revoscalepy)'
description: Gets a PySpark connection from the current Spark compute context.
keywords: ''
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
ms.openlocfilehash: b55d132805080ac8cd22a499a9e18ebc2a2e5f9e
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="rxgetpysparkconnection"></a>rx_get_pyspark_connection


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_get_pyspark_connection(compute_context: revoscalepy.computecontext.RxSpark.RxSpark)
```





## <a name="description"></a>Description

Gets a PySpark connection from the current Spark compute context.


## <a name="arguments"></a>Arguments


### <a name="computecontext"></a>compute_context

Compute context get created by rx_spark_connect.


## <a name="returns"></a>Returns

Object of python.context.SparkContext.


## <a name="example"></a>Example



```
from revoscalepy import rx_spark_connect, rx_get_pyspark_connection
from pyspark.sql import SparkSession
cc = rx_spark_connect(interop = "pyspark")
sc = rx_get_pyspark_connection(cc)
spark = SparkSession(sc)
df = spark.createDataFrame([('Monday',3012),('Friday',1354),('Sunday',5452)], ["DayOfWeek", "Sale"])
```

