---
title: summary.serviceDetails function (mrsdeploy) | Microsoft Docs
description: " Defines the R summary generic for serviceDetails during a  listServices(). "
keywords: (mrsdeploy), summary.serviceDetails
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
ms.openlocfilehash: 6d38f6aefab948a22d7a8147f8d73ce1bde8133f
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="summaryservicedetails-the-summary-generic-for-servicedetails"></a>summary.serviceDetails: The summary generic for `serviceDetails`. 
 ## <a name="description"></a>Description

Defines the R summary generic for `serviceDetails` during a `listServices()`.


 ## <a name="usage"></a>Usage

```   
 ## S3 method for class `serviceDetails':
summary  (o)

```

 ## <a name="arguments"></a>Arguments



 ### `o`
 The `serviceDetails` list of S3 objects. 



 ## <a name="see-also"></a>See Also

Other service methods: [deleteService](deleteService.md), [getService](getService.md), [listServices](listServices.md), [print.serviceDetails](print.serviceDetails.md), [publishService](publishService.md), [serviceOption](serviceOption.md), [updateService](updateService.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# --- print all ---
summary(listServices())
 ## End(Not run) 
```

