---
title: 'rx_spark_disconnect: Disconnect from remote Spark applications (revoscalepy)'
description: Shuts down the remote Spark application and switches to a local compute context. All rx* function calls after this will run in a local compute context. In pyspark-interop mode, if Spark application is started by pyspark APIs, rx_spark_disconnect will not shut down the remote Spark application but disassociate from it. Run ‘help(revoscalepy.rx_spark_connect)’ for more information about interop.
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
ms.openlocfilehash: e0b95ca3f8c731deceeb970df66aa01b2e8801c8
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="rxsparkdisconnect"></a>rx_spark_disconnect


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_spark_disconnect(compute_context=None)
```





## <a name="description"></a>Description

Shuts down the remote Spark application and switches to a local compute context.
All rx* function calls after this will run in a local compute context.
In pyspark-interop mode, if Spark application is started by pyspark APIs, rx_spark_disconnect will not shut down the remote Spark application but disassociate from it.
Run ‘help(revoscalepy.rx_spark_connect)’ for more information about interop.


## <a name="arguments"></a>Arguments


### <a name="computecontext"></a>compute_context

Spark compute context to be terminated by rx_spark_disconnect.
If input is None, then current compute context will be used.


## <a name="example"></a>Example



```
from revoscalepy import rx_spark_connect, rx_spark_disconnect
cc = rx_spark_connect()
rx_spark_disconnect(cc)
```

