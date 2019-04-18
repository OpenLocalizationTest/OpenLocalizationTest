---
title: 'rx_spark_remove_data: Manage cached data in Spark (revoscalepy)'
description: Use these functions to manage the objects cached in the Spark memory system. These functions are only applicable  when using RxSpark compute context.
keywords: spark, data
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
ms.openlocfilehash: efbcec574929e10a3a27b8c5e94f15f6c3b1fdb9
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="rxsparkremovedata"></a>rx_spark_remove_data


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_spark_remove_data(remove_list,
    compute_context: revoscalepy.computecontext.RxComputeContext.RxComputeContext = None)
```





## <a name="description"></a>Description

Use these functions to manage the objects cached in the Spark memory system. These functions are only applicable when using RxSpark compute context.


## <a name="arguments"></a>Arguments


### <a name="removelist"></a>remove_list

Cached object or a list of cached objects need to be deleted.


### <a name="computecontext"></a>compute_context

RxSpark compute context object.


## <a name="returns"></a>Returns

No return objs for rxSparkRemoveData.


## <a name="example"></a>Example



```
from revoscalepy import RxOrcData, rx_spark_connect, rx_spark_disconnect, rx_spark_list_data, rx_spark_cache_data, rx_spark_remove_data, rx_lin_mod
cc=rx_spark_connect()
col_info = {"DayOfWeek": {"type": "factor"}}

df = RxOrcData(file = "/share/sample_data/AirlineDemoSmallOrc", column_info = col_info)
df = rx_spark_cache_data(df, True)

# After the first run, a Spark data object is added into the list
rx_lin_mod("ArrDelay ~ DayOfWeek", data = df)

rx_spark_remove_data(df)
rx_spark_list_data(True)
rx_spark_disconnect(cc)
```

