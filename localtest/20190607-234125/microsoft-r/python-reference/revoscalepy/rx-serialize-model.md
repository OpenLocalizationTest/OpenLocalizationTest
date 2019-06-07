---
title: 'rx_serialize_model: Serialize a python model (revoscalepy)'
description: Serialize the given python model.
keywords: serialization
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
ms.openlocfilehash: e9f3328406b528904b97330a48f94e254a4573fc
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxserializemodel"></a>rx_serialize_model


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_serialize_model(model, realtime_scoring_only=False) -> bytes
```





## <a name="description"></a>Description

Serialize the given python model.


## <a name="arguments"></a>Arguments


### <a name="model"></a>model

Supported models are “rx_logit”, “rx_lin_mod”, “rx_dtree”, “rx_btrees”, “rx_dforest” and MicrosoftML models.


### <a name="realtimescoringonly"></a>realtime_scoring_only

Boolean flag indicating if model serialization is for real-time only.
Default to False


## <a name="returns"></a>Returns

Bytes of the serialized model.


## <a name="example"></a>Example



```
import os
from revoscalepy import RxOptions, RxXdfData, rx_serialize_model, rx_lin_mod
sample_data_path = RxOptions.get_option("sampleDataDir")
ds = RxXdfData(os.path.join(sample_data_path, "AirlineDemoSmall.xdf"))
linmod = rx_lin_mod("ArrDelay~DayOfWeek", ds)
s_linmod = rx_serialize_model(linmod, realtime_scoring_only = False)
```

