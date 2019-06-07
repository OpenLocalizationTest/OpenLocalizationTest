---
title: putLocalObject function (mrsdeploy) | Microsoft Docs
description: " Copy an object from the workspace of the local R session to the workspace  of the remote R session. "
keywords: (mrsdeploy), putLocalObject
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
ms.openlocfilehash: 2efef99823eda8f36a4917aa63dd303433876c7c
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="putlocalobject-copy-an-object-from-the-local-r-session-to-the-remote-r-session"></a>putLocalObject: Copy an object from the local R session to the remote R session. 
 ## <a name="description"></a>Description

Copy an object from the workspace of the local R session to the workspace of the remote R session.


 ## <a name="usage"></a>Usage

```   
  putLocalObject(obj, name = NULL)

```

 ## <a name="arguments"></a>Arguments



 ### `obj`
 A character vector containing the names of the R Objects in the local R session to load in the remote R session 



 ### `name`
 The name of an R list object (created if necessary) in the remote R session that will contain the R objects from the local R session.  If `name` is `NULL`, then R objects from the local R session will be loaded in the GlobalEnv of the remote R session. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="value"></a>Value

list of R objects or `NULL`

 ## <a name="see-also"></a>See Also

[getRemoteWorkspace](getRemoteWorkspace.md)

[getRemoteObject](getRemoteObject.md)

[putLocalWorkspace](putLocalWorkspace.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

aa<-rnorm(100)
bb<-rnorm(100)
putLocalObject(c("aa","bb"))
putLocalObject(c("aa","bb"), name="myObjsFromLocal")
 ## End(Not run) 
```

