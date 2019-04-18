---
title: deleteServicePool function (mrsdeploy) | Microsoft Docs
description: " Delete an existing dedicated pool for a published web service running on Machine Learning Server. "
keywords: (mrsdeploy), deleteServicePool
author: heidisteen
manager: cgronlun
ms.date: 02/05/2018
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
ms.openlocfilehash: 55bf46d4d6d4da98f5dffb986cfcf9d6caf10b81
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="deleteservicepool-delete-an-existing-dedicated-pool-for-a-published-web-service"></a>deleteServicePool: Delete an existing dedicated pool for a published web service 
 ## <a name="description"></a>Description

Delete an existing dedicated pool for a published web service running on Machine Learning Server.


 ## <a name="usage"></a>Usage

```   
  deleteServicePool(name, version)

```

 ## <a name="arguments"></a>Arguments



 ### `name`
 A string representing the web service name. To create or update  a dedicated pool, you must provide the specific name and version of the  service that the pool is associated with. 



 ### `version`
 A string representing the web service version. To create or  update a dedicated pool, you must provide the specific name and version of the  service that the pool is associated with. 



 ## <a name="see-also"></a>See Also

Other dedicated pool methods: [configureServicePool](ConfigureServicePool.md), [getPoolStatus](GetPoolStatus.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:


deleteServicePool(
   name = "myService",
   version = "v1"
)
 ## End(Not run) 
```

