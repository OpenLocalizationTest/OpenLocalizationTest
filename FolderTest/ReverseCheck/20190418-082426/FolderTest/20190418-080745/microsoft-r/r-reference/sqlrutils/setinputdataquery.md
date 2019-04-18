---
title: setInputDataQuery function (sqlrutils) | Microsoft Docs
description: " setInputDataQuery: assigns a query to the InputData parameter of the                  stored procedure that is going to populate the input                  data frame of the embedded R function in the next                  run of the stored procedure. "
keywords: (sqlrutils), setInputDataQuery
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
ms.openlocfilehash: e265c9afb77a5fcf4bd376795c2050d752d1385c
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="setinputdataquery-assign-a-query-to-the-input-data-parameter-of-the-sql-stored-procedure"></a>setInputDataQuery: Assign a Query to the Input Data Parameter of the SQL Stored Procedure 
 ## <a name="description"></a>Description

`setInputDataQuery`: assigns a query to the InputData parameter of the stored procedure that is going to populate the input data frame of the embedded R function in the next run of the stored procedure.


 ## <a name="usage"></a>Usage

```   
  setInputDataQuery(inputData, query)

```

 ## <a name="arguments"></a>Arguments



 ### `inputData`
 A character string, the name of the data frame input parameter into the R function. 



 ### `query`
 A character string representing a query. 



 ## <a name="value"></a>Value

InputData Object

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
  name <- InputParameter("predVarName", "character")
  sp_df_df <- StoredProcedure(score1, "sTest", id, model, name,
                          filePath = ".")
  # register the stored procedure with a database
  registerStoredProcedure(sp_df_df, conStr)
  # assign a different query to the InputData so that it only uses the firt 10 rows
  id <- setInputDataQuery(id, "SELECT top 10 * from cleanData")
  # assign a value to the name parameter
  name <- setInputParameterValue(name, "ArrDelayEstimate")
  # execute the stored procedure
  model <- executeStoredProcedure(sp_df_df, id, name, connectionString = conStr)
  model$data
 ## End(Not run) 
```

