---
title: " Generator for a PemaBaseClass reference class object "
description: " Generator for a PemaBaseClass reference class object to be used with pemaCompute. "
keywords: 'RevoPemaR, PemaBaseClass,  models '
author: richcalaway
ms.author: richcala
manager: cgronlun
ms.date: 03/23/2017
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ms.openlocfilehash: 818f9b92a050dddf2eedf05a94baebe6d136c255
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="pemabaseclass--generator-for-a-pemabaseclass-reference-class-object"></a>PemaBaseClass:  Generator for a PemaBaseClass reference class object 

 Applies to version 8.0.3 of package RevoPemaR.

 ## <a name="description"></a>Description

Generator for a PemaBaseClass reference class object to be used with pemaCompute.


 ## <a name="usage"></a>Usage

```   
  PemaBaseClass(...)

```


 ## <a name="arguments"></a>Arguments



 ###  <a name=""></a>...
  Arguments used in the constructor. Not used by the `PemaBaseClass` base class.  



 ## <a name="details"></a>Details

This is a base reference class for the construction of reference classes to be used for parallel external memory algorithms for use in [pemaCompute](pemacompute.md). See [PemaMean](pemamean.md) for a simple example.


 ## <a name="value"></a>Value

A `PemaBaseClass` reference class object.








 ## <a name="see-also"></a>See Also

setRefClass, [setPemaClass](setpemaclass.md), [pemaCompute](pemacompute.md), [PemaMean](pemamean.md)


 ## <a name="examples"></a>Examples

 ```


  # Show help for methods
  PemaBaseClass$help(initialize)
  PemaBaseClass$help(processData)
  PemaBaseClass$help(updateResults)
  PemaBaseClass$help(processResults)
```




