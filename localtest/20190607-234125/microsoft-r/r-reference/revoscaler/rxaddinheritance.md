---
title: rxAddInheritance function (revoAnalytics) | Microsoft Docs
description: "  Add a specific S3 class to the class of a compatible object. "
keywords: (revoAnalytics), rxAddInheritance, rxAddInheritance.default, rxAddInheritance.rxDTree, models, tree, classif, regression
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
ms.openlocfilehash: 170de49768790b83dedc39eb7ba758bcda824379
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxaddinheritance-add-inheritance-to-compatible-objects"></a>rxAddInheritance: Add Inheritance to Compatible Objects 
 ## <a name="description"></a>Description

Add a specific S3 class to the `"class"` of a compatible object.


 ## <a name="usage"></a>Usage

```   

  rxAddInheritance(x, inheritanceClass, ...)

 ## S3 method for class `rxDTree':
rxAddInheritance  (x, inheritanceClass = "rpart",    ...  )


```

 ## <a name="arguments"></a>Arguments



 ### `x`
  the object to which inheritance is to be added. Specifically, for `rxAddInheritance.rxDTree`, an object of class `rxDTree`. 


 ### `inheritanceClass`
  the class to be inherited from. Specifically, for `rxAddInheritance.rxDTree`, the class `"rpart"`. 


 ### ` ...`
  additional arguments to be passed directly to other methods. 




 ## <a name="details"></a>Details

The `rxAddInheritance` function is designed to be a general way to add inheritance to S3 objects that are compatible with the class for which inheritance is to be added. Note, however, that this approach is exactly as dangerous and error-prone as simply calling `class(x) <- c(class(x), inheritanceClass)`. 

It is expected that classes that are designed to mimic existing R classes, but not rely on them, will have their own specific `rxAddInheritance` methods to add the R class inheritance on request.

In the case of `rxDTree` objects, these were designed to be compatible with the `"rpart"` class. so adding **rpart** inheritance is guaranteed to work.


 ## <a name="value"></a>Value

The original object, modified to include `inheritanceClass` as part of its `"class"` attribute. 

In the case of `rxDTree` objects, the object may also be modified to include the `functions` component if it was previously `NULL`.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[rxDTree](rxDTree.md).

 ## <a name="examples"></a>Examples

 ```

  mtcarTree <- rxDTree(mpg ~ disp, data=mtcars)
  mtcarRpart <- rxAddInheritance(mtcarTree)
  require(rpart)
  printcp(mtcarRpart)
```





