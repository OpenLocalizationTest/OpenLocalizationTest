---
title: " Comute PEMA "
description: " Use a PemaBaseClass reference class object to perform a Parallel External Memory Algorithm computation. "
keywords: RevoPemaR, pemaCompute, models
author: richcalaway
ms.author: richcala
manager: cgronlun
ms.date: 03/23/2017
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ms.openlocfilehash: fa0d333d1bb8c2e5747aa5ecf5c1c77c612bbadc
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="pemacompute--compute-pema"></a>pemaCompute:  Compute PEMA 

 Applies to version 8.0.3 of package RevoPemaR.

 ## <a name="description"></a>Description

Use a PemaBaseClass reference class object to perform a Parallel External Memory Algorithm (PEMA) computation.


 ## <a name="usage"></a>Usage

```   
  pemaCompute(pemaObj, data = NULL, outData = NULL, overwrite = FALSE, append = "none",
      computeContext = NULL, initPema = TRUE, ...)

```

 ## <a name="arguments"></a>Arguments



 ### <a name="pemaobj"></a>pemaObj
  A [PemaBaseClass](pemabaseclass.md) reference class object containing the methods for the analysis.  


 ### <a name="data"></a>data
  A data frame or **RevoScaleR** data source object.  


 ### <a name="outdata"></a>outData
  An **RevoScaleR** data source object that has write capabilities, such as an .xdf file. Not used by all [PemaBaseClass](pemabaseclass.md) reference class objects.  



 ### <a name="overwrite"></a>overwrite
 logical value. If `TRUE`, an existing `outFile` will be overwritten. 



 ### <a name="append"></a>append
 either `"none"` to create a new file, `"rows"` to append rows to an existing file, or `"cols"` to append columns to an existing file. If `outFile` exists and `append` is `"none"`,  the `overwrite` argument must be set to `TRUE`. Ignored when `outData` is not specified or not relevant. You cannot append to `RxTextData` or `RxTeradata` data sources,  and appending is not supported for composite .xdf files or when using the `RxHadoopMR` compute context. 



 ### <a name="computecontext"></a>computeContext
  `NULL` or a **RevoScaleR** compute context object.  



 ### <a name="initpema"></a>initPema
  logical.  If `TRUE` the `initialize` method for the `pemaObj` object will be called before performing computations.  



 ###  <a name=""></a>...
  Other fields in the `PemaBaseClass` class to be utilized in the analysis.  



 ## <a name="details"></a>Details

The `pemaCompute` function provides a framework for writing parallel, external memory algorithms (PEMAs) that can be run serially on a single computer, and will be automatically parallelized when run on cluster supported by **RevoScaleR**.


 ## <a name="value"></a>Value

The value returned that returned by the `PemaBaseClass` `processResults` method.
Note that the reference class `PemaBaseClass` will be reinitialized at the beginning of the analysis unless `initPema` is set to `TRUE`, and will contain updated values upon completion.







 ## <a name="see-also"></a>See Also

[PemaBaseClass](pemabaseclass.md), [PemaMean](pemamean.md), [setPemaClass](setpemaclass.md)

 ## <a name="examples"></a>Examples

 ```


  # Instantiate an PemaMean reference class
  meanPemaObj <- PemaMean()
  meanPemaObj # See the initialized values of the fields

  # Compute the mean of Petal.Length from the iris data set
  # Call pemaCompute, specifying the custom analyis object, the data, and additional arg
  pemaCompute(pemaObj = meanPemaObj, data = iris, varName = "Petal.Length")

  meanPemaObj # Note that the reference class object has been updated
```




