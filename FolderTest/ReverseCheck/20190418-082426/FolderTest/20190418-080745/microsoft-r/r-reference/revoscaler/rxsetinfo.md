---
title: rxSetInfo function (revoAnalytics) | Microsoft Docs
description: " Set .xdf file or data frame information, such as a description "
keywords: '(revoAnalytics), rxSetInfo,  attribute '
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
ms.openlocfilehash: 9724663f833f72e214cfba0e9f7ee75a5435e750
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxsetinfo--set-info-such-as-a-description"></a>rxSetInfo:  Set info such as a description  
 ## <a name="description"></a>Description

Set .xdf file or data frame information, such as a description


 ## <a name="usage"></a>Usage

```   
  rxSetInfo(data, description = "")
  rxSetInfoXdf(file, description = "")

```


 ## <a name="arguments"></a>Arguments



 ### `data`
  An .xdf file name, an [RxXdfData](RxXdfData.md) object, or a data frame.  


 ### `file`
  An .xdf file name or an [RxXdfData](RxXdfData.md) object  



 ### `description`
  character string containing the file or data frame description  



 ## <a name="value"></a>Value

An [RxXdfData](RxXdfData.md) object representing the .xdf file, or a new data frame with the `.rxDescription` attribute set to the specified `description`.

 ## <a name="see-also"></a>See Also

[rxGetInfo](rxGetInfoXdf.md).


 ## <a name="examples"></a>Examples

 ```


  # Create a sample data frame and .xdf file
  outFile <- tempfile(pattern= ".rxTempFile", fileext = ".xdf")
  if (file.exists(outFile)) file.remove(outFile)

  origData <- data.frame(x=1:10)
  rxDataStep(inData = origData, outFile = outFile, rowsPerRead = 5)

  # Set a description in the data file
  myDescription <- "Hello Data File!"
  rxSetInfo( data = outFile, description = myDescription)
  rxGetInfo(outFile)

  # Read a data frame out of the output file    
  myData <- rxDataStep(outFile )
  # Look at its attribute
  attr(myData, ".rxDescription")    

  file.remove(outFile)

  myNewDescription = "Good-by data."
  myData <- rxSetInfo(data=myData, description = myNewDescription)
  rxGetInfo(myData)
```




