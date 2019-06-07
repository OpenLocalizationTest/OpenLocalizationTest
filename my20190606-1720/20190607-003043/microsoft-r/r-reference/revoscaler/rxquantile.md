---
title: rxQuantile function (revoAnalytics) | Microsoft Docs
description: " Quickly computes approximate quantiles (without sorting) "
keywords: (revoAnalytics), rxQuantile, univar
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
ms.openlocfilehash: 63e2f6b1b254b0adabc6708c902ae7c5a39d36a7
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxquantile--approximate-quantiles-for-xdf-files-and-data-frames"></a>rxQuantile:  Approximate Quantiles for .xdf Files and Data Frames  
 ## <a name="description"></a>Description

Quickly computes approximate quantiles (without sorting)


 ## <a name="usage"></a>Usage

```   
  rxQuantile(varName, data, pweights = NULL, fweights = NULL,
      probs = seq(0, 1, 0.25), names = TRUE,
      maxIntegerBins = 500000, multiple = NA, 
      numericBins = FALSE, numNumericBreaks = 1000,
      blocksPerRead = rxGetOption("blocksPerRead"),
      reportProgress = rxGetOption("reportProgress"), verbose = 0) 

```


 ## <a name="arguments"></a>Arguments



 ### `varName`
  A character string containing the name of the numeric variable for which to compute the quantiles.  


 ### `data`
  data frame, character string containing an .xdf file name (with path), or  [RxDataSource-class](RxDataSource-class.md) object representing the data set.  



 ### `pweights`
  character string specifying the variable to use as probability weights for the observations.  



 ### `fweights`
  character string specifying the variable to use as frequency weights for the observations.  



 ### `probs`
  numeric vector of probabilities with values in the [0,1] range.  


 ### `names`
  logical; if `TRUE`, the result has a `names` attribute.   



 ### `maxIntegerBins`
  integer. The maximum number of integer bins to use for integer data.  For exact results, this should be larger than the range of data.   However, larger values may increase memory requirements and computational time.  


 ### `multiple`
  numeric value to multiply data values by before computing integer bins.  


 ### `numericBins`
  logical. If `TRUE`, do not use integer approximations for bins.  



 ### `numNumericBreaks`
  integer.  The number of breaks to use in computing numeric bins. Ignored if `numericBins` is `FALSE`.  



 ### `blocksPerRead`
  number of blocks to read for each chunk of data read from an `.xdf` data source.  



 ### `reportProgress`
  integer value with options:  
*   `0`: no progress is reported. 
*   `1`: the number of processed rows is printed and updated. 
*   `2`: rows processed and timings are reported. 
*   `3`: rows processed and all timings are reported. 




 ### `verbose`
 integer value. If `0`, no additional output is printed.  If `1`, additional computational information may be printed.            




 ## <a name="details"></a>Details

rxQuantiles computes approximate quantiles by counting binned data, then computing a linear interpolation of the empirical cdf for continuous data or the inverse of empirical distribution function for integer data.  
If the binned data are integers, or can be converted to integers by multiplication, the computation is exact when integral bins are used.
The size of the bins can be controlled by using the `multiple` function if desired.

Missing values are removed before computing the quantiles.


 ## <a name="value"></a>Value

A vector the length of `probs` is returned; if `names = TRUE`, it has a names attribute. 

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)




 ## <a name="see-also"></a>See Also

quantile, [rxCube](rxCube.md).

 ## <a name="examples"></a>Examples

 ```

  # Estimate a GLM model and compute quantiles for the predictions
  claimsXdf <- file.path(rxGetOption("sampleDataDir"),"claims.xdf")
  claimsPred <- tempfile(pattern = "claimsPred", fileext = ".xdf")

  claimsGlm <- rxGlm(cost ~ age + car.age + type, family = Gamma,
                dropFirst = TRUE, data = claimsXdf)

  rxPredict(claimsGlm, data = claimsXdf, outData = claimsPred,
    writeModelVars = TRUE, overwrite = TRUE)

  predBreaks <- rxQuantile(data = claimsPred, varName = "cost_Pred",
    probs = seq(from = 0, to = 1, by = .1))

  predBreaks

  # Compare with the quantile function
  claimsPredDF <- rxDataStep(inData = claimsPred)
  quantile(claimsPredDF$cost_Pred, probs = seq(0, 1, by = .1), type = 4)

  file.remove(claimsPred)
```



