---
title: rxSerializeModel function (revoAnalytics) | Microsoft Docs
description: "   Serialize a **RevoScaleR**/**MicrosoftML** model in raw format to enable saving the model. This allows model to be loaded into SQL Server for real-time scoring. "
keywords: (revoAnalytics), rxSerializeModel, rxUnserializeModel
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
ms.openlocfilehash: 49a487143f30ad2e263e59f625a9a17f8c2f0ebe
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="rxserializemodel--revoscaler-model-serialization-and-unserialization"></a>rxSerializeModel:  RevoScaleR Model Serialization and Unserialization  
 ## <a name="description"></a>Description

Serialize a **RevoScaleR**/**MicrosoftML** model in raw format to enable saving the model. This allows model to be loaded into SQL Server for real-time scoring.


 ## <a name="usage"></a>Usage

```   
  rxSerializeModel(model, metadata = NULL, realtimeScoringOnly = FALSE, ...)

  rxUnserializeModel(serializedModel, ...)

```


 ## <a name="arguments"></a>Arguments



 ### `model`
 `RevoScaleR`/`MicrosoftML` model to be serialized 


 ### `metadata`
 Arbitrary metadata of `raw` type to be stored with the serialized model. Metadata will be returned when unserialized.  


 ### `realtimeScoringOnly`
 Drops fields not required for real-time scoring.  NOTE: Setting this flag could reduce the model size but `rxUnserializeModel` can no longer retrieve the RevoScaleR model 


 ### `serializedModel`
 Serialized model to be unserialized 




 ## <a name="details"></a>Details

`rxSerializeModel` converts models into `raw` bytes to allow them to be saved and used for real-time scoring.

The following is the list of models that are currently supported in real-time scoring:


* 
  **RevoScaleR**


  * 
    rxLogit

  * 
    rxLinMod

  * 
    rxBTrees

  * 
    rxDTree

  * 
    rxDForest




* 
  **MicrosoftML**


  * 
    rxFastTrees

  * 
    rxFastForest

  * 
    rxLogisticRegression

  * 
    rxOneClassSvm

  * 
    rxNeuralNet

  * 
    rxFastLinear






**RevoScaleR** models containing R transformations or transform based formula (e.g `"A ~ log(B)"`) are not supported in real-time scoring. Such transforms to input data may need to be handled before calling real-time scoring.

`rxUnserializeModel` method is used to retrieve the original R model object and metadata from the serialized raw model.


 ## <a name="value"></a>Value

`rxSerializeModel` returns a serialized model.

`rxUnserializeModel` returns original R model object. If metadata is also present returns a list containing the original model object and metadata.

 ## <a name="authors"></a>Author(s)

Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)




 ## <a name="see-also"></a>See Also


 ## <a name="examples"></a>Examples

 ```

  myIris <- iris
  myIris[1:5,]
  form <- Sepal.Length ~ Sepal.Width + Petal.Length + Petal.Width + Species
  irisLinMod <- rxLinMod(form, data = myIris)

  # Serialize model for scoring
  serializedModel <- rxSerializeModel(irisLinMod)

  # Save model to file or SQL Server (use rxWriteObject)
  # serialized model can now be used for real-time scoring

  unserializedModel <- rxUnserializeModel(serializedModel)
```

