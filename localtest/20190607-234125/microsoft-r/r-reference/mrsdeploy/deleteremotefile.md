---
title: deleteRemoteFile function (mrsdeploy) | Microsoft Docs
description: " Delete a file from the working directory of the remote R session. "
keywords: (mrsdeploy), deleteRemoteFile
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
ms.openlocfilehash: 44946ef3145f90ce0fd191b4a19c4dd2b77180d4
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="deleteremotefile-delete-a-file-from-the-remote-r-session"></a>deleteRemoteFile: Delete a file from the remote R session. 
 ## <a name="description"></a>Description

Delete a file from the working directory of the remote R session.


 ## <a name="usage"></a>Usage

```   
  deleteRemoteFile(filename)

```

 ## <a name="arguments"></a>Arguments



 ### `filename`
 Name of the file to delete. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="value"></a>Value

`TRUE` if successful.

 ## <a name="see-also"></a>See Also

[getRemoteFile](getRemoteFile.md)

[listRemoteFiles](listRemoteFiles.md)

[putLocalFile](putLocalFile.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

deleteRemoteFile("c:/data/test.csv")
 ## End(Not run) 
```

