---
title: 'rx_get_var_names: Variable names for a data source or data frame (revoscalepy)'
description: Read the variable names for data source or data frame
keywords: variables
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
ms.openlocfilehash: 749a4ecee72dddddff6e5b1bd814c6ec97f696bf
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxgetvarnames"></a>rx_get_var_names


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_get_var_names(data)
```





## <a name="description"></a>Description

Read the variable names for data source or data frame


## <a name="arguments"></a>Arguments


### <a name="data"></a>data

an RxDataSource object, a character string specifying the “.xdf” file, or a data frame.
If a Spark compute context is being used, this argument may also be an RxHiveData, RxOrcData, RxParquetData or RxSparkDataFrame object or a Spark data frame object from pyspark.sql.DataFrame.


## <a name="returns"></a>Returns

list of strings containing the names of the variables in the data source or data frame.


## <a name="see-also"></a>See also

[`rx_data_step`](rx-data-step.md), [`rx_get_info`](rx-get-info.md), [`rx_get_var_info`](rx-get-var-info.md).


## <a name="example"></a>Example



```
import os
from revoscalepy import RxOptions, RxXdfData, rx_get_var_names

sample_data_path = RxOptions.get_option("sampleDataDir")
claims_ds = RxXdfData(os.path.join(sample_data_path, "claims.xdf"))
info = rx_get_var_names(claims_ds)
print(info)
```


Output:



```
RowNum age car.age type cost number
```

