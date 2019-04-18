---
title: rxSparkCacheData {RevoScaleR} function (revoAnalytics) | Microsoft Docs
description: " Use this function to set the cache flag to control whether data objects should be cached in Spark memory system, applicable for RxXdfData, RxHiveData, RxParquetData, and RxOrcData.  "
keywords: (revoAnalytics), rxSparkCacheData {RevoScaleR}, rxSparkCacheData
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
ms.openlocfilehash: 153acb38a1ecc220aaa152630c06c2ad9f2515db
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="rxsparkcachedata-revoscaler--set-the-cache-flag-in-spark-compute-context"></a>rxSparkCacheData {RevoScaleR}:  Set the Cache Flag in Spark Compute Context  

 ## <a name="description"></a>Description

Use this function to set the cache flag to control whether data objects should be cached in Spark memory system, applicable for `RxXdfData`, `RxHiveData`, `RxParquetData`, and `RxOrcData`. 



 ## <a name="usage"></a>Usage

```   
  rxSparkCacheData(data, cache = TRUE)

```


 ## <a name="arguments"></a>Arguments



 ### `data`
 a data source that can be RxXdfData, RxHiveData, RxParquetData, or RxOrcData. RxTextData is currently not supported. 


 ### `cache`
 logical value controlling whether the data should be cached or not. If `TRUE`the data will be cached in the Spark memory system after the first use for performance enhancement. 




 ## <a name="details"></a>Details

Note that `RxHiveData` with `saveAsTempTable=TRUE` is always cached in memory regardless of the `cache` parameter setting in this function.


 ## <a name="value"></a>Value

data object with new cache flag. 


 ## <a name="see-also"></a>See Also

[rxSparkListData](rxSparkDataOps.md), [rxSparkRemoveData](rxSparkDataOps.md), [RxXdfData](RxXdfData.md), [RxHiveData](RxSparkData.md), [RxParquetData](RxSparkData.md), [RxOrcData](RxSparkData.md).

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

  hiveData <- RxHiveData(table = "mytable")

  ## this does not work. The cache flag of the input hiveData is not changed, so it is still FALSE.
  rxSparkCacheData(hiveData)
  rxImport(hiveData) # data is not cached

  ## this works. The cache flag of hiveData is now set to TRUE.
  hiveData <- rxSparkCacheData(hiveData)  
  rxImport(hiveData) # data is now cached

  ## set cache value to FASLE
  hiveData <- rxSparkCacheData(hiveData, FALSE)
 ## End(Not run) 
```

