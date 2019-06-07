---
title: downloadSnapshot function (mrsdeploy) | Microsoft Docs
description: " Downloads the specified snapshot from the R server in zip format. "
keywords: (mrsdeploy), downloadSnapshot
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
ms.openlocfilehash: bb1cf9808dec6ef647005f543a03c58f1548c9e7
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="downloadsnapshot-download-a-snapshot-from-the-r-server"></a>downloadSnapshot: Download a snapshot from the R server. 
 ## <a name="description"></a>Description

Downloads the specified snapshot from the R server in zip format.


 ## <a name="usage"></a>Usage

```   
  downloadSnapshot(snapshot_id, file = NULL)

```

 ## <a name="arguments"></a>Arguments



 ### `snapshot_id`
 Identifier of the snapshot to load. 



 ### `file`
 Name of a file to write the contents of the snapshot.  If `NULL`, (the default), then the raw vector of bytes will be returned. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="value"></a>Value

raw vector of bytes if `file=NULL` if successful.  If `file` not equal `NULL`, then `TRUE` will be returned.

 ## <a name="see-also"></a>See Also

[createSnapshot](createSnapshot.md)

[deleteSnapshot](deleteSnapshot.md)

[listSnapshots](listSnapshots.md)

[loadSnapshot](loadSnapshot.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

downloadSnapshot("8ce7eb47-3aeb-4c5a-b0a5-a2025f07d9cd")
downloadSnapshot("8ce7eb47-3aeb-4c5a-b0a5-a2025f07d9cd", file="snapshot.zip")
 ## End(Not run) 
```

