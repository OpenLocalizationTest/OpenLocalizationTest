---
title: rxDistributeJob function (revoAnalytics) | Microsoft Docs
description: " Allows distributed execution of a function in parallel across nodes (computers)  of a 'compute context' such as a cluster. A helper functions checks to see if the 'compute context' is appropriate. "
keywords: (revoAnalytics), rxDistributeJob, rxIsDistributedContext, IO
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
ms.openlocfilehash: 5b772ca587ba686caf38df5251dc3a7673f90650
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxdistributejob--distribute-job-across-nodes-of-a-cluster"></a>rxDistributeJob:  Distribute job across nodes of a cluster  
 ## <a name="description"></a>Description

Allows distributed execution of a function in parallel across nodes (computers) of a 'compute context' such as a cluster. A helper functions checks to see if the 'compute context' is appropriate.



 ## <a name="usage"></a>Usage

```   
  rxDistributeJob(matchCallList, matchCall)
  rxIsDistributedContext( computeContext = NULL, data = NULL)

```


 ## <a name="arguments"></a>Arguments



 ### `matchCallList`
  a list containing the function name and arguments, adjusting environments as needed 



 ### `matchCall`
  a call in which all of the specified arguments are specified by their full names;  typically the result of match.call 



 ### `computeContext`
 `NULL` or an [RxComputeContext](RxComputeContext.md) object. 



 ### `data`
 `NULL` or an [RxDataSource](RxDataSource.md) object.  If specified, compatibility of the data source with the 'dataDistType' in the compute context will be checked. 





 ## <a name="details"></a>Details

An example of usage can be found in the **RevoPemaR** package.



 ## <a name="value"></a>Value

The result of the distributed computation.

 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxExec](rxExec.md), [RxComputeContext](RxComputeContext.md), [rxSetComputeContext](rxSetComputeContext.md), [rxGetComputeContext](rxSetComputeContext.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:


# Example is provided in the RevoPemaR package

 ## End(Not run) 
```


