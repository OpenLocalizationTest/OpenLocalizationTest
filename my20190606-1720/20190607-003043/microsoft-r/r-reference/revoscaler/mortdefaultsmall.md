---
title: mortDefaultSmall data (revoAnalytics) | Microsoft Docs
description: " Simulated data on mortgage defaults. "
keywords: (revoAnalytics), mortDefaultSmall, mortDefaultSmall.xdf, mortDefaultSmall2000.csv, mortDefaultSmall2001.csv, mortDefaultSmall2002.csv, mortDefaultSmall2003.csv, mortDefaultSmall2004.csv, mortDefaultSmall2005.csv, mortDefaultSmall2006.csv, mortDefaultSmall2007.csv, mortDefaultSmall2008.csv, mortDefaultSmall2009.csv, datasets
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
ms.openlocfilehash: 0d335ff8b417b61bc5802f05bb95b2dda439fa38
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="mortdefaultsmall-smaller-mortgage-default-demonstration-data"></a>mortDefaultSmall: Smaller Mortgage Default Demonstration Data 
 ## <a name="description"></a>Description

Simulated data on mortgage defaults.


 ## <a name="format"></a>Format

An .xdf file with 50000 observations on the following 6 variables:


### `creditScore`
FICO credit scores (stored as an integer).


### `houseAge`
house age, by range (stored as integer).


### `yearsEmploy`
years employed at current employer (stored as integer).


### `ccDebt`
the amount of debt (stored as integer).


### `year`
year of the observation (stored as integer).


### `default`
1 if the homeowner was in default on the loan, 0 otherwise (stored as an integer).





 ## <a name="details"></a>Details

This data set simulates mortgage default data. The data set is created by looping over the input data files mortDefaultSmall200x.csv, each of which contains a year's worth of simulated data.


 ## <a name="source"></a>Source

Microsoft Corporation.


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="examples"></a>Examples

 ```

  mortDefaultSmall <- rxDataStep(data = file.path(rxGetOption("sampleDataDir"),
                                "mortDefaultSmall.xdf"))
  rxSummary(~ creditScore + houseAge, data = mortDefaultSmall)
```


