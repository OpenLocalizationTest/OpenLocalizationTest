---
title: loadSnapshot function (mrsdeploy) | Microsoft Docs
description: " Loads the specified snapshot from the R server into the remote session.The workspace is updated with the objects saved in the snapshot, and saved files are restored to the working directory. "
keywords: (mrsdeploy), loadSnapshot
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
ms.openlocfilehash: a3a574df5f70f95a16d1ad00547f0f75869ff846
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="loadsnapshot-load-a-snapshot-from-the-r-server-into-the-remote-session"></a>loadSnapshot: Load a snapshot from the R server into the remote session. 
 ## <a name="description"></a>Description

Loads the specified snapshot from the R server into the remote session. The workspace is updated with the objects saved in the snapshot, and saved files are restored to the working directory.


 ## <a name="usage"></a>Usage

```   
  loadSnapshot(snapshot_id)

```

 ## <a name="arguments"></a>Arguments



 ### `snapshot_id`
 Identifier of the snapshot to load. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="value"></a>Value

`TRUE` if successful.

 ## <a name="see-also"></a>See Also

[createSnapshot](createSnapshot.md)

[deleteSnapshot](deleteSnapshot.md)

[listSnapshots](listSnapshots.md)

[downloadSnapshot](downloadSnapshot.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

loadSnapshot("8ce7eb47-3aeb-4c5a-b0a5-a2025f07d9cd")
 ## End(Not run) 
```

