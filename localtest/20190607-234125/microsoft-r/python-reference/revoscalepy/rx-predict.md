---
title: 'rx_predict: Predicted Values and Residuals for rx_lin_mod, rx_logit, rx_dtree, (revoscalepy)'
description: Generic function to compute predicted values and residuals using rx_lin_mod, rx_logit, rx_dtree, rx_dforest and rx_btrees objects.
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
ms.openlocfilehash: 720c92c1d190a2a8c26ac717d2095e9cab9f6118
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxpredict"></a>rx_predict


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_predict(model_object=None, data=None, output_data=None, **kwargs)
```





## <a name="description"></a>Description

Generic function to compute predicted values and residuals using rx_lin_mod, rx_logit, rx_dtree, rx_dforest and rx_btrees objects.


## <a name="arguments"></a>Arguments


### <a name="modelobject"></a>model_object

object returned from a call to rx_lin_mod, rx_logit, rx_dtree, rx_dforest and rx_btrees. Objects with multiple dependent variables are not supported.


### <a name="data"></a>data

a data frame or an RxXdfData data source object to be used for predictions.
If a Spark compute context is being used, this argument may also be an RxHiveData, RxOrcData, RxParquetData or RxSparkDataFrame object or a Spark data frame object from pyspark.sql.DataFrame.


### <a name="outputdata"></a>output_data

an RxXdfData data source object or existing data frame to store predictions.


### <a name="kwargs"></a>kwargs

additional parameters


## <a name="returns"></a>Returns

a data frame or a data source object of prediction results.


## <a name="see-also"></a>See also

[`rx_predict_default`](rx-predict-default.md), [`rx_predict_rx_dtree`](rx-predict-rx-dtree.md), [`rx_predict_rx_dforest`](rx-predict-rx-dforest.md).


## <a name="example"></a>Example



```
import os
from revoscalepy import RxOptions, RxXdfData, rx_lin_mod, rx_predict, rx_data_step

sample_data_path = RxOptions.get_option("sampleDataDir")
mort_ds = RxXdfData(os.path.join(sample_data_path, "mortDefaultSmall.xdf"))
mort_df = rx_data_step(mort_ds)

lin_mod = rx_lin_mod("creditScore ~ yearsEmploy", mort_df)
pred = rx_predict(lin_mod, data = mort_df)
print(pred.head())
```


Output:



```
Rows Read: 100000, Total Rows Processed: 100000, Total Chunk Time: 0.058 seconds 
Rows Read: 100000, Total Rows Processed: 100000, Total Chunk Time: 0.006 seconds 
Computation time: 0.039 seconds.
Rows Read: 100000, Total Rows Processed: 100000, Total Chunk Time: Less than .001 seconds 
   creditScore_Pred
0        700.089114
1        699.834355
2        699.783403
3        699.681499
4        699.783403
```


Note: Function *rx_predict* does not run predictions but chooses the appropriate function [`rx_predict_default`](rx-predict-default.md), [`rx_predict_rx_dtree`](rx-predict-rx-dtree.md), or [`rx_predict_rx_dforest`](rx-predict-rx-dforest.md) based on the model which was given to it. Each of them has a different set of parameters described by their documentation. 
