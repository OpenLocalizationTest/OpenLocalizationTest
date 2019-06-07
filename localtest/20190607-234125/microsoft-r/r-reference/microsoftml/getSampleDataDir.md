---
title: 'getSampleDataDir function (MicrosoftML) '
description: " Location where downloaded sample data is stored. "
keywords: (MicrosoftML), getSampleDataDir, transform
author: heidisteen
manager: cgronlun
ms.date: 01/16/2019
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
ms.openlocfilehash: 30790429adf884a006b7b59df4b123a8f4cd6059
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="getsampledatadir-get-package-sample-data-location"></a>getSampleDataDir: Get Package Sample Data Location 
 ## <a name="description"></a>Description

Location where downloaded sample data is stored.


 ## <a name="usage"></a>Usage

```   
  getSampleDataDir(sampleDataDir = NULL, createDir = TRUE)

```

 ## <a name="arguments"></a>Arguments



 ### `sampleDataDir`
 Specifies the path to the location where downloaded sample data is (or is to be) stored or `NULL`. 



 ### `createDir`
 `TRUE` to create the directory if it does not exist; `FALSE` not to create the directory. 



 ## <a name="details"></a>Details

If `sampleDataDir` is `NULL`, the function first checks to see if an option has been set containing `sampleDataDir`, i.e. `getOption("sampleDataDir")`. If that is `NULL` too, a 'sampleDataDir' subdirectory of the current working directory is used. If `createDir` is `TRUE`, the directory is created if it does not exist.


 ## <a name="value"></a>Value

A character string containing the path to the location of the sample data.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="examples"></a>Examples

 ```

  # This example sets the option to be the same as the default
  options(sampleDataDir = file.path(getwd(), "sampleDataDir"))

  dataDir <- getSampleDataDir(createDir = FALSE)
```



