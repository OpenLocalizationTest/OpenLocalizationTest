---
title: Update the port values - Machine Learning Server
description: You can update the ports numbers for the web node, compute node, or deployr-rserve.
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 2/16/2018
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: c9f18de016a541a10ef24aa203c8438d1bb16517
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="update-port-values"></a>Update port values

**Applies to:  Machine Learning Server, Microsoft R Server**

You can update the ports numbers for the web node, compute node, or [deployr-rserve](https://github.com/Microsoft/deployr-rserve) (a forked version of RServe).

## <a name="machine-learning-server-93"></a>Machine Learning Server 9.3

In Machine Learning Server 9.3, you can use `admin` extension of the Azure Command Line Interface ([Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest)) to set up and manage your configuration, including updating the local 'admin' account password.

>[!Important]
>- This password is set while you are first configuring your nodes.
>- You do not need an Azure subscription to use this CLI. It is installed as part of Machine Learning Server and runs locally.  

To update port values:

1. On the machine hosting the node, launch a command-line window or terminal  with administrator (Windows) or root/sudo (Linux) privileges.

1. Run the command to update the port value(s), where `<Port>` should be replaced by the actual port number without the brackets.
   ```azurecli
   # With elevated privileges, run the following commands.
   # List current port values
   az ml admin port list

   # Update port values
   az ml admin port update --webnode <Port> --computenode <Port> --rserve <Port>
   ```

1. [Restart the node](configure-admin-cli-stop-start.md) for the change to go into effect. 

## <a name="earlier-versions-90---92"></a>Earlier versions: 9.0 - 9.2

To update port values:

1. Log in to the machine on which your web node or compute node is installed.

1. [Launch the administration utility](configure-admin-cli-launch.md) with administrator privileges (Windows) or root/sudo privileges (Linux).

1. From the main menu, choose the option **Change service ports**.

1. From the submenu, choose the port you want to update.

1. Enter the port number. 

   >The port number will be updated the next time the [service is restarted](configure-admin-cli-stop-start.md).
