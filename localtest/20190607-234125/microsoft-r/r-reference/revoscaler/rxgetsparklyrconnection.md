---
title: rxGetSparklyrConnection function (revoAnalytics) | Microsoft Docs
description: " Get a Spark compute context with sparklyr interop.  rxGetSparklyrConnection get sparklyr spark connection from created Spark compute context. "
keywords: (revoAnalytics), rxGetSparklyrConnection
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
ms.openlocfilehash: b4948938b55080307d9a76df3cc69fb750e0e8f6
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxgetsparklyrconnection-get-sparklyr-connection-from-spark-compute-context"></a>rxGetSparklyrConnection: Get sparklyr connection from Spark compute context 
 ## <a name="description"></a>Description
  Get a Spark compute context with sparklyr interop.
 `rxGetSparklyrConnection` get sparklyr spark connection from created Spark compute context.


 ## <a name="usage"></a>Usage

```   
  rxGetSparklyrConnection(
      computeContext = rxGetOption("computeContext"))

```


 ## <a name="arguments"></a>Arguments



 ### `computeContext`
 Compute context get created by `rxSparkConnect`. 




 ## <a name="value"></a>Value

object of sparklyr spark connection


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="examples"></a>Examples

 ```

  ## Not run:

library("sparklyr")
cc <- rxSparkConnect(interop = "sparklyr")
sc <- rxGetSparklyrConnection(cc)
iris_tbl <- copy_to(sc, iris)
 ## End(Not run) 
```

