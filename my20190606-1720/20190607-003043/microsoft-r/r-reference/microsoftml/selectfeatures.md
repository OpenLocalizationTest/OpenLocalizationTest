---
title: 'selectFeatures function (MicrosoftML) '
description: " The feature selection transform selects features from the specified variables using the specified mode. "
keywords: (MicrosoftML), selectFeatures, feature, selection, transform
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
ms.openlocfilehash: 3429bf8a3eb795e6300058ba96e6456748d97f3d
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="selectfeatures-machine-learning-feature-selection-transform"></a>selectFeatures: Machine Learning Feature Selection Transform 
 ## <a name="description"></a>Description

The feature selection transform selects features from the specified variables using the specified mode.


 ## <a name="usage"></a>Usage

```   
  selectFeatures(vars, mode, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `vars`
 A formula or a vector/list of strings specifying the name of variables upon which the feature selection is performed, if the mode is  minCount(). For example, `~ var1 + var2 + var3`. If mode is mutualInformation(), a formula or a named list of strings describing the dependent variable and the independent variables. For example, `label ~ ``var1 + var2 + var3`. 



 ### `mode`
 Specifies the mode of feature selection. This can be either  [minCount](minCount.md) or [mutualInformation](mutualInformation.md). 



 ### ` ...`
 Additional arguments to be passed directly to the Microsoft Compute Engine. 



 ## <a name="details"></a>Details

The feature selection transform selects features from the specified variables using one of the two modes: count or mutual information. For more information, see [minCount](minCount.md) and [mutualInformation](mutualInformation.md).


 ## <a name="value"></a>Value

A `maml` object defining the transform.

 ## <a name="see-also"></a>See Also

[minCount](minCount.md) [mutualInformation](mutualInformation.md)

 ## <a name="examples"></a>Examples

 ```

  trainReviews <- data.frame(review = c( 
          "This is great",
          "I hate it",
          "Love it",
          "Do not like it",
          "Really like it",
          "I hate it",
          "I like it a lot",
          "I kind of hate it",
          "I do like it",
          "I really hate it",
          "It is very good",
          "I hate it a bunch",
          "I love it a bunch",
          "I hate it",
          "I like it very much",
          "I hate it very much.",
          "I really do love it",
          "I really do hate it",
          "Love it!",
          "Hate it!",
          "I love it",
          "I hate it",
          "I love it",
          "I hate it",
          "I love it"),
       like = c(TRUE, FALSE, TRUE, FALSE, TRUE,
          FALSE, TRUE, FALSE, TRUE, FALSE, TRUE, FALSE, TRUE,
          FALSE, TRUE, FALSE, TRUE, FALSE, TRUE, FALSE, TRUE, 
          FALSE, TRUE, FALSE, TRUE), stringsAsFactors = FALSE
      )

      testReviews <- data.frame(review = c(
          "This is great",
          "I hate it",
          "Love it",
          "Really like it",
          "I hate it",
          "I like it a lot",
          "I love it",
          "I do like it",
          "I really hate it",
          "I love it"), stringsAsFactors = FALSE)

  # Use a categorical hash transform which generated 128 features.
  outModel1 <- rxLogisticRegression(like~reviewCatHash, data = trainReviews, l1Weight = 0, 
      mlTransforms = list(categoricalHash(vars = c(reviewCatHash = "review"), hashBits = 7)))
  summary(outModel1)

  # Apply a categorical hash transform and a count feature selection transform
  # which selects only those hash slots that has value.
  outModel2 <- rxLogisticRegression(like~reviewCatHash, data = trainReviews, l1Weight = 0, 
      mlTransforms = list(
    categoricalHash(vars = c(reviewCatHash = "review"), hashBits = 7), 
    selectFeatures("reviewCatHash", mode = minCount())))
  summary(outModel2)

  # Apply a categorical hash transform and a mutual information feature selection transform
  # which selects only 10 features with largest mutual information with the label.
  outModel3 <- rxLogisticRegression(like~reviewCatHash, data = trainReviews, l1Weight = 0, 
      mlTransforms = list(
    categoricalHash(vars = c(reviewCatHash = "review"), hashBits = 7), 
    selectFeatures(like ~ reviewCatHash, mode = mutualInformation(numFeaturesToKeep = 10))))
  summary(outModel3)
```





