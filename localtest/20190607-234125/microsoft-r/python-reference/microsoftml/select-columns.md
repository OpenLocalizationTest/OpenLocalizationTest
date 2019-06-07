---
title: 'select_columns: Selects a set of columns and drops all others'
description: Selects a set of columns to retrain, dropping all others.
keywords: transform, schema
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
ms.openlocfilehash: 012ded81cd395910eb6e4a0859d60855c756fe9f
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="microsoftmlselectcolumns-retains-columns-of-a-dataset"></a>*microsoftml.select_columns*: Retains columns of a dataset





## <a name="usage"></a>Usage



```
microsoftml.select_columns(cols: [list, str], **kargs)
```





## <a name="description"></a>Description

Selects a set of columns to retrain, dropping all others.


## <a name="arguments"></a>Arguments


### <a name="cols"></a>cols

A character string or list of the names of the variables to keep.


### <a name="kargs"></a>kargs

Additional arguments sent to compute engine.


## <a name="returns"></a>Returns

An object defining the transform.


## <a name="see-also"></a>See also

[`concat`](concat.md), [`drop_columns`](drop-columns.md).
