---
title: as.gbm function (revoAnalytics) | Microsoft Docs
description: " Converts objects containing decision tree results to an gbm object. "
keywords: (revoAnalytics), as.gbm, as.gbm.rxBTrees, as.gbm.rxDTree, as.gbm.rpart, category, models
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
ms.openlocfilehash: 53e1aad60f5ff9336f0b06c1fe91a69a55b16539
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="asgbm-conversion-of-an-rxbtrees-rxdtree-or-rpart-object-to-a-gbm-object"></a>as.gbm: Conversion of an rxBTrees, rxDTree, or rpart object to a gbm Object 
 ## <a name="description"></a>Description

Converts objects containing decision tree results to a gbm object.


 ## <a name="usage"></a>Usage

```   
 ## S3 method for class `rxBTrees':
as.gbm  (x, ...)
 ## S3 method for class `rxDTree':
as.gbm  (x, ...)
 ## S3 method for class `rpart':
as.gbm  (x, use.weight = TRUE, cat.start = 0L, shrinkage = 1.0, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `x`
  object of class rxBTrees, rxDTree, or rpart. 


 ### `use.weight`
  a logical value (default being `TRUE`) specifying if the majority splitting direction  at a node should be decided based on the sum of case weights or the number of observations when the split variable at the node is a factor or ordered factor  but a certain level is not present (or not defined for the factor). 


 ### `cat.start`
  an integer specifying the starting position to add the categorical splits from the current tree  in the list of all the categorical splits in the collection of trees. 


 ### `shrinkage`
  numeric scalar specifying the learning rate of the boosting procedure for the current tree. 


 ### ` ...`
 additional arguments to be passed directly to `as.gbm.rpart`. 




 ## <a name="details"></a>Details

These functions convert an existing object of class rxBTrees, rxDTree, or rpart to an object of class `gbm`, respectively.
The underlying structure of the output object will be a subset of that produced by an equivalent call to `gbm`. Often, this method can be used to coerce an object for use with the **pmml** package.
**RevoScaleR** model objects that contain `transforms` or a `transformFunc` are not supported.



 ## <a name="value"></a>Value

an object of class gbm.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxBTrees](rxBTrees.md), [rxDTree](rxDTree.md), rpart, gbm, [as.rpart](as.rpart.md).


 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# If the pmml and the gbm packages are installed 
library(pmml)
library(gbm)

mydata <- infert
form <- case ~ age + parity + education + spontaneous + induced
ntree <- 2

fit.btrees <- rxBTrees(form, data = mydata, nTree = ntree, 
    lossFunction = "gaussian", learningRate = 0.1)
fit.btrees
fit.btrees.gbm <- as.gbm(fit.btrees)
predict(fit.btrees.gbm, newdata = mydata, n.trees = ntree)
pmml(fit.btrees.gbm)

fit.gbm <- gbm(form, data = mydata, n.trees = ntree,
    distribution = "gaussian", shrinkage = 0.1)
fit.gbm
predict(fit.gbm, newdata = mydata, n.trees = ntree)
pmml(fit.gbm)
 ## End(Not run) 
```




