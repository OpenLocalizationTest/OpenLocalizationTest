---
title: 'rx_hadoop_make_dir: Execute Hadoop make directory commands (revoscalepy)'
description: Wraps the Hadoop fs -mkdir -p command.
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
ms.openlocfilehash: ca0ac639a9f2157086da0f47773066e07c746d26
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxhadoopmakedir"></a>rx_hadoop_make_dir


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_hadoop_make_dir(path: typing.Union[list, str])
```





## <a name="description"></a>Description

Wraps the Hadoop *fs -mkdir -p* command.


## <a name="arguments"></a>Arguments


### <a name="path"></a>path

Character string or list. A list of paths or A character string specifying location of one or more directories.


## <a name="example"></a>Example



```
from revoscalepy import rx_hadoop_make_dir
rx_hadoop_make_dir("/user/RevoShare/newUser")
```

