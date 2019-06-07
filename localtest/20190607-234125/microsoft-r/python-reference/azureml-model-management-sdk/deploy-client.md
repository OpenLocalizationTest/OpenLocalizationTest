---
title: 'DeployClient class: from azureml-model-management-sdk Python module in Machine Learning Server'
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
ms.openlocfilehash: 57b341177f9e5646647060c53084a9944060d990
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="class-deployclient"></a>Class DeployClient


## <a name="deployclient"></a>DeployClient



```
azureml.deploy.DeployClient(host, auth=None, use=None)
```




Defines the factory for creating Deployment Clients.

**Basic Usage Module implementation plugin with `use` property:**

Find and Load *module* from an import reference:



```
from azureml.deploy import DeployClient
from azureml.deploy.server import MLServer

host = 'http://localhost:12800'
ctx = ('username', 'password')
mls_client = DeployClient(host, use=MLServer, auth=ctx)
```


Find and Load *module* as defined by *use* from namespace str:



```
host = 'http://localhost:12800'
ctx = ('username', 'password')

mls_client = DeployClient(host, use=MLServer, auth=ctx)
mls_client = DeployClient(host, use='azureml.deploy.server.MLServer',
auth=ctx)
```


Find and Load *module* from a file/path tuple:



```
host = 'http://localhost:12800'
ctx = ('username', 'password')

use = ('azureml.deploy.server.MLServer', '/path/to/mlserver.py')
mls_client = DeployClient(host, use=use, auth=ctx)
```


Create a new Deployment Client.


### <a name="arguments"></a>Arguments


### <a name="host"></a>host

Server HTTP/HTTPS endpoint, including the port number.


### <a name="auth"></a>auth

(optional) Authentication context. Not all deployment clients require authentication. The *auth* is  **required** for **MLServer**


### <a name="use"></a>use

(required) Deployment implementation to use (ex) *use=’MLServer’* to use The ML Server.
