---
title: 'Batch class: from azureml-model-management-sdk Python module in Machine Learning Server'
description: ''
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 02/16/2018
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
ms.openlocfilehash: 70f0368736e592fc85e5d5b78c0634c3b52f07b7
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="class-batch"></a>Class Batch


## <a name="batch"></a>Batch



```
azureml.deploy.server.service.Batch(service, records=[], parallel_count=10,
    execution_id=None)
```




Manager of a service’s batch execution lifecycle.



## <a name="api"></a>api

```python
api
```




Gets the api endpoint.



## <a name="executionid"></a>execution_id

```python
execution_id
```




Gets this batch’s execution identifier if currently started, otherwise `None`.



## <a name="parallelcount"></a>parallel_count

```python
parallel_count
```




Gets this batch’s parallel count of threads.



```
records
```




Gets the batch input records.



```
results(show_partial_results=True)
```




Poll for batch results.


### <a name="arguments"></a>Arguments


### <a name="showpartialresults"></a>show_partial_results

To get partial execution results or not.
The default is to include partial results.


### <a name="returns"></a>Returns

An instance of [`BatchResponse`](batch-response.md).



## <a name="start"></a>start

```python
start()
```




Starts a batch execution for this service.


### <a name="returns"></a>Returns

An instance of itself [`Batch`](Batch.md).

## <a name="artifacts"></a>artifacts

```python
artifact(index, file_name)
```

Get the file artifact for this service batch execution *index*.

### <a name="arguments"></a>Arguments

### <a name="index"></a>index

Batch execution index.

### <a name="filename"></a>file_name

Artifact filename

### <a name="returns"></a>Returns

A single file artifact.

## <a name="cancel"></a>cancel

```python
cancel()
```

Cancel this batch execution.

## <a name="download"></a>download



```
download(index, file_name=None, destination=cwd())
```


Download the file artifact to file-system in the *destination*.

### <a name="arguments"></a>Arguments

### <a name="index"></a>index

Batch execution index.

### <a name="filename"></a>file_name

The file artifact name.

### <a name="destination"></a>destination

Download location.

### <a name="returns"></a>Returns

A *list* of downloaded file-paths.

## <a name="listartifacts"></a>list_artifacts

```python
list_artifacts(index)
```

List the file artifact names belonging to this service batch execution *index*.

### <a name="arguments"></a>Arguments

### <a name="index"></a>index

Batch execution index.

### <a name="returns"></a>Returns

A *list* of file artifact names.

Gets this batch’s parallel count of threads.

## <a name="records"></a>records

```python
records
```

Gets the batch input records.

## <a name="results"></a>results

```python
results(show_partial_results=True)
```

Poll batch results.

### <a name="arguments"></a>Arguments

### <a name="showpartialresults"></a>show_partial_results

To get partial execution results or not.

### <a name="returns"></a>Returns

An execution Self [*BatchResponse*](batch-response.md).
