---
title: RxInSqlServer-class class (revoAnalytics) | Microsoft Docs
description: " Creates a compute context for running Microsoft R Server analyses inside Microsoft SQL Server.  Currently only supported in Windows. "
keywords: (revoAnalytics), RxInSqlServer-class, doPreJobValidation,RxInSqlServer-method, initialize,RxInSqlServer-method, show,RxInSqlServer-method, classes
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
ms.openlocfilehash: ea5c74f32a38a7637dff442dcabe626717caf8a1
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxinsqlserver-class-class-rxinsqlserver"></a>RxInSqlServer-class: Class RxInSqlServer 
 ## <a name="description"></a>Description

Creates a compute context for running Microsoft R Server analyses inside Microsoft SQL Server.

Currently only supported in Windows.


 ## <a name="objects-from-the-class"></a>Objects from the Class 


Objects can be created by calls of the form .


 ## <a name="slots"></a>Slots 




### <a name="connectionstring"></a>`connectionString`:
Object of class `"character"` ~~ 



### <a name="wait"></a>`wait`:
Object of class `"logical"` ~~ 


### <a name="consoleoutput"></a>`consoleOutput`:
Object of class `"logical"` ~~ 


### <a name="autocleanup"></a>`autoCleanup`:
Object of class `"logical"` ~~ 




### <a name="datapath"></a>`dataPath`:
Object of class `"characterORNULL"` ~~ 



### <a name="packagestoload"></a>`packagesToLoad`:
Object of class `"characterORNULL"` ~~ 



### <a name="executiontimeout"></a>`executionTimeout`:
Object of class `"numeric"` ~~ 


### <a name="description"></a>`description`:
Object of class `"character"` ~~ 


### <a name="version"></a>`version`:
Object of class `"character"` ~~ 




 ## <a name="extends"></a>Extends 


Class RxDistributedHpa, directly.
Class RxComputeContext, by class "RxDistributedHpa", distance 2.
Class RxComputeContext, by class "RxLocalSeq", distance 1.

 ## <a name="methods"></a>Methods 




### `doPreJobValidation`
`signature(object = "RxInSqlServer")`: ... 


### `initialize`
`signature(.Object = "RxInSqlServer")`: ... 


### `show`
`signature(object = "RxInSqlServer")`: ... 





 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[RxInSqlServer](RxInSqlServer.md), [RxSqlServerData](RxSqlServerData.md)

 ## <a name="examples"></a>Examples

 ```

  showClass("RxInSqlServer")
```


