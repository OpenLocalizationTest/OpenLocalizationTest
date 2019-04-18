---
title: as.kmeans function (revoAnalytics) | Microsoft Docs
description: " Converts objects containing RevoScaleR-computed k-means clusters to an R kmeans object. "
keywords: (revoAnalytics), as.kmeans, as.kmeans.rxKmeans, category, models
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
ms.openlocfilehash: 86b8872977812d8a5f8e3743033d51e902ee886d
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="askmeans-conversion-of-a-revoscaler-rxkmeans-object-to-a-kmeans-object"></a>as.kmeans: Conversion of a RevoScaleR rxKmeans object to a kmeans Object 
 ## <a name="description"></a>Description

Converts objects containing RevoScaleR-computed k-means clusters to an R kmeans object.


 ## <a name="usage"></a>Usage

```   
 ## S3 method for class `rxKmeans':
as.kmeans  (x, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `x`
 object of class `"rxKmeans"`. 


 ### ` ...`
 additional arguments (currently not used). 




 ## <a name="details"></a>Details

This function converts an existing object of class `"rxKmeans"` an object of class `"kmeans"`.
The underlying structure of the output object will be a subset of that produced by an equivalent call to `kmeans`. Often, this method can be used to coerce an object for use with the **pmml** package. **RevoScaleR** model objects that contain `transforms` or a `transformFunc` are not supported.



 ## <a name="value"></a>Value

an object of class `"kmeans"`.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[as.lm](as.lm.md), [as.glm](as.glm.md), [as.rpart](as.rpart.md), [as.xtabs](as.xtabs.md), [rxKmeans](rxKmeans.md).


 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# If the pmml package is installed 
library(pmml)
form <- ~ height + weight
set.seed(17)
irow <- unique(sample.int(nrow(women), 4L, replace = TRUE))[seq(2)]
centers <- women[irow,, drop = FALSE]
rxKmeansObj <- rxKmeans(form, data = women, centers = centers)
pmml(as.kmeans(rxKmeansObj))
 ## End(Not run) 
```




