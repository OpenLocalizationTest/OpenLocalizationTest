---
title: 'DeployR Administration Console Help - DeployR 8.x '
description: Database Back and Restore in DeployR Administration Console
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 11/10/2017
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: 6fc4973170673bfeb6033f9b16de29b41c9c8455
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="restoring--backing-up-the-database"></a>Restoring & Backing Up the Database

You can back up and restore the DeployR database through the **Database** tab in the Administration Console.

In this tab, you can export the contents of the database used by DeployR into a ZIP file as a way to backup data or as the first step in migrating data between two or more DeployR-server instances. You can also import this content into the repository on this server instance from a previously exported ZIP file. 

_Figure: Database page_

![](media/deployr-admin-console-database/db-tab.png)  


**To back up the database data:**

1.  From the main menu, click **Database**.

1. In that tab, click **Backup DeployR Database**. A zip file is created and downloaded to your local machine.

<br>
<strong>To restore the database data</strong>

1.  From the main menu, click **Database**.

1. In that tab, click **Restore DeployR Database**. The **Database restore** page appears.

    _Figure: Database restore page_
    
    ![](media/deployr-admin-console-database/db-restore.png)

1. In the **Database restore** page, select the backup file.

1. Click **Restore** to restore the database.