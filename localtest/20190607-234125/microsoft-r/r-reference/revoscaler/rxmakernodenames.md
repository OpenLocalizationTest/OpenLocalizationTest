---
title: rxMakeRNodeNames function (revoAnalytics) | Microsoft Docs
description: " Converts valid computer names into valid R variable names.  Should only be used when you want to guarantee that host  names are usable as variable names. "
keywords: (revoAnalytics), rxMakeRNodeNames, IO
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
ms.openlocfilehash: 7612799283eb2b2ef4e50016b6f18e69a5fb4b4c
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxmakernodenames--converts-valid-computer-names-into-valid-r-variable-names"></a>rxMakeRNodeNames:  Converts valid computer names into valid R variable names.  
 ## <a name="description"></a>Description

Converts valid computer names into valid R variable names.  Should only be used when you want to guarantee that host names are usable as variable names.



 ## <a name="usage"></a>Usage

```   
  rxMakeRNodeNames( nodeNames )

```


 ## <a name="arguments"></a>Arguments



 ### `nodeNames`
 character vector of node names to be converted. 




 ## <a name="details"></a>Details

rxMakeRNodeNames will preform the following transformations on each element of the character vector passed:


1 Perform `toupper` on the name.

1 Remove all white space from the name.

1 If one exists, removes the first dot and all characters following it from the name.  (This has the effect of stripping the domain name off, if one exists.)

1 Changes any '-' (dash) characters to '_' (underscore) characters so that node names used as variables do not have to be quoted.



The names returned by this function are valid R names, that is, symbols, but they may no longer be valid computer node names. Do **not** use these names, or this function, in any context where the name may be used to query or control the actual computer; use the original computer name for that.  This function is intended to be used only to generate R variable names for processing or storing distributed computing results from the associated computer. Note also that once a host name has been converted into a guaranteed acceptable R variable name, it is impossible to guarantee the reverse conversion.


 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="examples"></a>Examples

 ```

  ## Not run:

rxMakeRNodeNames(rxGetNodes(myCluster))
rxMakeRNodeNames( c("cluster-head","worker1.foo.edu") )
 ## End(Not run) 
```


