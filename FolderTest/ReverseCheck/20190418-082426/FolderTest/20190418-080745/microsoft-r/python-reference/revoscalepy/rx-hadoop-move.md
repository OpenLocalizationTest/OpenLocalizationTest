---
title: 'rx_hadoop_move: Execute Hadoop move commands (revoscalepy)'
description: Wraps the Hadoop fs -mv command.
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
ms.openlocfilehash: 8ff7d7465139f1c404cb1f62c15b753824a2177d
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="rxhadoopmove"></a>rx_hadoop_move


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_hadoop_move(source: str, dest: str)
```





## <a name="description"></a>Description

Wraps the Hadoop *fs -mv* command.


## <a name="arguments"></a>Arguments


### <a name="source"></a>source

A character string specifying file(s) to be moved in HDFS


### <a name="dest"></a>dest

A character string specifying the destination of move in HDFS If *source* includes more than one file, *dest* must be a directory.


## <a name="example"></a>Example



```
from revoscalepy import rx_hadoop_move
rx_hadoop_move("/user/RevoShare/newUser/foo.txt","/user/RevoShare/newUser/bar.txt")
```

