---
title: rxPairwiseCrossTab function (revoAnalytics) | Microsoft Docs
description: " Apply a function 'FUN' to all pairwise combinations of the rows and columns of an xtabs object,  stratifying by higher dimensions. "
keywords: (revoAnalytics), rxPairwiseCrossTab, print.rxPairwiseCrossTabList, print.rxPairwiseCrossTabTable, htest
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
ms.openlocfilehash: ba42a3fd41166eb7eb5e67ddfa4847d798272c35
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxpairwisecrosstab--apply-function-to-pairwise-combinations-of-an-xtabs-object"></a>rxPairwiseCrossTab:  Apply Function to Pairwise Combinations of an xtabs Object 

 ## <a name="description"></a>Description

Apply a function 'FUN' to all pairwise combinations of the rows and columns of an xtabs object, stratifying by higher dimensions.



 ## <a name="usage"></a>Usage

```   
  rxPairwiseCrossTab(x, pooled = TRUE, FUN = rxRiskRatio, ...)
 ## S3 method for class `rxPairwiseCrossTabList':
print  (x, ...)
 ## S3 method for class `rxPairwiseCrossTabTable':
print  (x, digits = 3, scientific = FALSE, p.value.digits = 3, ...)

```


 ## <a name="arguments"></a>Arguments




 ### `x`
 an object of class xtabs, rxCrossTabs, or rxCube for `rxPairwiseCrossTab`. An object of class rxPairwiseCrossTabList or rxPairwiseCrossTabTable for the print methods of rxPairwiseCrossTabList and rxPairwiseCrossTabTable objects. 



 ### `pooled`
 logical value. If `TRUE`, the comparison groups are pooled.  Otherwise all pairwise comparisons are included. 



 ### `FUN`
 function that takes a two by two table and returns an object of class htest. 



 ### ` ...`
 additional arguments. 



 ### `digits`
 number of digits to use in printing numeric values. 



 ### `scientific`
 logical value. If `TRUE`, scientific notation is used to prin tnumeric values. 



 ### `p.value.digits`
 number of digits to use in printing p-values. 




 ## <a name="value"></a>Value
 a rxPairwiseCrossTabList object. 

 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxChiSquaredTest](rxChiSquaredTest.md), [rxFisherTest](rxChiSquaredTest.md), [rxKendallCor](rxChiSquaredTest.md), [rxMultiTest](rxMultiTest.md), [rxRiskRatio](rxRiskRatio.md), [rxOddsRatio](rxRiskRatio.md).


 ## <a name="examples"></a>Examples

 ```

  mtcarsDF <- rxFactors(datasets::mtcars, factorInfo = c("gear", "cyl", "vs"), 
                        varsToKeep = c("gear", "cyl", "vs"), sortLevels = TRUE)
  xtabObj <- rxCrossTabs(~ gear : cyl : vs, data = mtcarsDF, returnXtabs = TRUE)

  rxPairwiseCrossTab(xtabObj, FUN = rxRiskRatio)
  rxPairwiseCrossTab(xtabObj, pooled = FALSE, FUN = rxOddsRatio)
```



