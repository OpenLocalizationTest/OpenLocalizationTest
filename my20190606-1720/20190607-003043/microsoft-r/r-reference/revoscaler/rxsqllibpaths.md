---
title: rxSqlLibPaths function (revoAnalytics) | Microsoft Docs
description: " Gets the search path for the library trees for packages while executing inside the SQL Server, using [RxInSqlServer](RxInSqlServer.md) compute context or using T-SQL script with sp_execute_external_script stored procedure with embedded R script. "
keywords: (revoAnalytics), rxSqlLibPaths, use, packages, sql, install, uninstall, remove
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
ms.openlocfilehash: 7ac58ca27959cc6925c57e904d957619acbdf85b
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxsqllibpaths-search-paths-for-packages-in-sql-compute-context"></a>rxSqlLibPaths: Search Paths for Packages in SQL compute context 
 ## <a name="description"></a>Description

Gets the search path for the library trees for packages while executing inside the SQL Server, using [RxInSqlServer](RxInSqlServer.md) compute context or using T-SQL script with sp_execute_external_script stored procedure with embedded R script.


 ## <a name="usage"></a>Usage

```   
  rxSqlLibPaths(connectionString)

```

 ## <a name="arguments"></a>Arguments




 ### `connectionString`
 a `character` connection string for the SQL Server. This should be a local connection string (external connection strings are not supported while executing on a SQL Server). You can also specify [RxInSqlServer](RxInSqlServer.md) compute context object for input, from which the connection string will be extracted and used.  



 ## <a name="details"></a>Details

For [RxInSqlServer](RxInSqlServer.md) compute context, a user specified on the connection string must be a member of one of the following roles `'db_owner'` `'rpkgs-shared'`,  `'rpkgs-private'` or `'rpkgs-private'` in the database. When rxExec() function is called from a client machine with [RxInSqlServer](RxInSqlServer.md) compute context to execute the rx function on SQL Server, the `.libPaths()` is automatically updated to include the library paths returned by this [rxSqlLibPaths](rxSqlLibPaths.md) function.



 ## <a name="value"></a>Value
A character vector of the library paths containing both `"shared"` or `"private"` scope of the packages if the user specified in the connection string is allowed access. On access denied, it returns an empty character vector.


 ## <a name="see-also"></a>See Also

[rxPackage](rxPackage.md), .libPaths, [rxFindPackage](rxFindPackage.md), [rxInstalledPackages](rxInstalledPackages.md), [rxInstallPackages](rxInstallPackages.md),   
[rxRemovePackages](rxRemovePackages.md), [rxSyncPackages](rxSyncPackages.md), require

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

#
# An example sp_execute_external_script T-SQL code using rxSqlLibPaths()
#
declare @instance_name nvarchar(100) = @@SERVERNAME, @database_name nvarchar(128) = db_name();
exec sp_execute_external_script 
  @language = N'R',
  @script = N'
    connStr <- paste("Driver=SQL Server;Server=", instance_name, ";Database=", database_name, ";Trusted_Connection=true;", sep="");
    .libPaths(rxSqlLibPaths(connStr));
    print(.libPaths());
  ', 
  @input_data_1 = N'', 
  @params = N'@instance_name nvarchar(100), @database_name nvarchar(128)',
  @instance_name = @instance_name, 
  @database_name = @database_name;

 ## End(Not run) 
```








