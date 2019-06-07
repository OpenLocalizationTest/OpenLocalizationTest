---
title: 'RxRemoteJobStatus: Execution status of a remote job (revoscalepy)'
description: This enumeration represents the execution status of a remote Python job.  The enumeration is returned from the rx_get_job_status method and will indicate the current status of the job.  The enumeration has the following values indicating job status:FINISHED - The job has run to a successful completionFAILED - The job has failedCANCELED - The job was cancelled before it could run to successful completion by using rx_cancel_jobUNDETERMINED - The job’s status could not be determined, typically meaning it has been executed on the server and the job has already been cleaned up by calling rx_get_job_results or rx_cleanup_jobsRUNNING - The distributed computing job is currently executing on the serverQUEUED - The distributed computing job is currently awaiting execution on the server
keywords: remote, job
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
ms.openlocfilehash: 58d2f8f741fa31ef6a7986f7e903c653f8abfb90
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxremotejobstatus"></a>RxRemoteJobStatus


 



```
revoscalepy.RxRemoteJobStatus
```





## <a name="description"></a>Description

This enumeration represents the execution status of a remote Python job.  The enumeration is returned from the rx_get_job_status method and will indicate the current status of the job.  The enumeration has the following values indicating job status:

*FINISHED* - The job has run to a successful completion

*FAILED* - The job has failed

*CANCELED* - The job was canceled before it could run to successful completion by using *rx_cancel_job*

*UNDETERMINED* - The job’s status could not be determined, typically meaning it has been executed on the server and the job has already been cleaned up by calling *rx_get_job_results* or *rx_cleanup_jobs*

*RUNNING* - The distributed computing job is currently executing on the server

*QUEUED* - The distributed computing job is currently awaiting execution on the server


## <a name="see-also"></a>See also

`rx_get_job_status`


## <a name="example"></a>Example



```
from revoscalepy import RxInSqlServer
from revoscalepy import rx_exec
from revoscalepy import RxRemoteJobStatus
from revoscalepy import rx_get_job_status
from revoscalepy import rx_wait_for_job

connection_string = 'Driver=SQL Server;Server=.;Database=RevoTestDb;Trusted_Connection=True;'

# Setting wait to False allows the job to be run asynchronously
# Setting console_output to True allows us to get the console output of the distributed computing job
compute_context = RxInSqlServer(connection_string=connection_string,
                                num_tasks=1,
                                console_output=True,
                                wait=False)

def hello_from_sql():
    import time
    print('Hello from SQL server')
    time.sleep(3)
    return 'We just ran Python code asynchronously on a SQL server!'

job = rx_exec(function=hello_from_sql, compute_context=compute_context)

# Poll initial status
status = rx_get_job_status(job)

print(status)

if status == RxRemoteJobStatus.RUNNING or status == RxRemoteJobStatus.QUEUED :
# Wait for the job to finish or fail whatever the case may be
rx_wait_for_job(job)

# Poll final status
status = rx_get_job_status(job)

print(status)
```

