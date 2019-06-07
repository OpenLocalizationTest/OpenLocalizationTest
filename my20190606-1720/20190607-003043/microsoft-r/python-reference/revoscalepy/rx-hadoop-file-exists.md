---
title: 'rx_hadoop_file_exists: Execute Hadoop files exists commands (revoscalepy)'
description: Wraps the Hadoop fs -test -e command.
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
ms.openlocfilehash: 2a2bf6b1ebfa41f72fbe61401e89a2c082d9d304
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxhadoopfileexists"></a>rx_hadoop_file_exists


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_hadoop_file_exists(path: typing.Union[list, str])
```





## <a name="description"></a>Description

Wraps the Hadoop *fs -test -e* command.


## <a name="arguments"></a>Arguments


### <a name="path"></a>path

Character string or list. A list of paths or A character string specifying location of one or more files or directories.


## <a name="returns"></a>Returns

A bool value specifying whether file exists.


## <a name="example"></a>Example



```
from revoscalepy import rx_hadoop_file_exists
rx_hadoop_file_exists("/user/RevoShare/newUser/foo.txt")
```

