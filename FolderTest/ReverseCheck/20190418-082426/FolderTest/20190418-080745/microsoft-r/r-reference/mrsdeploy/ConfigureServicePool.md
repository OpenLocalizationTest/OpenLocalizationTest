---
title: configureServicePool function (mrsdeploy) | Microsoft Docs
description: " Create or Update a dedicated pool for a published web service running on Machine Learning Server. "
keywords: (mrsdeploy), configureServicePool
author: heidisteen
manager: cgronlun
ms.date: 01/18/2019
ms.topic: reference
ms.prod: microsoft-r
ms.service: ''
ms.assetid: ''
ROBOTS: ''
audience: ''
ms.devlang: ''
ms.reviewer: ''
ms.suite: ''
ms.tgt_pltfrm: ''
ms.technology: r-server
ms.custom: ''
ms.openlocfilehash: 56c2906e9b8ea2793e0b2dc5bf4bbd68b2f94513
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="configureservicepool-create-or-update-a-dedicated-pool-for-a-published-web-service"></a>configureServicePool: Create or Update a dedicated pool for a published web service 
 ## <a name="description"></a>Description

Create or update a dedicated pool for a published web service running on Machine Learning Server.


 ## <a name="usage"></a>Usage

```   
  configureServicePool(name, version, initialPoolSize = 0, maxPoolSize = 0)

```

 ## <a name="arguments"></a>Arguments



 ### `name`
 A string representing the web service name. To create or update a dedicated pool, you must provide the specific name and version of the  service that the pool is associated with.



 ### `version`
 A string representing the web service version. To create or update a dedicated pool, you must provide the specific name and version of the  service that the pool is associated with. 



 ### `initialPoolSize`
 An integer representing the initial pool size of the dedicated pool. This number of shells will be generated while creating the dedicated pool. If more shells are in need, the dedicated pool will continue  to create new shells in addition to the initial shells up to the maxPoolSize.



 ### `maxPoolSize`
 An integer representing the max pool size of the dedicated pool. This is the maximum number of shells that could be generated in the  dedicated pool during any period of time.



 ## <a name="see-also"></a>See Also

Other dedicated pool methods: [deleteServicePool](DeleteServicePool.md), [getPoolStatus](GetPoolStatus.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:



configureServicePool(
   name = "myService",
   version = "v1",
   initialPoolSize = 5,
   maxPoolSize = 10
)
 ## End(Not run) 
```

