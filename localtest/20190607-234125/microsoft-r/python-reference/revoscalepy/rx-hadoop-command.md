---
title: 'rx_hadoop_command: Execute Hadoop commands (revoscalepy)'
description: Executes arbitrary Hadoop commands and performs standard file operations in Hadoop.
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
ms.openlocfilehash: 3a3b67b043834c1efbe4ca709d7b39ee6c15875e
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxhadoopcommand"></a>rx_hadoop_command


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_hadoop_command(cmd: str) -> revoscalepy.functions.RxHadoopUtils.RxHadoopCommandResults
```





## <a name="description"></a>Description

Executes arbitrary Hadoop commands and performs standard file operations in Hadoop.


## <a name="arguments"></a>Arguments


### <a name="cmd"></a>cmd

A character string containing a valid Hadoop command, that is, the cmd portion of Hadoop Command. Embedded quotes are not permitted.


## <a name="returns"></a>Returns

Class RxHadoopCommandResults


## <a name="see-also"></a>See also

[`rx_hadoop_make_dir`](rx-hadoop-make-dir.md)
[`rx_hadoop_copy_from_local`](rx-hadoop-copy-from-local.md)
[`rx_hadoop_remove_dir`](rx-hadoop-remove-dir.md)
[`rx_hadoop_file_exists`](rx-hadoop-file-exists.md)
[`rx_hadoop_list_files`](rx-hadoop-list-files.md)


## <a name="example"></a>Example



```
from revoscalepy import rx_hadoop_command
rx_hadoop_command("version")
```

