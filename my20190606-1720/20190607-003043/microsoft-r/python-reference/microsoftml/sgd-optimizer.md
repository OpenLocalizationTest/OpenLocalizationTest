---
title: 'sgd_optimizer: sgd_optimizer'
description: Stochastic gradient descent optimizer.
keywords: optimizer, sgd
author: HeidiSteen
manager: cgronlun
ms.date: 09/05/2017
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ROBOTS: ''
audience: ''
ms.devlang: Python
ms.reviewer: ''
ms.suite: ''
ms.tgt_pltfrm: ''
ms.custom: ''
ms.openlocfilehash: 3b4bfa65f2a9af95b20968f323962bdd49d27258
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="microsoftmlsgdoptimizer-stochastic-gradient-descent"></a>*microsoftml.sgd_optimizer*: Stochastic gradient descent





## <a name="usage"></a>Usage



```
microsoftml.sgd_optimizer(learning_rate: numbers.Real = None,
    momentum: numbers.Real = None, nag: bool = None,
    weight_decay: numbers.Real = None,
    l_rate_red_ratio: numbers.Real = None,
    l_rate_red_freq: numbers.Real = None,
    l_rate_red_error_ratio: numbers.Real = None)
```





## <a name="description"></a>Description

Stochastic gradient descent optimizer.


## <a name="arguments"></a>Arguments


### <a name="learningrate"></a>learning_rate

Learning rate (settings).


### <a name="momentum"></a>momentum

Momentum Term (settings).


### <a name="nag"></a>nag

Use Nesterov’s accelerated gradient (settings).


### <a name="weightdecay"></a>weight_decay

Weight decay (settings).


### <a name="lrateredratio"></a>l_rate_red_ratio

Learning rate reduction ratio (settings).


### <a name="lrateredfreq"></a>l_rate_red_freq

Learning rate reduction ratio (settings).


### <a name="lraterederrorratio"></a>l_rate_red_error_ratio

Relative error reduction criterion for learning rate reduction (settings).


## <a name="see-also"></a>See also

[`adadelta_optimizer`](adadelta-optimizer.md)
