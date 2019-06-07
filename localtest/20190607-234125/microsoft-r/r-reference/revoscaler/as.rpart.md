---
title: as.rpart function (revoAnalytics) | Microsoft Docs
description: " Converts objects containing decision tree results to an rpart object. "
keywords: (revoAnalytics), as.rpart, as.rpart.rxDTree, category, models
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
ms.openlocfilehash: 748b12f7260667ca71d02b4617798f54813ef677
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="asrpart-conversion-of-a-revoscaler-rxdtree-object-to-a-rpart-object"></a>as.rpart: Conversion of a RevoScaleR rxDTree object to a rpart Object 
 ## <a name="description"></a>Description

Converts objects containing decision tree results to a rpart object.


 ## <a name="usage"></a>Usage

```   
 ## S3 method for class `rxDTree':
as.rpart  (x, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `x`
 object of class rxDTree. 


 ### ` ...`
 additional arguments (currently not used). 




 ## <a name="details"></a>Details

This function converts an existing object of class rxDTree an object of class `rpart`.
The underlying structure of the output object will be a subset of that produced by an equivalent call to `rpart`. Often, this method can be used to coerce an object for use with the **pmml** package.  **RevoScaleR** model objects that contain `transforms` or a `transformFunc` are not supported.



 ## <a name="value"></a>Value

an object of class rpart.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxDTree](rxDTree.md), [as.lm](as.lm.md), [as.kmeans](as.kmeans.md), [as.glm](as.glm.md), [as.xtabs](as.xtabs.md).


 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# If the pmml package is installed 
library(pmml)
infert.nrow <- nrow(infert)
infert.sub <- sample(infert.nrow, infert.nrow / 2)
infert.dtree <- rxDTree(case ~ age + parity + education + spontaneous + induced, 
    data = infert[infert.sub, ], cp = 0.01)
infert.dtree
pmml(as.rpart(infert.dtree))
 ## End(Not run) 
```




