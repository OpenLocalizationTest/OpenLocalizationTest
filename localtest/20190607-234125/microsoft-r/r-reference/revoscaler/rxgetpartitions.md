---
title: rxGetPartitions function (revoAnalytics) | Microsoft Docs
description: " Get partitions enumeration of a partitioned Xdf data source. "
keywords: (revoAnalytics), rxGetPartitions, GetPartitions
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
ms.openlocfilehash: a80c6a4a2157fc16384c2a8137b2a148b9d4aade
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxgetpartitions--get-partitions-of-a-partitioned-xdf-data-source"></a>rxGetPartitions:  Get Partitions of a Partitioned Xdf Data Source  

 ## <a name="description"></a>Description

Get partitions enumeration of a partitioned Xdf data source.


 ## <a name="usage"></a>Usage

```   
  rxGetPartitions(data)

```


 ## <a name="arguments"></a>Arguments



 ### `data`
 an existing partitioned data source object which was created by [RxXdfData](RxXdfData.md) with `createPartitionSet = TRUE` and constructed by [rxPartition](rxPartition.md). 



 ## <a name="details"></a>Details





 ## <a name="value"></a>Value

Data frame with `(n+1)` columns, the first `n` columns are partitioning columns specified by `varsToPartition` in [rxPartition](rxPartition.md) and the `(n+1)th` column is a data source column where each row contains an Xdf data source object of one partition.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

RXdfData, [rxPartition](rxPartition.md), [rxExecBy](rxExecBy.md)


 ## <a name="examples"></a>Examples

 ```

    # create an input Xdf data source
    inFile <- "claims.xdf"
    inFile <- file.path(dataPath = rxGetOption(opt = "sampleDataDir"), inFile)
    inXdfDS <- RxXdfData(file = inFile)

    # create an output partitioned Xdf data source
    outFile <- file.path(tempdir(), "partitionedClaims.xdf")
    outPartXdfDataSource <- RxXdfData(file = outFile, createPartitionSet = TRUE)

    # construct and save the partitioned Xdf to disk
    partDF <- rxPartition(inData = inXdfDS, outData = outPartXdfDataSource, varsToPartition = c("car.age"))

    # enumerate partitions
    partDF <- rxGetPartitions(outPartXdfDataSource)
    rxGetInfo(partDF, getVarInfo = TRUE)
    partDF$DataSource
```

