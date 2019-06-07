---
title: RxLocalSeq function (revoAnalytics) | Microsoft Docs
description: " Creates a local compute context object.   This is the main generator for S4 class RxLocalSeq. Computations using rxExec will be processed sequentially. This is the default compute context. "
keywords: (revoAnalytics), RxLocalSeq, IO
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
ms.openlocfilehash: 506861fdf72e6d75005717ee8ee707d3285c15e6
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxlocalseq-generate-local-compute-context"></a>RxLocalSeq: Generate Local Compute Context 
 ## <a name="description"></a>Description

Creates a local compute context object.  
This is the main generator for S4 class RxLocalSeq. Computations using rxExec will be processed sequentially. This is the default compute context.


 ## <a name="usage"></a>Usage

```   
  RxLocalSeq( object, dataPath = NULL, outDataPath = NULL )

```


 ## <a name="arguments"></a>Arguments



 ### `object`
 a compute context object. If `object` has slots for   `dataPath` and/or `outDataPath`, they will be copied to the  equivalent slots for the new `RxLocalSeq` object. Explicit specifications  of the `dataPath` and/or outDataPath arguments will override this.  


 ### `dataPath`
 `NULL` or character vector defining the search path(s) for the input data source(s). If not `NULL`, it overrides any specification for `dataPath` in [rxOptions](rxOptions.md) 


 ### `outDataPath`
 `NULL` or character vector defining the search path(s) for  new output data file(s).  If not `NULL`, this overrides any specification for `dataPath`in [rxOptions](rxOptions.md)  




 ## <a name="details"></a>Details

A job is associated with the compute context in effect at the time the job was submitted. If the compute context subsequently changes, the compute context of the job is not affected.

Note that `dataPath` and `outDataPath` are only utiltized by data sources used in **RevoScaleR** analyses. They do not alter the working directory for other R functions that read from or write to files.



 ## <a name="value"></a>Value

object of class RxLocalSeq.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxSetComputeContext](rxSetComputeContext.md), [rxExec](rxExec.md), [rxOptions](rxOptions.md), [RxComputeContext](RxComputeContext.md), [RxLocalParallel](RxLocalParallel.md), [RxLocalSeq-class](RxLocalSeq-class.md).


 ## <a name="examples"></a>Examples

 ```

  ## Not run:


# Create a local compute context object  
localContext <- RxLocalSeq()

# Tell RevoScaleR to use localContext compute context
rxSetComputeContext( localContext )

 ## End(Not run) 
```



