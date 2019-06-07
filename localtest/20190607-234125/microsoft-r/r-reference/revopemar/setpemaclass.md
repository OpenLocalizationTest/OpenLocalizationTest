---
title: " PEMA classes "
description: " Returns a generator function for creating analysis reference class objects to use in pemaCompute. "
keywords: RevoPemaR, setPemaClass, methods
author: richcalaway
ms.author: richcala
manager: cgronlun
ms.date: 03/23/2017
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ms.openlocfilehash: 79e3766da8d3345b2ef9f108a60bd63ee2e29491
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="setpemaclass--pema-classes"></a>setPemaClass:  PEMA classes 

 Applies to version 8.0.3 of package RevoPemaR.

 ## <a name="description"></a>Description

Returns a generator function for creating analysis reference class objects to use in pemaCompute.


 ## <a name="usage"></a>Usage

```   
  setPemaClass(Class, fields = character(), contains = character(), 
      methods = list(), where = topenv(parent.frame()), includeMethods = TRUE, ...)


```

 ## <a name="arguments"></a>Arguments



 ### <a name="class"></a>Class
  character string name for the class.  


 ### <a name="fields"></a>fields
  either a character vector of field names or a named list of the fields.   


 ### <a name="contains"></a>contains
  optional vector of super reference classes for this class. The fields  and class-based methods will be inherited.  



 ### <a name="methods"></a>methods
  a named list of function definitions that can be invoked on objects from this class.  



 ### <a name="where"></a>where
  the environment in which to store the class definition.  



 ### <a name="includemethods"></a>includeMethods
  logical.  If `TRUE`, methods (including those of parent classes) will be included when serializing.  



 ###  <a name=""></a>...
  other arguments to be passed to setRefClass.    



 ## <a name="details"></a>Details

See setRefClass for more information on arguments and using reference classes.
The `setPemaCLass` generator provides a framework for writing parallel, external memory algorithms (PEMAs) that can be run serially on a single computer, and will be automatically parallelized when run on cluster supported by **RevoScaleR**.


 ## <a name="value"></a>Value

returns a generator function suitable for creating objects from the class, invisibly.







 ## <a name="see-also"></a>See Also

[PemaBaseClass](pemabaseclass.md), setRefClass, [PemaMean](pemamean.md), [pemaCompute](pemacompute.md)


 ## <a name="examples"></a>Examples

 ```


  # A very simple example of computing a sum
  PemaSum <- setPemaClass("PemaSum", 
    contains = "PemaBaseClass",

    fields = list( 
        # list the fields (member variables)
        sum = "numeric",
        varName = "character"
        ),

    methods = list(
        # list the methods (member functions)
        initialize = function(varName = "", ...) 
        {
              'sum is initialized to 0'          
              # callSuper calls the method of the parent class
              callSuper(...)            
            usingMethods(.pemaMethods)  # Will include methods if includeMethods is TRUE        
              # Fields are modified in a method by using the non-local assignment operator
              varName <<- varName
            sum <<- 0
        },
        processData = function(dataList) 
        {
            'Updates the sum  from the current chunk of data.'
              sum <<- sum + sum(as.numeric(dataList[[varName]]), na.rm = TRUE)
            invisible(NULL)
        },
        updateResults = function(pemaSumObj)
        {
              'Updates the sum from another PemaSum object.'
              sum <<- sum + pemaMeanObj$sum
              invisible(NULL)
        },
        processResults = function()
          {
              'Returns the sum. No further computations required.'
            sum
        },
          getVarsToUse = function()
          {
              'Returns the varName.' 
              varName
          }
    )
  )

  pemaSumObj <- PemaSum()
  pemaCompute(pemaSumObj, data = iris, varName = "sepal.length")
```




