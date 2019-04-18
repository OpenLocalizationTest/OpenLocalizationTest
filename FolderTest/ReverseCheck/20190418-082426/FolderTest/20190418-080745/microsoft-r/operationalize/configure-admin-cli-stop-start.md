---
title: 'Stop or start web and compute nodes on Machine Learning Server '
description: Monitor, stop or start the services for web or compute nodes for Machine Learning Server operationalization
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 2/16/2018
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: 46728fe6af1a1e6f51bacfb9f8b73e92582598c4
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="monitor-stop-and-start-web--compute-nodes"></a>Monitor, stop, and start web & compute nodes

**Applies to:  Machine Learning Server, Microsoft R Server**

You can monitor, start, or stop all operationalization-related web and compute nodes on the Machine Learning Server machine at once.

## <a name="machine-learning-server-93"></a>Machine Learning Server 9.3

In Machine Learning Server 9.3, you can use `admin` extension of the Azure Command-Line Interface ([Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest)) to set up and manage your configuration, including stopping and starting services.

>[!Important]
>- You must first [set up your nodes](configure-machine-learning-server-one-box.md) before doing anything else with the `admin` extension of the CLI.
>- You do not need an Azure subscription to use this CLI. It is installed as part of Machine Learning Server and runs locally.  

1. On the machine hosting the node, launch a command-line window or terminal  with administrator (Windows) or root/sudo (Linux) privileges.

1. Run the command to either monitor, stop, or start a node.
   ```azurecli
   # With elevated privileges, run the following commands.

   # Monitor nodes 
   az ml admin node list

   # Start nodes on a machine
   az ml admin node start --computenode --webnode

   # Stop nodes on a machine
   az ml admin node stop --computenode --webnode

   # Get help on other permutations
   az ml admin node start --help
   az ml admin node stop --help
   ```

## <a name="earlier-versions-90---92"></a>Earlier versions: 9.0 - 9.2

To stop or start a web node or compute node:

1. [Launch the administration utility.](configure-admin-cli-launch.md)

1. From the main menu, choose the option **Stop and start services**.

1. From the submenu, choose which nodes to start or stop.

>[!Warning]
>If the following error occurs when attempting to start a web node "Microsoft.AspNetCore.Server.Kestrel.Internal.Networking.UvException: Error -97 EAFNOSUPPORT address family not supported", then disable IPv6 on your operating system.