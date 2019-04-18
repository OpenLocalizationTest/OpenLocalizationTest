---
title: 'rx_hadoop_remove_dir: Execute Hadoop remove directory commands (revoscalepy)'
description: Wraps the Hadoop fs -rm -r  or fs -rm -r -skipTrash command.
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
ms.openlocfilehash: bf8a7e81d97d8918eaf7423670929c2eed596de8
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="rxhadoopremovedir"></a>rx_hadoop_remove_dir


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_hadoop_remove_dir(path: typing.Union[list, str],
    skip_trash=False)
```





## <a name="description"></a>Description

Wraps the Hadoop *fs -rm -r*  or *fs -rm -r -skipTrash* command.


## <a name="arguments"></a>Arguments


### <a name="path"></a>path

Character string or list. A list of paths or A character string specifying location of one or more directories.

:param skip_trash. If True, removal bypasses the trash folder, if one has been set up.


## <a name="example"></a>Example



```
from revoscalepy import rx_hadoop_remove_dir
rx_hadoop_remove_dir("/user/RevoShare/newUser", skip_trash = True)
```

