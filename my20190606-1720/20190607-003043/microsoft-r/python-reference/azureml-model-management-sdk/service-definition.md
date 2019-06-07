---
title: 'ServiceDefinition class: from azureml-model-management-sdk Python module in Machine Learning Server'
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
ms.openlocfilehash: ce5b457cbbd6f6c49609b4e6080683ed3c533637
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="servicedefinition"></a>ServiceDefinition


## <a name="class-servicedefinition"></a>Class ServiceDefinition



```
azureml.deploy.operationalization.ServiceDefinition(name, op)
```




Bases: [`azureml.deploy.operationalization.OperationalizationDefinition`](operationalization-definition.md)

Service class defining a *standard* service’s properties for publishing.



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



## <a name="artifact"></a>artifact

```python
artifact(artifact)
```




Define a service’s optional supported file artifact by name. A convenience to calling `.artifacts(['file.png'])` with a list of one.


### <a name="arguments"></a>Arguments


### <a name="artifact"></a>artifact

A single file artifact by name.


### <a name="returns"></a>Returns

Self [`OperationalizationDefinition`](operationalization-definition.md) for fluent API chaining.



## <a name="artifacts"></a>artifacts

```python
artifacts(artifacts)
```




Defines a service’s optional supported file artifacts by name.


### <a name="arguments"></a>Arguments


### <a name="artifacts"></a>artifacts

A `list` of file artifacts by name.


### <a name="returns"></a>Returns

Self [`OperationalizationDefinition`](operationalization-definition.md) for fluent API chaining.



## <a name="codefn"></a>code_fn

```python
code_fn(code, init=None)
```




Set the service consume function as a function.

**Example:**



```
def init():
    pass

def score(df):
    pass

.code_fn(score, init)
```



### <a name="arguments"></a>Arguments


### <a name="code"></a>code

A function handle as a reference to run python code.


### <a name="init"></a>init

An optional function handle as a reference to initialize the service.


### <a name="returns"></a>Returns

Self [`OperationalizationDefinition`](operationalization-definition.md) for fluent API chaining.



## <a name="codestr"></a>code_str

```python
code_str(code, init=None)
```




Set the service consume function as a block of python code as a `str`.



```
init = 'import pandas as pd'
code = 'print(pd)'

.code_str(code, init)
```



### <a name="arguments"></a>Arguments


### <a name="code"></a>code

A block of python code as a `str`.


### <a name="init"></a>init

An optional block of python code as a `str` to initialize the service.


### <a name="returns"></a>Returns

A [`ServiceDefinition`](service-definition.md) for fluent API chaining.



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



## <a name="inputs"></a>inputs

```python
inputs(**inputs)
```




Defines a service’s optional supported inputs by name and type.

**Example:**



```
.inputs(a=float, b=int, c=str, d=bool, e='pandas.DataFrame')
```



### <a name="arguments"></a>Arguments


### <a name="inputs"></a>inputs

The inputs by name and type.


### <a name="returns"></a>Returns

Self [`OperationalizationDefinition`](operationalization-definition.md) for fluent API chaining.



## <a name="models"></a>models

```python
models(**models)
```




Include any model(s) used for this service.

**Example:**



```
cars_model = rx_lin_mod(formula="am ~ hp + wt",data=mtcars)

.models(cars_model=cars_model)
```



### <a name="arguments"></a>Arguments


### <a name="models"></a>models

Any models by name and value.


### <a name="returns"></a>Returns

Self [`OperationalizationDefinition`](operationalization-definition.md) for fluent API chaining.



## <a name="objects"></a>objects

```python
objects(**objects)
```




Include any object(s) used for this service.

**Example:**



```
x = 5
y = 'hello'

.objects(x=x, y=y)
```



### <a name="arguments"></a>Arguments


### <a name="objects"></a>objects

Any objects by name and value.


### <a name="returns"></a>Returns

Self [`OperationalizationDefinition`](operationalization-definition.md) for fluent API chaining.



## <a name="outputs"></a>outputs

```python
outputs(**outputs)
```




Defines a service’s optional supported outputs by name and type.

**Example:**



```
.outputs(a=float, b=int, c=str, d=bool, e='pandas.DataFrame')
```



### <a name="arguments"></a>Arguments


### <a name="outputs"></a>outputs

The outputs by name and type.


### <a name="returns"></a>Returns

Self [`OperationalizationDefinition`](operationalization-definition.md) for fluent API chaining.



## <a name="redeploy"></a>redeploy

```python
redeploy(force=False)
```




Bundle up the definition properties and update the service.


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
