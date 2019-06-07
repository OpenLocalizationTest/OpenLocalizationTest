---
title: RxLocalSeq-class class (revoAnalytics) | Microsoft Docs
description: "   Class for the RevoScaleR Local Compute Context.   "
keywords: (revoAnalytics), RxLocalSeq-class, show,RxLocalSeq-method, classes
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
ms.openlocfilehash: 4e03100aea05aa0009cd889df8c0f43454843757
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxlocalseq-class-class-rxlocalseq"></a>RxLocalSeq-class: Class RxLocalSeq 
 ## <a name="description"></a>Description

Class for the RevoScaleR Local Compute Context.  


 ## <a name="generators"></a>Generators 


The targeted generator [RxLocalSeq](RxLocalSeq.md) as well as the general generator [RxComputeContext](RxComputeContext.md).

 ## <a name="extends"></a>Extends 


Class RxComputeContext, directly.

 ## <a name="methods"></a>Methods 




### `show`
`signature(object = "RxLocalSeq")`: ...




 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[RxSpark](RxSpark.md), RxHadoopMR, [RxInSqlServer](RxInSqlServer.md), [RxLocalParallel](RxLocalParallel.md), [RxForeachDoPar](RxForeachDoPar.md), [RxComputeContext](RxComputeContext.md), [rxSetComputeContext](rxSetComputeContext.md).

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

myComputeContext <- RxComputeContext("RxLocalSeq")
is(myComputeContext, "RxComputeContext")
# [1] TRUE
is(myComputeContext, "RxLocalSeq")
# [1] TRUE
 ## End(Not run) 
```


