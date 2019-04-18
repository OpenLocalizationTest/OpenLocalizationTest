---
title: 'kernel function (MicrosoftML) '
description: " Kernels supported for use in computing inner products. "
keywords: (MicrosoftML), kernel, linearKernel, maKernel, polynomialKernel, rbfKernel, sigmoidKernel
author: heidisteen
manager: cgronlun
ms.date: 01/16/2019
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
ms.openlocfilehash: 5225ef09a07c97b719973df37d8b4287abe28858
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="kernel-kernel"></a>kernel: Kernel 
 ## <a name="description"></a>Description

Kernels supported for use in computing inner products.


 ## <a name="usage"></a>Usage

```   
  linearKernel(...)

  polynomialKernel(a = NULL, bias = 0, deg = 3, ...)

  rbfKernel(gamma = NULL, ...)

  sigmoidKernel(gamma = NULL, coef0 = 0, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `a`
 The numeric value for a in the term (a*<x,y> + b)^d. If not specified, `(1/(number of features)` is used. 



 ### `bias`
 The numeric value for b in the term `(a*<x,y> + b)^d`. 



 ### `deg`
 The integer value for d in the term `(a*<x,y> + b)^d`. 



 ### `gamma`
 The numeric value for gamma in the expression `tanh(gamma*<x,y> + c`). If not specified, `1/(number of features)` is used. 



 ### `coef0`
 The numeric value for c in the expression `tanh(gamma*<x,y> + c`). 



 ### ` ...`
 Additional arguments passed to the Microsoft ML compute engine. 



 ## <a name="details"></a>Details

These helper functions specify the kernel that is used for training in relevant algorithms. The kernals that are suppored: 


* 
 `linearKernel`: linear kernel.

* 
 `rbfKernel`: radial basis function kernel. 

* 
 `polynomialKernel`: polynomial kernel. 

* 
 `sigmoidKernel`: sigmoid kernel. 




 ## <a name="value"></a>Value

A character string defining the kernel.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="references"></a>References

[`  Estimating the Support of a High-Dimensional Distribution`](http://research.microsoft.com/pubs/69731/tr-99-87.pdf)


[`  New Support Vector Algorithms`](http://www.stat.purdue.edu/~yuzhu/stat598m3/Papers/NewSVM.pdf)



 ## <a name="see-also"></a>See Also

[rxOneClassSvm](rxOneClassSvm.md)

 ## <a name="examples"></a>Examples

 ```

  # Simulate some simple data
  set.seed(7)
  numRows <- 200
  normalData <- data.frame(day = 1:numRows)
  normalData$pageViews = runif(numRows, min = 10, max = 1000) + .5 * normalData$day
  testData <- data.frame(day = 1:numRows)
  # The test data has outliers above 1000
  testData$pageViews = runif(numRows, min = 10, max = 1400) + .5 * testData$day

  train <- function(kernelFunction, args=NULL) {
      model <- rxOneClassSvm(formula = ~pageViews + day, data = normalData,
      kernel = kernelFunction(args))
      scores <- rxPredict(model, data = testData, writeModelVars = TRUE)
      scores$groups = scores$Score > 0
      scores
  }
  display <- function(scores) {
      print(sum(scores$groups))
      rxLinePlot(pageViews ~ day, data = scores, groups = groups, type = "p",
       symbolColors = c("red", "blue"))
  }
  scores <- list()
  scores$rbfKernel <- train(rbfKernel)
  scores$linearKernel <- train(linearKernel)
  scores$polynomialKernel <- train(polynomialKernel, (a = .2))
  scores$sigmoidKernel <- train(sigmoidKernel)
  display(scores$rbfKernel)
  display(scores$linearKernel)
  display(scores$polynomialKernel)
  display(scores$sigmoidKernel)
```



