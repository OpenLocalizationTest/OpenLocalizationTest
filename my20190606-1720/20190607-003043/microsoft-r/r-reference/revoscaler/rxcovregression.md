---
title: rxCovCoef function (revoAnalytics) | Microsoft Docs
description: " Obtain covariance and correlation matrices for the coefficient estimates within rxLinMod,  rxLogit, and rxGlm objects and explanatory variables within rxLinMod and rxLogit objects. "
keywords: (revoAnalytics), rxCovCoef, rxCovCoef.rxLinMod, rxCovCoef.rxLogit, rxCovCoef.rxGlm, rxCorCoef, rxCorCoef.rxLinMod, rxCorCoef.rxLogit, rxCorCoef.rxGlm, rxCovData, rxCovData.rxLinMod, rxCovData.rxLogit, rxCorData, rxCorData.rxLinMod, rxCorData.rxLogit, models, regression
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
ms.openlocfilehash: c57b8673cccc2dc90841fb9d5fe5e6bbe9c6794a
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxcovcoef-covariance-and-correlation-matrices-for-linear-model-coefficients-and-explanatory-variables"></a>rxCovCoef: Covariance and Correlation Matrices for Linear Model Coefficients and Explanatory Variables 
 ## <a name="description"></a>Description

Obtain covariance and correlation matrices for the coefficient estimates within `rxLinMod`, `rxLogit`, and `rxGlm` objects and explanatory variables within `rxLinMod` and `rxLogit` objects.


 ## <a name="usage"></a>Usage

```   
  rxCovCoef(x)
  rxCorCoef(x)
  rxCovData(x)
  rxCorData(x)

```

 ## <a name="arguments"></a>Arguments



 ### `x`
 object of class `rxLinMod`, `rxLogit`, or `rxGlm` that  satisfies conditions in the Details section. 



 ## <a name="details"></a>Details

For `rxCovCoef` and `rxCorCoef`, the rxLinMod, rxLogit, or rxGlm object must have been fit with `covCoef = TRUE` and `cube = FALSE`. The degrees of freedom must be greater than 0.

For `rxCovData` and `rxCorData`, the rxLinMod or rxLogit object must have been fit with an intercept term as well as with `covData = TRUE` and `cube = FALSE`.


 ## <a name="value"></a>Value

If `p` is the number of columns in the model matrix, then

For `rxCovCoef` a `p x p` numeric matrix containing the covariances of the model coefficients.

For `rxCorCoef` a `p x p` numeric matrix containing the correlations amongst the model coefficients.

For `rxCovData` a `(p - 1) x (p - 1)` numeric matrix containing the covariances of the non-intercept terms in the model matrix.

For `rxCorData` a `(p - 1) x (p - 1)` numeric matrix containing the correlations amongst the non-intercept terms in the model matrix.

 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxLinMod](rxLinMod.md), [rxLogit](rxLogit.md), [rxCovCor](rxCovCor.md).

 ## <a name="examples"></a>Examples

 ```

  ## Example 1
  # Get the covariance matrix of the estimated model coefficients
  kyphXdfFileName <- file.path(rxGetOption("sampleDataDir"), "kyphosis.xdf")
  kyphLogitWithCovCoef <-
    rxLogit(Kyphosis ~ Age + Number + Start, data = kyphXdfFileName,
            covCoef = TRUE, reportProgress = 0)
  rxCovCoef(kyphLogitWithCovCoef)

  # Compare results with results from stats::glm function
  data(kyphosis, package = "rpart")
  kyphGlmSummary <-
    summary(glm(Kyphosis ~ Age + Number + Start, data = kyphosis,
                family = binomial()))
  kyphGlmSummary[["cov.scaled"]]


  ## Example 2
  # Get the covariance matrix of the data
  kyphXdfFileName <- file.path(rxGetOption("sampleDataDir"), "kyphosis.xdf")
  kyphLogitWithCovData <-
    rxLogit(Kyphosis ~ Age + Number + Start, data = kyphXdfFileName,
            covData = TRUE, reportProgress = 0)
  rxCovData(kyphLogitWithCovData)

  # Compare results with stats::cov function
  cov(kyphosis[2:4])


  ## Example 3
  # Find the correlation matrices for both the coefficient estimates and the
  # explanatory variables
  rxCorCoef(kyphLogitWithCovCoef)
  rxCorData(kyphLogitWithCovData)
```



