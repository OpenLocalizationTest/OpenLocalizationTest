---
title: remoteLoginAAD function (mrsdeploy) | Microsoft Docs
description: " Authenticates the user and creates a remote R session. "
keywords: (mrsdeploy), remoteLoginAAD
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
ms.openlocfilehash: 747c2381245e3dbf73309132bed5e9e723967ef5
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="remoteloginaad-remote-login-to-microsoft-r-server-using-azure-active-directory"></a>remoteLoginAAD: Remote login to Microsoft R Server using Azure Active directory. 
 ## <a name="description"></a>Description

Authenticates the user and creates a remote R session.


 ## <a name="usage"></a>Usage

```   
  remoteLoginAAD(deployr_endpoint, authuri = NULL, tenantid = NULL,
    clientid = NULL, resource = NULL, session = TRUE, diff = TRUE,
    commandline = TRUE, prompt = "REMOTE> ", username = NULL,
    password = NULL)

```

 ## <a name="arguments"></a>Arguments



 ### `deployr_endpoint`
 The Microsoft R Server HTTP/HTTPS endpoint, including the port number. 



 ### `authuri`
 The URI of the authentication service for Azure Active Directory. 



 ### `tenantid`
 The tenant ID of the Azure Active Directory account being used to authenticate. 



 ### `clientid`
 the client ID of the Application for the Azure Active Directory account. 



 ### `resource`
 The resource ID of the Application for the Azure Active Directory account. 



 ### `session`
 If `TRUE`,  create a remote session. 



 ### `diff`
 If `TRUE`, creates a 'diff' report showing differences between the local and remote sessions. Parameter is only valid if `session` parameter is `TRUE`. 



 ### `commandline`
 If `TRUE`,  creates a "REMOTE' command line in the R console. Parameter is only valid if `session` parameter is `TRUE`. 



 ### `prompt`
 The command prompt to be used for the remote session 



 ### `username`
 if `NULL`. the user will be prompted to enter username and password 



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

remoteLoginAAD("http://localhost:12800",
                   authuri = "https://login.windows.net",
                   tenantid = "myMRSServer.contoso.com",
                   clientid = "00000000-0000-0000-0000-000000000000",
                   resource = "00000000-0000-0000-0000-000000000000",
                   session=TRUE,
                   diff=TRUE,
                   commandline=TRUE)
 ## End(Not run) 
```

