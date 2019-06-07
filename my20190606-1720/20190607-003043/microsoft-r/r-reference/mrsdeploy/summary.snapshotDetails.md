---
title: summary.snapshotDetails function (mrsdeploy) | Microsoft Docs
description: " Defines the R summary generic for snapshotDetails during a  listSnapshots(). "
keywords: (mrsdeploy), summary.snapshotDetails
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
ms.openlocfilehash: b07173ef1ddaaece8e2bd7ddc883a68e1fe883c6
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="summarysnapshotdetails-the-summary-generic-for-snapshotdetails"></a>summary.snapshotDetails: The summary generic for `snapshotDetails`. 
 ## <a name="description"></a>Description

Defines the R summary generic for `snapshotDetails` during a `listSnapshots()`.


 ## <a name="usage"></a>Usage

```   
 ## S3 method for class `snapshotDetails':
summary  (o)

```

 ## <a name="arguments"></a>Arguments



 ### `o`
 The `snapshotDetails` list of S3 object. 



 ## <a name="see-also"></a>See Also

Other snapshot methods: [print.snapshotDetails](print.snapshotDetails.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# --- print all ---
summary(listSnapshots())
 ## End(Not run) 
```

