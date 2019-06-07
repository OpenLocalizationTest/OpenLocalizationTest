---
title: RxDataSource function (revoAnalytics) | Microsoft Docs
description: " A generator for RxDataSource S4 classes. "
keywords: (revoAnalytics), RxDataSource, file, connection
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
ms.openlocfilehash: be8547d5d8cac02a17b339a0480fc5e0e6533023
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxdatasource-revoscaler-data-source-class-generator"></a>RxDataSource: RevoScaleR Data Source: Class Generator 
 ## <a name="description"></a>Description

A generator for RxDataSource S4 classes.


 ## <a name="usage"></a>Usage

```   
    RxDataSource( class = NULL, dataSource = NULL,  ...)

```

 ## <a name="arguments"></a>Arguments



 ### `class`
 an optional character string specifying class name of the data source to be created, such as [RxTextData](RxTextData.md), [RxSpssData](RxSpssData.md), [RxSasData](RxSasData.md), [RxOdbcData](RxOdbcData.md), or [RxTeradata](RxTeradata.md). If the class of the input dataSource differs from `class`, contents of overlapping slots will be copied from the input data source to the  newly constructed data source. 


 ### `dataSource`
 an optional data source object to be cloned. 


 ### ` ...`
 any other arguments to be applied to the newly constructed data source. 



 ## <a name="details"></a>Details

If `class` is specified, the returned object will be of that class.
If not, the returned object will have the class of `dataSource`.
If both `class` and `dataSource` are specified, the contents of matching slots will be copied from the input `dataSource` to the output object. Additional arguments will then be applied.


 ## <a name="value"></a>Value

A type of RxDataSource data source object.

 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[RxDataSource-class](RxDataSource-class.md), [RxTextData](RxTextData.md), [RxSqlServerData](RxSqlServerData.md), [RxSpssData](RxSpssData.md), [RxSasData](RxSasData.md), [RxOdbcData](RxOdbcData.md), [RxTeradata](RxTeradata.md), [RxXdfData](RxXdfData.md).

 ## <a name="examples"></a>Examples

 ```


    claimsSpssName <- file.path(rxGetOption("sampleDataDir"), "claims.sav")
    claimsTextName <- file.path(rxGetOption("sampleDataDir"), "claims.txt")
    claimsColInfo <- list( 
        age = list(type = "factor", 
            levels = c("17-20", "21-24", "25-29", "30-34", "35-39", "40-49", "50-59", "60+")), 
            car.age = list(type = "factor", levels = c("0-3", "4-7", "8-9", "10+")), 
            type = list(type = "factor", levels = c("A", "B", "C", "D")) 
        ) 
    textDS <- RxTextData(file = claimsTextName, colInfo = claimsColInfo)

    # Create an SPSS data source from the text data source
    # The 'colInfo' will be carried over to the SPSS data source
    # and the file name will be replaced
    spssDS <- RxDataSource(class = "RxSpssData", dataSource = textDS, file = claimsSpssName)
```



