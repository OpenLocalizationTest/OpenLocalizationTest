---
title: getRemoteObject function (mrsdeploy) | Microsoft Docs
description: " Get an object from the workspace of the remote R session and load it into the workspace  of the local R session. "
keywords: (mrsdeploy), getRemoteObject
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
ms.openlocfilehash: 21a2a547fb6bc7649da8fc9bac747c2b283a0bb2
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="getremoteobject-get-an-object-from-the-remote-r-session"></a>getRemoteObject: Get an object from the remote R session. 
 ## <a name="description"></a>Description

Get an object from the workspace of the remote R session and load it into the workspace of the local R session.


 ## <a name="usage"></a>Usage

```   
  getRemoteObject(obj, name = NULL)

```

 ## <a name="arguments"></a>Arguments



 ### `obj`
 A character vector containing the names of the R objects in the remote R session  to load in the local R session. 



 ### `name`
 The name of an R list object (created if necessary) in the local R session that  will contain the R objects from the remote R session.  If `name` is `NULL`,  then R objects from the remote R session will be loaded in the GlobalEnv of the local R session. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="value"></a>Value

list of R objects or `NULL`

 ## <a name="see-also"></a>See Also

[getRemoteWorkspace](getRemoteWorkspace.md)

[putLocalObject](putLocalObject.md)

[putLocalWorkspace](putLocalWorkspace.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

remoteExecute("x<-rnorm(10);y<-rnorm(10);model<-lm(x~y)", writePlots=TRUE)
getRemoteObject("model")
getRemoteObject("model", name="myObjsFromRemote")
 ## End(Not run) 
```

