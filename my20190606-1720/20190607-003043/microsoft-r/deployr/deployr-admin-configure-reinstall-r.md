---
title: 'Upgrading or Reinstalling Microsoft R Server, Revolution R Open, or R - DeployR 8.x '
description: Reinstalling R on a machine with DeployR
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 11/10/2017
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: 485e840aab61db04ac808d36ad2c068272943ed1
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="upgrading-or-reinstalling-r"></a>Upgrading or Reinstalling R

**Applies to: DeployR 8.x** (See [comparison between 8.x and 9.x](../whats-new-in-r-server.md#8vs9))

>Looking to deploy with Machine Learning Server? [Start here](../what-is-operationalization.md).

## <a name="on-windows"></a>On Windows

### <a name="reinstalling-microsoft-r-server-for-deployr-enterprise"></a>Reinstalling Microsoft R Server for DeployR Enterprise

Carefully follow the order presented whenever you reinstall Microsoft R Server on a Windows machine hosting DeployR Enterprise:

On the main DeployR server machine:

1.  [Backup the DeployR database](deployr-common-administration-tasks.md).
2.  [Uninstall the DeployR main server](deployr-install-on-windows.md).
3.  Uninstall Microsoft R Server using the instructions provided with your existing version of Microsoft R Server.
4.  Install Microsoft R Server and all its prerequisites as described in the instructions provided with that version of Microsoft R Server.
5.  Reinstall the DeployR main server on [DeployR for Microsoft R Server](deployr-install-on-windows.md) | [DeployR 8.0.0](deployr-installing-configuring.md)
6.  [Restore the DeployR database](deployr-common-administration-tasks.md).

On each DeployR grid node machine:

1.  [Uninstall the DeployR grid node](deployr-install-on-windows.md).
2.  Uninstall Microsoft R Server using the instructions provided with your existing version of Microsoft R Server.
3.  Install Microsoft R Server and all its prerequisites as described in the instructions provided with that version of Microsoft R Server.
4.  Install the DeployR grid node on [DeployR for Microsoft R Server](deployr-install-on-windows.md) | [DeployR 8.0.0](deployr-installing-configuring.md).

>For each DeployR Enterprise instance, the server and grid nodes should all run the same version of R.

### <a name="reinstalling-rro-or-r-for-deployr-open"></a>Reinstalling RRO or R for DeployR Open

Carefully follow the order presented whenever you reinstall Revolution R Open or CRAN R on a machine hosting DeployR Open 8.0.0:

On the main DeployR Open server machine:

1.  [Backup the DeployR database](deployr-common-administration-tasks.md).
2.  [Uninstall the DeployR main server](deployr-installing-configuring.md).
3.  Uninstall Revolution R Open or CRAN R.
4.  Install Revolution R Open or CRAN R along with all of its prerequisites as described in the Revolution R Open or CRAN R installation instructions.
5.  [Reinstall the DeployR main server](deployr-installing-configuring.md).
6.  [Restore the DeployR database](deployr-common-administration-tasks.md).


### <a name="troubleshooting-on-windows"></a>Troubleshooting on Windows

If Microsoft R Server or Microsoft R Open is not reinstalled as described at the beginning of this document, then Rserve may be missing.

Try the following:

1.  [Run the diagnostics](deployr-admin-diagnostics-troubleshooting.md#diagnostic-testing) to determine whether the issue is on the main server or a grid node.
2.  If RServe is not running and you cannot find it in the `\bin\x64` subdirectory of the Microsoft R Server install directory, then you must reinstall as described above.
3.  If there are other issues reported in the [diagnostics log](deployr-admin-diagnostics-troubleshooting.md#inspecting-diagnostic-log-files), attempt to fix them now.
4.  Run the diagnostics again.

In the event that you need additional support, send the diagnostics tar/zip file to the Microsoft Corporation technical support team.

## <a name="on-linux"></a>On Linux


### <a name="reinstalling-microsoft-r-server-for-deployr-enterprise"></a>Reinstalling Microsoft R Server for DeployR Enterprise

Carefully follow the order presented whenever you reinstall Microsoft R Server on a Linux machine hosting DeployR for Microsoft R Server:

On the main DeployR server machine:

1.  [Stop DeployR](deployr-common-administration-tasks.md#startstop).
2.  Uninstall Microsoft R Server using the instructions provided with your existing version of Microsoft R Server.
3.  Install Microsoft R Server and all its prerequisites as described in the instructions provided with that version of Microsoft R Server.
4.  [Start DeployR](deployr-common-administration-tasks.md#startstop).

On each DeployR grid node machine:

1. Uninstall the DeployR grid node on [DeployR for Microsoft R Server](deployr-install-on-linux.md#uninstalling-deployr) | [DeployR 8.0.0](deployr-installing-configuring.md#uninstalling-deployr).
2.  Uninstall Microsoft R Server using the instructions provided with that product.
3.  Install Microsoft R Server and all its prerequisites as described in that product's instructions.
4.  [Install the DeployR grid node](). on [DeployR for Microsoft R Server](deployr-install-on-linux.md#install-deployr-grid-nodes) | [DeployR 8.0.0](deployr-installing-configuring.md#grid-node-install).

>For each DeployR Enterprise instance, the server and grid nodes should all run the same version of R.

### <a name="reinstalling-rro-or-r-for-deployr-open"></a>Reinstalling RRO or R for DeployR Open

Carefully follow the order presented whenever you reinstall Revolution R Open or CRAN R on a machine hosting DeployR Open 8.0.0:

On the main DeployR Open server machine:

1.  [Stop DeployR](deployr-common-administration-tasks.md#startstop).
2.  Uninstall Revolution R Open or CRAN R.
3.  Install Revolution R Open or CRAN R along with all of its prerequisites as described in the Revolution R Open or CRAN R installation instructions.
4.  [Start DeployR](deployr-common-administration-tasks.md#startstop).


### <a name="troubleshooting-on-linux"></a>Troubleshooting on Linux

If the issue is that Rserve is not running on a machine, then you'll need to restart it.

Try the following:

1.  [Run the diagnostics](deployr-admin-diagnostics-troubleshooting.md#diagnostic-testing) to determine whether the issue is on the main server or a grid node.
2.  Make sure there is [no activity on the DeployR grid.](deployr-admin-managing-the-grid.md#viewing-or-stopping-slot-activity)
3.  [Stop DeployR on the machine in question.](deployr-common-administration-tasks.md#startstop)
4.  Attempt to correct all issues reported in the [diagnostics log.](deployr-admin-diagnostics-troubleshooting.md#inspecting-diagnostic-log-files)
5.  [Start DeployR on the machine in question.](deployr-common-administration-tasks.md#startstop)
6.  Run the diagnostics again.

In the event that you need additional support, send the diagnostics tar/zip file to the Microsoft Corporation technical support team.
