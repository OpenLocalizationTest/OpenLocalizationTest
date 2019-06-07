---
title: rxFindFileInPath function (revoAnalytics) | Microsoft Docs
description: " Sequentially checks the entries in a delimited path string for a provided file name. "
keywords: (revoAnalytics), rxFindFileInPath, IO
author: heidisteen
manager: cgronlun
ms.date: 01/24/2018
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ROBOTS: ''
audience: ''
ms.devlang: ''
ms.reviewer: ''
ms.suite: ''
ms.tgt_pltfrm: ''
ms.custom: ''
ms.openlocfilehash: 039fdfff296ea2bad2ea3c109e485e3784eab8e5
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxfindfileinpath--finds-where-in-a-given-path-a-file-is"></a>rxFindFileInPath:  Finds where in a given path a file is.  
 ## <a name="description"></a>Description

Sequentially checks the entries in a delimited path string for a provided file name.



 ## <a name="usage"></a>Usage

```   
  rxFindFileInPath( path, fileName )

```


 ## <a name="arguments"></a>Arguments




 ### `path`
 character vector, compute context or job object.  This is a required parameter.   If a compute context is provided, the `dataPath` from that context (assuming it has one ) will be used;  if a job object is provided, that job object's compute context's `dataPath` will be used. If a character vector is provided, each element of the vector should contain one directory path.   If a character scalar is supplied, multiple directory paths can be contained by using the standard system  delimiters (":" for Linux and ";") to separate the entries within the path.  This allows system PATH's to  be parsed using this function. 



 ### `fileName`
 logical scalar.  This is a required parameter.  The name of the file being sought along the `path`. 





 ## <a name="details"></a>Details

This function will sequentially check the locations (directories) provided in the `path`.  Thus, if there exists more than one instance of a file with the same `fileName`, the first instance of a directory in the path containing the file will be the one returned.



 ## <a name="value"></a>Value

Returns NULL if the target file is not found in any of the possible locations, or the path to the file (not including the file name) if it is found.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# using a Linux environment PATH
rxFindFileInPath(path=Sys.getenv("PATH"), fileName="Revoscript")

# using a compute context
rxFindFileInPath(path=myComputeContext, fileName="myData" )

# for Windows
rxFindFileInPath(path="C:\data\remember\to\escape\backslashes;D:\other\data", fileName="myData" )

# for Linux
rxFindFileInPath(path="/mnt/data:/home/myName/data", fileName="myData" )

# using a vector of paths
rxFindFileInPath( path=c("/dir1","/dir2",/dir3/dir4"), fileName="myData" )
 ## End(Not run) 
```


