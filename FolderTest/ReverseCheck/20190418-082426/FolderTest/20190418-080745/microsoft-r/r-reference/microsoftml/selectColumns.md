---
title: 'selectColumns function (MicrosoftML) '
description: " Selects a set of columns to retrain, dropping all others. "
keywords: (MicrosoftML), selectColumns, transform
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
ms.openlocfilehash: 3db2a49353b08db03ca3df3946aec9d890217493
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
 # <a name="selectcolumns-selects-a-set-of-columns-dropping-all-others"></a>selectColumns: Selects a set of columns, dropping all others 
 ## <a name="description"></a>Description
 
Selects a set of columns to retrain, dropping all others.
 
 
 ## <a name="usage"></a>Usage

```   
  selectColumns(vars, ...)
 
```
 
 ## <a name="arguments"></a>Arguments

   
  
 ### `vars`
 Specifies character vector or list of the names of the variables to keep. 
  
  
  
 ### ` ...`
 Additional arguments sent to compute engine. 
  
 
 
 ## <a name="value"></a>Value
 
A `maml` object defining the transform.
 
 ## <a name="authors"></a>Author(s)
 
Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)

 
 
 
 
