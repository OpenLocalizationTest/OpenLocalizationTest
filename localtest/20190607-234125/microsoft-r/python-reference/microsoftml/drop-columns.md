---
title: 'drop_columns: Drops columns from the dataset'
description: Specified columns to drop from the dataset.
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
ms.openlocfilehash: 7596e8454e3d8ca60af7edb78884c812631cd03e
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="microsoftmldropcolumns-drops-columns-from-a-dataset"></a>*microsoftml.drop_columns*: Drops columns from a dataset





## <a name="usage"></a>Usage



```
microsoftml.drop_columns(cols: [list, str], **kargs)
```





## <a name="description"></a>Description

Specified columns to drop from the dataset.


## <a name="arguments"></a>Arguments


### <a name="cols"></a>cols

A character string or list of the names of the variables to drop.


### <a name="kargs"></a>kargs

Additional arguments sent to compute engine.


## <a name="returns"></a>Returns

An object defining the transform.


## <a name="see-also"></a>See also

[`concat`](concat.md), [`select_columns`](select-columns.md).
