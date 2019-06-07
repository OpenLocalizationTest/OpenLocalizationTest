---
title: 'mutualinformation_select: Machine Learning Mutual Information Mode Feature Selection Transform'
description: Selects the top k features across all specified columns ordered by their mutual information with the label column.
keywords: feature, selection, mutual, information
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
ms.openlocfilehash: 451ebe9e77bafbf6d3ef5dd100993e5a41353208
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="microsoftmlmutualinformationselect-feature-selection-based-on-mutual-information"></a>*microsoftml.mutualinformation_select*: Feature selection based on mutual information





## <a name="usage"></a>Usage



```
microsoftml.mutualinformation_select(cols: [list, str], label: str,
    num_features_to_keep: int = 1000, num_bins: int = 256, **kargs)
```





## <a name="description"></a>Description

Selects the top k features across all specified columns ordered by their mutual information with the label column.


## <a name="details"></a>Details

The mutual information of two random variables `X` and `Y` is a measure of the mutual dependence between the variables. Formally, the mutual information can be written as:

`I(X;Y) = E[log(p(x,y)) - log(p(x)) - log(p(y))]`

where the expectation is taken over the joint distribution of `X` and `Y`. Here `p(x,y)` is the joint probability density function of `X` and `Y`, `p(x)` and `p(y)` are the marginal probability density functions of `X` and `Y` respectively. In general, a higher mutual information between the dependent variable (or label) and an independent variable (or feature) means that the label has higher mutual dependence over that feature.

The mutual information feature selection mode selects the features based on the mutual information. It keeps the top `num_features_to_keep` features with the largest mutual information with the label.


## <a name="arguments"></a>Arguments


### <a name="cols"></a>cols

Specifies character string or list of the names of the variables to select.


### <a name="label"></a>label

Specifies the name of the label.


### <a name="numfeaturestokeep"></a>num_features_to_keep

If the number of features to keep is specified to be `n`, the transform picks the `n` features that have the highest mutual information with the dependent variable. The default value is 1000.


### <a name="numbins"></a>num_bins

Maximum number of bins for numerical values. Powers of 2 are recommended. The default value is 256.


### <a name="kargs"></a>kargs

Additional arguments sent to compute engine.


## <a name="returns"></a>Returns

An object defining the transform.


## <a name="see-also"></a>See also

[`count_select`](count-select.md)


## <a name="references"></a>References

[Wikipedia: Mutual Information](https://en.wikipedia.org/wiki/Mutual_information)
