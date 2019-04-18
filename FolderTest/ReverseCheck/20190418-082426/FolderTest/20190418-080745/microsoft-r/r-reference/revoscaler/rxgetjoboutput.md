---
title: rxGetJobOutput function (revoAnalytics) | Microsoft Docs
description: " Gets the console output from the various nodes in a non-waiting distributed computing job. "
keywords: (revoAnalytics), rxGetJobOutput, IO
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
ms.openlocfilehash: 000fb50094dd51095ca408c50effc35391999168
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxgetjoboutput--get-console-output-from-distributed-computing-job"></a>rxGetJobOutput:  Get Console Output from Distributed Computing Job  
 ## <a name="description"></a>Description

Gets the console output from the various nodes in a non-waiting distributed computing job.



 ## <a name="usage"></a>Usage

```   
  rxGetJobOutput(jobInfo)

```


 ## <a name="arguments"></a>Arguments



 ### `jobInfo`
 a job information object, such as that returned from a non-waiting,  distributed computation, for example, the `rxgLastPendingJob` object, if available. 




 ## <a name="details"></a>Details

During a job run, the state of the output is non-deterministic (that is, it may or may not be on disk, and what is on disk at any given point in time may not reflect the actual completion state of a job).

If `autoCleanup` has been set to `TRUE`, the console output will not persist after the job completes.

Unlike [rxGetJobResults](rxGetJobResults.md), this function does not remove any job information upon retrieval.


 ## <a name="value"></a>Value

This function is called for its side effect of printing console output; it does not have a useful return value.

 ## <a name="see-also"></a>See Also

[RxSpark](RxSpark.md), RxHadoopMR, [RxInSqlServer](RxInSqlServer.md), [rxGetJobs](rxGetJobs.md), [rxCleanupJobs](rxCleanup.md), [rxGetJobResults](rxGetJobResults.md), [rxExec](rxExec.md).

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# set up a non-waiting HPC Server compute context: 
myCluster <- RxSpark(nameNode = "my-name-service-server", port = 8020, wait = FALSE) 
rxOptions(computeContext=myCluster) 

myJob <- rxExec(function(){ print( "Hello World"); return ( 1 ) })
# The job output will contain the printed text "Hello World" from each node
rxGetJobOutput(myJob)
# The results object will be a list containing the value 1 for each node
rxGetJobResults(myJob)
# Get job results will remove the job object (by default)
# Another call to rxGetJobOutput(myJob) would return no output

 ## End(Not run) 
```


