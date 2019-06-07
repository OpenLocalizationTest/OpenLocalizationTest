---
title: 'getSentiment function (MicrosoftML) '
description: " Scores natual language text and creates a column that  contains probabilities that the sentiments in the text are positive. "
keywords: (MicrosoftML), getSentiment, nlp, sentiment, text, transform
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
ms.openlocfilehash: 32d99022b5e72fe870e4381c49ff433d2024fcfb
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="getsentiment-machine-learning-sentiment-analyzer-transform"></a>getSentiment: Machine Learning Sentiment Analyzer Transform 
 ## <a name="description"></a>Description

Scores natural language text and creates a column that contains probabilities that the sentiments in the text are positive.


 ## <a name="usage"></a>Usage

```   
  getSentiment(vars, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `vars`
 A character vector or list of variable names to transform. If named, the names represent the names of new variables to be created. 



 ### ` ...`
 Additional arguments sent to compute engine. 



 ## <a name="details"></a>Details

The `getSentiment` transform returns the probability that the sentiment of a natural text is positive. Currently supports  
only the English language.


 ## <a name="value"></a>Value

A `maml` object defining the transform.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxFastTrees](rxFastTrees.md), [rxFastForest](rxFastForest.md), [rxNeuralNet](rxNeuralNet.md), [rxOneClassSvm](rxOneClassSvm.md), [rxLogisticRegression](rxLogisticRegression.md), [rxFastLinear](rxFastLinear.md).

 ## <a name="examples"></a>Examples

 ```

  # Create the data
  CustomerReviews <- data.frame(Review = c(
    "I really did not like the taste of it",
    "It was surprisingly quite good!",
    "I will never ever ever go to that place again!!"),
    stringsAsFactors = FALSE)

  # Get the sentiment scores
  sentimentScores <- rxFeaturize(data = CustomerReviews, 
                                 mlTransforms = getSentiment(vars = list(SentimentScore = "Review")))

  # Let's translate the score to something more meaningful
  sentimentScores$PredictedRating <- ifelse(sentimentScores$SentimentScore > 0.6, 
                                            "AWESOMENESS", "BLAH")

  # Let's look at the results
  sentimentScores
```






