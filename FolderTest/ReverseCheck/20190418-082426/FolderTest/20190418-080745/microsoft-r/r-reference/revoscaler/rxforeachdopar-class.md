---
title: RxForeachDoPar-class class (revoAnalytics) | Microsoft Docs
description: "   Class for the RevoScaleR Compute Context using one of the foreach dopar back ends.   "
keywords: (revoAnalytics), RxForeachDoPar-class, show,RxForeachDoPar-method, classes
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
ms.openlocfilehash: 4301273571140307599db4f0578b535c14aca9c2
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxforeachdopar-class-class-rxforeachdopar"></a>RxForeachDoPar-class: Class RxForeachDoPar 
 ## <a name="description"></a>Description

Class for the RevoScaleR Compute Context using one of the foreach dopar back ends.  


 ## <a name="generators"></a>Generators 


The targeted generator [RxForeachDoPar](RxForeachDoPar.md) as well as the general generator [RxComputeContext](RxComputeContext.md).

 ## <a name="extends"></a>Extends 


Class RxComputeContext, directly.

 ## <a name="methods"></a>Methods 




### `show`
`signature(object = "RxForeachDoPar")`: ...




 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[RxComputeContext](RxComputeContext.md), [RxLocalSeq](RxLocalSeq.md), [RxLocalParallel](RxLocalParallel.md), [RxSpark](RxSpark.md), RxHadoopMR.


 ## <a name="examples"></a>Examples

 ```

  ## Not run:

myComputeContext <- RxComputeContext("RxForeachDoPar")
is(myComputeContext, "RxComputeContext")
# [1] TRUE
is(myComputeContext, "RxForeachDoPar")
# [1] TRUE
 ## End(Not run) 
```


