---
title: 'RxOptions: Global options for revoscalepy (revoscalepy)'
description: Functions to specify and retrieve options needed for revoscalepy computations. These need to be set only once to carry out multiple computations.
keywords: options
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
ms.openlocfilehash: e7bbf59f3f75aac138514777cae13402543fd094
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxoptions"></a>RxOptions


 



```
revoscalepy.RxOptions
```





## <a name="description"></a>Description

Functions to specify and retrieve options needed for revoscalepy computations. These need to be set only once to carry out multiple computations.


## <a name="arguments"></a>Arguments


### <a name="unittestdatadir"></a>unitTestDataDir

Character string specifying path to revoscalepy’s test data directory.


### <a name="sampledatadir"></a>sampleDataDir

Character string specifying path to revoscalepy’s sample data directory.


### <a name="blocksperread"></a>blocksPerRead

Default value to use for blocksPerRead argument for many revoscalepy functions. Represents the number of blocks to read within each read chunk.


### <a name="reportprogress"></a>reportProgress

Default value to use for reportProgress argument for many revoscalepy functions. Options are:

    0: no progress is reported.
    1: the number of processed rows is printed and updated.
    2: rows processed and timings are reported.
    3: rows processed and all timings are reported.


### <a name="rowdisplaymax"></a>RowDisplayMax

Integer value specifying the maximum number of rows to display when using the verbose argument in revoscalepy functions. The default of -1 displays all available rows.


### <a name="memstatsreset"></a>MemStatsReset

Boolean integer. If 1, reset memory status


### <a name="memstatsdiff"></a>MemStatsDiff

Boolean integer. If 1, the change of memory status is shown.


### <a name="numcorestouse"></a>NumCoresToUse

Integer value specifying the number of cores to use.
If set to a value higher than the number of available cores, the number of available cores will be used. If set to -1, the number of available cores will be used. Increasing the number of cores to use will also increase the amount of memory required for revoscalepy analysis functions.


### <a name="numdigits"></a>NumDigits

Controls the number of digits to to use when converting numeric data to or from strings, such as when printing numeric values or importing numeric data as strings. The default is the current value of options()$digits, which defaults to 7. Beyond fifteen digits, however, results are likely to be unreliable.


### <a name="showtransformfn"></a>ShowTransformFn

Bool value. If True, the transform function is shown.


### <a name="datapath"></a>DataPath

List of strings containing paths to search for local data sources. The default is to search just the current working directory. This will be ignored if dataPath is specified in the active compute context. See the Details section for more information regarding the path format.


### <a name="outdatapath"></a>OutDataPath

List of strings containing paths for writing new output data files. New data files will be written to the first path that exists. The default is to write to the current working directory. This will be ignored if outDataPath is specified in the active compute context.


### <a name="xdfcompressionlevel"></a>XdfCompressionLevel

Integer in the range of -1 to 9. The higher the value, the greater the amount of compression - resulting in smaller files but a longer time to create them.


### <a name="filesystem"></a>FileSystem

Character string or RxFileSystem object indicating type of file system; “native” or RxNativeFileSystem object can be used for the local operating system, or an RxHdfsFileSystem object for the Hadoop file system.


### <a name="usesparsecube"></a>UseSparseCube

Bool value. If True, sparse cube is used.


### <a name="rngbffersize"></a>RngBfferSize

A positive integer scalar specifying the buffer size for the Parallel Random Number Generators (RNGs) in MKL.


### <a name="dropmain"></a>DropMain

Bool value. If True, main-effect terms are dropped before their interactions.


### <a name="coeflabelstyle"></a>CoefLabelStyle

Character string specifying the coefficient label style. The default is “Revo”.


### <a name="numtasks"></a>NumTasks

Integer value. The default numTasks use in RxInSqlServer.


### <a name="unixpythonpath"></a>unixPythonPath

The path to Python executable on a Unix/Linux node.
By default it points to a path corresponding to this client’s version.


### <a name="tracelevel"></a>traceLevel

Specifies the traceLevel that ML server will run with. This parameter controls ML Server Logging features as well as Runtime Tracing of ScalePy functions. Levels are inclusive, (i.e. level 3:INFO includes levels 2:WARN and 1:ERROR log messages). The options are:

    0: DISABLED - Tracing/Logging disabled.
    1: ERROR - ERROR coded trace points are logged to MRS log files
    2: WARN - WARN and ERROR coded trace points are logged to MRS log files.
    3: INFO - INFO, WARN, and ERROR coded trace points are logged to MRS

        log files.

    4: DEBUG - All trace points are logged to MRS log files.
    5: RESERVED - If set, will log at DEBUG granularity
    6: RESERVED - If set, will log at DEBUG granularity
    7: TRACE - ScaleR functions Runtime Tracing is activated and MRS log

        level is set to DEBUG granularity.


## <a name="returns"></a>Returns

For RxOptions, a list containing the original RxOptions is returned.

If there is no argument specified, the list is returned explicitly, otherwise the list is returned as an invisible object. For RxGetOption, the current value of the requested option is returned.


## <a name="example"></a>Example



```
from revoscalepy import RxOptions
sample_data_path = RxOptions.get_option("sampleDataDir")
```

