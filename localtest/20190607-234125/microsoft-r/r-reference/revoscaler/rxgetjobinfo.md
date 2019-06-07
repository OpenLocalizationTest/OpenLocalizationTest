---
title: rxGetJobInfo function (revoAnalytics) | Microsoft Docs
description: " Gets job information for a given distributed computing job. "
keywords: (revoAnalytics), rxGetJobInfo, IO
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
ms.openlocfilehash: e7b0c8c576b3e7a3965c4c375bb594365540ca10
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxgetjobinfo--get-job-information-from-distributed-computing-job"></a>rxGetJobInfo:  Get Job Information from Distributed Computing Job  
 ## <a name="description"></a>Description

Gets job information for a given distributed computing job.



 ## <a name="usage"></a>Usage

```   
  rxGetJobInfo(object)

```


 ## <a name="arguments"></a>Arguments



 ### `object`
 an object containing `jobInfo` information, such as that returned from a non-waiting, distributed computation. 




 ## <a name="details"></a>Details

The object returned from a non-waiting, distributed computation contains job information together with other information.  The job information is used internally by such functions as `rxGetJobStatus`, `rxGetJobOutput`, and `rxGetJobResults`. It is sometimes useful to extract it for its own sake, as it contains complete information on the job's compute context as well as other information needed by the distributed computing resources.

For most users, the principal use of this function is to determine whether a given object actually contains job information. If the return value is not `NULL`, then the object contains job information. Note, however, that the structure of the job information is subject to change, so code that attempts to manipulate it directly is not guaranteed to be forward-compatible.


 ## <a name="value"></a>Value

the job information, if present, or `NULL`.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[RxSpark](RxSpark.md), RxHadoopMR, [RxInSqlServer](RxInSqlServer.md), [rxGetJobStatus](rxGetJobResults.md), [rxGetJobOutput](rxGetJobOutput.md), [rxGetJobResults](rxGetJobResults.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# set up a non-waiting HPC Server compute context: 
myCluster <- RxSpark(nameNode = "my-name-service-server", port = 8020, wait = FALSE) 
rxOptions(computeContext=myCluster) 

myJob <- rxExec(function(){ print( "Hello World"); return ( 1 ) })
# The job information consists of the job's compute context
# and other information needed to prepare and complete the job
rxGetJobInfo(myJob)
# The results object will be a list containing the value 1 for each node
rxGetJobResults(myJob)
# Get job results will remove the job object (by default)
# Another call to rxGetJobInfo(myJob) would return no output

 ## End(Not run) 
```


