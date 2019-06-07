---
title: rxGetVarNames function (revoAnalytics) | Microsoft Docs
description: " Read the variable names for data source or data frame "
keywords: (revoAnalytics), rxGetVarNames, attribute
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
ms.openlocfilehash: 55f7283c78e8984062b7af0add0cdc2a4613a5c3
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxgetvarnames-variable-names-for-a-data-source-or-data-frame"></a>rxGetVarNames: Variable names for a data source or data frame 
 ## <a name="description"></a>Description

Read the variable names for data source or data frame


 ## <a name="usage"></a>Usage

```   
  rxGetVarNames(data)

```

 ## <a name="arguments"></a>Arguments



 ### `data`
 an `RxDataSource` object, a character string specifying the .xdf file, or a data frame. 



 ## <a name="details"></a>Details

If colInfo is used in the data source to specify new column names, these new names will be used in the return value.


 ## <a name="value"></a>Value

character vector containing the names of the variables in the data source or data frame.

 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxGetVarInfo](rxGetVarInfo.md), [rxSetVarInfo](rxSetVarInfoXdf.md), [rxDataStep](rxDataStep.md), [rxGetInfo](rxGetInfoXdf.md).

 ## <a name="examples"></a>Examples

 ```

  # Specify name and location of sample data file
  censusWorkers <- file.path(rxGetOption("sampleDataDir"), "CensusWorkers")

  # Get the variable names
  varNames <- rxGetVarNames(censusWorkers)

  # Print the variable names
  varNames
```


