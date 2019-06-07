---
title: " Obtain Total System Memory "
description: " Uses operating system tools to return total system memory. "
keywords: ', totalSystemMemory,  sysdata '
author: richcalaway
ms.author: richcala
manager: cgronlun
ms.date: 03/27/2017
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ms.openlocfilehash: 10a65eadcc627d776cb9e0fa64b2666e7ae1168c
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="totalsystemmemory--obtain-total-system-memory"></a>totalSystemMemory:  Obtain Total System Memory  
 ## <a name="description"></a>Description

Uses operating system tools to return total system memory.


 ## <a name="usage"></a>Usage

```   
  totalSystemMemory()

```

 ## <a name="details"></a>Details

On Unix-alikes, checks the `/proc/meminfo` file for the total memory. If the system call returns an error, the function returns `NA`. On Windows systems, uses `wmic` to obtain the `TotalVisibleMemorySize`.


 ## <a name="value"></a>Value

A numeric value representing total system memory in kBytes, or `NA`.









 ## <a name="examples"></a>Examples

 ```

  totalSystemMemory()
```






