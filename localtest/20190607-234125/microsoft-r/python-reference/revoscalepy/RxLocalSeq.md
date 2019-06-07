---
title: 'RxLocalSeq: Generate local compute context (revoscalepy)'
description: Creates a local compute context object. Computations using rx_exec will be processed sequentially. This is the default compute context.
keywords: context, local
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
ms.openlocfilehash: 153326df4808ee7e406171d2770d7c92b08331b5
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxlocalseq"></a>RxLocalSeq


 



```
revoscalepy.RxLocalSeq
```





## <a name="description"></a>Description

Creates a local compute context object. Computations using rx_exec will be processed sequentially. This is the default compute context.


## <a name="returns"></a>Returns

Object of class `RxLocalSeq`.


## <a name="see-also"></a>See also

`RxComputeContext`, [`RxInSqlServer`](RxInSqlServer.md), [`rx_get_compute_context`](rx-get-compute-context.md), [`rx_set_compute_context`](rx-set-compute-context.md).


## <a name="example"></a>Example



```
from revoscalepy import RxLocalSeq
localcc = RxLocalSeq()
```

