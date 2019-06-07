---
title: rxRiskRatio function (revoAnalytics) | Microsoft Docs
description: " Calculate the relative risk and odds ratio on a two-by-two table. "
keywords: (revoAnalytics), rxRiskRatio, rxOddsRatio, htest
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
ms.openlocfilehash: 274686b23f1fff3a61f3dfce440cc5bf1757d0d9
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxriskratio--relative-risk-ratio-and-odds-ratio"></a>rxRiskRatio:  Relative Risk Ratio and Odds Ratio  

 ## <a name="description"></a>Description

Calculate the relative risk and odds ratio on a two-by-two table.



 ## <a name="usage"></a>Usage

```   
  rxRiskRatio(tbl, conf.level = 0.95, alternative = "two.sided")
  rxOddsRatio(tbl, conf.level = 0.95, alternative = "two.sided")

```


 ## <a name="arguments"></a>Arguments



 ### `tbl`
 two-by-two table. 


 ### `conf.level`
 level of the confidence interval. 


 ### `alternative`
 character string defining alternative hypothesis. Supported values are `"two.sided"`, `"less"`, or `"greater"`. 




 ## <a name="value"></a>Value

an object of class htest.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxChiSquaredTest](rxChiSquaredTest.md), [rxFisherTest](rxChiSquaredTest.md), [rxKendallCor](rxChiSquaredTest.md), [rxMultiTest](rxMultiTest.md), [rxPairwiseCrossTab](rxPairwiseCrosstab.md)


 ## <a name="examples"></a>Examples

 ```

  mtcarsDF <- rxFactors(datasets::mtcars, factorInfo = c("gear", "cyl", "vs"), 
                        varsToKeep = c("gear", "cyl", "vs"), sortLevels = TRUE)
  gearVsXtabs <- rxCrossTabs(~ gear : vs, data = mtcarsDF, returnXtabs = TRUE)
  rxRiskRatio(gearVsXtabs[1:2,])
  rxOddsRatio(gearVsXtabs[1:2,])
```



