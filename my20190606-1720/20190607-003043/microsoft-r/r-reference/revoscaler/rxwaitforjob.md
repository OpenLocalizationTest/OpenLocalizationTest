---
title: rxWaitForJob function (revoAnalytics) | Microsoft Docs
description: " Causes R to block on an existing distributed job until completion. "
keywords: (revoAnalytics), rxWaitForJob, rxWaitForJob,RxDistributedJob-method, rxWaitForJob,RxDistributedSqlServerJob-method, rxWaitForJob,RxDistributedTeradataJob-method, rxWaitForJob,RxDistributedHadoopMRJob-method, rxWaitForJob,ANY-method, IO
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
ms.openlocfilehash: bfc59c7f8177f564bf2a2428d8695bf84a7f62a9
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxwaitforjob--wait-for-distributed-job-to-complete"></a>rxWaitForJob:  Wait for Distributed Job to Complete  
 ## <a name="description"></a>Description

Causes R to block on an existing distributed job until completion.



 ## <a name="usage"></a>Usage

```   
  rxWaitForJob(jobInfo)

```


 ## <a name="arguments"></a>Arguments



 ### `jobInfo`
 A `jobInfo` object. 




 ## <a name="details"></a>Details

This function essentially changes a non-blocking distributed computing job to a blocking job. You can change a blocking job to non-blocking on Windows by pressing the Esc key, then using `rxGetJobStatus` and `rxGetJobResults` on the object `rxgLastPendingJob`. This function does not, however, modify the compute context.


 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="examples"></a>Examples

 ```

  ## Not run:

rxWaitForJob( rxgLastPendingJob )
rxWaitForJob( myNonWaitingJob )
 ## End(Not run) 
```


