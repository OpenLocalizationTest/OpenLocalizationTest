---
title: 'rx_get_job_output: Gets the console output from the various nodes in a non-waiting distributed computing job. (revoscalepy)'
description: During a job run, the state of the output is non-deterministic (that is, it may or may not be on disk, and what is on disk at any given point in time may not reflect the actual completion state of a job).If auto_cleanup has been set to True on the distributed computing job’s compute context, the console output will not persist after the job completes.Unlike rx_get_job_results, this function does not remove any job information upon retrieval.
keywords: job, output
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
ms.openlocfilehash: cd75767ab8daacdd8d39465fcac255e14a29b36f
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxgetjoboutput"></a>rx_get_job_output


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_get_job_output(job_info: revoscalepy.computecontext.RxRemoteJob.RxRemoteJob) -> str
```





## <a name="description"></a>Description

During a job run, the state of the output is non-deterministic (that is, it may or may not be on disk, and what is on disk at any given point in time may not reflect the actual completion state of a job).

If *auto_cleanup* has been set to *True* on the distributed computing job’s compute context, the console output will not persist after the job completes.

Unlike *rx_get_job_results*, this function does not remove any job information upon retrieval.


## <a name="arguments"></a>Arguments


### <a name="jobinfo"></a>job_info

The distributed computing job for which to retrieve the job output


## <a name="returns"></a>Returns

*str* that contains the console output for the nodes participating in the distributed computing job


## <a name="see-also"></a>See also

`rx_get_job_status`


## <a name="example"></a>Example



```
from revoscalepy import RxInSqlServer
from revoscalepy import rx_exec
from revoscalepy import rx_get_job_output
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

# Wait for the job to finish or fail whatever the case may be
rx_wait_for_job(job)

# Print out what our code printed on sql
output = rx_get_job_output(job)
print(output)
```

