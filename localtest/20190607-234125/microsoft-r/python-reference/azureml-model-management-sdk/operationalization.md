---
title: 'Operationalization class: from azureml-model-management-sdk Python module in Machine Learning Server'
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
ms.openlocfilehash: c8a8f5db3340e52516a9d889e787a513ae94c276
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="class-operationalization"></a>Class Operationalization


## <a name="operationalization"></a>Operationalization



```
azureml.deploy.operationalization.Operationalization
```




*Operationalization* is designed to be a low-level abstract foundation class from which other service operationalization attribute classes in the *mldeploy* package can be derived. It provides a standard template for creating attribute-based operationalization lifecycle phases providing a consistent  *__init()__*, *__del()__* sequence that chains initialization (initializer), authentication (authentication), and destruction (destructor) methods for the class hierarchy.



## <a name="authentication"></a>authentication

```python
authentication(context)
```




Authentication lifecycle method. Invokes the authentication entry-point for the class hierarchy.

An optional _noonp_ method where subclass implementers MAY provide this method definition by overriding.

Sub-class should override and implement.


### <a name="arguments"></a>Arguments


### <a name="context"></a>context

The optional authentication context as defined in the implementing sub-class.



## <a name="deleteservice"></a>delete_service

```python
delete_service(name, **opts)
```




Sub-class should override and implement.



## <a name="deployrealtime"></a>deploy_realtime

```python
deploy_realtime(name, **opts)
```




Sub-class should override and implement.



## <a name="deployservice"></a>deploy_service

```python
deploy_service(name, **opts)
```




Sub-class should override and implement.



## <a name="destructor"></a>destructor

```python
destructor()
```




Destroy lifecycle method. Invokes destructors for the class hierarchy.

An optional _noonp_ method where subclass implementers MAY provide this method definition by overriding.

Sub-class should override and implement.



## <a name="getservice"></a>get_service

```python
get_service(name, **opts)
```




Retrieve service meta-data from the name source and return a new service instance.

Sub-class should override and implement.



## <a name="initializer"></a>initializer

```python
initializer(api_client, config, adapters=None)
```




Init lifecycle method, invoked during construction. Sets up attributes and invokes initializers for the class hierarchy.

An optional _noonp_ method where subclass implementers MAY provide this method definition by overriding.

Sub-class should override and implement.



## <a name="listservices"></a>list_services

```python
list_services(name=None, **opts)
```




Sub-class should override and implement.



## <a name="realtimeservice"></a>realtime_service

```python
realtime_service(name)
```




Begin fluent API chaining of properties for defining a *real-time* web service.

**Example:**



```
client.realtime_service('scoring')
   .description('A new real-time web service')
   .version('v1.0.0')
```



### <a name="arguments"></a>Arguments


### <a name="name"></a>name

The web service name.


### <a name="returns"></a>Returns

A [`RealtimeDefinition`](realtime-definition.md) instance for fluent API chaining.



```
redeploy_realtime(name, force=False, **opts)
```




Sub-class should override and implement.



## <a name="redeployservice"></a>redeploy_service

```python
redeploy_service(name, force=False, **opts)
```




Sub-class should override and implement.



## <a name="service"></a>service

```python
service(name)
```




Begin fluent API chaining of properties for defining a *standard* web service.

**Example:**



```
client.service('scoring')
   .description('A new web service')
   .version('v1.0.0')
```



### <a name="arguments"></a>Arguments


### <a name="name"></a>name

The web service name.


### <a name="returns"></a>Returns

A [`ServiceDefinition`](service-definition.md) instance for fluent API chaining.
