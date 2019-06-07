---
title: rxMultiTest function (revoAnalytics) | Microsoft Docs
description: " Collects a list of tests for variable independence into a table. "
keywords: (revoAnalytics), rxMultiTest, print.rxMultiTest, htest
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
ms.openlocfilehash: 3ff58a08a47efd804f2806a767874a8422ed7a94
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxmultitest--multiple-variable-independence-tests"></a>rxMultiTest:  Multiple Variable Independence Tests  

 ## <a name="description"></a>Description

Collects a list of tests for variable independence into a table.



 ## <a name="usage"></a>Usage

```   
  rxMultiTest(tests, title = NULL)

 ## S3 method for class `rxMultiTest':
print  (x, ...)

```


 ## <a name="arguments"></a>Arguments



 ### `tests`
 a list of objects of class htest. 



 ### `title`
 a title for the multiTest table. If `NULL`, the title is determined from  the method slot of the htest. 



 ### `x`
 object of class rxMultiTest. 



 ### ` ...`
 additional arguments to the print method. 




 ## <a name="value"></a>Value

an object of class rxMultiTest.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxChiSquaredTest](rxChiSquaredTest.md), [rxFisherTest](rxChiSquaredTest.md), [rxKendallCor](rxChiSquaredTest.md), [rxPairwiseCrossTab](rxPairwiseCrosstab.md), [rxRiskRatio](rxRiskRatio.md), [rxOddsRatio](rxRiskRatio.md).


 ## <a name="examples"></a>Examples

 ```

  data(mtcars) 
  tests <- list(t.test(mpg ~ vs, data = mtcars),
             t.test(hp ~ vs, data = mtcars))
  rxMultiTest(tests)
```



