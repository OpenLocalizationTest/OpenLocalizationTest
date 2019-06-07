---
title: rxMarginals function (revoAnalytics) | Microsoft Docs
description: " Obtain marginal statistics on rxCrossTabs contingency tables. "
keywords: (revoAnalytics), rxMarginals, rxMarginals.rxCrossTabs, category, models
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
ms.openlocfilehash: 56eecaaa4cbfdf441443dc113eca2b369edb2954
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxmarginals-marginal-table-statistics"></a>rxMarginals: Marginal Table Statistics 
 ## <a name="description"></a>Description

Obtain marginal statistics on `rxCrossTabs` contingency tables.


 ## <a name="usage"></a>Usage

```   
 ## S3 method for class `rxCrossTabs':
rxMarginals  (x, output = "sums", ...)

```

 ## <a name="arguments"></a>Arguments



 ### `x`
 object of class rxCrossTabs. 



 ### `output`
 character string specifying the type of output to display.  Choices are `"sums"`, `"counts"` and `"means"`. 



 ### ` ...`
 additional arguments to be passed directly to the underlying print method for the output list object. 



 ## <a name="details"></a>Details

Developed primarily as a method to access marginal statistics from [rxCrossTabs](rxCrossTabs.md) generated cross-tabulations.


 ## <a name="value"></a>Value

list for each contingency table stored in an rxCrossTabs object. Each element of the list contains a list of the marginal means (row, column, and grand) if `output` is `"means"` or marginal sums otherwise.

 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxCrossTabs](rxCrossTabs.md)

 ## <a name="examples"></a>Examples

 ```

  admissions <- as.data.frame(UCBAdmissions)
  rxMarginals(rxCrossTabs(Freq ~ Gender : Admit, data = admissions, margin = TRUE,
                          means = FALSE))
  rxMarginals(rxCrossTabs(Freq ~ Gender : Admit, data = admissions, margin = TRUE,
                          means = TRUE))
```



