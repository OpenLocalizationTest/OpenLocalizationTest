---
title: rxStopEngine function (revoAnalytics) | Microsoft Docs
description: " rxStopEngine stops the remote Spark application. "
keywords: (revoAnalytics), rxStopEngine, rxStopEngine,RxSpark-method, rxStopEngine,RxDistributedHpa-method, rxStopEngine,RxHadoopMR-method, rxStopEngine,RxInSqlServer-method, rxStopEngine,RxLsfCluster-method, computecontext
author: heidisteen
manager: cgronlun
ms.date: 01/24/2018
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ROBOTS: ''
audience: ''
ms.devlang: ''
ms.reviewer: ''
ms.suite: ''
ms.tgt_pltfrm: ''
ms.custom: ''
ms.openlocfilehash: 5f12c5ee22ca8a5334627ec45257ef50c9b47553
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxstopengine-stop-distributed-computing-engine"></a>rxStopEngine: Stop Distributed Computing Engine 
 ## <a name="description"></a>Description

`rxStopEngine` stops the remote Spark application.


 ## <a name="usage"></a>Usage

```   
  rxStopEngine(computeContext,   ...  )
  rxStopEngine(computeContext, scope = "session")

```

 ## <a name="arguments"></a>Arguments



 ### `computeContext`
 a valid [RxDistributedHpa-class](RxDistributedHpa-class.md). Currently only [RxSpark](RxSpark.md) is supported.  



 ### `scope`
 only used in `rxStopEngine` for `RxSpark`; a single `character` that takes the value of either:  
*   `"session"`: stop engine applications running in the current R session. 
*   `"user"`: stop engine applications running by the current user. 





 ## <a name="details"></a>Details

This function stops distributed computing engine applications with scope set to either "session" or "user". Specifically, for the [RxSpark](RxSpark.md) compute context it stops the remote Spark application(s).


 ## <a name="value"></a>Value

No useful return value.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[RxSpark](RxSpark.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

rxStopEngine( computeContext )
rxStopEngine( computeContext , scope = "user" )
 ## End(Not run) 
```


