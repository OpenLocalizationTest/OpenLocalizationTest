---
title: rxOpen-methods methods (revoAnalytics) | Microsoft Docs
description: " These functions manage **RevoScaleR** data source objects. "
keywords: (revoAnalytics), rxOpen-methods, rxOpen, rxClose, rxIsOpen, rxReadNext, rxWriteNext, rxClose-methods, rxIsOpen-methods, rxReadNext-methods, rxWriteNext-methods, rxOpen,RxDataSource-method, rxClose,RxDataSource-method, rxIsOpen,RxDataSource-method, rxReadNext,RxDataSource-method, rxWriteNext,data.frame,RxDataSource-method, methods, file, connection
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
ms.openlocfilehash: e9cdf9e847783bc5c830b579d23b64e4ef33dddb
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxopen-methods-managing-revoscaler-data-source-objects"></a>rxOpen-methods: Managing RevoScaleR Data Source Objects 
 ## <a name="description"></a>Description

These functions manage **RevoScaleR** data source objects.


 ## <a name="usage"></a>Usage

```   
  rxOpen(src, mode = "r")
  rxClose(src, mode = "r")
  rxIsOpen(src, mode = "r")
  rxReadNext(src)
  rxWriteNext(from, to, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `from`
 data frame object. 


 ### `src`
 RxDataSource object. 


 ### `to`
 RxDataSource object. 


 ### `mode`
 character string specifying the mode (`r` or `w`) to open the file. 


 ### ` ...`
 any other arguments to be passed on. 



 ## <a name="value"></a>Value

For `rxOpen` and `rxClose`, a logical indicating whether the operation was successful.
For `rxIsOpen`, a logical indicating whether or not the RxDataSource is open for the specified `mode`.
For `rxReadNext`, either a data frame or a list depending upon the value of the `returnDataFrame` property within `src`.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[rxNewDataSource](rxNew.md), [RxXdfData](RxXdfData.md).

 ## <a name="examples"></a>Examples

 ```

  ds <- RxXdfData(file.path(rxGetOption("sampleDataDir"), "claims.xdf"))
  # ds contains only one block of data
  rxOpen(ds) # must open the file before rxReadNext
  rxReadNext(ds) # get the first block
  rxReadNext(ds)
  rxClose(ds)

  # Use a data source to compute means by processing the data in chunks
  # Data processing functions: for each chunk, compute sums of columns and
  # number of rows, then update the results computed from previous chunks
  processData <- function(dframe)
    list(sumCols = colSums(dframe), numRows = nrow(dframe))
  updateResults <- function(x, y)
    list(sumCols = x$sumCols + y$sumCols, numRows = x$numRows + y$numRows)

  # Create data source
  censusWorkers <- file.path(rxGetOption("sampleDataDir"), "CensusWorkers.xdf")
  ds <- RxXdfData(censusWorkers, varsToKeep = c("age", "incwage"),
                  blocksPerRead = 2)

  # Process data and update results
  rxOpen(ds)
  resList <- processData(rxReadNext(ds))
  while(TRUE)
  {
      df <- rxReadNext(ds)
      if (nrow(df) == 0)
          break
      resList <- updateResults(resList, processData(df))
  }
  rxClose(ds)

  # Compute the means of the variables from the accumulated results
  varMeans <- resList$sumCols / resList$numRows
  varMeans
```




