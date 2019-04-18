---
title: 'OperationalizationDefinition class: from azureml-model-management-sdk Python module in Machine Learning Server'
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
ms.openlocfilehash: cc3fd43f1c1bd3122195166cf5154d33df11057b
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="class-operationalizationdefinition"></a>Class OperationalizationDefinition


## <a name="operationalizationdefinition"></a>OperationalizationDefinition



```
azureml.deploy.operationalization.OperationalizationDefinition(name, op,
    defs_extent={})
```




Base abstract class defining a service’s properties.

Create a new publish definition.


### <a name="arguments"></a>Arguments


### <a name="name"></a>name

The web service name.


### <a name="op"></a>op

A reference to the deploy client instance.


### <a name="defsextent"></a>defs_extent

A mixin of subclass specific definitions.

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

To be implemented by subclasses.


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

To be implemented by subclasses.


### <a name="returns"></a>Returns

A new instance of [`Service`](service.md) representing the service *deployed*.



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
