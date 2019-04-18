---
title: 'RealtimeDefinition class: from azureml-model-management-sdk Python module in Machine Learning Server'
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
ms.openlocfilehash: 379fa29d33c45fb4ff1bfb4726c1ba545ab7519f
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="class-realtimedefinition"></a>Class RealtimeDefinition


## <a name="realtimedefinition"></a>RealtimeDefinition



```
azureml.deploy.operationalization.RealtimeDefinition(name, op)
```




Bases: [`azureml.deploy.operationalization.OperationalizationDefinition`](operationalization-definition.md)

Real-time class defining a *real-time* service’s properties for publishing.



```python
alias(alias)
```




Set the optional service function name alias to use in order to consume the service.

**Example:**



```
service = client.service('score-service').alias('score').deploy()

# `score()` is the function that will call the `score-service`
result = service.score()
```



### <a name="arguments"></a>Arguments


### <a name="alias"></a>alias

The service function name alias to use in order to consume the service.


### <a name="returns"></a>Returns

Self [`OperationalizationDefinition`](operationalization-definition.md) for fluent API.



## <a name="deploy"></a>deploy

```python
deploy()
```




Bundle up the definition properties and publish the service.


### <a name="returns"></a>Returns

A new instance of [`Service`](service.md) representing the service *deployed*.



## <a name="description"></a>description

```python
description(description)
```




Set the service’s optional description.


### <a name="arguments"></a>Arguments


### <a name="description"></a>description

The description of the service.


### <a name="returns"></a>Returns

Self [`OperationalizationDefinition`](operationalization-definition.md) for fluent API.



## <a name="redeploy"></a>redeploy

```python
redeploy(force=False)
```




Bundle up the definition properties and update the service.


### <a name="returns"></a>Returns

A new instance of [`Service`](service.md) representing the service *deployed*.



## <a name="serializedmodel"></a>serialized_model

```python
serialized_model(model)
```




Serialized model.


### <a name="arguments"></a>Arguments


### <a name="model"></a>model

The required serialized model used for this real-time service.


### <a name="returns"></a>Returns

Self [`OperationalizationDefinition`](operationalization-definition.md) for fluent API chaining.



## <a name="version"></a>version

```python
version(version)
```




Set the service’s optional version.


### <a name="arguments"></a>Arguments


### <a name="version"></a>version

The version of the service.


### <a name="returns"></a>Returns

Self [`OperationalizationDefinition`](operationalization-definition.md) for fluent API.
