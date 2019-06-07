---
title: putLocalFile function (mrsdeploy) | Microsoft Docs
description: " Uploads a file from the local machine and writes it to the working directory of the remote R session. This function is often used if a 'data' file needs to be accessed by a script running on the remote R session. "
keywords: (mrsdeploy), putLocalFile
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
ms.openlocfilehash: a76861a0c1122c4720f27e6e047712f70bce0ea8
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="putlocalfile-upload-a-file-from-the-local-machine-to-the-remote-r-session"></a>putLocalFile: Upload a file from the local machine to the remote R session. 
 ## <a name="description"></a>Description

Uploads a file from the local machine and writes it to the working directory of the remote R session. This function is often used if a 'data' file needs to be accessed by a script running on the remote R session.


 ## <a name="usage"></a>Usage

```   
  putLocalFile(filename)

```

 ## <a name="arguments"></a>Arguments



 ### `filename`
 Name of the file to copy. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="value"></a>Value

`TRUE` if successful.

 ## <a name="see-also"></a>See Also

[getRemoteFile](getRemoteFile.md)

[deleteRemoteFile](deleteRemoteFile.md)

[listRemoteFiles](listRemoteFiles.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

putLocalFile("c:/data/test.csv")
putLocalFile("c:/data/test.png", as="raw")
 ## End(Not run) 
```

