---
title: 'rx_cleanup_jobs:  (revoscalepy)'
description: Removes the artifacts for the specified jobs.If job_info_list is a RxRemoteJob object, rx_cleanup_jobs attempts to remove the artifacts. However, if the job has successfully completed and force is False, rx_cleanup_jobs issues a warning saying to either set force=True or use rx_get_job_results to get the results and delete the artifacts.If job_info_list is a list of jobs, rx_cleanup_jobs attempts to apply the cleanup rules for a single job to each element in the list.
keywords: cleanup, job
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
ms.openlocfilehash: bff4c0663bda73a9b4fcc99d441c6c2f617829ba
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxcleanupjobs"></a>rx_cleanup_jobs


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_cleanup_jobs(job_info_list: typing.Union[revoscalepy.computecontext.RxRemoteJob.RxRemoteJob,
    list], force: bool = False, verbose: bool = True)
```





## <a name="description"></a>Description

Removes the artifacts for the specified jobs.

If *job_info_list* is a *RxRemoteJob* object, *rx_cleanup_jobs* attempts to remove the artifacts. However, if the job has successfully completed and *force* is *False*, *rx_cleanup_jobs* issues a warning saying to either set *force=True* or use *rx_get_job_results* to get the results and delete the artifacts.

If *job_info_list* is a list of jobs, *rx_cleanup_jobs* attempts to apply the cleanup rules for a single job to each element in the list.


## <a name="arguments"></a>Arguments


### <a name="jobinfolist"></a>job_info_list

The jobs for which to remove the artifacts, this can be a list of jobs or a single job


### <a name="force"></a>force

*True* indicates the cleanup should happen regardless of whether or not the job status can be determined and job results have already been retrieved. *False* indicates that the should be cleaned up by calling *rx_get_job_results* or the job should have completed unsuccessfully (such as by using rx_cancel_job).


### <a name="verbose"></a>verbose

If *True*, will print the directories/records being deleted.


## <a name="returns"></a>Returns

This function does not return a value


## <a name="see-also"></a>See also


## <a name="example"></a>Example



```
import time
from revoscalepy import RxInSqlServer
from revoscalepy import RxSqlServerData
from revoscalepy import rx_dforest
from revoscalepy import rx_cancel_job
from revoscalepy import RxRemoteJobStatus
from revoscalepy import rx_get_job_status
from revoscalepy import rx_cleanup_jobs

connection_string = 'Driver=SQL Server;Server=.;Database=RevoTestDb;Trusted_Connection=True;'
airline_data_source = RxSqlServerData(sql_query='select * from airlinedemosmall',
                                      connection_string=connection_string,
                                      column_info={
                                          'ArrDelay': {'type': 'integer'},
                                          'CRSDepTime': {'type': 'float'},
                                          'DayOfWeek': {
                                              'type': 'factor',
                                              'levels': ['Monday', 'Tuesday', 'Wednesday', 'Thursday',
                                                         'Friday',
                                                         'Saturday', 'Sunday']
                                          }
                                      })

# Setting wait to False allows the job to be run asynchronously
compute_context = RxInSqlServer(connection_string=connection_string,
                                num_tasks=1,
                                auto_cleanup=False,
                                wait=False)

job = rx_dforest(formula='ArrDelay ~ DayOfWeek',
                 seed=1,
                 data=airline_data_source,
                 compute_context=compute_context)

# Poll until status is RUNNING
status = rx_get_job_status(job)
while status == RxRemoteJobStatus.QUEUED:
    time.sleep(1)
    status = rx_get_job_status(job)

if status == RxRemoteJobStatus.RUNNING :
    # Cancel the job
    rx_cancel_job(job)

# Only canceled or failed jobs can be cleaned up
if status == RxRemoteJobStatus.CANCELED or status == RxRemoteJobStatus.FAILED :
    # Cleanup after the job
    rx_cleanup_jobs(job)
```

