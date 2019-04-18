---
title: " Generator for an PemaByGroup reference class object "
description: " Generator for an PemaByGroup reference class object to be used with pemaCompute. This will compute arbitrary statistics by a grouping variable in a data set. "
keywords: 'RevoPemaR, PemaByGroup,  models '
author: richcalaway
ms.author: richcala
manager: cgronlun
ms.date: 03/23/2017
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ms.openlocfilehash: 90dbd84460907531354ee4be6d3c861b775f1c5d
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="pemabygroup--generator-for-an-pemabygroup-reference-class-object"></a>PemaByGroup:  Generator for an PemaByGroup reference class object 

 Applies to version 8.0.3 of package RevoPemaR.

 ## <a name="description"></a>Description

Generator for an PemaByGroup reference class object to be used with pemaCompute. This will compute arbitrary statistics by a grouping variable in a data set.


 ## <a name="usage"></a>Usage

```   
  PemaByGroup(...)

```


 ## <a name="arguments"></a>Arguments



 ###  <a name=""></a>...
  Arguments used in the constructor. See Details section. 



 ## <a name="details"></a>Details

This is an example of a parallel external memory algorithm for use with [pemaCompute](pemacompute.md). User-specified arguments for the `initalize` method are:

groupByVar = "character", computeVars = "character", fnList = "ANY", sep = "character",  

* 
 `groupByVar`: character string containing name of grouping variable.  It can be a factor, character, or integer vector.

* 
 `computeVars`: character vector containing the name of one or more variables on which to compute the by-group statistics.

* 
 `fnList`: a named list of lists specifying functions and argument values.  
The first element of each function list should be the function. The second element of the function list should be named the name of the argument for the data vector or list of data vectors to process.  
 The value should be set to `NULL` or the names of additional variables to be included in an input data list.

* 
 `sep`: the separator to use in creating the variable name(s) for the computed statistic(s).  It will take the form of `varName.fnName` where the `.` is replaced by `sep`.




 ## <a name="value"></a>Value

An `PemaByGroup` reference class object.








 ## <a name="see-also"></a>See Also

setRefClass, [PemaBaseClass](pemabaseclass.md)

 ## <a name="examples"></a>Examples

 ```


  # Show help for methods
  PemaByGroup$help(initialize)
  PemaByGroup$help(processData)
  PemaByGroup$help(updateResults)
  PemaByGroup$help(processResults)
```




