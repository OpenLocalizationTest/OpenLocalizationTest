---
title: listSnapshots function (mrsdeploy) | Microsoft Docs
description: " Get a list of all the snapshots on the R server that are available to the current user. "
keywords: (mrsdeploy), listSnapshots
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
ms.openlocfilehash: 11fece2f8022b6855df0c84590d87a04222d4f43
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="listsnapshots-get-a-list-of-snapshots-for-the-current-user"></a>listSnapshots: Get a list of snapshots for the current user. 
 ## <a name="description"></a>Description

Get a list of all the snapshots on the R server that are available to the current user.


 ## <a name="usage"></a>Usage

```   
  listSnapshots()

```

 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="value"></a>Value

A character vector containing the snapshot IDs.

 ## <a name="see-also"></a>See Also

[createSnapshot](createSnapshot.md)

[deleteSnapshot](deleteSnapshot.md)

[loadSnapshot](loadSnapshot.md)

[downloadSnapshot](downloadSnapshot.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

snapshots<-listSnapshots()
 ## End(Not run) 
```

