---
title: 'DeployR Administration Console Help - DeployR 8.x '
description: Intro to DeployR Administration Console Help
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 11/10/2017
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: 0fc50b44608d1784907105e23820052f1f44b990
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="about-deployr-administration-console"></a>About DeployR Administration Console

<!--**THIS TOPIC APPLIES TO:** ![](./media/deployr-admin-console-about/checkmark.jpeg) DeployR for Microsoft R Server 8.0.5 ![](./media/deployr-admin-console-about/checkmark.jpeg) DeployR Enterprise and Open (8.0.0)-->

The DeployR Administration Console, which is delivered with DeployR, is an easy-to-use web interface that facilitates the proper management and administration of your DeployR deployment. Accordingly, the following functions are supported in the console:

-   The creation and management of [user accounts](deployr-admin-console-user-accounts.md)
-   The creation and management of [roles](deployr-admin-console-permissions-with-roles.md), which are used to grant users permissions and to restrict access to R scripts
-   The import and export of [R scripts](deployr-admin-console-managing-r-scripts.md)
-   The creation and management of [R boundaries](deployr-admin-managing-r-boundaries.md), which are used to constrain runtime resource usage
-   The creation and management of [IP filters](deployr-admin-managing-access-with-ip-filters.md)
-   The backup and restore of [database contents](deployr-admin-console-database.md)
-   The management of node resources on the DeployR [grid](deployr-admin-managing-the-grid.md)
-   The management of DeployR [server policies](deployr-admin-managing-server-policies.md)
-   The [monitoring of events on the grid](deployr-admin-monitoring-events.md)

## <a name="who-can-access-the-administration-console"></a>Who Can Access the Administration Console

Only the `admin` user account, representing the administrator, has access to this console and can:

- Create and manage user accounts, roles, R boundaries, and IP filters
- Import and export scripts for preserving backups or for the purposes of migration
- Manage DeployR grid node resources and the server policies

## <a name="how-to-access-the-administration-console"></a>How to Access the Administration Console

>You cannot log in to DeployR from multiple accounts using a single brand of browser program. To use two or more accounts concurrently, you'll need to log in to each one in a separate brand of browser. 

**To access and log in to the Administration Console after installation:**

1.  In a browser window, enter the Administration Console’s URL:

        https://<DEPLOYR-IP-ADDRESS>:<PORT>/deployr/administration
    where `<DEPLOYR_SERVER_IP>` is the IP address of the DeployR machine and where `<PORT>` is the port number used during installation. 

2.  Click **Administration Console Log In** in the upper right to log in. If this is your first time using the Administration Console, try one of the [preconfigured users](deployr-admin-console-user-accounts.md#preconfigured-user-accounts).

3. Click **Log In**.

<br>
<strong>To log out of the Administration Console:</strong>

+ Click **Log Out** in the upper right corner of the console.
 
>See the [Scale & Throughput Guide](deployr-admin-scale-and-throughput.md) for help in planning the provisioning of server and grid capacity.
