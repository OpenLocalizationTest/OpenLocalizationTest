---
title: rxCancelJob function (revoAnalytics) | Microsoft Docs
description: " Causes R to cancel an existing distributed computing job. "
keywords: (revoAnalytics), rxCancelJob, rxCancelJob,list-method, rxCancelJob,RxDistributedJob-method, rxCancelJob,RxDistributedHadoopMRJob-method, rxCancelJob,RxDistributedSqlServerJob-method, rxCancelJob,RxDistributedTeradataJob-method, rxCancelJob,ANY-method, IO
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
ms.openlocfilehash: 9fa46686ed52694aa6c6d10ea6c2c361ac66b098
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxcanceljob--cancel-distributed-computing-job"></a>rxCancelJob:  Cancel Distributed Computing Job  
 ## <a name="description"></a>Description

Causes R to cancel an existing distributed computing job.



 ## <a name="usage"></a>Usage

```   
  rxCancelJob( jobInfo, consoleOutput = NULL)

```


 ## <a name="arguments"></a>Arguments



 ### `jobInfo`
 a jobInfo object, such as that returned by [rxExec](rxExec.md) or one of the  RevoScaleR analysis functions in a non-waiting compute context, or the current contents of the `rxgLastPendingJob` object. 


 ### `consoleOutput`
 If `NULL`, the `consoleOutput` value assigned to  the job by the compute context at launch is used.  If `TRUE`, any console output present at the time the job is canceled is displayed.  If `FALSE`, no console output  is displayed. 



 ## <a name="details"></a>Details

This function does not attempt to retrieve any output objects; if the output is desired, the `consoleOutput` flag can be used to display it. This function does, however, remove all job-related artifacts from the distributed computing resources, including any job results.

On Windows, if you press ESC to interrupt a job and then call `rxCancelJob`, you may get an error message if the job was not completely submitted before you pressed ESC.


 ## <a name="value"></a>Value

`TRUE` if the job is successfully canceled; `FALSE` otherwise.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxGetJobs](rxGetJobs.md), RxHadoopMR.

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

rxCancelJob( rxgLastPendingJob, consoleOutput = TRUE )
rxCancelJob( myNonWaitingJob, consoleOutput = FALSE )
 ## End(Not run) 
```


