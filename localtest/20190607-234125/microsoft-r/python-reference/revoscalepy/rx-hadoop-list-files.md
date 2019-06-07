---
title: 'rx_hadoop_list_files: Execute Hadoop list files commands (revoscalepy)'
description: Wraps the Hadoop fs -ls or -lsr command.
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
ms.openlocfilehash: b1e2cf647cb61b9a5c6c51b297d2803fc0d108e2
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxhadooplistfiles"></a>rx_hadoop_list_files


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_hadoop_list_files(path: typing.Union[list, str],
    recursive=False)
```





## <a name="description"></a>Description

Wraps the Hadoop *fs -ls* or *-lsr* command.


## <a name="arguments"></a>Arguments


### <a name="path"></a>path

Character string or list. A list of paths or A character string specifying location of one or more files or directories.


### <a name="recursive"></a>recursive

Bool value. If True, directory listings are recursive.


## <a name="example"></a>Example



```
from revoscalepy import rx_hadoop_list_files
rx_hadoop_list_files("/user/RevoShare/newUser")
```

