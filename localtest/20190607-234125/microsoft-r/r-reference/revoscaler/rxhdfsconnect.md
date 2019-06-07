---
title: rxHdfsConnect function (revoAnalytics) | Microsoft Docs
description: " Establishes a connection from RevoScaleR to the Hadoop Distributed File System (HDFS).  "
keywords: (revoAnalytics), rxHdfsConnect, file, connection
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
ms.openlocfilehash: 9440363f6ff8ab5b0f3cab8a7c417bb38885cd7d
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxhdfsconnect--establish-a-connection-to-the-hadoop-distributed-file-system"></a>rxHdfsConnect:  Establish a Connection to the Hadoop Distributed File System  
 ## <a name="description"></a>Description

Establishes a connection from RevoScaleR to the Hadoop Distributed File System (HDFS). 


 ## <a name="usage"></a>Usage

```   
  rxHdfsConnect(hostName, portNumber)

```

 ## <a name="arguments"></a>Arguments



 ### `hostName`
  character string specifying the host name of your Hadoop name node.  


 ### `portNumber`
  integer scalar specifying the port number of your Hadoop name node.  



 ## <a name="details"></a>Details

If you accept the install time option to specify a default HDFS connection, you are prompted for a host name and port number for your Hadoop name node, which are stored as environment variables `REVOHADOOPHOST` and `REVOHADOOPPORT`. If these environment variables are set, this function is called by Rprofile.site on startup.

After establishing the connection, this function sets the `rxOptions` for `hdfsHost` and `hdfsPort`, and subsequent calls to `RxHdfsFileSystem` should be done using the default values of `hostName` and `port`.

It is important that this function be called before any functions that call into **rJava**, in particular before initializing **rhdfs**.


 ## <a name="value"></a>Value

invisibly, the return value of `rxOptions`.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxOptions](rxOptions.md), `link{RxHdfsFileSystem}`

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

rxHdfsConnect(hostName = "sandbox-01", port = 8020)

myHDFS <- RxHdfsFileSystem()
 ## End(Not run) 
```



