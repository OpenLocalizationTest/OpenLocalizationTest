---
title: rxCompressXdf function (revoAnalytics) | Microsoft Docs
description: " Compress one or more .xdf files "
keywords: (revoAnalytics), rxCompressXdf, manip, file
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
ms.openlocfilehash: 8a176c690bac8beec33fb20acc1d84096a31a1ce
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxcompressxdf--compress-xdf-files"></a>rxCompressXdf:  Compress .xdf files  
 ## <a name="description"></a>Description

Compress one or more .xdf files


 ## <a name="usage"></a>Usage

```   
  rxCompressXdf(inFile, outFile = NULL, xdfCompressionLevel = 1, overwrite = FALSE, reportProgress = rxGetOption("reportProgress"))

```

 ## <a name="arguments"></a>Arguments



 ### `inFile`
  An .xdf file name, an RxXdfData data source, a directory containing .xdf files, or a vector of .xdf file names or RxXdfData data sources to compress  


 ### `outFile`
  An .xdf file name, an RxXdfData data source, a directory, or a vector of .xdf file names or RxXdfData data sources to contain the compressed files.  


 ### `xdfCompressionLevel`
 integer in the range of -1 to 9.  The higher the value, the greater the  amount of compression - resulting in smaller files but a longer time to create them. If  `xdfCompressionLevel` is set to 0, there will be no compression and files will be compatible  with the 6.0 release of Revolution R Enterprise.  If set to -1, a default level of compression  will be used.   


 ### `overwrite`
  If `outFile` is specified and is different from `inFile`, `overwrite` must be set to `TRUE` to have `outFile` overwritten.  


 ### `reportProgress`
  integer value with options:  
*   `0`: no progress is reported. 
*   `1`: the number of processed rows is printed and updated. 
*   `2`: rows processed and timings are reported. 
*   `3`: rows processed and all timings are reported. 




 ## <a name="details"></a>Details

`rxCompressXdf` uses ZLIB to compress `.xdf` files in blocks.  The auto compression level of -1 is equivalent to approximately 6.  Typically setting the `xdfCompressionLevel` to 1 will provide an adequate amount of compression at the fastest speed.


 ## <a name="value"></a>Value

A vector of [RxXdfData](RxXdfData.md) data sources

 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxImport](rxImport.md), [rxDataStep](rxDataStep.md), [RxXdfData](RxXdfData.md),

 ## <a name="examples"></a>Examples

 ```


  # Get location of sample uncompressed .xdf file
  sampleXdf <- file.path(rxGetOption("sampleDataDir"), "AirlineDemoSmallUC.xdf")

  # Create name for a temporary file
  compressXdf <- tempfile(pattern = ".rxCompress", fileext = ".xdf")    

  # Create a new compressed .xdf file from the sample file
  newDS <- rxCompressXdf(inFile = sampleXdf, outFile = compressXdf, xdfCompressionLevel = 1)

  # Get information about files and compare sizes
  sampleFileInfo <- file.info(sampleXdf)
  compressFileInfo <- file.info(compressXdf)
  sampleFileInfo$size
  compressFileInfo$size

  # Clean-up
  file.remove(compressXdf)
```



