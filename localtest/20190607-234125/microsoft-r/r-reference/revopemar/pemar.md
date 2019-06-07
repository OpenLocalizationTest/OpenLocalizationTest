---
title: " RevoPemaR: Parallel External Memory Algorithms in R "
description: A package that provides a framework for creating Parallel External Memory Algorithms in R using R Reference Classes.
keywords: RevoPemaR, RevoPemaR-package, package
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 01/29/2018
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ms.openlocfilehash: 2daebbced0a0ca958f14f121b95a1eb2d43774d3
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="revopemar-package"></a>RevoPemaR package

The **RevoPemaR** package provides a framework for creating Parallel External Memory Algorithms in R using R Reference Classes.

| Package details | |
|--------|-|
| Current version: |  10.0.0 |
| Built on: | R 3.2.2 |
| Package distribution: | [Machine Learning Server (Hadoop)](../../install/machine-learning-server-hadoop-install.md)  

 
## <a name="how-to-use-revopemar"></a>How to use RevoPemaR

When used with the **RevoScaleR** package, analyses can be distributed automatically on Hadoop clusters using Cloudera's CDH or Hortonworks' HDP. For more information, see [Get started with PemaR functions in Microsoft R](https://msdn.microsoft.com/microsoft-r/pemar-getting-started).

In an R session, load **RevoPemaR** from the command line by typing`library(RevoPemaR)`.

> [!Note]
> You can load this library on computer that does not have Hadoop (for example, on an R Client instance) if you change the compute context to Hadoop MapReduce or Spark and execute the code in that compute context.

## <a name="function-list"></a>Function list

|Class | Description |
|------|-------------|
|[PemaBaseClass](pemabaseclass-class.md) |A base reference class generator for parallel external memory algorithms.|
|[setPemaClass](setpemaclass.md)|Returns a generator function for creating a parallel external memory algorithm reference class.|
|[pemaCompute](pemacompute.md) |Estimates a parallel external memory algorithm as described by a PEMA reference class object. |

## <a name="next-steps"></a>Next steps

Add R packages to your computer by running setup for R Server or R Client: 

+ [R Client](../../r-client/what-is-microsoft-r-client.md) 
+ [R Server](../../what-is-microsoft-r-server.md)

## <a name="see-also"></a>See also

 [Package Reference](../introducing-r-server-r-package-reference.md)    