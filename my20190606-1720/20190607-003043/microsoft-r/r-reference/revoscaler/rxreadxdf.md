---
title: rxReadXdf function (revoAnalytics) | Microsoft Docs
description: " Read data from an .xdf file into a data frame. "
keywords: (revoAnalytics), rxReadXdf, file, connection
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
ms.openlocfilehash: fb9dfb2f66e1a6df8eab379df2a8a5be549e419f
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxreadxdf-read-xdf-file"></a>rxReadXdf: Read .xdf File 
 ## <a name="description"></a>Description

Read data from an .xdf file into a data frame.


 ## <a name="usage"></a>Usage

```   
  rxReadXdf(file, varsToKeep = NULL, varsToDrop = NULL, rowVarName = NULL,
            startRow = 1, numRows = -1, returnDataFrame = TRUE,
            stringsAsFactors = FALSE, maxRowsByCols = NULL,
            reportProgress = rxGetOption("reportProgress"), readByBlock = FALSE,
            cppInterp = NULL) 

```

 ## <a name="arguments"></a>Arguments



 ### `file`
 either an RxXdfData object or a character string specifying the .xdf file. 



 ### `varsToKeep`
 character vector of variable names to include when reading from the input data file. If `NULL`, argument is ignored. Cannot be used with `varsToDrop`. 



 ### `varsToDrop`
 character vector of variable names to exclude when reading from the input data file. If `NULL`, argument is ignored. Cannot be used with `varsToKeep`. 



 ### `rowVarName`
 optional character string specifying the variable in the data file to use as row names for the output data frame. 



 ### `startRow`
 starting row for retrieval. 



 ### `numRows`
 number of rows of data to retrieve. If -1, all are read. 



 ### `returnDataFrame`
 logical indicating whether or not to create a data frame. If `FALSE`, a list is returned. 



 ### `stringsAsFactors`
 logical indicating whether or not to convert strings into factors in R. 



 ### `maxRowsByCols`
 the maximum size of a data frame that will be read in, measured by the number of rows times the number of columns. If the numer of rows times the number of columns being extracted from the .xdf file exceeds this, a warning will be reported and a smaller number of rows will be read in than requested. If `maxRowsByCols` is set to be too large, you may experience problems  from loading a huge data frame into memory. To extract a subset of rows  and/or columns from an .xdf file, use [rxDataStep](rxDataStep.md). 



 ### `reportProgress`
 integer value with options:  
*   `0`: no progress is reported. 
*   `1`: the number of processed rows is printed and updated. 
*   `2`: rows processed and timings are reported. 
*   `3`: rows processed and all timings are reported. 




 ### `readByBlock`
 read data by blocks. This argument is deprecated. 



 ### `cppInterp`
 list of information sent to C++ interpreter. 



 ## <a name="value"></a>Value

if `returnDataFrame` is `TRUE`, a data frame is returned. Otherwise a list is returned.

 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxImport](rxImport.md), [rxDataStep](rxDataStep.md).

 ## <a name="examples"></a>Examples

 ```

  # Example reading the first 10 rows from the CensusWorkers xdf file
  censusWorkers <- file.path(rxGetOption("sampleDataDir"), "CensusWorkers")
  myCensusDF <- rxReadXdf(censusWorkers, numRows = 10)
  myCensusDF
```



