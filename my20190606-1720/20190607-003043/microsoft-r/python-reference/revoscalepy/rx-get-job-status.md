---
title: 'rx_get_job_status: Obtain Distributed Computing Job Status (revoscalepy)'
description: Obtain distributed computing processing status for the specified job.
keywords: job, status
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
ms.openlocfilehash: de499058afe5a39a0215ffdbc23c4ef62b27ebe3
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxgetjobstatus"></a>rx_get_job_status


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_get_job_status(job_info: revoscalepy.computecontext.RxRemoteJob.RxRemoteJob) -> revoscalepy.computecontext.RxJob.RxRemoteJobStatus
```





## <a name="description"></a>Description

Obtain distributed computing processing status for the specified job.


## <a name="arguments"></a>Arguments


### <a name="jobinfo"></a>job_info

A job object as returned by rx_exec or a revoscalepy analysis function, if available.


## <a name="returns"></a>Returns

A RxRemoteJobStatus enumeration value that designates the status of the remote job


## <a name="see-also"></a>See also

`rx_get_job_results`
`RxRemoteJobStatus`


## <a name="example"></a>Example



```
from revoscalepy import RxInSqlServer
from revoscalepy import rx_exec
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

# Wait for the job to finish or fail whatever the case may be
rx_wait_for_job(job)

# Poll final status
status = rx_get_job_status(job)

print(status)
```

