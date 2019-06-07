---
title: rxGetAvailableNodes function (revoAnalytics) | Microsoft Docs
description: " Gets a list of operational nodes on a cluster. Note that this function will attempt to connect to the cluster when executed. "
keywords: (revoAnalytics), rxGetAvailableNodes, IO
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
ms.openlocfilehash: e0c4164c816dcb71557e8a2a5337d120e96d8c2f
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxgetavailablenodes--gets-a-list-of-operational-nodes-on-a-cluster"></a>rxGetAvailableNodes:  Gets a list of operational nodes on a cluster.  
 ## <a name="description"></a>Description

Gets a list of operational nodes on a cluster.
Note that this function will attempt to connect to the cluster when executed.



 ## <a name="usage"></a>Usage

```   
  rxGetAvailableNodes(computeContext,  makeRNodeNames = FALSE)

```


 ## <a name="arguments"></a>Arguments



 ### `computeContext`
 A distributed compute context (preferred, see [RxComputeContext](RxComputeContext.md))  or a `jobInfo` object 



 ### `makeRNodeNames`
 logical. If `TRUE`, names of the nodes will be normalized for use  as R variables.  See [rxMakeRNodeNames](rxMakeRNodeNames.md) for details on name mangling. 




 ## <a name="value"></a>Value

a character vector of node names, or `NULL`.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxGetNodeInfo](rxGetNodeInfo.md)
[RxComputeContext](RxComputeContext.md)
[rxGetJobs](rxGetJobs.md)
[rxMakeRNodeNames](rxMakeRNodeNames.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

rxGetAvailableNodes( myCluster )
 ## End(Not run) 
```


