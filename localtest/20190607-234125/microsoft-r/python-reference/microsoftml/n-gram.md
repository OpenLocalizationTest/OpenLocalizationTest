---
title: 'n_gram: n_gram'
description: Extracts NGrams from text and convert them to vector using dictionary.
keywords: N-Grams
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
ms.openlocfilehash: 8b03bc2bc9687f49c16e95d55cf8b3a8333f7de7
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="microsoftmlngram-converts-text-into-features-using-n-grams"></a>*microsoftml.n_gram*: Converts text into features using n-grams





## <a name="usage"></a>Usage



```
microsoftml.n_gram(ngram_length: numbers.Real = 1,
    skip_length: numbers.Real = 0, all_lengths: bool = True,
    max_num_terms: list = [10000000], weighting: str = 'Tf')
```





## <a name="description"></a>Description

Extracts NGrams from text and convert them to vector using dictionary.


## <a name="arguments"></a>Arguments


### <a name="ngramlength"></a>ngram_length

Ngram length (settings).


### <a name="skiplength"></a>skip_length

Maximum number of tokens to skip when constructing an ngram (settings).


### <a name="alllengths"></a>all_lengths

Whether to include all ngram lengths up to NgramLength or only NgramLength (settings).


### <a name="maxnumterms"></a>max_num_terms

Maximum number of ngrams to store in the dictionary (settings).


### <a name="weighting"></a>weighting

The weighting criteria (settings).


## <a name="see-also"></a>See also

[n_gram_hash](n-gram-hash.md), [featurize_text](featurize-text.md)
