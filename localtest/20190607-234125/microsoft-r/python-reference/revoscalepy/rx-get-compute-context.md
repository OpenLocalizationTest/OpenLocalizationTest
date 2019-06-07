---
title: 'rx_get_compute_context: Gets the current compute context (revoscalepy)'
description: Gets the active compute context for revoscalepy computations
keywords: context
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
ms.openlocfilehash: b954d5395f2c3f56a72b4ad357bc2753875db7a3
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxgetcomputecontext"></a>rx_get_compute_context


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_get_compute_context() -> revoscalepy.computecontext.RxComputeContext.RxComputeContext
```





## <a name="description"></a>Description

Gets the active compute context for revoscalepy computations


## <a name="arguments"></a>Arguments


### <a name="computecontext"></a>compute_context

Character string specifying class name or description of the specific class to instantiate, or an existing RxComputeContext object.
Choices include: “RxLocalSeq” or “local”, “RxInSqlServer”.


## <a name="returns"></a>Returns

rx_set_compute_context returns the previously active compute context invisibly. rx_get_compute_context returns the active compute context.


## <a name="see-also"></a>See also

`RxComputeContext`, [`RxLocalSeq`](RxLocalSeq.md), [`RxInSqlServer`](RxInSqlServer.md), [`rx_set_compute_context`](rx-set-compute-context.md).


## <a name="example"></a>Example



```
from revoscalepy import RxLocalSeq, RxInSqlServer, rx_get_compute_context, rx_set_compute_context

local_cc = RxLocalSeq()
sql_server_cc = RxInSqlServer('Driver=SQL Server;Server=.;Database=RevoTestDb;Trusted_Connection=True;')
previous_cc = rx_set_compute_context(sql_server_cc)
rx_get_compute_context()
```

