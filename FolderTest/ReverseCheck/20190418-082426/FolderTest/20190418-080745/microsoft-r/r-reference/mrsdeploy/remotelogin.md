---
title: remoteLogin function (mrsdeploy) | Microsoft Docs
description: " Authenticates the user and creates a remote R session. "
keywords: (mrsdeploy), remoteLogin
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
ms.openlocfilehash: 84a5dfe97d8e01930b18a6ee9787baaa5c15dcc4
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="remotelogin-remote-login-to-the-microsoft-r-server"></a>remoteLogin: Remote login to the Microsoft R Server 
 ## <a name="description"></a>Description

Authenticates the user and creates a remote R session.


 ## <a name="usage"></a>Usage

```   
  remoteLogin(deployr_endpoint, session = TRUE, diff = TRUE,
    commandline = TRUE, prompt = "REMOTE> ", username = NULL,
    password = NULL)

```

 ## <a name="arguments"></a>Arguments



 ### `deployr_endpoint`
 The Microsoft R Server HTTP/HTTPS endpoint, including the port number. 



 ### `session`
 If `TRUE`,  create a remote session. 



 ### `diff`
 If `TRUE`, creates a 'diff' report showing differences between the local and remote sessions. Parameter is only valid if `session` parameter is `TRUE`. 



 ### `commandline`
 If `TRUE`,  creates a "REMOTE' command line in the R console. 'REMOTE' command line is used to interact with the remote R session.  Parameter is only valid if `session` parameter is `TRUE`. 



 ### `prompt`
 The command prompt to be used for the remote session 



 ### `username`
 if `NULL`, the user will be prompted to enter username and password 



 ### `password`
 if `NULL`, the user will be prompted to enter username and password 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)



 ## <a name="see-also"></a>See Also

[remoteLogout](remoteLogout.md)

[remoteCommandLine](remoteCommandLine.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

remoteLogin("https://localhost:1280", session=TRUE, diff=TRUE, commandline=TRUE)
 ## End(Not run) 
```

