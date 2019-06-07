---
title: 'loss functions function (MicrosoftML) '
description: " The loss functions for classification and regression. "
keywords: (MicrosoftML), loss functions, expLoss, hingeLoss, logLoss, poissonLoss, smoothHingeLoss, squaredLoss, loss
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
ms.openlocfilehash: 45b9e31a75b8ece2d6d63f740f6ab7108f4d0f9e
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="loss-functions-classification-and-regression-loss-functions"></a>loss functions: Classification and Regression Loss functions 
 ## <a name="description"></a>Description

The loss functions for classification and regression.


 ## <a name="usage"></a>Usage

```   
  expLoss(beta = 1, ...)

  hingeLoss(margin = 1, ...)

  logLoss(...)

  smoothHingeLoss(smoothingConst = 1, ...)

  poissonLoss(...)

  squaredLoss(...)

```

 ## <a name="arguments"></a>Arguments



 ### `beta`
 Specifies the numeric value of beta (dilation). The default value  is 1. 



 ### `margin`
 Specifies the numeric margin value. The default value is 1. 



 ### `smoothingConst`
 Specifies the numeric value of the smoothing constant. The default value is 1. 



 ### ` ...`
 hidden argument. 



 ## <a name="details"></a>Details

A loss function measures the discrepancy between the prediction of a machine learning algorithm and the supervised output and represents the cost of being wrong. 

The classification loss functions supported are:


* 
 `logLoss` 

* 
 `expLoss` 

* 
 `hingeLoss` 

* 
 `smoothHingeLoss`


The regression loss functions supported are:


* 
 `poissonLoss` 

* 
 `squaredLoss`.




 ## <a name="value"></a>Value

A character string defining the loss function.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxFastLinear](rxFastLinear.md), [rxNeuralNet](rxNeuralNet.md)

 ## <a name="examples"></a>Examples

 ```

  train <- function(lossFunction) {

      result <- rxFastLinear(isCase ~ age + parity + education + spontaneous + induced,
                    transforms = list(isCase = case == 1), lossFunction = lossFunction,
                    data = infert,
                    type = "binary")
      coef(result)[["age"]]
  }

  age <- list()
  age$LogLoss <- train(logLoss())
  age$LogLossHinge <- train(hingeLoss())
  age$LogLossSmoothHinge <- train(smoothHingeLoss())
  age
```



