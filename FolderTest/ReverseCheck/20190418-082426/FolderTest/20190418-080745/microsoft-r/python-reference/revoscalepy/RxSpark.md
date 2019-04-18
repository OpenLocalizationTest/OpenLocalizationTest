---
title: 'RxSpark: Generate spark compute context (revoscalepy)'
description: Creates the compute context for running revoscalepy analysis on Spark. Note that the use of rx_spark_connect() is recommended over RxSpark() as rx_spark_connect() supports persistent mode with in-memory caching. Run help(revoscalepy.rx_spark_connect) for more information.
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
ms.openlocfilehash: 209ec4c94535c19e27710406328225fd27f54490
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="rxspark"></a>RxSpark


 



```
revoscalepy.RxSpark(hdfs_share_dir: str = '/user/RevoShare\766RR78ROCWFDMK$',
    share_dir: str = '/var/RevoShare\766RR78ROCWFDMK$',
    user: str = '766RR78ROCWFDMK$', name_node: str = None,
    master: str = 'yarn', port: int = None,
    auto_cleanup: bool = True, console_output: bool = False,
    packages_to_load: list = None, idle_timeout: int = 3600,
    num_executors: int = None, executor_cores: int = None,
    executor_mem: str = None, driver_mem: str = None,
    executor_overhead_mem: str = None, extra_spark_config: str = '',
    spark_reduce_method: str = 'auto', tmp_fs_work_dir: str = None,
    persistent_run: bool = False, wait: bool = True, **kwargs)
```





## <a name="description"></a>Description

Creates the compute context for running revoscalepy analysis on Spark.
Note that the use of rx_spark_connect() is recommended over RxSpark() as rx_spark_connect() supports persistent mode with in-memory caching.
Run *help(revoscalepy.rx_spark_connect)* for more information.
