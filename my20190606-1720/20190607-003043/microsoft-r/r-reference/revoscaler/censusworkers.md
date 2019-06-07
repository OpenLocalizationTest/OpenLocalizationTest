---
title: CensusWorkers data (revoAnalytics) | Microsoft Docs
description: " A small subset of the IPUMS 5% sample of the 2000 U.S. Census data containing information on the working population from Connecticut, Indiana, and Washington. "
keywords: (revoAnalytics), CensusWorkers, CensusWorkers.xdf, datasets
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
ms.openlocfilehash: fa01dec30311cac1ba36210f2732c982394bb8db
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="censusworkers-subset-of-ipums-2000-us-census-data"></a>CensusWorkers: Subset of IPUMS 2000 U.S. Census Data 
 ## <a name="description"></a>Description

A small subset of the IPUMS 5% sample of the 2000 U.S. Census data containing information on the working population from Connecticut, Indiana, and Washington.


 ## <a name="format"></a>Format

An .xdf file with 351121 observations on the following 6 variables:


### `age`
integer variable containing ages.


### `incwage`
integer variable containing wage and salary income. The value 999999 from the original data has been converted to missing.


### `perwt`
integer variable containing person weights, that is, a frequency weight for each person record. This is treated as integer data in R.


### `sex`
factor variable sex with levels `Male` and `Female`.


### `wkswork1`
integer variable containing the weeks worked the previous year.


### `state`
factor variable containing the state with levels `Connecticut`, `Indiana`, and `Washington`.





 ## <a name="details"></a>Details

The 5% 2000 U.S. Census sample is a stratified 5% sample of households, produced and maintained by the Minnesota Population Center at the University of Minnesota as part of the *Integrated Public Use Microdata Series*, or IPUMS. The full data set contains 14,583,731 rows with 265 variables. This data was converted to the .xdf format, using  the SPSS dictionary provided on the IPUMS web site to obtain variable labels, value labels, and value codes. The subsample was taken using the following rowSelection:
`(age >= 20) & (age <= 65) & (wkswork1 > 20) &
``(stateicp == "Connecticut" | stateicp == "Washington" | stateicp == "Indiana")`


 ## <a name="source"></a>Source

Minnesota Population Center, University of Minnesota.
*Integration Public Use Microdata Series*. [`http://www.ipums.org`](http://www.ipums.org) .


 ## <a name="authors"></a>Author(s)
 Microsoft Corporation [`Microsoft Technical Support`](https://go.microsoft.com/fwlink/?LinkID=698556&clcid=0x409)


 ## <a name="see-also"></a>See Also

[CensusUS5Pct2000](CensusUS5Pct2000.md)

 ## <a name="examples"></a>Examples

 ```

  censusWorkers <- file.path(rxGetOption("sampleDataDir"),
                             "CensusWorkers.xdf")
  rxSummary(~ age + incwage, data = censusWorkers)
```


