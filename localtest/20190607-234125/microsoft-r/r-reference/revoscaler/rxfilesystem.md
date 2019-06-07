---
title: RxFileSystem function (revoAnalytics) | Microsoft Docs
description: " This is the main generator for RxFileSystem S3 classes. "
keywords: (revoAnalytics), RxFileSystem, print.RxFileSystem, file, connection
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
ms.openlocfilehash: 9484a3be198482155c97c2eb8861ce6bafc12ca3
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxfilesystem-revoscaler-file-system-object-generator"></a>RxFileSystem: RevoScaleR File System object generator 
 ## <a name="description"></a>Description

This is the main generator for RxFileSystem S3 classes.


 ## <a name="usage"></a>Usage

```   
    RxFileSystem( fileSystem, ...)

     ## S3 method for class `RxFileSystem':
print  ( x, ... )

```

 ## <a name="arguments"></a>Arguments



 ### `fileSystem`
 character string specifying class name or file system type  existing `RxFileSystem` object.  Choices include: "RxNativeFileSystem" or "native", or "RxHdfsFileSystem" or "hdfs". Optional arguments `hostName` and `port` may be specified for HDFS file systems.  


 ### `x`
 an RxFileSystem object.  


 ### ` ...`
 other arguments are passed to the underlying function.  



 ## <a name="details"></a>Details

This is a wrapper to specific generator functions for the RevoScaleR file system classes. For example, the RxHdfsFileSystem class uses function [RxHdfsFileSystem](RxHdfsFileSystem.md) as a generator. Therefore either `RxHdfsFileSystem()` or `RxFileSystem("hdfs")` will create an RxHdfsFileSystem object.


 ## <a name="value"></a>Value

A type of RxFileSystem file system object. This object may be used in [rxSetFileSystem](rxSetFileSystem.md), [rxOptions](rxOptions.md), [RxTextData](RxTextData.md), or [RxXdfData](RxXdfData.md) to set the file system.

 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[RxNativeFileSystem](RxNativeFileSystem.md), [RxHdfsFileSystem](RxHdfsFileSystem.md), [rxSetFileSystem](rxSetFileSystem.md), [rxOptions](rxOptions.md), [RxXdfData](RxXdfData.md), [RxTextData](RxTextData.md).

 ## <a name="examples"></a>Examples

 ```

  # Setup to run analyses to use HDFS file system
  ## Not run:

# Example 1
myHdfsFileSystem1 <- RxFileSystem(fileSystem = "hdfs")
rxSetFileSystem(fileSystem = myHdfsFileSystem1 )

# Example 2
myHdfsFileSystem2 <- RxFileSystem(fileSystem = "hdfs", hostName = "myHost", port = 8020)
rxSetFileSystem(fileSystem = myHdfsFileSystem2 )
 ## End(Not run) 
```



