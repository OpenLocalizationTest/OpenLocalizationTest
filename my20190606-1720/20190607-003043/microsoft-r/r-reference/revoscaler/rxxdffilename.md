---
title: rxXdfFileName-methods methods (revoAnalytics) | Microsoft Docs
description: " Get the .xdf file path from a character string or RxXdfData object. "
keywords: (revoAnalytics), rxXdfFileName-methods, rxXdfFileName, rxXdfFileName,RxXdfData-method, rxXdfFileName,character-method, rxXdfFileName,ANY-method, methods, file, connection
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
ms.openlocfilehash: 2170d1f02c87a98a74876f90d76cea82184e95b3
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxxdffilename-methods-retrieve-xdf-file-name"></a>rxXdfFileName-methods: Retrieve .xdf file name 
 ## <a name="description"></a>Description

Get the .xdf file path from a character string or RxXdfData object.


 ## <a name="usage"></a>Usage

```   
  rxXdfFileName( x )

```

 ## <a name="arguments"></a>Arguments



 ### `x`
 character string containing the file name or an RxXdfData object. 



 ## <a name="value"></a>Value

a character string containing the path and name of the .xdf file

 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[RxXdfData](RxXdfData.md)

 ## <a name="examples"></a>Examples

 ```

  # Create an RxXdfData object
  ds <- RxXdfData(file.path(rxGetOption("sampleDataDir"), "claims.xdf"))
  # Retrieve the file name with path
  fileName <- rxXdfFileName(ds)
  fileName
```




