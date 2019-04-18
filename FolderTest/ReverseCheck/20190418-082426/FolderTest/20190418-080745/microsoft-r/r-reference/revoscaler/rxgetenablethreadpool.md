---
title: rxGetEnableThreadPool function (revoAnalytics) | Microsoft Docs
description: " Gets or sets the current state of the thread pool (in a ready state or created ad hoc). "
keywords: (revoAnalytics), rxGetEnableThreadPool, rxSetEnableThreadPool, iteration
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
ms.openlocfilehash: ee6c0d1f9869a8242ad6c953ae03a4ca97d188f8
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxgetenablethreadpool--get-or-set-thread-pool-state"></a>rxGetEnableThreadPool:  Get or Set Thread Pool State  
 ## <a name="description"></a>Description

Gets or sets the current state of the thread pool (in a ready state or created ad hoc).



 ## <a name="usage"></a>Usage

```   
  rxGetEnableThreadPool()
  rxSetEnableThreadPool( enable )

```

 ## <a name="arguments"></a>Arguments



 ### `enable`
  Logical scalar. If `TRUE`, the thread pool is instantiated and maintained in a ready state. If `FALSE`, threads are created in an ad hoc fashion; that is, they are created as needed.  



 ## <a name="details"></a>Details

The `rxSetEnableThreadPool` function is used on Linux to turn the thread pool on and off.  When the thread pool is on, it means that there exists a pool of threads that persist between calls, and are ready for processing.  
When the thread pool is off, it means that threads will be created on an ad hoc basis when calls requiring threading are made. By default, the thread pool is turned off to allow R processes that have loaded RevoScaleR to fork successfully as a mechanism for spawning (for example, by the `multicore` package).

On the Windows platform, the thread pool always persists, regardless of any user settings. 

There is a significant speed increase associated with having the thread pool ready and waiting to do work.  If you are sure that you will not be using any spawning mechanism that uses fork, you may want to put the following at the end of your Rprofile.site.  Make absolutely sure that it is after any lines that are used to load RevoScaleR:

` invisible( rxSetEnableThreadPool( TRUE ) ) `

The following are possible cases where fork may be called.  Obviously, this is not an all-inclusive list:



* 
  `nohup` to launch jobs.  This will cause a fork to be called.

* 
  Using `multicore` and/or `doMC` to launch R processes with RevoScaleR



Note that when using [rxExec](rxExec.md), the default behavior for any worker node process on a Linux host will be to have the thread pool off (set to create threads in an ad hoc manner).  If the function passed to [rxExec](rxExec.md) is going to make multiple calls into RevoScaleR functions, you will probably want to include a call to `rxSetEnableThreadPool(TRUE)` as the first line of the function that you pass to [rxExec](rxExec.md).

For distributed HPA functions run on worker nodes, threading is always automatically handled for the user.

The `rxGetEnableThreadPool` function can be used to determine whether the thread pool is instantiated or not.  Note that on Windows, it will always be instantiated; on Linux, whether it is always instantiated or created on an ad hoc basis is controlled by `rxSetEnableThreadPool`.  At startup on Linux, the thread pool state wil be off; that is, threads will be created on an ad hoc basis.


 ## <a name="value"></a>Value

`rxSetEnableThreadPool` returns the state of the thread pool prior to making the call (as opposed to the updated state).  Thus, this function returns `TRUE` if the thread pool was instantiated and in a ready state prior to making the call, or `FALSE` if the thread pool was set to be created in an ad hoc fashion. 

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxOptions](rxOptions.md)


 ## <a name="examples"></a>Examples

 ```

  ## Not run:

rxGetEnableThreadPool()
rxSetEnableThreadPool(TRUE)
rxGetEnableThreadPool()
  ## End(Not run) 
```


