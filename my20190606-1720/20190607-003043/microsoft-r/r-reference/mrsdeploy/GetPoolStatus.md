---
title: getPoolStatus function (mrsdeploy) | Microsoft Docs
description: " Get the status of the dedicated pool for a published web service running on Machine Learning Server. "
keywords: (mrsdeploy), getPoolStatus
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
ms.openlocfilehash: 8e36ded8ab0836a720a6cb551f42adce0e7a6f85
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="getpoolstatus-get-the-status-of-the-dedicated-pool-for-a-published-web-service"></a>getPoolStatus: Get the status of the dedicated pool for a published web service 
 ## <a name="description"></a>Description

Get the status of the dedicated pool for a published web service running on Machine Learning Server.


 ## <a name="usage"></a>Usage

```   
  getPoolStatus(name, version)

```

 ## <a name="arguments"></a>Arguments



 ### `name`
 A string representing the web service name. To the dedicated pool status, you must provide the specific name and version of the  service that the pool is associated with. 



 ### `version`
 A string representing the web service version. To check the dedicated pool status, you must provide the specific name and version of the  service that the pool is associated with. 



 ## <a name="see-also"></a>See Also

Other dedicated pool methods: [configureServicePool](ConfigureServicePool.md), [deleteServicePool](DeleteServicePool.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:


getPoolStatus(
   name = "myService",
   version = "v1"
)
 ## End(Not run) 
```

