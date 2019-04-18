---
title: rxDTreeBestCp function (revoAnalytics) | Microsoft Docs
description: " Attempts to find the cp for optimal model pruning, where optimal is defined by default in terms of the 1 Standard Error criterion of Breiman, et al. "
keywords: (revoAnalytics), rxDTreeBestCp, models, tree, classif, regression
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
ms.openlocfilehash: 4650479640720bf484e17d0240b8be6828b9b19e
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxdtreebestcp--find-the-best-value-of-cp-for-pruning-rxdtree-object"></a>rxDTreeBestCp:  Find the Best Value of cp for Pruning rxDTree Object  
 ## <a name="description"></a>Description

Attempts to find the cp for optimal model pruning, where optimal is defined by default in terms of the 1 Standard Error criterion of Breiman, et al.


 ## <a name="usage"></a>Usage

```   
  rxDTreeBestCp(x, nstd = 1L)

```


 ## <a name="arguments"></a>Arguments



 ### `x`
  an object of class `rxDTree`.  


 ### `nstd`
  number of standard errors of cross-validation error to define optimality.  The default, 1, causes `rxDTreeBestCp` to find the simplest model within one standard error of the minimum cross-validation error.  



 ## <a name="details"></a>Details

The `rxDTreeBestCp` function is intended to help automate the `rxDTree` model fitting function, by applying the 1 Standard Error Criterion of Breiman, et al., to a fitted `rxDTree` object. Using the `pruneCp="auto"` option in `rxDTree` causes `rxDTreeBestCp` to be called on the fitted model and the result of that computation supplied as the argument to `prune.rxDTree`, thus allowing the model to be fitted and pruned in a single call.


 ## <a name="value"></a>Value

a numeric scalar.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="references"></a>References

Breiman, L., Friedman, J. H., Olshen, R. A. and Stone, C. J. (1984) *Classification and Regression Trees*.
Wadsworth.


 ## <a name="see-also"></a>See Also

[rxDTree](rxDTree.md), [prune.rxDTree](prune.rxDTree.md).

 ## <a name="examples"></a>Examples

 ```

  claimsXdf <- file.path(rxGetOption("sampleDataDir"),"claims.xdf")
  claims.dtree <- rxDTree(cost ~ age + car.age + type,
    data = claimsXdf)
  claimsCp <- rxDTreeBestCp(claims.dtree)
  claims.dtree1 <- prune.rxDTree(claims.dtree, cp=claimsCp)
  claims.dtree2 <- rxDTree(cost ~ age + car.age + type, 
      data = claimsXdf, pruneCp="auto")
  ## claims.dtree1 and claims.dtree2 should differ only in their 
  ## "call" component
  claims.dtree1[[3]] <- claims.dtree2[[3]] <- NULL
  all.equal(claims.dtree1, claims.dtree2)
```







