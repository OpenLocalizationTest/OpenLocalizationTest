---
title: as.lm function (revoAnalytics) | Microsoft Docs
description: " Converts objects containing linear model results to an lm object. "
keywords: (revoAnalytics), as.lm, as.lm.rxLinMod, category, models
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
ms.openlocfilehash: 4ee44673cc1c63d87ba8022a7ddd9fb078272770
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="aslm-conversion-of-a-revoscaler-rxlinmod-object-to-an-lm-object"></a>as.lm: Conversion of a RevoScaleR rxLinMod object to an lm Object 
 ## <a name="description"></a>Description

Converts objects containing linear model results to an lm object.


 ## <a name="usage"></a>Usage

```   
 ## S3 method for class `rxLinMod':
as.lm  (x, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `x`
 object of class rxLinMod. 


 ### ` ...`
 additional arguments (currently not used). 




 ## <a name="details"></a>Details

This function converts an existing object of class rxLinMod an object of class lm.
The underlying structure of the output object will be a subset of that produced by an equivalent call to lm. Often, this method can be used to coerce an object for use with the **pmml** package.  **RevoScaleR** model objects that contain `transforms` or a `transformFunc` are not supported.



 ## <a name="value"></a>Value

an object of class lm.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxLinMod](rxLinMod.md), lm, [as.glm](as.glm.md), [as.kmeans](as.kmeans.md), [as.rpart](as.rpart.md), [as.xtabs](as.xtabs.md).


 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# If the pmml package is installed 
library(pmml)
rxObj <- rxLinMod(Sepal.Length ~ Sepal.Width + Petal.Length, data=iris)
pmml(as.lm(rxObj))
 ## End(Not run) 
```




