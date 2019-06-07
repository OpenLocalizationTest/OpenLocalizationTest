---
title: 'n_gram_hash: n_gram_hash'
description: Extracts NGrams from text and convert them to vector using hashing trick.
keywords: N-Grams, hash
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
ms.openlocfilehash: aa49d59695371457b4fbd133316af271937160d6
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="microsoftmlngramhash-converts-text-into-features-using-hashed-n-grams"></a>*microsoftml.n_gram_hash*: Converts text into features using hashed n-grams





## <a name="usage"></a>Usage



```
microsoftml.n_gram_hash(hash_bits: numbers.Real = 16,
    ngram_length: numbers.Real = 1, skip_length: numbers.Real = 0,
    all_lengths: bool = True, seed: numbers.Real = 314489979,
    ordered: bool = True, invert_hash: numbers.Real = 0)
```





## <a name="description"></a>Description

Extracts NGrams from text and convert them to vector using hashing trick.


## <a name="arguments"></a>Arguments


### <a name="hashbits"></a>hash_bits

Number of bits to hash into. Must be between 1 and 30, inclusive. (settings).


### <a name="ngramlength"></a>ngram_length

Ngram length (settings).


### <a name="skiplength"></a>skip_length

Maximum number of tokens to skip when constructing an ngram (settings).


### <a name="alllengths"></a>all_lengths

Whether to include all ngram lengths up to ngramLength or only ngramLength (settings).


### <a name="seed"></a>seed

Hashing seed (settings).


### <a name="ordered"></a>ordered

Whether the position of each source column should be included in the hash (when there are multiple source columns). (settings).


### <a name="inverthash"></a>invert_hash

Limit the number of keys used to generate the slot name to this many. 0 means no invert hashing, -1 means no limit. (settings).


## <a name="see-also"></a>See also

[n_gram](n-gram.md), [featurize_text](featurize-text.md)
