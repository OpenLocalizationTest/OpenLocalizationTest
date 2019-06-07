---
title: explore function (olapR) | Microsoft Docs
description: "   Allows for exploration of cube metadata "
keywords: (olapR), explore
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
ms.openlocfilehash: c7df21f638e1e0353820b82c3bf881b4f3a211e2
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="explore-olapr-explore-method"></a>explore: olapR explore Method 

 ## <a name="description"></a>Description

Allows for exploration of cube metadata



 ## <a name="usage"></a>Usage

```   
  explore(olapCnn, cube = NULL, dimension = NULL, hierarchy = NULL, level = NULL)

```


 ## <a name="arguments"></a>Arguments



 ### `olapCnn`
 Object of class "OlapConnection" returned by `OlapConnection()` 


 ### `cube`
 A string specifying a cube name 


 ### `dimension`
 A string specifying a dimension name 


 ### `hierarchy`
 A string specifying a hierarchy name 


 ### `level`
 A string specifying a level name 




 ## <a name="details"></a>Details

`explore` 



 ## <a name="value"></a>Value

Prints cube metadata. Returns NULL.
An error is thrown if arguments are invalid.


 ## <a name="note"></a>Note

Arguments must be specified in order. For example: In order to explore hierarchies, a dimension and a cube must be specified.



 ## <a name="references"></a>References
  See [execute2D](Execute2D.md) or [executeMD](ExecuteMD.md) for references.  


 ## <a name="see-also"></a>See Also

query`, `[OlapConnection](OlapConnection.md)`, `[executeMD](ExecuteMD.md)`, `[execute2D](Execute2D.md)


 ## <a name="examples"></a>Examples

 ```

  cnnstr <- "Data Source=localhost; Provider=MSOLAP;"
  ocs <- OlapConnection(cnnstr)

  #Exploring Cubes
  explore(ocs)
  #Analysis Services Tutorial
  #Internet Sales
  #Reseller Sales
  #Sales Summary
  #[1] TRUE

  #Exploring Dimensions
  explore(ocs, "Analysis Services Tutorial")
  #Customer
  #Date
  #Due Date
  #Employee
  #Internet Sales Order Details
  #Measures
  #Product
  #Promotion
  #Reseller
  #Reseller Geography
  #Sales Reason
  #Sales Territory
  #Ship Date
  #[1] TRUE

  #Exploring Hierarchies
  explore(ocs, "Analysis Services Tutorial", "Product")
  #Category
  #Class
  #Color
  #Days To Manufacture
  #Dealer Price
  #End Date
  #List Price
  #Model Name
  #Product Categories
  #Product Line
  #Product Model Lines
  #Product Name
  #Reorder Point
  #Safety Stock Level
  #Size
  #Size Range
  #Standard Cost
  #Start Date
  #Status
  #Style
  #Subcategory
  #Weight
  #[1] TRUE

  #Exploring Levels
  explore(ocs, "Analysis Services Tutorial", "Product", "Product Categories")
  #(All)
  #Category
  #Subcategory
  #Product Name
  #[1] TRUE

  #Exploring Members
  #NOTE: -> indicates that the following member is a child of the previous member
  explore(ocs, "Analysis Services Tutorial", "Product", "Product Categories", "Category")
  #Accessories
  #Bikes
  #Clothing
  #Components
  #Assembly Components
  #-> Assembly Components
  #--> Assembly Components
```

