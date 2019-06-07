---
title: 'rx_set_compute_context: Sets the compute context (revoscalepy)'
description: Sets the active compute context for revoscalepy computations
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
ms.openlocfilehash: e22edfb54cc71ad0f108a0a54ee4ec268cad8395
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxsetcomputecontext"></a>rx_set_compute_context


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_set_compute_context(compute_context: revoscalepy.computecontext.RxComputeContext.RxComputeContext) -> revoscalepy.computecontext.RxComputeContext.RxComputeContext
```





## <a name="description"></a>Description

Sets the active compute context for revoscalepy computations


## <a name="arguments"></a>Arguments


### <a name="computecontext"></a>compute_context

Character string specifying class name or description of the specific class to instantiate, or an existing RxComputeContext object.
Choices include: “RxLocalSeq” or “local”, “RxInSqlServer”.


## <a name="returns"></a>Returns

rx_set_compute_context returns the previously active compute context invisibly. rx_get_compute_context returns the active compute context.


## <a name="see-also"></a>See also

`RxComputeContext`, [`RxLocalSeq`](RxLocalSeq.md), [`RxInSqlServer`](RxInSqlServer.md), [`rx_get_compute_context`](rx-get-compute-context.md).


## <a name="example"></a>Example



```
from revoscalepy import RxLocalSeq, RxInSqlServer, rx_get_compute_context, rx_set_compute_context

local_cc = RxLocalSeq()
sql_server_cc = RxInSqlServer('Driver=SQL Server;Server=.;Database=RevoTestDb;Trusted_Connection=True;')
previous_cc = rx_set_compute_context(sql_server_cc)
rx_get_compute_context()
```

