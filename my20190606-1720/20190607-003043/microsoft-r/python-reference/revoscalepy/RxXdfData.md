---
title: 'RxXdfData: Class generator for XDF data source objects (revoscalepy)'
description: Main generator for class RxXdfData, which extends RxDataSource.
keywords: datasource, xdf
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
ms.openlocfilehash: c4452950d3c33595a0f02ffeb709065e127cd01e
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxxdfdata"></a>RxXdfData


 



```
revoscalepy.RxXdfData(file: str, vars_to_keep=None, vars_to_drop=None,
    return_data_frame=True, strings_as_factors=False, blocks_per_read=1,
    file_system: typing.Union[str,
    revoscalepy.datasource.RxFileSystem.RxFileSystem] = 'native',
    create_composite_set=None, create_partition_set=None,
    blocks_per_composite_file=3)
```





## <a name="description"></a>Description

Main generator for class RxXdfData, which extends RxDataSource.


## <a name="arguments"></a>Arguments


### <a name="file"></a>file

Character string specifying the location of the data. For single Xdf, it is a ‘.xdf’ file. For composite Xdf, it is a directory like ‘/tmp/airline’. When using distributed compute contexts like RxSpark, a directory should be used since those compute contexts always use composite Xdf.


### <a name="varstokeep"></a>vars_to_keep

List of strings of variable names to keep around during operations. If None, argument is ignored. Cannot be used with vars_to_drop.


### <a name="varstodrop"></a>vars_to_drop

list of strings of variable names to drop from operations. If None, argument is ignored. Cannot be used with vars_to_keep.


### <a name="returndataframe"></a>return_data_frame

Bool value indicating whether or not to convert the result to a data frame.


### <a name="stringsasfactors"></a>strings_as_factors

Bool value indicating whether or not to convert strings into factors (for reader mode only).


### <a name="blocksperread"></a>blocks_per_read

Number of blocks to read for each chunk of data read from the data source.


### <a name="filesystem"></a>file_system

Character string or RxFileSystem object indicating type of file system; “native” or RxNativeFileSystem object can be used for the local operating system. If None, the file system will be set to that in the current compute context, if available, otherwise the fileSystem option.


### <a name="createcompositeset"></a>create_composite_set

Bool value or None. Used only when writing.
If True, a composite set of files will be created instead of a single ‘.xdf’ file. Subdirectories ‘data’ and ‘metadata’ will be created. In the ‘data’ subdirectory, the data will be split across a set of ‘.xdfd’ files (see blocks_per_composite_file below for determining how many blocks of data will be in each file). In the ‘metadata’ subdirectory there is a single ‘.xdfm’ file, which contains the meta data for all of the ‘.xdfd’ files in the ‘data’ subdirectory. When the compute context is RxSpark, a composite set of files is always created.


### <a name="createpartitionset"></a>create_partition_set

Bool value or None. Used only when writing.
If True, a set of files for partitioned Xdf will be created when assigning this RxXdfData object for outData of rxPartition. Subdirectories ‘data’ and ‘metadata’ will be created. In the ‘data’ subdirectory, the data will be split across a set of ‘.xdf’ files (each file stores data of a single data partition, see rxPartition for details). In the ‘metadata’ subdirectory there is a single ‘.xdfp’ file, which contains the meta data for all of the ‘.xdf’ files in the ‘data’ subdirectory. The partitioned Xdf object is currently supported only in rxPartition and rxGetPartitions


### <a name="blockspercompositefile"></a>blocks_per_composite_file

Integer value. If create_composite_set=True, this will be the number of blocks put into each ‘.xdfd’ file in the composite set. RxSpark compute context will optimize the number of blocks based upon HDFS and Spark settings.


## <a name="returns"></a>Returns

Object of class `RxXdfData`.


## <a name="example"></a>Example



```
import os
from revoscalepy import rx_data_step, RxOptions, RxXdfData
sample_data_path = RxOptions.get_option("sampleDataDir")
ds = RxXdfData(os.path.join(sample_data_path, "kyphosis.xdf"))
kyphosis = rx_data_step(ds)
```

