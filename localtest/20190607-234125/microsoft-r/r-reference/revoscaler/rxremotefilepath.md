---
title: rxRemoteFilePath function (revoAnalytics) | Microsoft Docs
description: This is a utility function to automatically build a path according to file path rules of the remote compute context platform.
keywords: (revoAnalytics), rxRemoteFilePath, IO
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
ms.openlocfilehash: 65652e5b04016d9e6c628c52f2b45bcc2a95b045
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxremotefilepath-merge-path-using-the-remote-platforms-separator"></a>rxRemoteFilePath: Merge path using the remote platform's separator. 
 ## <a name="description"></a>Description
 This is a utility function to automatically build a path according to file path rules of the remote compute context platform. 

 ## <a name="usage"></a>Usage

```   rxRemoteFilePath(  ...  , computeContext) 
```

 ##Arguments



 ### ` ...`
 character strings containing parts of the path to be merged. 


 ### `computeContext`
 An [RxComputeContext](RxComputeContext.md) context object specifying the platform information. 



 ##Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ##See Also

[RxComputeContext](RxComputeContext.md),
RxHadoopMR,
[RxSpark](RxSpark.md).

 ##Examples
 ```

  ## <a name="not-run"></a>Not run:

  # <a name="myhadoopcc-is-an-rxhadoopmr-compute-context"></a>myHadoopCC is an RxHadoopMR compute context
   myFilePath <- rxRemoteFilePath("/var/RevoShare", "testDir", myHadoopCC)
 ## <a name="endnot-run"></a>End(Not run) 


```



