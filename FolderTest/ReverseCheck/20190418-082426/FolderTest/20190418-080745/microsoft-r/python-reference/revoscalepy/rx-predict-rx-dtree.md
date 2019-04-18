---
title: 'rx_predict_rx_dtree: Prediction for Large Data Classification and Regression Trees (revoscalepy)'
description: Calculate predicted or fitted values for a data set from an rx_dtree object.
keywords: predict
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
ms.openlocfilehash: 66c3f9b9f28ebec72806ca87a17920d1bd0e8b25
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="rxpredictrxdtree"></a>rx_predict_rx_dtree


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_predict_rx_dtree(model_object=None,
    data: revoscalepy.datasource.RxDataSource.RxDataSource = None,
    output_data: typing.Union[revoscalepy.datasource.RxDataSource.RxDataSource,
    str] = None, predict_var_names: list = None,
    write_model_vars: bool = False,
    extra_vars_to_write: list = None, append: typing.Union[list,
    str] = 'none', overwrite: bool = False, type: typing.Union[list,
    str] = None, remove_missings: bool = False,
    compute_residuals: bool = False, residual_type: typing.Union[list,
    str] = 'usual', residual_var_names: list = None,
    blocks_per_read: int = None, report_progress: int = None,
    verbose: int = 0, xdf_compression_level: int = None,
    compute_context=None, **kwargs)
```





## <a name="description"></a>Description

Calculate predicted or fitted values for a data set from an rx_dtree object.


## <a name="arguments"></a>Arguments


### <a name="modelobject"></a>model_object

Object returned from a call to rx_dtree.


### <a name="data"></a>data

A data frame or an RxXdfData data source object to be used for predictions.
If a Spark compute context is being used, this argument may also be an RxHiveData, RxOrcData, RxParquetData or RxSparkDataFrame object or a Spark data frame object from pyspark.sql.DataFrame.


### <a name="outputdata"></a>output_data

An RxXdfData data source object or existing data frame to store predictions.


### <a name="predictvarnames"></a>predict_var_names

List of strings specifying name(s) to give to the prediction results


### <a name="writemodelvars"></a>write_model_vars

Bool value. If True, and the output data set is different from the input data set, variables in the model will be written to the output data set in addition to the predictions (and residuals, standard errors, and confidence bounds, if requested). If variables from the input data set are transformed in the model, the transformed variables will also be included.


### <a name="extravarstowrite"></a>extra_vars_to_write

None or list of strings of additional variables names from the input data or transforms to include in the output_data. If write_model_vars is True, model variables will be included as well.


### <a name="append"></a>append

Either “none” to create a new file or “rows” to append rows to an existing file. If output_data exists and append is “none”, the overwrite argument must be set to True. Ignored for data frames.


### <a name="overwrite"></a>overwrite

Bool value. If True, an existing output_data will be overwritten.
overwrite is ignored if appending rows. Ignored for data frames.


### <a name="type"></a>type

the type of prediction desired. Supported choices are: “vector”, “prob”, “class”, and “matrix”.


### <a name="removemissings"></a>remove_missings

Bool value. If True, rows with missing values are removed.


### <a name="computeresiduals"></a>compute_residuals

Bool value. If True, residuals are computed.


### <a name="residualtype"></a>residual_type

Indicates the type of residual desired.


### <a name="residualvarnames"></a>residual_var_names

List of strings specifying name(s) to give to the residual results.


### <a name="blocksperread"></a>blocks_per_read

Number of blocks to read for each chunk of data read from the data source. If the data and output_data are the same file, blocks_per_read must be 1.


### <a name="reportprogress"></a>report_progress

Integer value with options: 0: No progress is reported.
1: The number of processed rows is printed and updated.
2: Rows processed and timings are reported.
3: Rows processed and all timings are reported.


### <a name="verbose"></a>verbose

Integer value. If 0, no additional output is printed. If 1, additional summary information is printed.


### <a name="xdfcompressionlevel"></a>xdf_compression_level

Integer in the range of -1 to 9 indicating the compression level for the output data if written to an .xdf file.


### <a name="computecontext"></a>compute_context

A RxComputeContext object for prediction.


### <a name="kwargs"></a>kwargs

Additional parameters


## <a name="returns"></a>Returns

A data frame or a data source object of prediction results.


## <a name="see-also"></a>See also

[`rx_predict`](rx-predict.md).


## <a name="example"></a>Example



```
import os
from revoscalepy import rx_dtree, rx_predict_rx_dtree, rx_import, RxOptions, RxXdfData
sample_data_path = RxOptions.get_option("sampleDataDir")
ds = RxXdfData(os.path.join(sample_data_path, "kyphosis.xdf"))
kyphosis = rx_import(input_data = ds)

# classification
formula = "Kyphosis ~ Number + Start"
method = "class"
parms = {'prior': [0.8, 0.2], 'loss': [0, 2, 3, 0], 'split': "gini"}
cost = [2,3]
dtree = rx_dtree(formula, data = kyphosis, pweights = "Age", method = method, parms = parms, cost = cost, max_num_bins = 100)
rx_pred = rx_predict_rx_dtree(dtree, data = kyphosis)
rx_pred.head()

# regression
formula = "Age ~ Number + Start"
method = "anova"
parms = {'prior': [0.8, 0.2], 'loss': [0, 2, 3, 0], 'split': "gini"}
cost = [2,3]
dtree = rx_dtree(formula, data = kyphosis, pweights = "Kyphosis", method = method, parms = parms, cost = cost, max_num_bins = 100)
rx_pred = rx_predict_rx_dtree(dtree, data = kyphosis)
rx_pred.head()
```

