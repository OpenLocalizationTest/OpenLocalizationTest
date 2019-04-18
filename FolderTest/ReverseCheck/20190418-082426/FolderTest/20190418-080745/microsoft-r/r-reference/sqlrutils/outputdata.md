---
title: OutputData function (sqlrutils) | Microsoft Docs
description: " OutputData: generates an OutputData Object that captures the information about the data frame that needs to be returned after the execution of the R function embedded into the stored procedure. This object must be created if the R function is returning a named list, where one of the items in the list is a data frame. The return list can contain at most one data frame. "
keywords: (sqlrutils), OutputData
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
ms.openlocfilehash: 1cd334eac6bed9f446fa979ffb8de1b953e02e18
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="outputdata-output-data-for-sql-stored-procedure-class-generator"></a>OutputData: Output Data for SQL Stored Procedure: Class Generator 
 ## <a name="description"></a>Description

`OutputData`: generates an OutputData Object that captures the information about the data frame that needs to be returned after the execution of the R function embedded into the stored procedure.
This object must be created if the R function is returning a named list, where one of the items in the list is a data frame. The return list can contain at most one data frame.


 ## <a name="usage"></a>Usage

```   
  OutputData(name)

```

 ## <a name="arguments"></a>Arguments



 ### `name`
 A character string, the name of the data frame variable. 



 ## <a name="value"></a>Value

OutputData Object

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

  # See ?StoredProcedure for creating the "cleandata" table.

  # train 2 takes a data frame with clean data and outputs a model
  # as well as the data on the basis of which the model was built
  train2 <- function(in_df) {
  in_df[,"DayOfWeek"] <- factor(in_df[,"DayOfWeek"], levels=c("Monday","Tuesday","Wednesday","Thursday","Friday","Saturday","Sunday"))
    # The model formula
    formula <- ArrDelay ~ CRSDepTime + DayOfWeek + CRSDepHour:DayOfWeek
    # Train the model
    rxSetComputeContext("local")
    mm <- rxLinMod(formula, data=in_df, transformFunc=NULL, transformVars=NULL)
    mm <- rxSerializeModel(mm)
    return(list(mm = mm, in_df = in_df))
  }
  # create InpuData Object for an input parameter that is a data frame
  # note: if the input parameter is not a data frame use InputParameter object
  id <- InputData(name = "in_df",
                  defaultQuery = paste0("select top 10000 ArrDelay,CRSDepTime,",
                                        "DayOfWeek,CRSDepHour from cleanData"))
  out1 <- OutputData("in_df")
  # create an OutputParameter object for the variable "mm" inside the return list
  out2 <- OutputParameter("mm", "raw")
  # connections string
  conStr <- paste0("Driver={ODBC Driver 13 for SQL Server};Server=.;Database=RevoTestDB;",
                   "Trusted_Connection=Yes;")
  # create the stored procedure object
  sp_df_op <- StoredProcedure(train2, "spTest2", id, out1, out2,
                          filePath = ".")

  registerStoredProcedure(sp_df_op, conStr)
  result <- executeStoredProcedure(sp_df_op, connectionString = conStr)
  # Get back the linear model.
  mm <- rxUnserializeModel(result$params$op1)
 ## End(Not run) 
```

