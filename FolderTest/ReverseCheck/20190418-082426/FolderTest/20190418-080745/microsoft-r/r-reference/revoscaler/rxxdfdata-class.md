---
title: RxXdfData-class class (revoAnalytics) | Microsoft Docs
description: " Xdf data source connection class. "
keywords: (revoAnalytics), RxXdfData-class, colnames,RxXdfData-method, dim,RxXdfData-method, dimnames,RxXdfData-method, formula,RxXdfData-method, length,RxXdfData-method, names,RxXdfData-method, names<-,RxXdfData-method, row.names,RxXdfData-method, show,RxXdfData-method, str,RxXdfData-method, classes
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
ms.openlocfilehash: 29fc2a249184501d28a17ea7af73d4539cb07034
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxxdfdata-class-class-rxxdfdata"></a>RxXdfData-class: Class RxXdfData 
 ## <a name="description"></a>Description

Xdf data source connection class.


 ## <a name="generators"></a>Generators 


The targeted generator [RxXdfData](RxXdfData.md) as well as the general generator [rxNewDataSource](rxNew.md).

 ## <a name="extends"></a>Extends 


Class RxFileData, directly.
Class RxDataSource, by class RxFileData.


 ## <a name="methods"></a>Methods 




### `colnames`
`signature(x = "RxXdfData")`: ... 


### `dim`
`signature(x = "RxXdfData")`: ... 


### `dimnames`
`signature(x = "RxXdfData")`: ... 


### `formula`
`signature(x = "RxXdfData")`: ... 


### `length`
`signature(x = "RxXdfData")`: ... 


### `names`
`signature(x = "RxXdfData")`: ... 


### `names<-`
`signature(x = "RxXdfData")`: ... 


### `row.names`
`signature(x = "RxXdfData")`: ... 


### `show`
`signature(object = "RxXdfData")`: ... 


### `str`
`signature(object = "RxXdfData")`: ... 





 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[RxDataSource-class](RxDataSource-class.md), [RxXdfData](RxXdfData.md), [rxNewDataSource](rxNew.md)


 ## <a name="examples"></a>Examples

 ```

  DS <- RxXdfData(file.path(rxGetOption("sampleDataDir"), "fourthgraders.xdf"))
  head(DS)
  tail(DS)
  names(DS)
  dim(DS)
  dimnames(DS)
  nrow(DS)
  ncol(DS)
  str(DS)

  # formula examples
  formula(DS)
  formula(DS, varsToDrop = "male")
  formula(DS, depVar = "height")
  formula(DS, depVar = "height", inter = list(c("male", "eyecolor")))

  # summarize variables in data source
  summary(DS)

  # renaming variables in .xdf file via replacement method
  XDF <- file.path(tempdir(), "iris.xdf")
  rxDataStep(iris, XDF, overwrite = TRUE)
  irisDS <- RxXdfData(XDF)
  names(irisDS)
  names(irisDS) <- c("cow","horse","chicken","goat","squirrel")
  names(irisDS)
  if (file.exists(XDF)) file.remove(XDF)
```



