---
title: serviceOption function (mrsdeploy) | Microsoft Docs
description: " Retrieve, set, and list the different service options. "
keywords: (mrsdeploy), serviceOption
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
ms.openlocfilehash: f18a29bbc93586996c16386de78789c5e896a2bf
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="serviceoption-retrieve-set-and-list-the-different-service-options"></a>serviceOption: Retrieve, set, and list the different service options. 
 ## <a name="description"></a>Description

Retrieve, set, and list the different service options.


 ## <a name="usage"></a>Usage

```   
  serviceOption()

```

 ## <a name="arguments"></a>Arguments



 ### `name`
 The option name. 



 ### `value`
 The option value to be set. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="value"></a>Value

A list of the current service options.

 ## <a name="see-also"></a>See Also

Other service methods: [deleteService](deleteService.md), [getService](getService.md), [listServices](listServices.md), [print.serviceDetails](print.serviceDetails.md), [publishService](publishService.md), [summary.serviceDetails](summary.serviceDetails.md), [updateService](updateService.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:


# --- set option name|value
opts <- serviceOption()
opts$set('base_dir', getwd())

# --- get option
opts <- serviceOption()
base_dir <- opts$get('base_dir')

# --- list options
options <- serviceOption()$get()
 ## End(Not run) 
```

