---
title: rxCleanupJobs function (revoAnalytics) | Microsoft Docs
description: " Removes artifacts created while executing a distributed computing job. "
keywords: (revoAnalytics), rxCleanupJobs, IO
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
ms.openlocfilehash: 4a2d49e67ca36b40562d8233b0fbc88205af8785
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxcleanupjobs--cleanup-of-a-distributed-computing-job-or-jobs"></a>rxCleanupJobs:  Cleanup of a Distributed Computing Job or Jobs.  
 ## <a name="description"></a>Description

Removes artifacts created while executing a distributed computing job.



 ## <a name="usage"></a>Usage

```   
  rxCleanupJobs(jobInfoList, force = FALSE, verbose = TRUE)

```


 ## <a name="arguments"></a>Arguments



 ### `jobInfoList`
 `rxJobInfo` object or a list of job objects that can be obtained  from [rxGetJobs](rxGetJobs.md). 



 ### `force`
 logical scalar. If `TRUE`, forces removal of job directories even if  there are retrievable results or if the current job state is undetermined. 



 ### `verbose`
 logical scalar.  If `TRUE`, will print the directories/records being deleted. 




 ## <a name="details"></a>Details

If `jobInfoList` is a `jobInfo` object, `rxCleanupJobs` attempts to remove the artifacts.
However, if the job has successfully completed and `force=FALSE`, `rxCleanupJobs` issues a warning saying to either set `force=TRUE` or use [rxGetJobResults](rxGetJobResults.md) to get the results and delete the artifacts.  

If `jobInfoList` is a list of jobs, `rxCleanupJobs` attempts to apply the cleanup rules for a single job to each element in the list.



 ## <a name="value"></a>Value

This function is called for its side effects (removing job artifacts); it does not have a useful return value.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxGetJobs](rxGetJobs.md), [rxGetJobOutput](rxGetJobOutput.md), [RxSpark](RxSpark.md), [RxHadoopMR](RevoScaleR-deprecated.md), [rxGetJobResults](rxGetJobResults.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

rxCleanupJobs(jobInfoList = myJobs, force = TRUE)

rxCleanupJobs(rxGetJobs(rxGetOption("computeContext")))
 ## End(Not run) 
```


