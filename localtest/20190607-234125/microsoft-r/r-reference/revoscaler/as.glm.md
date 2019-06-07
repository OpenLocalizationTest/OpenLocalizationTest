---
title: as.glm function (revoAnalytics) | Microsoft Docs
description: " Converts objects containing generalized linear model results to a glm object. "
keywords: (revoAnalytics), as.glm, as.glm.rxLogit, as.glm.rxGlm
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
ms.openlocfilehash: 8bb7eef61daa057c2b2122935831a6743a7444ae
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="asglm-conversion-of-a-revoscaler-rxlogit-or-rxglm-object-to-a-glm-object"></a>as.glm: Conversion of a RevoScaleR rxLogit or rxGlm object to a glm Object 
 ## <a name="description"></a>Description

Converts objects containing generalized linear model results to a glm object.


 ## <a name="usage"></a>Usage

```   
 ## S3 method for class `rxLogit':
as.glm  (x, ...)
 ## S3 method for class `rxGlm':
as.glm  (x, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `x`
 object of class rxLogit or rxGlm. 


 ### ` ...`
 additional arguments (currently not used). 




 ## <a name="details"></a>Details

This function converts an existing object of class [rxLogit](rxLogit.md) or [rxGlm](rxGLM.md) to an object of class glm.
The underlying structure of the output object will be a subset of that produced by an equivalent call to glm. Often, this method can be used to coerce an object for use with the **pmml** package. **RevoScaleR** model objects that contain `transforms` or a `transformFunc` are not supported.



 ## <a name="value"></a>Value

an object of class lm.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxLogit](rxLogit.md), [rxGlm](rxGLM.md), glm, [as.lm](as.lm.md), [as.kmeans](as.kmeans.md), [as.rpart](as.rpart.md), [as.xtabs](as.xtabs.md).


 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# If the pmml package is installed 
library(pmml)
form <- case ~ age + parity + spontaneous + induced
rxObj <- rxLogit(form, data=infert, reportProgress = 0)
pmml(as.glm(rxObj))
 ## End(Not run) 
```

