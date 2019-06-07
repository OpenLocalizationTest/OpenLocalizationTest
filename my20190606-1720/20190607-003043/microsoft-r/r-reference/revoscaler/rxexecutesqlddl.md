---
title: rxExecuteSQLDDL function (revoAnalytics) | Microsoft Docs
description: " Execute a command to define, manipulate, or control SQL data (but not  return data). "
keywords: '(revoAnalytics), rxExecuteSQLDDL, rxExecuteSQLDDL,RxDataSource-method,  ~kwd1 ,  ~kwd2 '
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
ms.openlocfilehash: d3a5910975ae22d8e3c9d4c658501108ca6d38be
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxexecutesqlddl--execute-sql-command-for-data-manipulation-definition-or-control"></a>rxExecuteSQLDDL:  Execute SQL Command for Data Manipulation, Definition, or Control  
 ## <a name="description"></a>Description

Execute a command to define, manipulate, or control SQL data (but not return data).


 ## <a name="usage"></a>Usage

```   
  rxExecuteSQLDDL(src, ...)

```


 ## <a name="arguments"></a>Arguments



 ### `src`
  An RxOdbcData data source.  


 ### ` ...`
  Additional arguments, typically `sSQLString=` supplied with a character string specifying the SQL command to be executed. The typical SQL commands are `CREATE TABLE` and `DROP TABLE`.  




 ## <a name="value"></a>Value

Returns `NULL`; executed for its side-effect (the manipulation of the SQL data source).


 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)





 ## <a name="see-also"></a>See Also

[RxOdbcData](RxOdbcData.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:


# Note: for improved security, read connection string from a file, such as
# conString <- readLines("conString.txt")

conString <- "Driver=Teradata;DBCNAME=myDb;Database=test;Uid=tester;pwd=pwd;"
outOdbcDS <- RxOdbcData(table = "MyClaims",           
                        connectionString = conString,
                        useFastRead=TRUE)                           
rxOpen(outOdbcDS, "w")                       
rxExecuteSQLDDL(outOdbcDS, sSQLString = paste("CREATE TABLE [MyClaims]([RowNum] [int] NULL, [age] [char](5) NULL, ",
        "[car_age] [char](3) NULL, [type] [char](1) NULL, ", " [cost] [float] NULL, [number] [float] NULL);", sep=""))
inTextData <- RxTextData(file = file.path(rxGetOption("sampleDataDir"), "claims.txt"),
                        stringsAsFactors = TRUE, useFastRead = TRUE)
outOdbcDS <- RxOdbcData(table = "MyClaims",           
                        connectionString = conString,
                        useFastRead=TRUE)                           
rxDataStep(inData = inTextData, outFile = outOdbcDS)   
   ## End(Not run) 
```





