---
title: RxDataSource-class class (revoAnalytics) | Microsoft Docs
description: "   Base class for all Microsoft R Services Compute Engine data sources.   "
keywords: (revoAnalytics), RxDataSource-class, names,RxDataSource-method, show,RxDataSource-method, classes
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
ms.openlocfilehash: 58199bfc36724634108dd7cf389c64abc7628d78
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxdatasource-class-class-rxdatasource"></a>RxDataSource-class: Class RxDataSource 
 ## <a name="description"></a>Description

Base class for all Microsoft R Services Compute Engine data sources.  


 ## <a name="objects-from-the-class"></a>Objects from the Class 


A virtual class: No objects may be created from it.

 ## <a name="generator"></a>Generator 


The generator for classes that extend RxDataSource is [rxNewDataSource](rxNew.md).  

 ## <a name="methods"></a>Methods 


The following methods are defined for classes that extend RxDataSource:



### `names`
`signature(x = "RxDataSource")`: ... 


### `[rxOpen](rxOpen-methods.md)`
`signature(src = "RxDataSource")`: ... 


### `[rxClose](rxOpen-methods.md)`
`signature(src = "RxDataSource")`: ... 


### `[rxReadNext](rxOpen-methods.md)`
`signature(src = "RxDataSource")`: ... 


### `[rxWriteNext](rxOpen-methods.md)`
`signature(from = "data.frame", to = "RxDataSource", verbose = 0)`: ... 




 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[RxXdfData-class](RxXdfData-class.md), [RxXdfData](RxXdfData.md), [RxTextData](RxTextData.md), [RxSasData](RxSasData.md), [RxSpssData](RxSpssData.md), [RxOdbcData](RxOdbcData.md), [RxTeradata](RxTeradata.md), [rxNewDataSource](rxNew.md), [rxOpen](rxOpen-methods.md), [rxReadNext](rxOpen-methods.md), [rxWriteNext](rxOpen-methods.md).

 ## <a name="examples"></a>Examples

 ```

  fileName <- file.path(rxGetOption("sampleDataDir"), "claims.xdf")
  ds <- rxNewDataSource("RxXdfData", fileName)
  is(ds, "RxXdfData")
  # [1] TRUE
  is(ds, "RxDataSource")
  # [1] TRUE
```


