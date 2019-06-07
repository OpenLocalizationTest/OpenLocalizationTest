---
title: 'rx_hadoop_copy: Execute Hadoop copy commands (revoscalepy)'
description: Wraps the Hadoop fs -cp command.
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
ms.openlocfilehash: baf0172ec46d37c490f1c9873ea201da49d8c2d5
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxhadoopcopy"></a>rx_hadoop_copy


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_hadoop_copy(source: str, dest: str)
```





## <a name="description"></a>Description

Wraps the Hadoop *fs -cp* command.


## <a name="arguments"></a>Arguments


### <a name="source"></a>source

A character string specifying file(s) to be copied in HDFS


### <a name="dest"></a>dest

A character string specifying the destination of a copy in HDFS If *source* includes more than one file, *dest* must be a directory.


## <a name="example"></a>Example



```
from revoscalepy import rx_hadoop_copy
rx_hadoop_copy("/user/RevoShare/newUser/foo.txt","/user/RevoShare/newUser/bar.txt")
```

