---
title: registerStoredProcedure function (sqlrutils) | Microsoft Docs
description: " registerStoredProcedure: Uses the StoredProcedure object to register the stored procedure with the specified database "
keywords: (sqlrutils), registerStoredProcedure
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
ms.openlocfilehash: 19fb3f281aee45943855f18dc34e0135c4dac1d2
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="registerstoredprocedure-register-a-sql-stored-procedure-with-a-database"></a>registerStoredProcedure: Register a SQL Stored Procedure with a Database 
 ## <a name="description"></a>Description

`registerStoredProcedure`: Uses the StoredProcedure object to register the stored procedure with the specified database


 ## <a name="usage"></a>Usage

```   
  registerStoredProcedure(sqlSP, connectionString = NULL)

```

 ## <a name="arguments"></a>Arguments



 ### `sqlSP`
 a valid StoredProcedure object 



 ### `connectionString`
 A character string (must be provided if the StoredProcedure object was created without a connection string) 



 ## <a name="value"></a>Value

TRUE on success, FALSE on failure

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

 # See ?StoredProcedure for creating the "cleandata" table.

 # train 1 takes a data frame with clean data and outputs a model
 train1 <- function(in_df) {
  in_df[,"DayOfWeek"] <- factor(in_df[,"DayOfWeek"], levels=c("Monday","Tuesday","Wednesday","Thursday","Friday","Saturday","Sunday"))
  # The model formula
  formula <- ArrDelay ~ CRSDepTime + DayOfWeek + CRSDepHour:DayOfWeek
  # Train the model
  rxSetComputeContext("local")
  mm <- rxLinMod(formula, data=in_df)
  mm <- rxSerializeModel(mm)
  return(list("mm" = mm))
 }
 # create InpuData Object for an input parameter that is a data frame
 # note: if the input parameter is not a data frame use InputParameter object
 id <- InputData(name = "in_df",
               defaultQuery = paste0("select top 10000 ArrDelay,CRSDepTime,",
                                     "DayOfWeek,CRSDepHour from cleanData"))

 # create an OutputParameter object for the variable inside the return list
 # note: if that variable is a data frame use OutputData object
 out <- OutputParameter("mm", "raw")

 # connections string
 conStr <- paste0("Driver={ODBC Driver 13 for SQL Server};Server=.;Database=RevoTestDB;",
                 "Trusted_Connection=Yes;")
 # create the stored procedure object
 sp_df_op <- StoredProcedure("train1", "spTest1", id, out,
                        filePath = ".")
 # register the stored procedure with the database
 registerStoredProcedure(sp_df_op, conStr)
 model <- executeStoredProcedure(sp_df_op, connectionString = conStr)

 # Getting back the model by unserializing it.
 mm <- rxUnserializeModel(model$params$op1)
 ## End(Not run) 
```

