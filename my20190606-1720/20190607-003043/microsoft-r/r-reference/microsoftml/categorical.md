---
title: 'categorical function (MicrosoftML) '
description: " Categorical transform that can be performed on data before  training a model. "
keywords: (MicrosoftML), categorical, transform
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
ms.openlocfilehash: faff2d2e2aba41d30f83be479041cefea2061ee5
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="categorical-machine-learning-categorical-data-transform"></a>categorical: Machine Learning Categorical Data Transform 
 ## <a name="description"></a>Description

Categorical transform that can be performed on data before training a model.


 ## <a name="usage"></a>Usage

```   
  categorical(vars, outputKind = "ind", maxNumTerms = 1e+06, terms = "",
    ...)

```

 ## <a name="arguments"></a>Arguments



 ### `vars`
 A character vector or list of variable names to transform. If named, the names represent the names of new variables to be created. 



 ### `outputKind`
 A character string that specifies the kind of output kind.   
*   `"ind"`: Outputs an indicator vector. The input column is a vector   of categories, and the output contains one indicator vector per slot in   the input column.    
*   `"bag"`: Outputs a multi-set vector. If the input column is a  vector of categories, the output contains one vector, where the value in   each slot is the number of occurrences of the category in the input  vector. If the input column contains a single category, the indicator  vector and the bag vector are equivalent   
*   `"key"`: Outputs an index. The output is an integer ID (between 1 and the number of categories in the dictionary) of the category.   
 The default value is `"ind"`. 



 ### `maxNumTerms`
 An integer that specifies the maximum number of  categories to include in the dictionary. The default value is 1000000. 



 ### `terms`
 Optional character vector of terms or categories. 



 ### ` ...`
 Additional arguments sent to compute engine. 



 ## <a name="details"></a>Details

The `categorical` transform passes through a data set, operating on text columns, to build a dictionary of categories. For each row, the entire text string appearing in the input column is defined as a category. The output of the categorical transform is an indicator vector.
Each slot in this vector corresponds to a category in the dictionary, so its length is the size of the built dictionary. The categorical transform can be applied to one or more columns, in which case it builds a separate dictionary for each column that it is applied to.

`categorical` is not currently supported to handle factor data.


 ## <a name="value"></a>Value

A `maml` object defining the transform.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxFastTrees](rxFastTrees.md), [rxFastForest](rxFastForest.md), [rxNeuralNet](rxNeuralNet.md), [rxOneClassSvm](rxOneClassSvm.md), [rxLogisticRegression](rxLogisticRegression.md).

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


  # Use a categorical transform: the entire string is treated as a category
  outModel1 <- rxLogisticRegression(like~reviewCat, data = trainReviews, 
      mlTransforms = list(categorical(vars = c(reviewCat = "review"))))
  # Note that 'I hate it' and 'I love it' (the only strings appearing more than once)
  # have non-zero weights
  summary(outModel1)

  # Use the model to score
  scoreOutDF1 <- rxPredict(outModel1, data = testReviews, 
      extraVarsToWrite = "review")
  scoreOutDF1
```



