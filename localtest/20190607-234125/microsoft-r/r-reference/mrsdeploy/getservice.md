---
title: getService function (mrsdeploy) | Microsoft Docs
description: " Get a web service for consumption on running on R Server. "
keywords: (mrsdeploy), getService
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
ms.openlocfilehash: ae93c4057cff432235e851f3cd50d30dc98b0cb3
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="getservice-get-a-web-service-for-consumption"></a>getService: Get a web service for consumption. 
 ## <a name="description"></a>Description

Get a web service for consumption on running on R Server.


 ## <a name="usage"></a>Usage

```   
  getService(name, v = character(0), destination = NULL)

```

 ## <a name="arguments"></a>Arguments



 ### `name`
 The web service name. 



 ### `v`
 The web service version. 



 ### `destination`
 (optional) The codegen output directory location. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="see-also"></a>See Also

Other service methods: [deleteService](deleteService.md), [listServices](listServices.md), [print.serviceDetails](print.serviceDetails.md), [publishService](publishService.md), [serviceOption](serviceOption.md), [summary.serviceDetails](summary.serviceDetails.md), [updateService](updateService.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# Discover the `add-service` version `1.0.1`
api <- getService("add-service", "1.0.1")
 ## End(Not run) 
```

