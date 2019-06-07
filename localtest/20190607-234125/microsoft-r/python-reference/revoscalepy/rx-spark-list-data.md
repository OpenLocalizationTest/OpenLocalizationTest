---
title: 'rx_spark_list_data: Functions for object management in Spark (revoscalepy)'
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
ms.openlocfilehash: 614155f57dc204386dfa1e371b2fa83f01665dff
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxsparklistdata"></a>rx_spark_list_data


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_spark_list_data(show_description: bool,
    compute_context: revoscalepy.computecontext.RxComputeContext.RxComputeContext = None)
```





## <a name="description"></a>Description

Use these functions to manage the objects cached in the Spark memory system. These functions are only applicable when using RxSpark compute context.


## <a name="arguments"></a>Arguments


### <a name="showdescription"></a>show_description

Bool value, indicating whether or not to print out the detail to console.


### <a name="computecontext"></a>compute_context

RxSpark compute context object.


## <a name="returns"></a>Returns

List of all objects cached in Spark memory system for rxSparkListData.


## <a name="example"></a>Example



```
from revoscalepy import RxOrcData, rx_spark_connect, rx_spark_list_data, rx_lin_mod, rx_spark_cache_data
rx_spark_connect()
col_info = {"DayOfWeek": {"type": "factor"}}
df = RxOrcData(file = "/share/sample_data/AirlineDemoSmallOrc", column_info = col_info)
df = rx_spark_cache_data(df, True)

# After the first run, a Spark data object is added into the list
rx_lin_mod("ArrDelay ~ DayOfWeek", data = df)
rx_spark_list_data(True)
```

