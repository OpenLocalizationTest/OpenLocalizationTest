---
title: 'rx_partition: Partition by key value and save to a partitioned .xdf (revoscalepy)'
description: Partition input data sources by key values and save the results to a partitioned .xdf file on disk.
keywords: partition
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
ms.openlocfilehash: d550b0df8f6f9baef03ef44892ac76d96398022e
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxpartition"></a>rx_partition


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_partition(input_data: typing.Union[revoscalepy.datasource.RxDataSource.RxDataSource,
    pandas.core.frame.DataFrame, str],
    output_data: revoscalepy.datasource.RxXdfData.RxXdfData,
    vars_to_partition: typing.Union[typing.List[str], str],
    append: str = 'rows', overwrite: bool = False,
    **kwargs) -> pandas.core.frame.DataFrame
```





## <a name="description"></a>Description

Partition input data sources by key values and save the results to a partitioned .xdf file on disk.


## <a name="arguments"></a>Arguments


### <a name="inputdata"></a>input_data

Either a data source object, a character string specifying a ‘.xdf’ file, or a Pandas data frame object.


### <a name="outputdata"></a>output_data

A partitioned data source object created by RxXdfData with create_partition_set = True.


### <a name="varstopartition"></a>vars_to_partition

List of strings of variable names to be used for partitioning the input data set.


### <a name="append"></a>append

Either “none” to create a new file or “rows” to append rows to an existing file. If output_data exists and append is “none”, the overwrite argument must be set to True.


### <a name="overwrite"></a>overwrite

Bool value. If True, an existing output_data will be overwritten.
overwrite is ignored if appending rows.


### <a name="kwargs"></a>kwargs

Additional arguments.


## <a name="returns"></a>Returns

A Pandas data frame of partitioning values and data sources, each row in the Pandas data frame represents one partition and the data source in the last variable holds the data of a specific partition.


## <a name="see-also"></a>See also

[`rx_exec_by`](rx-exec-by.md).
[`RxXdfData`](RxXdfData.md).


## <a name="example"></a>Example



```
import os, tempfile
from revoscalepy import RxOptions, RxXdfData, rx_partition
data_path = RxOptions.get_option("sampleDataDir")

# input xdf data source
xdf_file = os.path.join(data_path, "claims.xdf")
xdf_ds = RxXdfData(xdf_file)

# create a partitioned xdf data source object
out_xdf_file = os.path.join(tempfile._get_default_tempdir(), "outPartitions")
out_xdf = RxXdfData(out_xdf_file, create_partition_set = True)

# do partitioning for input data set
partitions = rx_partition(input_data = xdf_ds, output_data = out_xdf, vars_to_partition = ["car.age","type"])
print(partitions)
```

