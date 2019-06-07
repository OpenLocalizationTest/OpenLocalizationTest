---
title: pow function (revoAnalytics) | Microsoft Docs
description: " Formula expression functions for **RevoScaleR**. "
keywords: (revoAnalytics), pow, models
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
ms.openlocfilehash: 2faabe244b429d9fd6a8eab0053f45c277bcbf71
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="pow-formula-expression-functions-for-revoscaler"></a>pow: Formula Expression Functions for RevoScaleR 
 ## <a name="description"></a>Description

Formula expression functions for **RevoScaleR**.


 ## <a name="usage"></a>Usage

```   
  pow(x, exponent)

```

 ## <a name="arguments"></a>Arguments



 ### `x`
 variable name 


 ### `exponent`
 number to use as an exponent 



 ## <a name="details"></a>Details

Many of the primary analysis functions in **RevoScaleR** require a formula argument. Arithmetic expressions in those arguments provide flexibility in the model. This man page lists the functions in **RevoScaleR** that are not native to R.

`pow` performs the power transformation `x^exponent`.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxFormula](rxFormula.md), [rxTransform](rxTransform.md), [rxCrossTabs](rxCrossTabs.md), [rxCube](rxCube.md), [rxLinMod](rxLinMod.md), [rxLogit](rxLogit.md), [rxSummary](rxSummary.md).

 ## <a name="examples"></a>Examples

 ```

  # define local data.frame
  admissions <- as.data.frame(UCBAdmissions)

  # cross-tabulation
  rxCrossTabs(pow(Freq, 2) ~ Gender : Admit, data = admissions)
  rxCrossTabs(Freq^2 ~ Gender : Admit, data = admissions)

  # linear modeling
  rxLinMod(pow(Freq, 2) ~ Gender + Admit, data = admissions)
  rxLinMod(Freq^2 ~ Gender + Admit, data = admissions)

  # model summarization
  rxSummary(~ pow(Freq, 2) + Gender + Admit, data = admissions)
  rxSummary(~ I(Freq^2) + Gender + Admit, data = admissions)
```


