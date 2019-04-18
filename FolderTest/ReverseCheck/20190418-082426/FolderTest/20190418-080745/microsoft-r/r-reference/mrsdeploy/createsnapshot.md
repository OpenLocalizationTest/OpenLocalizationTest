---
title: createSnapshot function (mrsdeploy) | Microsoft Docs
description: " Creates a snapshot of the remote R session and saves it on the server. Both the workspace and the files in the working directory are saved. "
keywords: (mrsdeploy), createSnapshot
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
ms.openlocfilehash: 235927d196fd14cf75c86a022f6e06186a5a5292
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="createsnapshot-create-a-snapshot-of-the-remote-r-session"></a>createSnapshot: Create a snapshot of the remote R session. 
 ## <a name="description"></a>Description

Creates a snapshot of the remote R session and saves it on the server. Both the workspace and the files in the working directory are saved.


 ## <a name="usage"></a>Usage

```   
  createSnapshot(name)

```

 ## <a name="arguments"></a>Arguments



 ### `name`
 Name describing the snapshot to be saved. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="value"></a>Value

`snapshot_id` if successful.

 ## <a name="see-also"></a>See Also

[deleteSnapshot](deleteSnapshot.md)

[listSnapshots](listSnapshots.md)

[loadSnapshot](loadSnapshot.md)

[downloadSnapshot](downloadSnapshot.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

snapshot_id<-createSnapshot()
 ## End(Not run) 
```

