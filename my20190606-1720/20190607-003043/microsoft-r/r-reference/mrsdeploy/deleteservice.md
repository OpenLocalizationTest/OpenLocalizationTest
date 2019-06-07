---
title: deleteService function (mrsdeploy) | Microsoft Docs
description: " Delete a web service on an R Server instance. "
keywords: (mrsdeploy), deleteService
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
ms.openlocfilehash: 639f13989b3ccafde0c00322c1df01d80e3d92af
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="deleteservice-delete-a-web-service"></a>deleteService: Delete a web service.
 ## <a name="description"></a>Description

Delete a web service on an R Server instance.


 ## <a name="usage"></a>Usage

```   
  deleteService(name, v)

```

 ## <a name="arguments"></a>Arguments



 ### `name`
 The web service name. 



 ### `v`
 The web service version. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="see-also"></a>See Also

Other service methods: [getService](getService.md), [listServices](listServices.md), [print.serviceDetails](print.serviceDetails.md), [publishService](publishService.md), [serviceOption](serviceOption.md), [summary.serviceDetails](summary.serviceDetails.md), [updateService](updateService.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# Delete the `add-service` version `1.0.1`
deleteService("add-service", "1.0.1")
 ## End(Not run) 
```

