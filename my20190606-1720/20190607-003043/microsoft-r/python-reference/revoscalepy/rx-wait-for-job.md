---
title: 'rx_wait_for_job: Wait for Distributed Job to Complete (revoscalepy)'
description: Causes Python to block on an existing distributed job until completion.  This effectively turns a non-blocking job into a blocking job.
keywords: wait, job
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
ms.openlocfilehash: a7ec557b9c6b8ba983e2683224bfaa0994e26fcc
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxwaitforjob"></a>rx_wait_for_job


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_wait_for_job(job_info: revoscalepy.computecontext.RxRemoteJob.RxRemoteJob)
```





## <a name="description"></a>Description

Causes Python to block on an existing distributed job until completion.  This effectively turns a non-blocking job into a blocking job.


## <a name="arguments"></a>Arguments


### <a name="jobinfo"></a>job_info

A jobInfo object.


## <a name="see-also"></a>See also


## <a name="example"></a>Example



```
from revoscalepy import RxInSqlServer
from revoscalepy import RxSqlServerData
from revoscalepy import rx_logit
from revoscalepy import rx_wait_for_job
from revoscalepy import rx_get_job_results

connection_string = 'Driver=SQL Server;Server=.;Database=RevoTestDb;Trusted_Connection=True;'
airline_data_source = RxSqlServerData(sql_query='select top 1000 * from airlinedemosmall',
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
compute_context = RxInSqlServer(connection_string=connection_string, num_tasks=1, wait=False)

def transform_late(dataset, context):
    dataset['Late'] = dataset['ArrDelay'] > 15
    return dataset

# Since wait is set to False on the compute_context rx_logit will return a job rather than the model
job = rx_logit(formula='Late ~ DayOfWeek',
               data=airline_data_source,
               compute_context=compute_context,
               transform_function=transform_late,
               transform_variables=['ArrDelay'])

# Wait for the job to finish
rx_wait_for_job(job)
model = rx_get_job_results(job)
print(model)
```

