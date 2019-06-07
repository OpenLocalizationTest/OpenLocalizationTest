---
title: RxLocalParallel-class class (revoAnalytics) | Microsoft Docs
description: "   Class for the RevoScaleR Local Parallel Compute Context.   "
keywords: (revoAnalytics), RxLocalParallel-class, show,RxLocalParallel-method, classes
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
ms.openlocfilehash: 0370730d96774e20fec66cddad854a124d16a3df
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxlocalparallel-class-class-rxlocalparallel"></a>RxLocalParallel-class: Class RxLocalParallel 
 ## <a name="description"></a>Description

Class for the RevoScaleR Local Parallel Compute Context.  


 ## <a name="generators"></a>Generators 


The targeted generator [RxLocalParallel](RxLocalParallel.md) as well as the general generator [RxComputeContext](RxComputeContext.md).

 ## <a name="extends"></a>Extends 


Class RxComputeContext, directly.

 ## <a name="methods"></a>Methods 




### `show`
`signature(object = "RxLocalParallel")`: ...




 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

RxHadoopMR, [RxSpark](RxSpark.md), [RxInSqlServer](RxInSqlServer.md), [RxLocalSeq](RxLocalSeq.md).

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

myComputeContext <- RxComputeContext("RxLocalParallel")
is(myComputeContext, "RxComputeContext")
# [1] TRUE
is(myComputeContext, "RxLocalParallel")
# [1] TRUE
 ## End(Not run) 
```


