---
title: rxSparkListData, rxSparkRemoveData {RevoScaleR} function (revoAnalytics) | Microsoft Docs
description: " Use these functions to manage the objects cached in the Spark memory system. These functions are only applicable when using [RxSpark](RxSpark.md) compute context. "
keywords: (revoAnalytics), rxSparkListData, rxSparkRemoveData {RevoScaleR}, rxSparkListData, rxSparkRemoveData
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
ms.openlocfilehash: f547afbff084010213c299f11e44ae1b184ba40f
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxsparklistdata-rxsparkremovedata-revoscaler-manage-cached-data-in-spark"></a>rxSparkListData, rxSparkRemoveData {RevoScaleR}: Manage Cached Data in Spark 
 ## <a name="description"></a>Description

Use these functions to manage the objects cached in the Spark memory system. These functions are only applicable when using [RxSpark](RxSpark.md) compute context.


 ## <a name="usage"></a>Usage

```   
  rxSparkListData(showDescription=TRUE,
      computeContext = rxGetOption("computeContext"))

  rxSparkRemoveData(list,
      computeContext = rxGetOption("computeContext"))    

```


 ## <a name="arguments"></a>Arguments



 ### `list`
 list of cached objects need to be deleted. 


 ### `showDescription`
 logical indicating whether or not to print out the detail to console. 


 ### `computeContext`
 `RxSpark` compute context object. 




 ## <a name="value"></a>Value

List of all objects cached in Spark memory system for `rxSparkListData`.

No return values for `rxSparkRemoveData`.


 ## <a name="examples"></a>Examples

 ```

  ## Not run:

cc <- rxSparkConnect()

colInfo = list( DayOfWeek = list(type = "factor"))
df <- RxParquetData(file = "/tmp/AirlineDemoSmall.parquet", colInfo = colInfo)

### example for rxSparkListData

## No object in list, because no algorithm has been run 
rxSparkListData()

rxLogit((ArrDelay>0) ~ CRSDepTime + DayOfWeek, data = df)

## After the first run, a Spark data object is added into the list
rxSparkListData()

### example for rxSparkRemoveData

## remove an object
rxSparkRemoveData(df)

## remove all cached objs
rxSparkRemoveData(rxSparkListData())

rxSparkDisconnect(cc)
 ## End(Not run) 
```

