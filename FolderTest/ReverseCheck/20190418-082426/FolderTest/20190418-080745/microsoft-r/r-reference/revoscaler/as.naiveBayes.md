---
title: as.naiveBayes function (revoAnalytics) | Microsoft Docs
description: " Converts RevoScaleR rxNaiveBayes objects to a (limited) e1071 naiveBayes object. "
keywords: (revoAnalytics), as.naiveBayes, as.naiveBayes.rxNaiveBayes, category, models
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
ms.openlocfilehash: f236ee90b0a427deee95eabf10fe0ef0e5e913b1
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="asnaivebayes-conversion-of-a-revoscaler-rxnaivebayes-object-to-a-e1071-naivebayes-object"></a>as.naiveBayes: Conversion of a RevoScaleR rxNaiveBayes object to a e1071 naiveBayes object 
 ## <a name="description"></a>Description

Converts RevoScaleR rxNaiveBayes objects to a (limited) e1071 naiveBayes object.


 ## <a name="usage"></a>Usage

```   
 ## S3 method for class `rxNaiveBayes':
as.naiveBayes  (x, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `x`
 object of class rxNaiveBayes. 


 ### ` ...`
 additional arguments (currently not used). 




 ## <a name="details"></a>Details

This function converts an existing object of class `rxNaiveBayes` to an object of class `naiveBayes` in the **e1071** package.
The underlying structure of the output object will be a subset of that produced by an equivalent call to `naiveBayes`. **RevoScaleR** model objects that contain `transforms` or a `transformFunc` are not supported.



 ## <a name="value"></a>Value

an object of class naiveBayes from **e1071**.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxNaiveBayes](rxNaiveBayes.md), [as.lm](as.lm.md), [as.kmeans](as.kmeans.md), [as.glm](as.glm.md), [as.gbm](as.gbm.md), [as.xtabs](as.xtabs.md).


 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# If the e1071 package is installed 
library(e1071)
rxBayes1 <- rxNaiveBayes(Kyphosis ~ Start + Age + Number + Start, data = kyphosis)
as.naiveBayes(rxBayes1)
 ## End(Not run) 
```




