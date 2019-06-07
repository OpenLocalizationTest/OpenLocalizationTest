---
title: Class RxInTeradata
description: " Creates a compute context for running Microsoft R Server analyses inside a Teradata database cluster. "
keywords: ', RxInTeradata-class, doPreJobValidation,RxInTeradata-method, initialize,RxInTeradata-method, show,RxInTeradata-method, classes'
author: heidisteen
manager: cgronlun
ms.date: 08/04/2017
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
ms.openlocfilehash: d8b6f0a7578359c9f6c900b5f275e6892b51e2ea
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxinteradata-class-class-rxinteradata"></a>RxInTeradata-class: Class RxInTeradata 
 ## <a name="description"></a>Description

DEPRECATED: Creates a compute context for running Microsoft R Server analyses inside a Teradata database cluster.


 ## <a name="objects-from-the-class"></a>Objects from the Class 


Objects can be created by calls of the form .


 ## <a name="slots"></a>Slots 




### <a name="remotesharedir"></a>`remoteShareDir`:
Object of class `"character"` ~~ 


### <a name="connectionstring"></a>`connectionString`:
Object of class `"character"` ~~ 


### <a name="sharedir"></a>`shareDir`:
Object of class `"character"` ~~ 


### <a name="revopath"></a>`revoPath`:
Object of class `"characterORNULL"` ~~ 


### <a name="wait"></a>`wait`:
Object of class `"logical"` ~~ 


### <a name="consoleoutput"></a>`consoleOutput`:
Object of class `"logical"` ~~ 


### <a name="autocleanup"></a>`autoCleanup`:
Object of class `"logical"` ~~ 


### <a name="configfile"></a>`configFile`:
Object of class `"characterORNULL"` ~~ 


### <a name="workingdir"></a>`workingDir`:
Object of class `"characterORNULL"` ~~ 


### <a name="datapath"></a>`dataPath`:
Object of class `"characterORNULL"` ~~ 


### <a name="minelems"></a>`minElems`:
Object of class `"numeric"` ~~ 


### <a name="maxelems"></a>`maxElems`:
Object of class `"numeric"` ~~ 


### <a name="exclusive"></a>`exclusive`:
Object of class `"logical"` ~~ 


### <a name="nodes"></a>`nodes`:
Object of class `"characterORNULL"` ~~ 


### <a name="datadisttype"></a>`dataDistType`:
Object of class `"character"` ~~ 


### <a name="packagestoload"></a>`packagesToLoad`:
Object of class `"characterORNULL"` ~~ 


### <a name="email"></a>`email`:
Object of class `"characterORNULL"` ~~ 


### <a name="resultstimeout"></a>`resultsTimeout`:
Object of class `"numeric"` ~~ 


### <a name="description"></a>`description`:
Object of class `"character"` ~~ 


### <a name="version"></a>`version`:
Object of class `"character"` ~~ 




 ## <a name="extends"></a>Extends 


Class RxDistributedHpa, directly.
Class RxComputeContext, by class "RxDistributedHpa", distance 2.

 ## <a name="methods"></a>Methods 




### `doPreJobValidation`
`signature(object = "RxInTeradata")`: ... 


### `initialize`
`signature(.Object = "RxInTeradata")`: ... 


### `show`
`signature(object = "RxInTeradata")`: ... 









 ## <a name="see-also"></a>See Also

[RxInTeradata](RxInTeradata.md), [RxTeradata](RxTeradata.md)

 ## <a name="examples"></a>Examples

 ```

  showClass("RxInTeradata")
```


