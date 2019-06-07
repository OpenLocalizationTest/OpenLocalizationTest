---
title: 'RevoScaleR-defunct function (RevoScaleR) '
description: " The functions or variables listed here are no longer part of RevoScaleR as they are no longer needed.  "
keywords: (RevoScaleR), RevoScaleR-defunct, rxGetVarInfoXdf, rxGetInfoXdf
author: heidisteen
manager: cgronlun
ms.date: 09/07/2017
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
ms.openlocfilehash: 6259528470749e2fd69b05cd63a64b92e1ea3050
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="revoscaler-defunct-defunct-functions-in-revoscaler"></a>RevoScaleR-defunct: Defunct functions in RevoScaleR 
 ## <a name="description"></a>Description
 
The functions or variables listed here are no longer part of RevoScaleR as they are no longer needed. 
 
 
 ## <a name="usage"></a>Usage

```   
                  
  rxGetVarInfoXdf(file, getValueLabels = TRUE, varsToKeep = NULL,
                  varsToDrop = NULL, computeInfo = FALSE) 
                  
  rxGetInfoXdf(file, getVarInfo = FALSE, getBlockSizes = FALSE,
               getValueLabels = NULL, varsToKeep = NULL, varsToDrop = NULL,
               startRow = 1, numRows = 0, computeInfo = FALSE, verbose = 0)                 
                  
 
```
 
 ## <a name="arguments"></a>Arguments

   
    
 ### `file`
 either an RxXdfData object or a character string specifying the .xdf file. If a local compute context is being used, this argument may also be a list of data sources,  in which case the output will be returned in a named list. See the details section for more information. 
  
  
    
 ### `getValueLabels`
 logical value. If `TRUE`, value labels (including factor  levels) are included in the output if present. 
  
  
    
 ### `getVarInfo`
 logical value. If `TRUE`, variable information is returned. 
  
  
    
 ### `getBlockSizes`
 logical value. If `TRUE`, block sizes are returned in the output for an .xdf file, and when printed the first 10 block sizes are shown. 
  
  
    
 ### `varsToKeep`
 character vector of variable names for which information is returned. If `NULL`, argument is ignored. Cannot be used with `varsToDrop`. 
  
  
    
 ### `varsToDrop`
 character vector of variable names for which information is not returned. If `NULL`, argument is ignored. Cannot be used with `varsToKeep`. 
  
  
    
 ### `startRow`
 starting row for retrieval of data if a data frame or .xdf file. 
  
  
    
 ### `numRows`
 number of rows of data to retrieve if a data frame or .xdf file. 
  
  
    
 ### `computeInfo`
 logical value. If `TRUE`,  variable information  (e.g., high/low values) for non-xdf data sources will be computed  by reading through the data set. 
  
  
    
 ### `verbose`
 integer value. If `0`, no additional output is printed.  If `1`, additional summary information is printed for an .xdf file. 
  
 
 
 ## <a name="details"></a>Details
 
[rxGetVarInfo](rxGetVarInfoXdf.md) should be used instead of `rxgetvarinfo`.
[rxGetInfo](rxGetInfoXdf.md) should be used instead of `rxGetInfoXdf`.
 
 

 
 
 
 ## <a name="see-also"></a>See Also
 
[rxGetVarInfo](rxgetvarinfo.md), [rxGetInfo](rxGetInfoXdf.md), [RevoScaleR-deprecated](RevoScaleR-deprecated.md).
   
