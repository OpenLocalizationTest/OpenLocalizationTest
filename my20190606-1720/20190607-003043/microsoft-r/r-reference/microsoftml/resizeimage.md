---
title: 'resizeImage function (MicrosoftML) '
description: " Resizes an image to a specified dimension using a specified resizing method. "
keywords: (MicrosoftML), resizeImage, image, transform
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
ms.openlocfilehash: 6a5473f0e59d9ad1d552815d63d3c44a9c6ffda6
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="resizeimage-machine-learning-resize-image-transform"></a>resizeImage: Machine Learning Resize Image Transform 
 ## <a name="description"></a>Description

Resizes an image to a specified dimension using a specified resizing method.


 ## <a name="usage"></a>Usage

```   
  resizeImage(vars, width = 224, height = 224, resizingOption = "IsoCrop")

```

 ## <a name="arguments"></a>Arguments



 ### `vars`
 A named list of character vectors of input variable names and the name of the output variable. Note that the input variables must be of the same type. For one-to-one mappings between input and output variables, a named character vector can be used. 



 ### `width`
 Specifies the width of the scaled image in pixels. The default value is 224. 



 ### `height`
 Specifies the height of the scaled image in pixels. The default value is 224. 



 ### `resizingOption`
 Specified the resizing method to use. Note that all methods are using bilinear interpolation. The options are:  
*   `"IsoPad"`: The image is resized such that the aspect ratio is preserved.  If needed, the image is padded with black to fit the new width or height.  
*   `"IsoCrop"`: The image is resized such that the aspect ratio is preserved.  If needed, the image is cropped to fit the new width or height.  
*   `"Aniso"`: The image is stretched to the new width and height, without   preserving the aspect ratio. 
 The default value is `"IsoPad"`. 



 ## <a name="details"></a>Details

`resizeImage` resizes an image to the specified height and width using a specified resizing method. The input variables to this transform must be images, typically the result of the `loadImage` transform.


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




