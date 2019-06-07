---
title: rxNaiveBayes function (revoAnalytics) | Microsoft Docs
description: "     Fit Naive Bayes Classifiers on an .xdf file or data frame     for small or large data using parallel external memory algorithm. "
keywords: (revoAnalytics), rxNaiveBayes, print.rxNaiveBayes, models, tree, classif, classification
author: heidisteen
manager: cgronlun
ms.date: 01/24/2018
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
ms.openlocfilehash: 2f5a137f1526f50f1b4901ddb861d328aae6b6a8
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxnaivebayes-parallel-external-memory-algorithm-for-naive-bayes-classifiers"></a>rxNaiveBayes: Parallel External Memory Algorithm for Naive Bayes Classifiers 
 ## <a name="description"></a>Description

Fit Naive Bayes Classifiers on an .xdf file or data frame for small or large data using parallel external memory algorithm.


 ## <a name="usage"></a>Usage

```   
  rxNaiveBayes(formula, data, smoothingFactor = 0,   ...  )

```

 ## <a name="arguments"></a>Arguments



 ### `formula`
  formula as described in [rxFormula](rxFormula.md).     


 ### `data`
  either a data source object, a character string  specifying a .xdf file, or a data frame object. 


 ### `smoothingFactor`
  a positive smoothing factor to account for cases not present in the training data.  It avoids modeling issues by preventing zero conditional probability estimates. 


 ### ` ...`
  additional arguments to be passed directly to [rxSummary](rxSummary.md) such as `byTerm`, `rowSelection`, `pweights`, `fweights`, `transforms`, `transformObjects`, `transformFunc`,  `transformVars`, `transformPackages`, `transformEnvir`,  `useSparseCube`, `removeZeroCounts`, `blocksPerRead`,  `reportProgress`, `verbose`, `xdfCompressionLevel`.   



 ## <a name="value"></a>Value

an `"rxNaiveBayes"` object containing the following components:


* `apriori` -  a vector of prior class probabilities for the dependent variable.


* `tables` -  a list of tables, one for each predictor variable.   
   * For a categorical variable, the table contains the conditional probabilities of the variable given the target class.  
   * For a numeric variable, the table contains the mean and standard deviation of the variable given the target class.  



* `levels` -  the levels of the dependent variable.


* `call` -  the matched call.




 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)



 ## <a name="references"></a>References

Naive Bayes classifier [`https://en.wikipedia.org/wiki/Naive_Bayes_classifier`](https://en.wikipedia.org/wiki/Naive_Bayes_classifier)
.


 ## <a name="see-also"></a>See Also

[rxPredict.rxNaiveBayes](rxPredict.rxNaiveBayes.md).

 ## <a name="examples"></a>Examples

 ```

  # multi-class classification with an .xdf file
  claimsXdf <- file.path(rxGetOption("sampleDataDir"),"claims.xdf")
  claims.nb <- rxNaiveBayes(type ~ age + cost, data = claimsXdf)
  claims.nb

  # prediction
  claims.nb.pred <- rxPredict(claims.nb, claimsXdf)
  claims.nb.pred
  table(claims.nb.pred[["type_Pred"]], rxDataStep(claimsXdf)[["type"]])
```





