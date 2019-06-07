---
title: 'ServiceResponse class: from azureml-model-management-sdk Python module in Machine Learning Server'
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
ms.openlocfilehash: 13c8325f8c7bae35966298d7ab4a867067231d8f
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="class-serviceresponse"></a>Class ServiceResponse


## <a name="serviceresponse"></a>ServiceResponse



```
azureml.deploy.server.service.ServiceResponse(api, response, output_schema)
```




Represents the response from a service invocation. The response will contain any outputs and file artifacts produced in addition to any console output or errors messages.



## <a name="api"></a>api

```python
api
```




Gets the api endpoint.



## <a name="artifact"></a>artifact

```python
artifact(artifact_name, decode=True, encoding=None)
```




A convenience function to look up a file artifact by name and optionally base64 decode it.


### <a name="arguments"></a>Arguments


### <a name="artifactname"></a>artifact_name

The name of the file artifact.


### <a name="decode"></a>decode

Whether to decode the Base64 encoded artifact string. The default is `True`.


### <a name="encoding"></a>encoding

The encoding scheme to be used. The default is to apply no encoding. For a list of all encoding schemes please visit *Standard Encodings:*
[https://docs.python.org/3/library/codecs.html#standard-encodings](https://docs.python.org/3/library/codecs.html#standard-encodings)


### <a name="returns"></a>Returns

The file artifact as a Base64 encoded string if `decode=False` otherwise the decoded string.



## <a name="artifacts"></a>artifacts

```python
artifacts
```




Gets the non-decoded response file artifacts if present.
:returns: A `list` of non-decoded response file artifacts if present.



## <a name="consoleoutput"></a>console_output

```python
console_output
```




Gets the console output if present.



## <a name="error"></a>error 

```python
error
```




Gets the error if present.



## <a name="output"></a>output

```python
output(output)
```




    A convenience function to look up an output value by name.


### <a name="arguments"></a>Arguments


### <a name="output"></a>output

The name of the output.


### <a name="returns"></a>Returns

The service output’s value.



## <a name="outputs"></a>outputs

```python
outputs
```




Gets the response outputs if present.



## <a name="rawoutputs"></a>raw_outputs

```python
raw_outputs
```




Gets the raw response outputs if present.
