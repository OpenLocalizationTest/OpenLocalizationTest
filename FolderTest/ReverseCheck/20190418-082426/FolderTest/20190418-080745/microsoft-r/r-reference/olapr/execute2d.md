---
title: execute2D function (olapR) | Microsoft Docs
description: "   Takes a Query object or an MDX string, and returns the result as a data frame. "
keywords: (olapR), execute2D
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
ms.openlocfilehash: 7aa95d506f0cea626fbd727504beeb05c389b4c3
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="execute2d-olapr-execute2d-methods"></a>execute2D: olapR execute2D Methods 

 ## <a name="description"></a>Description

Takes a Query object or an MDX string, and returns the result as a data frame.



 ## <a name="usage"></a>Usage

```   
  execute2D(olapCnn, query)
  execute2D(olapCnn, mdx)

```


 ## <a name="arguments"></a>Arguments



 ### `olapCnn`
 Object of class "OlapConnection" returned by `OlapConnection()` 


 ### `query`
 Object of class "Query" returned by `Query()` 


 ### `mdx`
 String specifying a valid MDX query 




 ## <a name="details"></a>Details

If a query is provided: `execute2D` validates a query object (optional), generates an mdx query string from the query object, executes the mdx query across, and returns the result as a data frame.

If an MDX string is provided: `execute2D` executes the mdx query, and returns the result as a data frame.



 ## <a name="value"></a>Value

A data frame if the MDX command returned a result-set. 
`TRUE` and a warning if the query returned no data. An error if the query is invalid


 ## <a name="note"></a>Note

Multi-dimensional query results are flattened to 2D using a standard flattening algorithm.



 ## <a name="references"></a>References

Creating a Demo OLAP Cube (the same as the one used in the examples): [`https://msdn.microsoft.com/en-us/library/ms170208.aspx`](https://msdn.microsoft.com/en-us/library/ms170208.aspx)




 ## <a name="see-also"></a>See Also

[Query](Query.md)`, `[OlapConnection](OlapConnection.md)`, `[executeMD](ExecuteMD.md)`, `[explore](Explore.md)`, `data.frame


 ## <a name="examples"></a>Examples

 ```

  cnnstr <- "Data Source=localhost; Provider=MSOLAP;"
  olapCnn <- OlapConnection(cnnstr)

  qry <- Query()

  cube(qry) <- "[Analysis Services Tutorial]"
  columns(qry) <- c("[Measures].[Internet Sales Count]", "[Measures].[Internet Sales-Sales Amount]")
  rows(qry) <- c("[Product].[Product Line].[Product Line].MEMBERS") 
  pages(qry) <- c("[Sales Territory].[Sales Territory Region].[Sales Territory Region].MEMBERS")

  result1 <- execute2D(olapCnn, qry)

  mdx <- "SELECT {[Measures].[Internet Sales Count], [Measures].[Internet Sales-Sales Amount]} ON AXIS(0), {[Product].[Product Line].[Product Line].MEMBERS} ON AXIS(1), {[Sales Territory].[Sales Territory Region].[Sales Territory Region].MEMBERS} ON AXIS(2) FROM [Analysis Services Tutorial]"

  result2 <- execute2D(olapCnn, mdx)
```

