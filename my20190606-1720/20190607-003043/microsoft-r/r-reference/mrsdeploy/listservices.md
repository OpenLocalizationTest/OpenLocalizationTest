---
title: listServices function (mrsdeploy) | Microsoft Docs
description: " List the different published web services on the R Server instance. "
keywords: (mrsdeploy), listServices
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
ms.openlocfilehash: c3906c8551f5275f012ca9d51fb78caef6d9c765
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="listservices-list-the-different-published-web-services"></a>listServices: List the different published web services. 
 ## <a name="description"></a>Description

List the different published web services on the R Server instance.


 ## <a name="usage"></a>Usage

```   
  listServices(name = character(0), v = character(0))

```

 ## <a name="arguments"></a>Arguments



 ### `name`
 When a name is specified, returns only web services with that  name. Use quotes around the name string, such as "MyService". 



 ### `v`
 When specified, returns only web services with that version. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)


The service `name` and service `v` version are optional. This call allows you to retrieve service information regarding:



1 All services published

1 All versioned services for a specific named service

1 A specific version for a named service



Users can use this information along with the `discover_service` operation to interact with and consume the web service.


 ## <a name="value"></a>Value

A list of services and service information.

 ## <a name="see-also"></a>See Also

Other service methods: [deleteService](deleteService.md), [getService](getService.md), [print.serviceDetails](print.serviceDetails.md), [publishService](publishService.md), [serviceOption](serviceOption.md), [summary.serviceDetails](summary.serviceDetails.md), [updateService](updateService.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:


# --- List all published services
services <- listServices()

# --- List all published versions of a service
services <- listServices("transmission")

# --- List a specific service version
service <- listServices("transmission", "1.0.1")
 ## End(Not run) 
```

