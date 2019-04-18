---
title: 'rx_hadoop_copy_to_local: Execute Hadoop copyToLocal commands (revoscalepy)'
description: Wraps the Hadoop fs -copyToLocal command.
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
ms.openlocfilehash: 38e0f3c8b67b724646c5c0981047838249b40794
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="rxhadoopcopytolocal"></a>rx_hadoop_copy_to_local


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_hadoop_copy_to_local(source: str, dest: str)
```





## <a name="description"></a>Description

Wraps the Hadoop *fs -copyToLocal* command.


## <a name="arguments"></a>Arguments


### <a name="source"></a>source

A character string specifying file(s) to be copied in HDFS


### <a name="dest"></a>dest

A character string specifying the destination of a copy in Local File System If *source* includes more than one file, *dest* must be a directory.


## <a name="example"></a>Example



```
from revoscalepy import rx_hadoop_copy_to_local
rx_hadoop_copy_to_local("/user/RevoShare/foo.txt", "/tmp/foo.txt")
```

