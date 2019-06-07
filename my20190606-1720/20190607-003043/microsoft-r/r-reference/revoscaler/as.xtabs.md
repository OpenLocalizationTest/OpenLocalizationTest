---
title: as.xtabs function (revoAnalytics) | Microsoft Docs
description: " Converts objects containing cross tabulation results to an xtabs object. "
keywords: (revoAnalytics), as.xtabs, as.xtabs.rxCrossTabs, as.xtabs.rxCube, category, models
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
ms.openlocfilehash: eefec52e42ced204d49f065dd24ad228ebd146af
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="asxtabs-conversion-of-a-revoscaler-cross-tabulation-object-to-an-xtabs-object"></a>as.xtabs: Conversion of a RevoScaleR Cross Tabulation Object to an xtabs Object 
 ## <a name="description"></a>Description

Converts objects containing cross tabulation results to an xtabs object.


 ## <a name="usage"></a>Usage

```   
 ## S3 method for class `rxCrossTabs':
as.xtabs  (x, ...)
 ## S3 method for class `rxCube':
as.xtabs  (x, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `x`
 object of class rxCrossTabs or rxCube. 


 ### ` ...`
 additional arguments (currently not used). 




 ## <a name="details"></a>Details

This function converts an existing object of class rxCrossTabs or rxCube into an xtabs object.
The underlying structure of the output object will be the same as that produced by an equivalent call to xtabs. However, you should expect the `"call"` attribute to be different, since it is a copy of the original call stored in the rxCrossTabs or rxCube input object.
Often, this method can be used to coerce an object for use with the **pmml** package. **RevoScaleR** model objects that contain `transforms` or a `transformFunc` are not supported.



 ## <a name="value"></a>Value

an object of class xtabs.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxCrossTabs](rxCrossTabs.md), [rxCube](rxCube.md), xtabs, [as.lm](as.lm.md), [as.kmeans](as.kmeans.md), [as.rpart](as.rpart.md), [as.glm](as.glm.md).


 ## <a name="examples"></a>Examples

 ```

  # Define function to compare xtabs and as.xtabs output
  "as.xtabs.check" <- function(convertedXtabsObject, xtabsObject)
  {
      attr(convertedXtabsObject, "call") <- attr(xtabsObject, "call") <- NULL
      all.equal(convertedXtabsObject, xtabsObject)
  }

  # Create a data set
  set.seed(100)
  divs <- letters[1:5]
  glads <- c("spartacus", "crixus")
  romeDF <- data.frame( division = rep(divs, 5L), 
                        score = runif(25, min = 0, max = 10), 
                        rank = runif(25, min = 1, max = 100), 
                        gladiator = c(rep(glads[1L], 12L), rep(glads[2L], 13L)),
                        arena = sample(c("colosseum", "ludus", "market"), 25L, replace = TRUE))

  # Compare xtabs and as.xtabs(rxCrossTabs(..., returnXtabs = FALSE))  
  # results for a 3-way interaction with no dependent variables
  z1 <- rxCrossTabs(~ division : gladiator : arena, data = romeDF, returnXtabs = FALSE)
  z2 <- xtabs(~ division + gladiator + arena, romeDF)
  as.xtabs.check(as.xtabs(z1), z2) # TRUE

  # Compare xtabs and as.xtabs(rxCube(...)) results for a 3-way interaction
  # with no dependent variable
  z1 <- rxCube(~ division : gladiator : arena, data = romeDF, means = FALSE)
  z2 <- xtabs(~ division + gladiator + arena, romeDF)
  as.xtabs.check(as.xtabs(z1), z2) # TRUE
```




