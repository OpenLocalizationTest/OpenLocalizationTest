---
title: rxNewDataSource function (revoAnalytics) | Microsoft Docs
description: " This is the main generator for RxDataSource S4 classes. "
keywords: (revoAnalytics), rxNewDataSource, rxNewDataSource,character-method, file, connection
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
ms.openlocfilehash: f661800ec465764cb848051f1f1edbcfc1c0cd97
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxnewdatasource-revoscaler-data-sources-class-generator"></a>rxNewDataSource: RevoScaleR Data Sources: Class Generator 
 ## <a name="description"></a>Description

This is the main generator for RxDataSource S4 classes.


 ## <a name="usage"></a>Usage

```   
 ## S4 method for class `character':
rxNewDataSource  (name, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `name`
 character name of the specific class to instantiate. 


 ### ` ...`
 any other arguments are passed to the class generator `name`. 



 ## <a name="details"></a>Details

This is a wrapper to specific class generator functions for the RCE data source classes. For example, the RxXdfData class uses function [RxXdfData](RxXdfData.md) as a generator. Therefore either `RxXdfData(...)` or `rxNewDataSource("RxXdfData", ...)` will create an RxXdfData instance.


 ## <a name="value"></a>Value

RxDataSource data source object. This object may be used to open and close the actual RevoScaleR data sources.

 ## <a name="side-effects"></a>Side Effects 


This function creates the data source instance in the Microsoft R Services Compute Engine, but does not actually open the data. The methods [rxOpen](rxOpen-methods.md) and [rxClose](rxOpen-methods.md) will open and close the data.

 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[RxXdfData](RxXdfData.md), [RxTextData](RxTextData.md), [RxSasData](RxSasData.md), [RxSpssData](RxSpssData.md), [RxOdbcData](RxOdbcData.md), [RxTeradata](RxTeradata.md), [rxOpen](rxOpen-methods.md), [rxReadNext](rxOpen-methods.md).

 ## <a name="examples"></a>Examples

 ```

  fileName <- file.path(rxGetOption("sampleDataDir"), "claims.xdf")
  ds <- rxNewDataSource("RxXdfData", fileName)
  rxOpen(ds)
  myData <- rxReadNext(ds)
  rxClose(ds)
```



