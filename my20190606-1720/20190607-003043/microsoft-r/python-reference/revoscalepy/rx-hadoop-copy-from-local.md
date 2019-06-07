---
title: 'rx_hadoop_copy_from_local: Execute Hadoop copyFromLocal commands (revoscalepy)'
description: Wraps the Hadoop fs -copyFromLocal command.
keywords: Hadoop Command
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
ms.openlocfilehash: 3cd8346513efdad27d8ddba68df9c1ad32089ebd
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxhadoopcopyfromlocal"></a>rx_hadoop_copy_from_local


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_hadoop_copy_from_local(source: str, dest: str)
```





## <a name="description"></a>Description

Wraps the Hadoop *fs -copyFromLocal* command.


## <a name="arguments"></a>Arguments


### <a name="source"></a>source

A character string specifying file(s) in Local File System


### <a name="dest"></a>dest

A character string specifying the destination of a copy in HDFS If *source* includes more than one file, *dest* must be a directory.


## <a name="example"></a>Example



```
from revoscalepy import rx_hadoop_copy_from_local
rx_hadoop_copy_from_local("/tmp/foo.txt", "/user/RevoShare/newUser")
```

