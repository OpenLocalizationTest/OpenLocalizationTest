---
title: 'RxNativeFileSystem: Class generator for the native file system (revoscalepy)'
description: Main generator class for objects repreresenting the native file system.
keywords: filesystem native
author: HeidiSteen
manager: cgronlun
ms.date: 01/26/2018
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ROBOTS: ''
audience: ''
ms.devlang: Python
ms.reviewer: ''
ms.suite: ''
ms.tgt_pltfrm: ''
ms.custom: ''
ms.openlocfilehash: 4115ce363f21e522972d2faf2994545b99bd5c59
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxnativefilesystem"></a>RxNativeFileSystem


 



```
revoscalepy.RxNativeFileSystem
```





## <a name="description"></a>Description

Main generator class for objects representing the native file system.


## <a name="returns"></a>Returns

An RxNativeFileSystem file system object. This object may be used in [`RxOptions`](RxOptions.md), [`RxTextData`](RxTextData.md), or [`RxXdfData`](RxXdfData.md) to set the file system.


## <a name="see-also"></a>See also

[`RxOptions`](RxOptions.md)
[`RxTextData`](RxTextData.md)
[`RxXdfData`](RxXdfData.md)
[`RxFileSystem`](RxFileSystem.md)


## <a name="example"></a>Example



```
from revoscalepy import RxNativeFileSystem
fs = RxNativeFileSystem()
print(fs.file_system_type())
```

