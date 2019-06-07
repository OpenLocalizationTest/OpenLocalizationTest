---
title: deleteSnapshot function (mrsdeploy) | Microsoft Docs
description: " Deletes the specified snapshot from the repository on the R Server. "
keywords: (mrsdeploy), deleteSnapshot
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
ms.openlocfilehash: a26bd318cb73cf2afd6e38e6a05dc3ff2d154038
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="deletesnapshot-delete-a-snapshot-from-the-r-server"></a>deleteSnapshot: Delete a snapshot from the R server. 
 ## <a name="description"></a>Description

Deletes the specified snapshot from the repository on the R Server.


 ## <a name="usage"></a>Usage

```   
  deleteSnapshot(snapshot_id)

```

 ## <a name="arguments"></a>Arguments



 ### `snapshot_id`
 Identifier of the snapshot to delete. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="value"></a>Value

`TRUE` if successful.

 ## <a name="see-also"></a>See Also

[createSnapshot](createSnapshot.md)

[listSnapshots](listSnapshots.md)

[loadSnapshot](loadSnapshot.md)

[downloadSnapshot](downloadSnapshot.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

deleteSnapshot("8ce7eb47-3aeb-4c5a-b0a5-a2025f07d9cd")
 ## End(Not run) 
```

