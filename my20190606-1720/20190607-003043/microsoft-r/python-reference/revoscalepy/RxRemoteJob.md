---
title: 'RxRemoteJob,close,deserialize_job,deserialize_jobs,resolve_context: Closes a remote job (revoscalepy)'
description: Closes the remote job, purging all associated job-related data. You can reference a job by its ID, or call close() to purge jobs in a given compute context.
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
ms.openlocfilehash: c97c6ee8b06b8e9c0653dac3c18698133f75788c
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxremotejob"></a>RxRemoteJob


 



```
revoscalepy.RxRemoteJob(compute_context: revoscalepy.computecontext.RxComputeContext.RxComputeContext,
    job_id: str = None)
```





## <a name="description"></a>Description

Closes the remote job, purging all associated job-related data. You can reference a job by its ID, or call close() to purge jobs in a given compute context.



```
close()
```




Closes the remote job, purging all the data associated with the job



```
deserialize_job(job_id: str) -> revoscalepy.computecontext.RxRemoteJob.RxRemoteJob
```




Deserializes a RxRemoteJob given the job ID


## <a name="returns"></a>Returns

The job that was deserialized



```
deserialize_jobs() -> list
```




Deserializes the existing jobs that have not been cleaned up by calling close().


## <a name="returns"></a>Returns

The deserialized jobs



```
resolve_context() -> revoscalepy.computecontext.RxComputeContext.RxComputeContext
```




Resolves the `RxComputeContext` that is associated with the job


## <a name="returns"></a>Returns

The `RxComputeContext` that is associated with the job or `None` if the compute context isn’t valid
