---
title: 'rx_read_xdf: Read an XDF data source object (revoscalepy)'
description: Read data from an “.xdf” file into a data frame.
keywords: xdf
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
ms.openlocfilehash: 4d7187c04ad04418d1d6dfb58dee325f30f23adf
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="rxreadxdf"></a>rx_read_xdf


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_read_xdf(file: str, vars_to_keep: list = None,
    vars_to_drop: list = None, row_var_name: str = None,
    start_row: int = 1, num_rows: int = None,
    return_data_frame: bool = True,
    strings_as_factors: bool = False,
    max_rows_by_columns: int = None, report_progress: int = None,
    read_by_block: bool = False, cpp_interp: list = None)
```





## <a name="description"></a>Description

Read data from an “.xdf” file into a data frame.


## <a name="arguments"></a>Arguments


### <a name="file"></a>file

Either an RxXdfData object or a character string specifying the “.xdf” file.


### <a name="varstokeep"></a>vars_to_keep

List of strings of variable names to include when reading from the input data file. If None, argument is ignored. Cannot be used with vars_to_drop.


### <a name="varstodrop"></a>vars_to_drop

List of strings of variable names to exclude when reading from the input data file. If None, argument is ignored. Cannot be used with vars_to_keep.


### <a name="rowvarname"></a>row_var_name

Optional character string specifying the variable in the data file to use as row names for the output data frame.


### <a name="startrow"></a>start_row

Starting row for retrieval.


### <a name="numrows"></a>num_rows

Number of rows of data to retrieve. If -1, all are read.


### <a name="returndataframe"></a>return_data_frame

Bool indicating whether or not to create a data frame. If False, a list is returned.


### <a name="stringsasfactors"></a>strings_as_factors

Bool indicating whether or not to convert strings into factors.


### <a name="maxrowsbycolumns"></a>max_rows_by_columns

The maximum size of a data frame that will be read in, measured by the number of rows times the number of columns. If the number of rows times the number of columns being extracted from the “.xdf” file exceeds this, a warning will be reported and a smaller number of rows will be read in than requested. If max_rows_by_columns is set to be too large, you may experience problems from loading a huge data frame into memory. To extract a subset of rows and/or columns from an “.xdf” file, use rx_data_step.


### <a name="reportprogress"></a>report_progress

Integer value with options: 0: No progress is reported.
1: The number of processed rows is printed and updated.
2: Rows processed and timings are reported.
3: Rows processed and all timings are reported.


### <a name="readbyblock"></a>read_by_block

Read data by blocks. This argument is deprecated.


### <a name="cppinterp"></a>cpp_interp

List of information sent to C++ interpreter.


## <a name="returns"></a>Returns

a data frame.


## <a name="see-also"></a>See also

[`rx_import`](rx-import.md), [`rx_data_step`](rx-data-step.md).


## <a name="example"></a>Example



```
import os
from revoscalepy import RxOptions, rx_read_xdf

sample_data_path = RxOptions.get_option("sampleDataDir")
mort_file = os.path.join(sample_data_path, "mortDefaultSmall.xdf")
mort_df = rx_read_xdf(mort_file, num_rows = 10)
print(mort_df)
```


Output:



```

Rows Processed: 10
Time to read data file: 0.00 secs.
Time to convert to data frame: less than .001 secs.
   creditScore  houseAge  yearsEmploy  ccDebt  year  default
0          691        16            9    6725  2000        0
1          691         4            4    5077  2000        0
2          743        18            3    3080  2000        0
3          728        22            1    4345  2000        0
4          745        17            3    2969  2000        0
5          539        15            3    4588  2000        0
6          724         6            5    4057  2000        0
7          659        14            3    6456  2000        0
8          621        18            3    1861  2000        0
9          720        14            7    4568  2000        0
```

