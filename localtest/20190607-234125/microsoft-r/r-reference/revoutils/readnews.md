---
title: Read R or Package NEWS Files
description: Read the R NEWS file or a package's NEWS or NEWS.Rd file.
keywords: ', readNews, utilities, documentation'
author: richcalaway
ms.author: richcala
manager: cgronlun
ms.date: 03/27/2017
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ms.openlocfilehash: ae83556580853a98d3eb14aa064181fb1bf978e2
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="readnews-read-r-or-package-news-files"></a>readNews: Read R or Package NEWS Files 
 ## <a name="description"></a>Description
 Read the R NEWS file or a package's NEWS or NEWS.Rd file. 
 
 ## <a name="usage"></a>Usage

```   
  readNews(package)
 
```
 
 ## <a name="arguments"></a>Arguments

   
    
 ### <a name="package"></a>package
 a character string specifying the package for which you'd like to read the  news. If missing, the R NEWS is displayed. 
  
 
 
 
 ## <a name="details"></a>Details
 
The R NEWS file is displayed using `RShowDoc` or `file.show`, depending on whether the system appears capable of launching a browser. Similarly, package NEWS.Rd files are displayed using `browseURL` or `file.show`.

This function should not be confused with readNEWS in the **tools** package, which performs a different kind of reading.
 
 
 ## <a name="value"></a>Value
 
`NULL` is returned invisibly.
 
 
 
 
 
