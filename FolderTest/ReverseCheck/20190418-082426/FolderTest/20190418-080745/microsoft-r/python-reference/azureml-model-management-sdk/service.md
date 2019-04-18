---
title: 'Service class: from azureml-model-management-sdk Python module in Machine Learning Server'
description: ''
keywords: ''
author: HeidiSteen
manager: cgronlun
ms.date: 09/20/2017
ms.topic: reference
ms.prod: mlserver
ms.author: heidist
ms.service: ''
ms.assetid: ''
ROBOTS: ''
audience: ''
ms.devlang: Python
ms.reviewer: ''
ms.suite: ''
ms.tgt_pltfrm: ''
ms.custom: ''
ms.openlocfilehash: 2016121891e2cfdbdaad01e644d65325b10cb467
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="class-service"></a>Class Service


## <a name="service"></a>Service



```
azureml.deploy.server.service.Service(service, http_client)
```




Dynamic object for service consumption and batching based on service metadata attributes.



## <a name="batch"></a>batch

```
batch(records, parallel_count=10)
```




Register a set of input records for batch execution on this service.


### <a name="arguments"></a>Arguments


### <a name="records"></a>records

The *data.frame* or *list* of input records to execute.


### <a name="parallelcount"></a>parallel_count

Number of threads used to process entries in the batch. Default value is 10. Please make sure not to use too high of a number because it might negatively impact performance.


### <a name="returns"></a>Returns

The [`Batch`](batch.md) instance to control this service’s batching lifecycle.



## <a name="capabilities"></a>capabilities

```python
capabilities()
```




Provides the following information describing the holdings of this service:

* *api* -  The API REST endpoint. 

* *name* - The service name. 

* *version* - The service version. 

* *published_by* - The service publishing author. 

* *runtime* - The service runtime context _R|Python_. 

* *description* - The service description. 

* *creation_time* - The service publish timestamp. 

* *snapshot_id* - The snapshot identifier this service is bound with. 

* *inputs* - The input schema name/type definition. 

* *outputs* - The output schema name/type definition. 

* *inputs_encoded* - The input schema name/type encoded to python. 

* *outputs_encoded* - The output schema name/type encoded to python. 

* *artifacts* - The supported generated files. 

* *operation_id* - The function `alias`. 

* *swagger* - The API REST endpoint to this service’s *swagger.json* document. 


### <a name="returns"></a>Returns

A `dict` of key/values describing the service.



## <a name="getbatch"></a>get_batch

```python
get_batch(execution_id)
```




Retrieves the service batch based on an execution identifier.


### <a name="arguments"></a>Arguments


### <a name="executionid"></a>execution_id

The identifier of the batch execution.


### <a name="returns"></a>Returns

The [`Batch`](batch.md) instance to control this service’s batching lifecycle.



## <a name="listexecutions"></a>list_executions

```python
list_batch_executions()
```




Gets all batch execution identifiers currently queued for this service.


### <a name="returns"></a>Returns

A `list` of execution identifiers.



## <a name="swagger"></a>swagger

```python
swagger()
```




Retrieves the *swagger.json* for this service (see [http://swagger.io/](http://swagger.io/)).


### <a name="returns"></a>Returns

The swagger document for this service as a json `str`.
