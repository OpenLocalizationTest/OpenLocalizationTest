---
title: 'rx_privacy_control: Changes the opt-in state for anonymous usage collection (revoscalepy)'
description: Used for opting out of telemetry data collection, which is enabled by default.
keywords: privacy, telemetry
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
ms.openlocfilehash: 24a4fad55aac3756e18893f6a3cc490e735e705a
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="rxprivacycontrol"></a>rx_privacy_control


 


## <a name="usage"></a>Usage



```
revoscalepy.rx_privacy_control(enable: bool = None)
```





## <a name="description"></a>Description

Used for opting out of telemetry data collection, which is enabled by default.


## <a name="arguments"></a>Arguments


### <a name="optin"></a>opt_in

A bool value that specifies whether to opt in (True) or out (False) of anonymous data usage collection.
If not specified, the value is returned.


## <a name="example"></a>Example



```
import revoscalepy
revoscalepy.rx_privacy_control(False)
```

