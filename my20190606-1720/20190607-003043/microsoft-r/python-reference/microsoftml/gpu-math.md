---
title: 'gpu_math: gpu_math'
description: NVidia CUDA implementation.
keywords: neural network, math, gpu
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
ms.openlocfilehash: 74bd0e7a6309d5119651387b363dbb843a556e08
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="microsoftmlgpumath-acceleration-with-nvidia-cuda"></a>*microsoftml.gpu_math*: Acceleration with NVidia CUDA





## <a name="usage"></a>Usage



```
microsoftml.gpu_math(gpu_id: numbers.Real = -1,
    cu_dnn: bool = False, cu_dnn_algo: str = 'ImplicitPrecompGemm')
```





## <a name="description"></a>Description

NVidia CUDA implementation.


## <a name="arguments"></a>Arguments


### <a name="gpuid"></a>gpu_id

GPU device id (settings).


### <a name="cudnn"></a>cu_dnn

Use cuDNN on GPU (settings).


### <a name="cudnnalgo"></a>cu_dnn_algo

cuDNN optimization options (settings).


## <a name="see-also"></a>See also

[`avx_math`](avx-math.md), [`clr_math`](clr-math.md), [`mkl_math`](mkl-math.md), [`sse_math`](sse-math.md)
