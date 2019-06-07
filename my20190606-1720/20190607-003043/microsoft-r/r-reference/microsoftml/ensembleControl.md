---
title: 'ensembleControl function (MicrosoftML) '
description: " Control the parameters used to create an ensemble. "
keywords: (MicrosoftML), ensembleControl
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
ms.openlocfilehash: 6858207d14b0ecd52c8774f2a73bf8d39dde3347
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="ensemblecontrol-ensemblecontrol"></a>ensembleControl: ensembleControl 
 ## <a name="description"></a>Description
 
Control the parameters used to create an ensemble.
 
 
 ## <a name="usage"></a>Usage

```   
  ensembleControl(randomSeed = NULL, modelCount = 1, replace = FALSE,
    sampRate = ifelse(replace, 1, 0.632), splitData = FALSE,
    combineMethod = NULL, ...)
 
```
 
 ## <a name="arguments"></a>Arguments

   
  
 ### `randomSeed`
 Specifies the random seed. The default value is `NULL`. 
  
  
  
 ### `modelCount`
 Specifies the number of models to train. The default value is `1`, meaning no ensembling occurs. 
  
  
  
 ### `replace`
 A logical value specifying if the sampling of observations should be done with  or without replacement. The default value is `FALSE`. 
  
  
  
 ### `sampRate`
 a scalar of positive value specifying the percentage of observations to sample for  each trainer. The default is 1.0 for sampling with replacement (i.e., replace=TRUE) and 0.632  for sampling without replacement (i.e., replace=FALSE). 
  
  
  
 ### `splitData`
 A logical value that specifies whether or not to train the base models  on non-overlapping partitions. The default is `FALSE`.  It is available only for `RxSpark` compute context and is ignored for others. 
  
  
  
 ### `combineMethod`
 Specifies the method used to combine the models:   
*   `median` to compute the median of the individual model outputs,   
*   `average` to compute the average of the individual model outputs and   
*   `vote` to compute (pos-neg) / the total number of models, where 'pos' is the number of positive outputs  and 'neg' is the number of negative outputs. 
 The default value is `median`. 
  
  
  
 ### ` ...`
 Not used currently. 
  
 
 
 ## <a name="value"></a>Value
 
A list of ensemble parameters.
 
 
