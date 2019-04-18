---
title: RxNativeFileSystem function (revoAnalytics) | Microsoft Docs
description: " This is the main generator for RxNativeFileSystem S3 class. "
keywords: (revoAnalytics), RxNativeFileSystem, file, connection
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
ms.openlocfilehash: 90dd56cf4d91037a31511fd3594294713fecc663
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxnativefilesystem-revoscaler-native-file-system-object-generator"></a>RxNativeFileSystem: RevoScaleR Native File System Object Generator 
 ## <a name="description"></a>Description

This is the main generator for RxNativeFileSystem S3 class.


 ## <a name="usage"></a>Usage

```   
    RxNativeFileSystem()

```


 ## <a name="value"></a>Value

An RxNativeFileSystem file system object. This object may be used in [rxSetFileSystem](rxSetFileSystem.md), [rxOptions](rxOptions.md), [RxTextData](RxTextData.md), or [RxXdfData](RxXdfData.md) to set the file system.

 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[RxFileSystem](RxFileSystem.md), [RxHdfsFileSystem](RxHdfsFileSystem.md), [rxSetFileSystem](rxSetFileSystem.md), [rxOptions](rxOptions.md), [RxXdfData](RxXdfData.md), [RxTextData](RxTextData.md).

 ## <a name="examples"></a>Examples

 ```

  # Setup to run analyses to use HDFS file system, then native
  ## Not run:

myHdfsFileSystem <- RxHdfsFileSystem(hostName = "myHost", port = 8020)
rxSetFileSystem(fileSystem = myHdfsFileSystem )
# Perform other tasks
# Reset to native file system
rxSetFileSystem(fileSystem = RxNativeFileSystem())
 ## End(Not run) 
```



