---
title: OlapConnection function (olapR) | Microsoft Docs
description: "   OlapConnection constructs a OlapConnection object. "
keywords: (olapR), OlapConnection
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
ms.openlocfilehash: 2c11ebe3193d06c73def9c9c0c699525db068885
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="olapconnection-olapr-olapconnection-creation"></a>OlapConnection: olapR OlapConnection Creation 

 ## <a name="description"></a>Description

`OlapConnection` constructs a "OlapConnection" object.



 ## <a name="usage"></a>Usage

```   
  OlapConnection(connectionString="Data Source=localhost; Provider=MSOLAP;")

  is.OlapConnection(ocs)

  print.OlapConnection(ocs)

```


 ## <a name="arguments"></a>Arguments



 ### `connectionString`
 A valid connection string for connecting to Analysis Services 


 ### `ocs`
 An object of class "OlapConnection" 




 ## <a name="details"></a>Details

`OlapConnection` validates and holds an Analysis Services connection string. By default, Analysis Services returns the first cube of the first database. To connect to a specific database, use the Initial Catalog parameter.



 ## <a name="value"></a>Value

`OlapConnection` returns an object of type "OlapConnection". A warning is shown if the connection string is invalid.


 ## <a name="references"></a>References
  For more information on Analysis Services connection strings: [`https://docs.microsoft.com/sql/analysis-services/instances/connection-string-properties-analysis-services`](https://docs.microsoft.com/sql/analysis-services/instances/connection-string-properties-analysis-services)



 ## <a name="see-also"></a>See Also

[Query](Query.md), [executeMD](ExecuteMD.md), [execute2D](Execute2D.md)`, `[explore](Explore.md)


 ## <a name="examples"></a>Examples

 ```


  # Create the connection string. For a named instance, escape the instance name: localhost\my-other-instance
  cnnstr <- "Data Source=localhost; Provider=MSOLAP; initial catalog=AdventureWorksCube"
  olapCnn <- OlapConnection(cnnstr)
```

