---
title: rxFindPackage function (revoAnalytics) | Microsoft Docs
description: " Find the path for one or more packages for a compute context. "
keywords: (revoAnalytics), rxFindPackage, packages, sql, install, uninstall, remove, use
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
ms.openlocfilehash: ccbd6a268518f8fd2ccfb94944f54773708ecf7e
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxfindpackage-find-packages-for-compute-context"></a>rxFindPackage: Find Packages for Compute Context 
 ## <a name="description"></a>Description

Find the path for one or more packages for a compute context.


 ## <a name="usage"></a>Usage

```   

  rxFindPackage(package, computeContext = NULL, allNodes = FALSE, lib.loc = NULL, quiet = TRUE,
               verbose = getOption("verbose"))


```

 ## <a name="arguments"></a>Arguments




 ### `package`
 character vector of name(s) of packag(es). 



 ### `computeContext`
 an [RxComputeContext](RxComputeContext.md) or equivalent character string or `NULL`.   If set to the default of `NULL`, the currently active compute context is used. Supported compute contexts are [RxInSqlServer](RxInSqlServer.md) and [RxLocalSeq](RxLocalSeq.md). 



 ### `allNodes`
 logical 



 ### `lib.loc`
 a character vector describing the location of R library trees to search through, or `NULL`.  The default value of `NULL` corresponds to checking the loaded namespace, then all libraries currently known in  `.libPaths()`. In [RxInSqlServer](RxInSqlServer.md) only `NULL` is supported. 



 ### `quiet`
 logical. If `FALSE`, warnings or an error is given if the package is not found. 



 ### `verbose`
 logical. If `TRUE`, additional diagnostics are printed if available. 



 ## <a name="details"></a>Details

This is a wrapper for find.package. See the help file for additional details.



 ## <a name="value"></a>Value

A character vector of paths of package directories. If using a distributed compute context with the `allNodes` set to `TRUE`, a list of lists with a character vector of paths from each node will be returned.   



 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxPackage](rxPackage.md), find.package, [rxInstalledPackages](rxInstalledPackages.md), [rxInstallPackages](rxInstallPackages.md),   
[rxRemovePackages](rxRemovePackages.md), [rxSyncPackages](rxSyncPackages.md), [rxSqlLibPaths](rxSqlLibPaths.md),   
require

 ## <a name="examples"></a>Examples

 ```

  #
  # Find the paths for the RevoScaleR and lattice packages
  #
  packagePaths <- rxFindPackage(package = c("RevoScaleR", "lattice"))
  packagePaths

  ## Not run:

#
# Find the path of the RevoScaleR package on a SQL Server compute context
#
sqlServerCompute <- RxInSqlServer(connectionString = 
    "Driver=SQL Server;Server=myServer;Database=TestDB;Uid=myID;Pwd=myPwd;")
sqlPackagePaths <- rxFindPackage(package = "RevoScaleR", computeContext = sqlServerCompute)
 ## End(Not run) 
```








