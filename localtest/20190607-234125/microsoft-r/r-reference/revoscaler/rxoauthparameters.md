---
title: rxOAuthParameters function (revoAnalytics) | Microsoft Docs
description: " Method to create parameter list to be used for getting an OAuth2 token. "
keywords: (revoAnalytics), rxOAuthParameters, file, connection
author: heidisteen
manager: cgronlun
ms.date: 01/24/2018
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ROBOTS: ''
audience: ''
ms.devlang: ''
ms.reviewer: ''
ms.suite: ''
ms.tgt_pltfrm: ''
ms.custom: ''
ms.openlocfilehash: b5001e3ef182681bd5b4c8a3eb358d81f7d9482c
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxoauthparameters-oauth2-token-request"></a>rxOAuthParameters: OAuth2 Token request 
 ## <a name="description"></a>Description

Method to create parameter list to be used for getting an OAuth2 token.


 ## <a name="usage"></a>Usage

```   
      rxOAuthParameters(authUri = NULL, tenantId = NULL, clientId = NULL, resource = NULL, username = NULL, password = NULL, authToken= NULL, useWindowsAuth = FALSE)


```

 ## <a name="arguments"></a>Arguments




 ### `authUri`
 Optional string containing OAuth Authentication URI - default NULL  


 ### `tenantId`
 Optional string containing OAuth Tenant ID - default NULL  


 ### `clientId`
 Optional string containing OAuth ClientID - default NULL  


 ### `resource`
 Optional string containing OAuth Resource  - default NULL  


 ### `username`
 Optional string containing OAuth Username - default NULL  


 ### `password`
 Optional string containing OAuth Password - default NULL  


 ### `authToken`
 Optional string containing a valid OAuth token to be used for WebHdfs requests - default NULL  


 ### `useWindowsAuth`
 Optional Flag indicating if Windows Authentication should be used for obtaining the OAuth token (applicable only on Windows) - default NULL  




 ## <a name="details"></a>Details

Reading from HDFS file system via WebHdfs can only be done by first obtaining a OAuth2 token. This function allows the specification of parameters that can be set to retreive a token.



 ## <a name="value"></a>Value

An rxOAuthParameters list object. This object may be used in [RxHdfsFileSystem](RxHdfsFileSystem.md) to set the OAuth request method for WebHdfs usage.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[RxHdfsFileSystem](RxHdfsFileSystem.md)

 ## <a name="examples"></a>Examples

 ```

  # Setup to run analyses to use HDFS with access via WebHdfs and OAuth2
  ## Not run:

oAuth <- rxOAuthParameters(authUri = "https://login.windows.net/",
            tenantId = "mytest.onmicrosoft.com",
            clientId = "872cd9fa-d31f-45e0-9eab-6e460a02d1e2", 
            resource = "https://KonaCompute.net/", 
            username = "me@mytest.onmicrosoft.com", 
            password = "password")

myHdfsFileSystem <- RxHdfsFileSystem(hostName = "myHost", port = 443, useWebHdfs = TRUE, oAuthParameters = oAuth)
rxSetFileSystem(fileSystem = myHdfsFileSystem )
 ## End(Not run) 
```



