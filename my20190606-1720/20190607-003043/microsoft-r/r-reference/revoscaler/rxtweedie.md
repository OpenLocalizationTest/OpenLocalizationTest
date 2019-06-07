---
title: rxTweedie function (revoAnalytics) | Microsoft Docs
description: " Produces a dummy generalized linear model family object that can be used with rxGlm to fit  Tweedie generalized linear regression models. This does NOT produce a full family object, but gives  rxGlm enough information to call a C++ implementation that fits a Tweedie model. The excellent  R package **tweedie** by Gordon Smyth does provide a full Tweedie family object, and that can also be  used with rxGlm. "
keywords: (revoAnalytics), rxTweedie, regression
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
ms.openlocfilehash: bcba3df689503f7e1510c9f0f2c30621c836887f
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxtweedie-tweedie-generalized-linear-models"></a>rxTweedie: Tweedie Generalized Linear Models 
 ## <a name="description"></a>Description

Produces a dummy generalized linear model family object that can be used with `rxGlm` to fit Tweedie generalized linear regression models. This does NOT produce a full family object, but gives `rxGlm` enough information to call a C++ implementation that fits a Tweedie model. The excellent R package **tweedie** by Gordon Smyth does provide a full Tweedie family object, and that can also be used with `rxGlm`.


 ## <a name="usage"></a>Usage

```   
  rxTweedie(var.power = 0, link.power = 1 - var.power)

```

 ## <a name="arguments"></a>Arguments



 ### `var.power`
 index of power variance function. 


 ### `link.power`
 index of power link function. Setting `link.power` to `0`  produces a `log` link function. Setting it to `1` is the identity link.  The default is a canonical link  equal to `1 - var.power` 




 ## <a name="details"></a>Details

This provides a way to specify the var.power and the link.power arguments to the Tweedie distribution for `rxGlm`.



 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="references"></a>References

Peter K Dunn (2011). tweedie: Tweedie exponential family models. R package version 2.1.1.  



 ## <a name="see-also"></a>See Also

[rxGlm](rxGLM.md)


 ## <a name="examples"></a>Examples

 ```

  # In the claims data, the cost is set to NA if no claim was made
  # Convert NA to 0 for the cost, and read data into a data frame

  claimsXdf <- file.path(rxGetOption("sampleDataDir"),"claims.xdf")
  claims <- rxDataStep(inData = claimsXdf, 
             transforms = list(cost = ifelse(is.na(cost), 0, cost)))

  # Estimate using a Tweedie family                           
  claimsTweedie <- rxGlm(cost ~ age + car.age + type , 
      data=claims, family = rxTweedie(var.power = 1.5)) 
  summary(claimsTweedie)

  # Re-estimate using a Tweedie family setting link.power to 0,
  # resulting in a log link function                          
  claimsTweedie <- rxGlm(cost ~ age + car.age + type , 
      data=claims, family = rxTweedie(var.power = 1.5, link.power = 0)) 
  summary(claimsTweedie)
```



