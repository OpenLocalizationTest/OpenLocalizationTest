---
title: 'RxSparkData: Base class generator for Spark data (revoscalepy)'
description: Base class for all revoscalepy Spark data sources, including RxHiveData, RxOrcData, RxParquetData and RxSparkDataFrame. It is intended to be called from those subclasses instead of directly.
keywords: ''
author: HeidiSteen
manager: cgronlun
ms.date: 01/26/2018
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
ms.openlocfilehash: cfd5fbae6610db351c4f5e5ef5ad3d785f905d41
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxsparkdata"></a>RxSparkData


 



```
revoscalepy.RxSparkData(column_info: dict = None,
    df_source: str = None, df_type: str = None,
    write_factors_as_indexes: bool = False, **kwargs)
```





## <a name="description"></a>Description

Base class for all revoscalepy Spark data sources, including RxHiveData, RxOrcData, RxParquetData and RxSparkDataFrame.
It is intended to be called from those subclasses instead of directly.
