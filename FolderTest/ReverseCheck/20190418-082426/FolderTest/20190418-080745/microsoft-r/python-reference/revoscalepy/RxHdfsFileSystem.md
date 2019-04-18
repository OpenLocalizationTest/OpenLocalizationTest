---
title: 'RxHdfsFileSystem: Class generator for an HDFS file system object (revoscalepy)'
description: Main generator class for RxHdfsFileSystem.
keywords: filesystem hdfs
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
ms.openlocfilehash: df8429a3a7846cee03eb728fae68fbf43ed58637
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="rxhdfsfilesystem"></a>RxHdfsFileSystem


 



```
revoscalepy.RxHdfsFileSystem(host_name=None, port=None)
```





## <a name="description"></a>Description

Main generator class for RxHdfsFileSystem.


## <a name="returns"></a>Returns

An RxHdfsFileSystem file system object.
This object may be used in [`RxOptions`](RxOptions.md), [`RxTextData`](RxTextData.md), [`RxXdfData`](RxXdfData.md), [`RxParquetData`](RxParquetData.md), or [`RxOrcData`](RxOrcData.md) to set the file system.


## <a name="see-also"></a>See also

[`RxOptions`](RxOptions.md)
[`RxTextData`](RxTextData.md)
[`RxXdfData`](RxXdfData.md)
[`RxParquet`](RxParquetData.md)
[`RxOrcData`](RxOrcData.md)
[`RxFileSystem`](RxFileSystem.md)


## <a name="example"></a>Example



```
from revoscalepy import RxHdfsFileSystem
fs = RxHdfsFileSystem()
print(fs.file_system_type())
from revoscalepy import RxXdfData
xdf_data = RxXdfData("/tmp/hdfs_file", file_system = fs)
```

