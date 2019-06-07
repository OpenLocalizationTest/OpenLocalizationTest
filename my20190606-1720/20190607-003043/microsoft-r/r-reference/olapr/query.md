---
title: Query function (olapR) | Microsoft Docs
description: "   Query constructs a Query object. Set functions are used to build and modify the Query axes and cube name. "
keywords: (olapR), Query
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
ms.openlocfilehash: 6cbe7ea731d91fca1ec9aca7987c981aaf0cd216
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="query-olapr-query-construction"></a>Query: olapR Query Construction 

 ## <a name="description"></a>Description

`Query` constructs a "Query" object. Set functions are used to build and modify the Query axes and cube name.



 ## <a name="usage"></a>Usage

```   
  Query(validate = FALSE)

  cube(qry)
  cube(qry) <- cubeName

  columns(qry)
  columns(qry) <- axis

  rows(qry)
  rows(qry) <- axis

  pages(qry)
  pages(qry) <- axis

  chapters(qry)
  chapters(qry) <- axis

  axis(qry, n)
  axis(qry, n) <- axis

  slicers(qry)
  slicers(qry) <- axis

  compose(qry)

  is.Query(qry)

```


 ## <a name="arguments"></a>Arguments



 ### `validate`
 A logical (TRUE, FALSE, NA) specifying whether the Query should be validated during execution 


 ### `qry`
 An object of class "Query" returned by `Query` 


 ### `cubeName`
 A string specifying the name of the cube to query 


 ### `axis`
 A vector of strings specifying an axis. See example below. 


 ### `n`
 An integer representing the axis number to be set. axis(qry, 1) == columns(qry), axis(qry, 2) == pages(qry), etc. 




 ## <a name="details"></a>Details

`Query` is the constructor for the Query object. Set functions are used to specify what the Query should return. Queries are passed to the `Execute2D` and `ExecuteMD` functions. `compose` takes the Query object and generates an MDX string equivalent to the one that the Execute functions would generate and use.



 ## <a name="value"></a>Value

`Query` returns an object of type "Query". 
`cube` returns a string. 
`columns` returns a vector of strings. 
`rows` returns a vector of strings. 
`pages` returns a vector of strings. 
`sections` returns a vector of strings. 
`axis` returns a vector of strings. 
`slicers` returns a vector of strings. 
`compose` returns a string. 
`is.Query` returns a boolean.


 ## <a name="note"></a>Note

- A Query object is not as powerful as pure MDX. If the Query API is not sufficient, try using an MDX Query string with one of the Execute functions.



 ## <a name="references"></a>References
  See [execute2D](Execute2D.md) or [executeMD](ExecuteMD.md) for references.  


 ## <a name="see-also"></a>See Also

[execute2D](Execute2D.md), [executeMD](ExecuteMD.md), [OlapConnection](OlapConnection.md)`, `[explore](Explore.md)


 ## <a name="examples"></a>Examples

 ```

  qry <- Query(validate = TRUE)

  cube(qry) <- "[Analysis Services Tutorial]"

  columns(qry) <- c("[Measures].[Internet Sales Count]", "[Measures].[Internet Sales-Sales Amount]")
  rows(qry) <- c("[Product].[Product Line].[Product Line].MEMBERS") 
  axis(qry, 3) <- c("[Date].[Calendar Quarter].MEMBERS")

  slicers(qry) <- c("[Sales Territory].[Sales Territories].[Sales Territory Region].[Northwest]")

  print(cube(qry)) #[Analysis Services Tutorial]
  print(axis(qry, 2)) #c("[Product].[Product Line].[Product Line].MEMBERS") 

  print(compose(qry))  #SELECT {[Measures].[Internet Sales Count], [Measures].[Internet Sales-Sales Amount]} ON AXIS(0), {[Product].[Product Line].[Product Line].MEMBERS} ON AXIS(1), {[Date].[Calendar Quarter].MEMBERS} ON AXIS(2) FROM [Analysis Services Tutorial] WHERE {[Sales Territory].[Sales Territories].[Sales Territory Region].[Northwest]}
```

