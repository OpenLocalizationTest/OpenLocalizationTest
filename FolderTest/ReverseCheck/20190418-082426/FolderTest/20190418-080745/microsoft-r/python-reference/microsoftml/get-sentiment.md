---
title: 'get_sentiment: Machine Learning Sentiment Analyzer Transform'
description: Scores natural language text and assesses the probability the sentiments are positive.
keywords: transform, text, sentiment, nlp
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
ms.openlocfilehash: 4089503beb4c8bcd070a3eedd97b508e4d015396
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="microsoftmlgetsentiment-sentiment-analysis"></a>*microsoftml.get_sentiment*: Sentiment analysis





## <a name="usage"></a>Usage



```
microsoftml.get_sentiment(cols: [str, dict, list], **kargs)
```





## <a name="description"></a>Description

Scores natural language text and assesses the probability the sentiments are positive.


## <a name="details"></a>Details

The `get_sentiment` transform returns the probability that the sentiment of a natural text is positive. Currently supports only the English language.


## <a name="arguments"></a>Arguments


### <a name="cols"></a>cols

A character string or list of variable names to transform. If `dict`, the names represent the names of new variables to be created.


### <a name="kargs"></a>kargs

Additional arguments sent to compute engine.


## <a name="returns"></a>Returns

An object defining the transform.


## <a name="see-also"></a>See also

[`featurize_text`](featurize-text.md).


## <a name="example"></a>Example



```
'''
Example with get_sentiment and rx_logistic_regression.
'''
import numpy
import pandas
from microsoftml import rx_logistic_regression, rx_featurize, rx_predict, get_sentiment

# Create the data
customer_reviews = pandas.DataFrame(data=dict(review=[
            "I really did not like the taste of it",
            "It was surprisingly quite good!",
            "I will never ever ever go to that place again!!"]))
            
# Get the sentiment scores
sentiment_scores = rx_featurize(
    data=customer_reviews,
    ml_transforms=[get_sentiment(cols=dict(scores="review"))])
    
# Let's translate the score to something more meaningful
sentiment_scores["eval"] = sentiment_scores.scores.apply(
            lambda score: "AWESOMENESS" if score > 0.6 else "BLAH")
print(sentiment_scores)
```


Output:



```
Beginning processing data.
Rows Read: 3, Read Time: 0, Transform Time: 0
Beginning processing data.
Elapsed time: 00:00:02.4327924
Finished writing 3 rows.
Writing completed.
                                            review    scores         eval
0            I really did not like the taste of it  0.461790         BLAH
1                  It was surprisingly quite good!  0.960192  AWESOMENESS
2  I will never ever ever go to that place again!!  0.310344         BLAH
```

