---
title: 'concat function (MicrosoftML) '
description: " Combines several columns into a single vector-valued column. "
keywords: (MicrosoftML), concat, transform
author: heidisteen
manager: cgronlun
ms.date: 01/16/2019
ms.topic: reference
ms.prod: mlserver
ms.service: ''
ms.assetid: ''
ROBOTS: ''
audience: ''
ms.devlang: ''
ms.reviewer: ''
ms.suite: ''
ms.tgt_pltfrm: ''
ms.custom: ''
ms.openlocfilehash: db484d9de470e81dbd3762b51bf61223d99f0ad6
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="concat-machine-learning-concat-transform"></a>concat: Machine Learning Concat Transform 
 ## <a name="description"></a>Description

Combines several columns into a single vector-valued column.


 ## <a name="usage"></a>Usage

```   
  concat(vars, ...)

```

 ## <a name="arguments"></a>Arguments



 ### `vars`
 A named list of character vectors of input variable names and the name of the output variable. Note that all the input variables must be of the same type. It is possible to produce multiple output columns  with the concatenation transform. In this case, you need to use a list of  vectors to define a one-to-one mapping between input and output variables. For example, to concatenate columns InNameA and InNameB into column OutName1 and also columns InNameC and InNameD into column OutName2, use the list:  (list(OutName1 = c(InNameA, InNameB), outName2 = c(InNameC, InNameD))) 



 ### ` ...`
 Additional arguments sent to the compute engine 



 ## <a name="details"></a>Details

`concat` creates a single vector-valued column from multiple  
columns. It can be performed on data before training a model. The concatenation  
can significantly speed up the processing of data when the number of columns is as large as hundreds to thousands.


 ## <a name="value"></a>Value

A `maml` object defining the concatenation transform.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="see-also"></a>See Also

[featurizeText](featurizeText.md), [categorical](categorical.md), [categoricalHash](categoricalHash.md), [rxFastTrees](rxFastTrees.md), [rxFastForest](rxFastForest.md), [rxNeuralNet](rxNeuralNet.md), [rxOneClassSvm](rxOneClassSvm.md), [rxLogisticRegression](rxLogisticRegression.md).

 ## <a name="examples"></a>Examples

 ```

  testObs <- rnorm(nrow(iris)) > 0
  testIris <- iris[testObs,]
  trainIris <- iris[!testObs,]

  multiLogitOut <- rxLogisticRegression(
          formula = Species~Features, type = "multiClass", data = trainIris,
          mlTransforms = list(concat(vars = list(
              Features = c("Sepal.Length", "Sepal.Width", "Petal.Length", "Petal.Width")
            ))))
  summary(multiLogitOut)
```



