---
title: 'categoricalHash function (MicrosoftML) '
description: " Categorical hash transform that can be performed on data before  training a model. "
keywords: (MicrosoftML), categoricalHash, transform
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
ms.openlocfilehash: 1af80923fa909b621dceab1ab41caefd5ca4b019
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="categoricalhash-machine-learning-categorical-hashdata-transform"></a>categoricalHash: Machine Learning Categorical HashData Transform 
 ## <a name="description"></a>Description

Categorical hash transform that can be performed on data before training a model.


 ## <a name="usage"></a>Usage

```   
  categoricalHash(vars, hashBits = 16, seed = 314489979, ordered = TRUE,
    invertHash = 0, outputKind = "Bag", ...)

```

 ## <a name="arguments"></a>Arguments



 ### `vars`
 A character vector or list of variable names to transform. If named, the names represent the names of new variables to be created. 



 ### `hashBits`
 An integer specifying the number of bits to hash into.  Must be between 1 and 30, inclusive. The default value is 16. 



 ### `seed`
 An integer specifying the hashing seed. The default value is 314489979. 



 ### `ordered`
 `TRUE` to include the position of each term in the  hash. Otherwise, `FALSE`. The default value is `TRUE`. 



 ### `invertHash`
 An integer specifying the limit on the number of keys  that can be used to generate the slot name. `0` means no invert  hashing; `-1` means no limit. While a zero value gives better  performance, a non-zero value is needed to get meaningful coefficient names. The default value is `0`. 



 ### `outputKind`
 A character string that specifies the kind of output kind.   
*   `"ind"`: Outputs an indicator vector. The input column is a vector   of categories, and the output contains one indicator vector per slot in   the input column.    
*   `"bag"`: Outputs a multi-set vector. If the input column is a  vector of categories, the output contains one vector, where the value in   each slot is the number of occurrences of the category in the input  vector. If the input column contains a single category, the indicator  vector and the bag vector are equivalent   
*   `"key"`: Outputs an index. The output is an integer ID (between 1 and the number of categories in the dictionary) of the category.   
 The default value is `"Bag"`. 



 ### ` ...`
 Additional arguments sent to the compute engine. 



 ## <a name="details"></a>Details

`categoricalHash` converts a categorical value into an indicator array by hashing the value and using the hash as an index in the bag.  If the input column is a vector, a single indicator bag is returned for it.

`categoricalHash` does not currently support handling factor data.


 ## <a name="value"></a>Value

a `maml` object defining the transform.

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


  # Use a categorical hash transform
  outModel2 <- rxLogisticRegression(like~reviewCatHash, data = trainReviews, 
      mlTransforms = list(categoricalHash(vars = c(reviewCatHash = "review"))))
  # Weights are similar to categorical
  summary(outModel2)

  # Use the model to score
  scoreOutDF2 <- rxPredict(outModel2, data = testReviews, 
      extraVarsToWrite = "review")
  scoreOutDF2
```



