---
title: Uninstall Machine Learning Server for Hadoop
description: How to uninstall Machine Learning Server on a Hadoop cluster.
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 02/16/2018
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: ca05bfb2e596e5c6be833132059ee5fc42fe32b9
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="uninstall-machine-learning-server-for-hadoop"></a>Uninstall Machine Learning Server for Hadoop

**Applies to:  Machine Learning Server 9.2.1 | 9.3**

This article explains how to uninstall Machine Learning Server running in a Spark cluster. 

+ Remove components on edge nodes
+ Remove components on data nodes

You can uninstall existing software and upgrade to newer versions node by node across the cluster, but don’t try to submit any jobs until all nodes are at the same functional level.

## <a name="uninstall-edge-nodes"></a>Uninstall edge nodes

1. List the packages from Microsoft.

   + On RHEL: `yum list \*microsoft\*`   
   + On Ubuntu: `apt list --installed | grep microsoft`  
   + On SUSE: `zypper search \*microsoft-r\*`    

2. Operationalization features run on edge nodes. On a 9.3.0 installation, this is the [azureml-model-management library](../python-reference/azureml-model-management-sdk/azureml-model-management-sdk.md) or [mrsdeploy](../r-reference/mrsdeploy/mrsdeploy-package.md), which you can uninstall using the syntax from the previous step. Multiple packages provide the feature. Uninstall each one in the following order:

   **On CentOS and RHEL**

   + `yum erase microsoft-mlserver-adminutil-9.3`
   + `yum erase microsoft-mlserver-webnode-9.3`
   + `yum erase microsoft-mlserver-computenode-9.3`

   **On Ubunute**

   + `apt-get purge microsoft-mlserver-adminutil-9.3` 
   + `apt-get purge microsoft-mlserver-webnode-9.3` 
   + `apt-get purge microsoft-mlserver-computenode-9.3`  
 
   **On SUSE**

   + `zypper remove microsoft-mlserver-adminutil-9.3`   
   + `zypper remove microsoft-mlserver-webnode-9.3`   
   + `zypper remove microsoft-mlserver-computenode-9.3`   

## <a name="uninstall-data-nodes"></a>Uninstall data nodes

1. On root@, uninstall Microsoft R Open (MRO) first. This action removes any dependent packages used only by MRO, which includes packages like microsoft-mlserver-packages-r. 

   + On RHEL: `yum erase microsoft-r-open-mro-3.4.3`     
   + On Ubuntu: `apt-get purge microsoft-r-open-mro-3.4.3`  
   + On SUSE: `zypper remove microsoft-r-open-mro-3.4.3`    

2. Remove the Machine Learning Server Python packages:

   + On RHEL: `yum erase microsoft-mlserver-python-9.3.0`     
   + On Ubuntu: `apt-get purge microsoft-mlserver-python-9.3.0`  
   + On SUSE: `zypper remove microsoft-mlserver-python-9.3.0`

3. Remove the Hadoop package:

   + On RHEL: `yum erase microsoft-mlserver-hadoop-9.3.0`     
   + On Ubuntu: `apt-get purge microsoft-mlserver-hadoop-9.3.0`  
   + On SUSE: `zypper remove microsoft-mlserver-hadoop-9.3.0`

4. Re-list the packages from Microsoft to check for remaining files:

   + On RHEL: `yum list \*microsoft\*`   
   + On Ubuntu: `apt list --installed | grep microsoft`  
   + On SUSE: `zypper search \*microsoft-r\*`  

   On Ubuntu, you have `dotnet-runtime-2.0.0`. [NET Core](https://docs.microsoft.com/dotnet/core/index) is a cross-platform, general purpose development platform maintained by Microsoft and the .NET community on GitHub. This package could be providing infrastructure to other applications on your computer. If Machine learning Server is the only Microsoft software you have, you can remove it now.

5. After packages are uninstalled, remove remaining files. On root@, determine whether additional files still exist:

   + `$ ls /opt/microsoft/mlserver/9.3.0/`

6. Remove the entire directory:

   + `$ rm -fr ls /opt/microsoft/mlserver/9.3.0/`

RM removes the folder. Parameter "f" is for force and "r" for recursive, deleting everything under microsoft/mlserver. This command is destructive and irrevocable, so be sure you have the correct directory before you press Enter.

<a name="installed-packages"></a>

## <a name="package-list"></a>Package list

Machine Learning Server for Hadoop adds the following packages at a minimum. When uninstalling software, refer to this list when searching for packages to remove.

    dotnet-host-2.0.0
    dotnet-hostfxr-2.0.0
    dotnet-runtime-2.0.0 
    
    microsoft-mlserver-adminutil-9.3
    microsoft-mlserver-all-9.3.0 
    microsoft-mlserver-computenode-9.3
    microsoft-mlserver-config-rserve-9.3 
    microsoft-mlserver-hadoop-9.3.0
    microsoft-mlserver-mlm-py-9.3.0 
    microsoft-mlserver-mlm-r-9.3.0
    microsoft-mlserver-mml-py-9.3.0
    microsoft-mlserver-mml-r-9.3.0
    microsoft-mlserver-packages-py-9.3.0 
    microsoft-mlserver-packages-r-9.3.0
    microsoft-mlserver-python-9.3.0 
    microsoft-mlserver-webnode-9.3
    microsoft-r-open-foreachiterators-3.4.3 
    microsoft-r-open-mkl-3.4.3
    microsoft-r-open-mro-3.4.3 
    azure-cli-2.0.25-1.el7.x86_64


## <a name="see-also"></a>See also

+ [Install Machine Learning Server](r-server-install.md)
+ [Supported platforms](r-server-install-supported-platforms.md)  
+ [Known Issues](../resources-known-issues.md)  