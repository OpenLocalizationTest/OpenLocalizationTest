---
title: RxComputeContext-class class (revoAnalytics) | Microsoft Docs
description: "   Base class for all RevoScaleR Compute Contexts.   "
keywords: (revoAnalytics), RxComputeContext-class, show,RxComputeContext-method, classes
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
ms.openlocfilehash: dd855c6818d71ae829679a51fbdec06a504766d4
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxcomputecontext-class-class-rxcomputecontext"></a>RxComputeContext-class: Class RxComputeContext 
 ## <a name="description"></a>Description

Base class for all RevoScaleR Compute Contexts.  


 ## <a name="objects-from-the-class"></a>Objects from the Class 


A virtual class: No objects may be created from it.

 ## <a name="generator"></a>Generator 


The generator for classes that extend RxComputeContext is [RxComputeContext](RxComputeContext.md).  


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)
 
 
 ##<a name="see-also"></a>See Also
 
[RxHadoopMR](RevoScaleR-deprecated.md), [RxSpark](RxSpark.md), [RxInSqlServer](RxInSqlServer.md), [RxLocalSeq](RxLocalSeq.md), [RxLocalParallel](RxLocalParallel.md), [RxForeachDoPar](RxForeachDoPar.md).

 ## <a name="examples"></a>Examples

 ```

  myComputeContext <- RxComputeContext("local")
  is(myComputeContext, "RxComputeContext")
  # [1] TRUE
  is(myComputeContext, "RxLocalSeq")
  # [1] TRUE
```


