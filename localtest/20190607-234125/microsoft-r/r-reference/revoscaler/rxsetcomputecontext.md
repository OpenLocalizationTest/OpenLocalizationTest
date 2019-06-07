---
title: rxSetComputeContext function (revoAnalytics) | Microsoft Docs
description: " Get or set the active compute context for RevoScaleR computations "
keywords: (revoAnalytics), rxSetComputeContext, rxGetComputeContext, IO
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
ms.openlocfilehash: 7b991f3e3295490dc2e4cf7639212205fa5e6333
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxsetcomputecontext-get-and-set-the-compute-context"></a>rxSetComputeContext: Get and Set the compute context 
 ## <a name="description"></a>Description

Get or set the active compute context for RevoScaleR computations


 ## <a name="usage"></a>Usage

```   

  rxSetComputeContext(computeContext, ...) 

  rxGetComputeContext() 

```

 ## <a name="arguments"></a>Arguments



 ### `computeContext`
 character string specifying class name or description of the specific  class to instantiate, or an existing `RxComputeContext` object.  Choices include: `"RxLocalSeq"` or `"local"`, `"RxLocalParallel"` or `"localpar"`,  `"RxSpark"` or `"spark"`,  `"RxHadoopMR"` or `"hadoopmr"`,    and `"RxForeachDoPar"` or `"dopar"`. 



 ### ` ...`
 any other arguments are passed to the class generator determined from `computeContext`. 




 ## <a name="value"></a>Value

`rxSetComputeContext` returns the previously active compute context invisibly.
`rxGetComputeContext` returns the active compute context.



 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[RxComputeContext](RxComputeContext.md), [rxOptions](rxOptions.md), [rxGetOption](rxOptions.md)
[rxExec](rxExec.md).

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

origComputeContext <- rxSetComputeContext("localpar")
x <- 1:10
rxExec(print, x, elemType = "cores", timesToRun = 10)
rxSetComputeContext( origComputeContext )
 ## End(Not run) 
```



