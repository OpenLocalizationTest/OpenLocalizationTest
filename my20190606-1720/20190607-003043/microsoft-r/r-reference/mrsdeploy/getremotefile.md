---
title: getRemoteFile function (mrsdeploy) | Microsoft Docs
description: " Get the content of a file from the working directory of the remote R session. "
keywords: (mrsdeploy), getRemoteFile
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
ms.openlocfilehash: dfc9d1b0800f3e8b4a68b8fd252c2df0c1bb94a4
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="getremotefile-get-the-content-of-a-file-from-remote-r-session"></a>getRemoteFile: Get the content of a file from remote R session. 
 ## <a name="description"></a>Description

Get the content of a file from the working directory of the remote R session.


 ## <a name="usage"></a>Usage

```   
  getRemoteFile(filename, as = "text")

```

 ## <a name="arguments"></a>Arguments



 ### `filename`
 Name of the file in the remote working directory. 



 ### `as`
 The content type of the file ("text" or "raw").  For binary files use 'raw'. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="value"></a>Value

raw vector of bytes if `as="raw"`. Otherwise, the text content of the file, or `NULL` if the file content cannot be retrieved.

 ## <a name="see-also"></a>See Also

[deleteRemoteFile](deleteRemoteFile.md)

[listRemoteFiles](listRemoteFiles.md)

[putLocalFile](putLocalFile.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

content<-getRemoteFile("test.csv")

raw_content<-getRemoteFile("test.png", as="raw")
fh = file("test.png", "wb")
writeBin(raw_content, fh)
close(fh)
 ## End(Not run) 
```

