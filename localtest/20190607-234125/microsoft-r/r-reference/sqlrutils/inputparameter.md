---
title: InputParameter function (sqlrutils) | Microsoft Docs
description: " InputParameter: generates an InputParameter Object, that captures the information about the input parameters of the R function that is to be embedded into a SQL Server Stored Procesure. Those will become the input parameters of the stored procedure. Supported R types of the input parameters are POSIXct, numeric, character, integer, logical, and raw. "
keywords: (sqlrutils), InputParameter
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
ms.openlocfilehash: dfd432e54789107d06c2eb8a08305d96b6212bbd
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="inputparameter-input-parameter-for-sql-stored-procedure-class-generator"></a>InputParameter: Input Parameter for SQL Stored Procedure: Class Generator 
 ## <a name="description"></a>Description

`InputParameter`: generates an InputParameter Object, that captures the information about the input parameters of the R function that is to be embedded into a SQL Server Stored Procesure. Those will become the input parameters of the stored procedure. Supported R types of the input parameters are POSIXct, numeric, character, integer, logical, and raw.


 ## <a name="usage"></a>Usage

```   
  InputParameter(name, type, defaultValue = NULL, defaultQuery = NULL,
  value = NULL, enableOutput = FALSE)

```

 ## <a name="arguments"></a>Arguments



 ### `name`
 A character string, the name of the input parameter object. 



 ### `type`
 A character string representing the R type of the input parameter object. 



 ### `defaultValue`
 Default value of the parameter. Not supported for "raw". 



 ### `defaultQuery`
 A character string specifying the default query that will retrieve the data if a different query is not provided at the time of the execution of the stored procedure. 



 ### `value`
 A value that will be used for the parameter in the next run of the stored procedure. 



 ### `enableOutput`
 Make this an Input/Output Parameter 



 ## <a name="value"></a>Value

InputParameter Object

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

  # See ?StoredProcedure for creating the `cleandata` table.
  # and ?executeStoredProcedure for creating the `rdata` table. 

  # score1 makes a batch prediction given clean data(indata),
  # model object(model_param), and the new name of the variable
  # that is being predicted
  score1 <- function(indata, model_param, predVarName) {
  indata[,"DayOfWeek"] <- factor(indata[,"DayOfWeek"], levels=c("Monday","Tuesday","Wednesday","Thursday","Friday","Saturday","Sunday"))
  # The connection string
  conStr <- paste("Driver={ODBC Driver 13 for SQL Server};Server=.;Database=RevoTestDB;",
                  "Trusted_Connection=Yes;", sep = "")
  # The compute context
  computeContext <- RxInSqlServer(numTasks=4, connectionString=conStr)
  mm <- rxReadObject(as.raw(model_param))
  # Predict
  result <- rxPredict(modelObject = mm,
                      data = indata,
                      outData = NULL,
                      predVarNames = predVarName,
                      extraVarsToWrite = c("ArrDelay"),
                      writeModelVars = TRUE,
                      overwrite = TRUE)
}
# connections string
conStr <- paste0("Driver={ODBC Driver 13 for SQL Server};Server=.;Database=RevoTestDB;",
                 "Trusted_Connection=Yes;")
# create InpuData Object for an input parameter that is a data frame
id <- InputData(name = "indata", defaultQuery = "SELECT * from cleanData")
# InputParameter for the model_param input variable
model <- InputParameter("model_param", "raw",
                        defaultQuery =
                          "select top 1 value from rdata where [key] = 'linmod.v1'")
# InputParameter for the predVarName variable
name <- InputParameter("predVarName", "character", value = "ArrDelayEstimate")
sp_df_df <- StoredProcedure(score1, "sTest", id, model, name,
                        filePath = ".")
 ## End(Not run) 
```

