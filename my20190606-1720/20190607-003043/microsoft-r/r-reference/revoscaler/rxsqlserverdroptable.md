---
title: rxSqlServerDropTable function (revoAnalytics) | Microsoft Docs
description: " Execute a SQL statement that drops a table or checks for existence. "
keywords: (revoAnalytics), rxSqlServerDropTable, rxSqlServerTableExists, file
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
ms.openlocfilehash: adf28eb5da6dc2d5d74614a45cc86d83f53eafde
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxsqlserverdroptable--rxsqlserverdroptable"></a>rxSqlServerDropTable:  rxSqlServerDropTable  
 ## <a name="description"></a>Description

Execute a SQL statement that drops a table or checks for existence.


 ## <a name="usage"></a>Usage

```   
  rxSqlServerTableExists(table, connectionString = NULL)
  rxSqlServerDropTable(table, connectionString = NULL)

```


 ## <a name="arguments"></a>Arguments



 ### `table`
  character string specifying a table name or an [RxSqlServerData](RxSqlServerData.md)data source that has the `table` specified.  



 ### `connectionString`
 `NULL` or character string specifying the connection string.  If `NULL`, the connection string from the currently  active compute context will be used if available.  



 ### ` ...`
  Additional arguments to be passed through.  




 ## <a name="details"></a>Details

An SQL query is passed to the ODBC driver.


 ## <a name="value"></a>Value

`rxSqlServerTableExists` returns `TRUE` is the table exists, `FALSE` otherwise.
`rxSqlServerDropTable` returns `TRUE` is the table is successfully dropped, `FALSE` otherwise (for example, if the table did not exist).


 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)





 ## <a name="see-also"></a>See Also

[RxInSqlServer](RxInSqlServer.md), [RxSqlServerData](RxSqlServerData.md).

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

# With an RxInSqlServer active compute context
tempTable <- "rxTempTest"
if (rxSqlServerTableExists(tempTable)) rxSqlServerDropTable(tempTable)
 ## End(Not run) 
```




