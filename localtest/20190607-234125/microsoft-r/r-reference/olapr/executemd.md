---
title: executeMD function (olapR) | Microsoft Docs
description: "   Takes a Query object or an MDX string, and returns the result as a multi-dimensional array. "
keywords: (olapR), executeMD
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
ms.openlocfilehash: aace0565f6463bf57cb2b46531337c39d2a95b52
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="executemd-olapr-executemd-methods"></a>executeMD: olapR executeMD Methods 

 ## <a name="description"></a>Description

Takes a Query object or an MDX string, and returns the result as a multi-dimensional array.



 ## <a name="usage"></a>Usage

```   
  executeMD(olapCnn, query)
  executeMD(olapCnn, mdx)

```


 ## <a name="arguments"></a>Arguments



 ### `olapCnn`
 Object of class "OlapConnection" returned by `OlapConnection()` 


 ### `query`
 Object of class "Query" returned by `Query()` 


 ### `mdx`
 String specifying a valid MDX query 




 ## <a name="details"></a>Details

If a Query is provided: `executeMD` validates a Query object (optional), generates an mdx query string from the Query object, executes the mdx query across an XMLA connection, and returns the result  as a multi-dimensional array.

If an MDX string is provided: `executeMD` executes the mdx query across an XMLA connection, and returns the result  as a multi-dimensional array.



 ## <a name="value"></a>Value

Returns a multi-dimensional array.
Returns an error if the Query is invalid.


 ## <a name="note"></a>Note





 ## <a name="references"></a>References

Creating a Demo OLAP Cube (the same as the one used in the examples): [`https://msdn.microsoft.com/en-us/library/ms170208.aspx`](https://msdn.microsoft.com/en-us/library/ms170208.aspx)




 ## <a name="see-also"></a>See Also

[Query](Query.md), [OlapConnection](OlapConnection.md)`, `[execute2D](Execute2D.md)`, `[explore](Explore.md)`, `array


 ## <a name="examples"></a>Examples

 ```

  cnnstr <- "Data Source=localhost; Provider=MSOLAP;"
  olapCnn <- OlapConnection(cnnstr)

  qry <- Query()

  cube(qry) <- "[Analysis Services Tutorial]"
  columns(qry) <- c("[Measures].[Internet Sales Count]", "[Measures].[Internet Sales-Sales Amount]")
  rows(qry) <- c("[Product].[Product Line].[Product Line].MEMBERS") 
  pages(qry) <- c("[Sales Territory].[Sales Territory Region].[Sales Territory Region].MEMBERS")

  result1 <- executeMD(olapCnn, qry)

  mdx <- "SELECT {[Measures].[Internet Sales Count], [Measures].[Internet Sales-Sales Amount]} ON AXIS(0), {[Product].[Product Line].[Product Line].MEMBERS} ON AXIS(1), {[Sales Territory].[Sales Territory Region].[Sales Territory Region].MEMBERS} ON AXIS(2) FROM [Analysis Services Tutorial]"

  result2 <- executeMD(olapCnn, mdx)
```

