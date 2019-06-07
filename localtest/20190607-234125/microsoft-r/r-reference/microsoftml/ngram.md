---
title: 'ngram function (MicrosoftML) '
description: " Feature Extractors that can be used with mtText. "
keywords: (MicrosoftML), ngram, ngramCount, ngramHash, transform
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
ms.openlocfilehash: eaf13cfb94fc78cdf749a5e94ac23683a50eb262
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="ngram-machine-learning-feature-extractors"></a>ngram: Machine Learning Feature Extractors 
 ## <a name="description"></a>Description

Feature Extractors that can be used with mtText.


 ## <a name="usage"></a>Usage

```   
  ngramCount(ngramLength = 1, skipLength = 0, maxNumTerms = 1e+07,
    weighting = "tf")

  ngramHash(ngramLength = 1, skipLength = 0, hashBits = 16,
    seed = 314489979, ordered = TRUE, invertHash = 0)

```

 ## <a name="arguments"></a>Arguments



 ### `ngramLength`
 An integer that specifies the maximum number of tokens to take when constructing an n-gram. The default value is 1. 



 ### `skipLength`
 An integer that specifies the maximum number of tokens to skip when constructing an n-gram. If the value specified as skip length is `k`, then n-grams can contain up to k skips (not necessarily consecutive). For example, if `k=2`, then the 3-grams extracted from the text "the sky is blue today" are: "the sky is", "the sky blue", "the sky today", "the is blue", "the is today" and "the blue today". The default  value is 0. 



 ### `maxNumTerms`
 An integer that specifies the maximum number of categories  to include in the dictionary. The default value is 10000000. 



 ### `weighting`
 A character string that specifies the weighting criteria:  
*   `"tf"`: to use term frequency.    
*   `"idf"`: to use inverse document frequency.   
*   `"tfidf"`: to use both term frequency and inverse document   frequency.   




 ### `hashBits`
 integer value. Number of bits to hash into. Must be between 1 and 30, inclusive. 



 ### `seed`
 integer value. Hashing seed. 



 ### `ordered`
 `TRUE` to include the position of each term in the  hash. Otherwise, `FALSE`. The default value is `TRUE`. 



 ### `invertHash`
 An integer specifying the limit on the number of keys  that can be used to generate the slot name. `0` means no invert  hashing; `-1` means no limit. While a zero value gives better  performance, a non-zero value is needed to get meaningful coefficient names. 



 ## <a name="details"></a>Details

`ngramCount` allows defining arguments for count-based feature extraction. It accepts following options: `ngramLength`, `skipLength`, `maxNumTerms` and `weighting`.

`ngramHash` allows defining arguments for hashing-based feature extraction.  It accepts the following options: `ngramLength`, `skipLength`, `hashBits`, `seed`, `ordered` and `invertHash`.


 ## <a name="value"></a>Value

A character string defining the transform.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[featurizeText](featurizeText.md).

 ## <a name="examples"></a>Examples

 ```

   myData <- data.frame(opinion = c(
      "I love it!",
      "I love it!",
      "Love it!",
      "I love it a lot!",
      "Really love it!",
      "I hate it",
      "I hate it",
      "I hate it.",
      "Hate it",
      "Hate"),
      like = rep(c(TRUE, FALSE), each = 5),
      stringsAsFactors = FALSE)

  outModel1 <- rxLogisticRegression(like~opinionCount, data = myData, 
      mlTransforms = list(featurizeText(vars = c(opinionCount = "opinion"), 
          wordFeatureExtractor = ngramHash(invertHash = -1, hashBits = 3)))) 
  summary(outModel1)   

  outModel2 <- rxLogisticRegression(like~opinionCount, data = myData, 
      mlTransforms = list(featurizeText(vars = c(opinionCount = "opinion"), 
          wordFeatureExtractor = ngramCount(maxNumTerms = 5, weighting = "tf"))))         
  summary(outModel2)
```



