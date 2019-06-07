---
title: " Generator for an PemaMean reference class object "
description: " Generator for an PemaMean reference class object, inheriting from PemaBaseClass, to be used with pemaCompute. "
keywords: 'RevoPemaR, PemaMean,  models '
author: richcalaway
ms.author: richcala
manager: cgronlun
ms.date: 03/23/2017
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ms.openlocfilehash: 8dd62398834a1579ce308b47b18775b774a80057
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="pemamean--generator-for-an-pemamean-reference-class-object"></a>PemaMean:  Generator for an PemaMean reference class object 

 Applies to version 8.0.3 of package RevoPemaR.

 ## <a name="description"></a>Description

Generator for an PemaMean reference class object, inheriting from PemaBaseClass, to be used with pemaCompute.


 ## <a name="usage"></a>Usage

```   
  PemaMean(...)

```


 ## <a name="arguments"></a>Arguments




 ###  <a name=""></a>...
  Arguments used in the constructor. See Details section.  



 ## <a name="details"></a>Details

This is a simple example of a parallel external memory algorithm for use with [pemaCompute](pemacompute.md). The `varName`argument for the constructor is a character string containing the name of the variable in the data set to use for computations.


 ## <a name="value"></a>Value

An `PemaMean` reference class object.








 ## <a name="see-also"></a>See Also

setRefClass, [setPemaClass](setpemaclass.md), [PemaBaseClass](pemabaseclass.md)

 ## <a name="examples"></a>Examples

 ```


  # Show help for methods
  PemaMean$help(initialize)
  PemaMean$help(processData)
  PemaMean$help(updateResults)
  PemaMean$help(processResults)
```




