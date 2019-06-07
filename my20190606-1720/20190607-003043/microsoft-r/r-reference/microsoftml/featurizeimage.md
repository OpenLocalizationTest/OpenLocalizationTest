---
title: 'featurizeImage function (MicrosoftML) '
description: " Featurizes an image using a pre-trained deep neural network model. "
keywords: (MicrosoftML), featurizeImage, alexnet, cnn, dnn, featurize, image, resnet, transform
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
ms.openlocfilehash: 98bed00746d0af55c3b8c31cc4efe8d1b20a0748
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="featurizeimage-machine-learning-image-featurization-transform"></a>featurizeImage: Machine Learning Image Featurization Transform 
 ## <a name="description"></a>Description

Featurizes an image using a pre-trained deep neural network model.


 ## <a name="usage"></a>Usage

```   
  featurizeImage(var, outVar = NULL, dnnModel = "Resnet18")

```

 ## <a name="arguments"></a>Arguments



 ### `var`
 Input variable containing extracted pixel values. 



 ### `outVar`
 The prefix of the output variables containing the image features. If null, the input variable name will be used. The default value is `NULL`. 



 ### `dnnModel`
 The pre-trained deep neural network. The possible options are:  
*   `"resnet18"` 
*   `"resnet50"` 
*   `"resnet101"` 
*   `"alexnet"`  
 The default value is `"resnet18"`. See [`Deep Residual Learning for Image Recognition`](http://www.cv-foundation.org/openaccess/content_cvpr_2016/html/He_Deep_Residual_Learning_CVPR_2016_paper.html)  for details about ResNet. 



 ## <a name="details"></a>Details

`featurizeImage` featurizes an image using the specified pre-trained deep neural network model. The input variables to this transform must be extracted pixel values.


 ## <a name="value"></a>Value

A `maml` object defining the transform.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="examples"></a>Examples

 ```

  train <- data.frame(Path = c(system.file("help/figures/RevolutionAnalyticslogo.png", package = "MicrosoftML")), Label = c(TRUE), stringsAsFactors = FALSE)

  # Loads the images from variable Path, resizes the images to 1x1 pixels and trains a neural net.
  model <- rxNeuralNet(
      Label ~ Features,
      data = train,
      mlTransforms = list(
          loadImage(vars = list(Features = "Path")),
          resizeImage(vars = "Features", width = 1, height = 1, resizing = "Aniso"),
          extractPixels(vars = "Features")
          ),
      mlTransformVars = "Path",
      numHiddenNodes = 1,
      numIterations = 1)

  # Featurizes the images from variable Path using the default model, and trains a linear model on the result.
  model <- rxFastLinear(
      Label ~ Features,
      data = train,
      mlTransforms = list(
          loadImage(vars = list(Features = "Path")),
          resizeImage(vars = "Features", width = 224, height = 224), # If dnnModel == "AlexNet", the image has to be resized to 227x227.
          extractPixels(vars = "Features"),
          featurizeImage(var = "Features")
          ),
      mlTransformVars = "Path")
```









