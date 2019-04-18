---
title: listRemoteFiles function (mrsdeploy) | Microsoft Docs
description: " Get a list of files in the working directory of the remote R session. "
keywords: (mrsdeploy), listRemoteFiles
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
ms.openlocfilehash: 66b6e0141e151601fd7a8d178892483a116072a7
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="listremotefiles-get-a-list-of-files-from-the-remote-r-session"></a>listRemoteFiles: Get a list of files from the remote R session. 
 ## <a name="description"></a>Description

Get a list of files in the working directory of the remote R session.


 ## <a name="usage"></a>Usage

```   
  listRemoteFiles()

```

 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="value"></a>Value

A character vector containing the file names in the working directory of the remote session.

 ## <a name="see-also"></a>See Also

[getRemoteFile](getRemoteFile.md)

[deleteRemoteFile](deleteRemoteFile.md)

[putLocalFile](putLocalFile.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

files<-listRemoteFiles()
 ## End(Not run) 
```

