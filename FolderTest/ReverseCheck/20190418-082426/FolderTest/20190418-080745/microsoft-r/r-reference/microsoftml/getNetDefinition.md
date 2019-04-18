---
title: 'getNetDefinition function (MicrosoftML) '
description: " Returns the Net# definition from a trained neural network model. "
keywords: (MicrosoftML), getNetDefinition, transform
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
ms.openlocfilehash: 29ee2846e14973b9aa269d9bbcdac78fd120bd75
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="getnetdefinition-get-the-net-definition-from-a-trained-neural-network-model"></a>getNetDefinition: Get the Net# definition from a trained neural network model 
 ## <a name="description"></a>Description

Returns the Net# definition from a trained neural network model.


 ## <a name="usage"></a>Usage

```   
  getNetDefinition(model, getWeights = TRUE)

```

 ## <a name="arguments"></a>Arguments



 ### `model`
 The previously trained neural network model. 



 ### `getWeights`
 If `TRUE`, the weights are included in the returned Net# definition. 



 ## <a name="details"></a>Details

Returns the Net# definition from a trained neural network model. It is useful for implementing a form of continued training, where the initial weights of the model are obtained from a previously trained model. Because only the weights are initialized from the trained model (but not gradients, momentum etc.), the training is not really resumed where it was left at the end of training of the first model.


 ## <a name="value"></a>Value

A character string containing the Net# definition.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="examples"></a>Examples

 ```

  # Train a neural network on the iris dataset for 10 iterations.
  model1 <- rxNeuralNet(
      formula = Species~Sepal.Length + Sepal.Width + Petal.Length + Petal.Width, 
      data = iris, 
      numHiddenNodes=10, 
      type="multi", 
      numIterations=10, 
      optimizer=adaDeltaSgd())

  # Train another neural network on the iris dataset, initializing the topology and weights
  # from the previously trained model.
  model2 <- rxNeuralNet(
      formula = Species~Sepal.Length + Sepal.Width + Petal.Length + Petal.Width, 
      data = iris, 
      netDefinition=getNetDefinition(model1), 
      type="multi", 
      numIterations=10, 
      optimizer = adaDeltaSgd())
```



