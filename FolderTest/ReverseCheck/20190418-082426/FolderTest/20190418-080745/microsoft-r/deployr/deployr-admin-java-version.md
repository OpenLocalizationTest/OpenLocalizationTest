---
title: 'Update DeployR after Java update - DeployR 8.x '
description: Update DeployR after Java update
keywords: DeployR, JRE, JDK, Java, Update
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 11/10/2017
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: f99a01de169e85c66d75575028c039d674d5270f
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="updating-deployr-configuration-after-java-version-update"></a>Updating DeployR Configuration after Java Version Update

**Applies to: DeployR 8.x**   (See [comparison between 8.x and 9.x](../whats-new-in-r-server.md#8vs9))

>Looking to deploy with Machine Learning Server? [Start here](../what-is-operationalization.md).

This topic describes how to update the configuration of DeployR (Apache Tomcat, etc.) after a Java JRE/JDK.


**To update the configuration for the new Java version:**

1. Open a command prompt/terminal window with administrator/root/sudo privileges:

1. [Stop DeployR](deployr-common-administration-tasks.md#startstop).

1. Go to the Apache Tomcat directory. For example, on Windows the default location is `C:\Program Files\Microsoft\DeployR-8.0.5\Apache_Tomcat\bin`.

1. At the prompt, enter the following command to start the utility:
   ```NA
   tomcat7w.exe //MS//Apache-Tomcat-for-DeployR-8.0.5
   ```

1. In the dialog, enter the new Java version to be used for DeployR.
 
1. Click **OK** to save these settings.

1. [Restart DeployR](deployr-common-administration-tasks.md#startstop).
 

