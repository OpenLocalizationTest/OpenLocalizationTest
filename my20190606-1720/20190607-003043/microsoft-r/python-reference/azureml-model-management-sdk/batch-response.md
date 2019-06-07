---
title: 'BatchResponse class: from azureml-model-management-sdk Python module in Machine Learning Server'
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
ms.openlocfilehash: b84ccba5a20ea4978a75354972be2e9df7ef824b
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="class-batchresponse"></a>Class BatchResponse


## <a name="batchresponse"></a>BatchResponse



```
azureml.deploy.server.service.BatchResponse(api, execution_id, response,
    output_schema)
```




Represents a service’s entire batch execution response at a particular state in time. Using this, a batch execution index can be supplied to the `execution(index)` function in order to retrieve the service’s [`ServiceResponse`](service-response.md).



## <a name="api"></a>api

```python
api
```




Gets the api endpoint.



## <a name="completeditemcount"></a>completed_item_count

```python
completed_item_count
```




Gets the number of completed batch results processed thus far.
:returns: The number of completed batch results processed thus far.



## <a name="execution"></a>execution

```python
execution(index)
```




Extracts the service execution results within the batch at this execution *index*.


### <a name="arguments"></a>Arguments


### <a name="index"></a>index

The batch execution index.


### <a name="returns"></a>Returns

The execution results [`ServiceResponse`](service-response.md).



## <a name="executionid"></a>execution_id

```python
execution_id
```




Gets this batch’s execution identifier if a batch has been started, otherwise `None`.
:returns: This batch’s execution identifier if a batch has been started, otherwise `None`.



## <a name="totalitemcount"></a>total_item_count

```python
total_item_count
```




Gets the total number of batch results processed in any state.
:returns: The total number of batch results processed in any state.
