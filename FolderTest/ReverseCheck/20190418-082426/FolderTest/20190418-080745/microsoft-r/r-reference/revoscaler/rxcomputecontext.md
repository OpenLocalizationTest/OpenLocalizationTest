---
title: RxComputeContext function (revoAnalytics) | Microsoft Docs
description: " This is the main generator for RxComputeContext S4 classes. "
keywords: (revoAnalytics), RxComputeContext, file, connection
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
ms.openlocfilehash: 12261ff4f038e83714acd7479b0071dc890602ed
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxcomputecontext-revoscaler-compute-contexts-class-generator"></a>RxComputeContext: RevoScaleR Compute Contexts: Class Generator 
 ## <a name="description"></a>Description

This is the main generator for RxComputeContext S4 classes.


 ## <a name="usage"></a>Usage

```   
    RxComputeContext( computeContext, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `computeContext`
 character string specifying class name or description of the specific  class to instantiate, or an existing `RxComputeContext` object.  Choices include: "RxLocalSeq" or "local", "RxLocalParallel" or "localpar", "RxSpark" or "spark",  "RxHadoopMR" or "hadoopmr", "RxInSqlServer" or "sqlserver", and "RxForeachDoPar" or "dopar". 


 ### ` ...`
 any other arguments are passed to the class generator determined from `context`. 



 ## <a name="details"></a>Details

This is a wrapper to specific class generator functions for the RevoScaleR compute context classes. For example, the RxInSqlServer class uses function [RxInSqlServer](RxInSqlServer.md) as a generator. Therefore either `RxInSqlServer(...)` or `RxComputeContext("RxInSqlServer", ...)` will create an RxInSqlServer instance.


 ## <a name="value"></a>Value

A type of RxComputeContext compute context object. This object may be used to in [rxSetComputeContext](rxSetComputeContext.md) or [rxOptions](rxOptions.md) to set the compute context.

 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[RxComputeContext-class](RxComputeContext-class.md), [RxHadoopMR](RevoScaleR-deprecated.md), [RxSpark](RxSpark.md), [RxInSqlServer](RxInSqlServer.md), [RxLocalSeq](RxLocalSeq.md), [RxLocalParallel](RxLocalParallel.md), [RxForeachDoPar](RxForeachDoPar.md), [rxSetComputeContext](rxSetComputeContext.md), [rxOptions](rxOptions.md), [rxExec](rxExec.md).

 ## <a name="examples"></a>Examples

 ```

  # Setup to run analyses on a SQL Server
  ## Not run:


# Note: for improved security, read connection string from a file, such as
# connectionString <- readLines("connectionString.txt")

connectionString <- "Server=MyServer;Database=MyDatabase;UID=MyUser;PWD=MyPassword"
sqlQuery <- "WITH nb AS (SELECT 0 AS n UNION ALL SELECT n+1 FROM nb where n < 9) SELECT n1.n+10*n2.n+100*n3.n+1 AS n, ABS(CHECKSUM(NewId())) 

myServer <- RxComputeContext("RxInSqlServer",
        sqlQuery = sqlQuery, connectionString = connectionString)                 
rxSetComputeContext(computeContext = myServer )
 ## End(Not run) 
```



