---
title: rxRemoteGetId function (revoAnalytics) | Microsoft Docs
description: " Provides a unique identifier for the process in the range [1:N] where N is the number of processes. "
keywords: (revoAnalytics), rxRemoteGetId, IO
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
ms.openlocfilehash: 38ed14e3b3a450a7f445cbc4617858e90ab0a56f
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxremotegetid--provides-a-unique-identifier-for-the-process"></a>rxRemoteGetId:  Provides a unique identifier for the process.  
 ## <a name="description"></a>Description

Provides a unique identifier for the process in the range [1:N] where N is the number of processes.



 ## <a name="usage"></a>Usage

```   
  rxRemoteGetId()

```

 ## <a name="details"></a>Details

This function is intended for use in calls to [rxExec](rxExec.md) to identify the process performing a given computation.  

You can also use `rxRemoteGetId` to obtain separate random number seeds.
See the examples.


 ## <a name="value"></a>Value

In a distributed compute context, this returns the parametric ID for each node or core that executes the function.
If the compute context is local, this always returns `-1`.


 ## <a name="examples"></a>Examples

 ```

  ## Not run:

rxExec(rxRemoteGetId)

# set a seed on each node before generating random numbers
myNorm <- function(x)
{
    set.seed(rxRemoteGetId())
    rnorm(x)
}
rxExec(myNorm, ARGS=as.list(1:5))
 ## End(Not run) 
```


