---
title: " Get Path to Package Repositories "
description: " `getRevoRepos` returns the path to either the Revolution Analytics CRAN mirror or the versioned package source repository maintained by Microsoft. "
keywords: ', getRevoRepos,  ~kwd1 ,  ~kwd2 '
author: richcalaway
ms.author: richcala
manager: cgronlun
ms.date: 03/27/2017
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ms.openlocfilehash: 561309e17cec6d91fc654e5ecf32fbb43a580b5d
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="getrevorepos--get-path-to-revolution-analytics-package-repositories"></a>getRevoRepos:  Get Path to Revolution Analytics Package Repositories  
 ## <a name="description"></a>Description

`getRevoRepos` returns the path to either the Revolution Analytics CRAN mirror or the versioned package source repository maintained by Revolution Analytics.


 ## <a name="usage"></a>Usage

```   
  getRevoRepos(version = paste(unlist(unclass(getRversion()))[1:2], collapse = "."), CRANmirror = FALSE)

```

 ## <a name="arguments"></a>Arguments



 ### <a name="version"></a>version
  A string or floating-point literal representing an R version from 2.9 or later. (2.10 is a valid version, but the versioned package source repository does not exist for this version of R.) This argument is ignored if `CRANmirror=TRUE`.  


 ### <a name="cranmirror"></a>CRANmirror
  A logical flag. If `TRUE`, the path to the Revolution Analytics CRAN mirror is returned.  



 ## <a name="value"></a>Value

A character string containing the path to the versioned package source repository or the Revolution Analytics CRAN mirror.












 ## <a name="examples"></a>Examples

 ```

    getRevoRepos(CRANmirror=TRUE)
```



