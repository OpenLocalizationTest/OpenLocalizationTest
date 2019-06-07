---
title: Kyphosis data (revoAnalytics) | Microsoft Docs
description: " The kyphosis data in .xdf format. "
keywords: (revoAnalytics), Kyphosis, kyphosis.xdf, datasets
author: heidisteen
manager: cgronlun
ms.date: 01/24/2018
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
ms.openlocfilehash: bf9f2f5d1d448751245d874c1c0b4641b37dd848
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="kyphosis-data-on-a-post-operative-spinal-defect"></a>Kyphosis: Data on a Post-Operative Spinal Defect 
 ## <a name="description"></a>Description

The kyphosis data in .xdf format.


 ## <a name="format"></a>Format

An .xdf file with 81 observations on 4 variables. For a complete description of the variables, see kyphosis.


 ## <a name="source"></a>Source

John M. Chambers and Trevor Hastie, Ed., (1992) *Statistical Models in S*. Belmont, CA. Wadsworth.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

kyphosis

 ## <a name="examples"></a>Examples

 ```

  Kyphosis <- rxDataStep(inData = file.path(rxGetOption("sampleDataDir"),
                        "kyphosis.xdf"))
  rxSummary(~ Kyphosis + Age + Number + Start, data = Kyphosis)
```


