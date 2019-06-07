---
title: 'Uninstall Microsoft R Client to upgrade to a newer version - Machine Learning Server '
description: Explains how to uninstall Microsoft R Client. You do not have to uninstall R Client before installing a more recent version.
keywords: R Client, Microsoft R Client, remove, uninstall, uninstallation
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 02/16/2018
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: 203c0f81b45a70ba7dda9d02afa9558555d498d8
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="uninstall-microsoft-r-client"></a>Uninstall Microsoft R Client 

This article explains how to uninstall Microsoft R Client. **You do not have to uninstall R Client before installing a more recent version.**

## <a name="uninstall-on-windows"></a>Uninstall on Windows

+ Remove Microsoft R Client like other applications using the Add/Remove dialog on Windows.

+ Alternately, you can use the same setup file used to install R Client to remove the program by specifying the /uninstall option on the command line such as: ```RClientSetup.exe /uninstall```


## <a name="uninstall-on-linux"></a>Uninstall on Linux

## <a name="program-version-and-file-locations"></a>Program version and file locations

As a first step, use your package manager to list the currently installed Machine Learning Server packages. (Typically, CentOS and Red Hat systems use **yum**, Ubuntu systems use **apt-get**, and SLES systems use **zypper**):

If your package manager is **yum**:

    yum list \*microsoft-r\*

If your package manager is **apt-get**:

    apt list \*microsoft-r\*

If your package manager is **zypper**:

    zypper search \*microsoft-r\*

## <a name="general-instructions-for-all-versions"></a>General instructions for all versions

Packages are registered in a database that tracks all package installations in the cluster. To update the database, use a package manager to remove the package: **yum** for Red Hat and CentOS, **zypper** for SUSE, or **apt-get** for Ubuntu.

Log in as root or a user with `sudo` privileges. If you are using `sudo`, precede commands requiring root privileges with `sudo` (for example, `sudo yum erase microsoft-r-server-mro-8.0`).

## <a name="how-to-uninstall"></a>How to uninstall

1. Uninstall Microsoft R Open (MRO) and remove any dependent packages used only by MRO:

        yum erase microsoft-r-server-mro-x.x        #(CentOS/RHEL systems))
        apt-get remove microsoft-r-server-mro-x.x   # (Ubuntu systems)
        zypper remove microsoft-r-server-mro-x.x    # (SLES systems)

   where x.x is the version number.

2. On the root node, verify the location of other files that need to be removed: `

        ls /usr/lib64/microsoft-r

3. Remove the entire directory:

        rm -fr /usr/lib64/microsoft-r

The **rm** command removes the folder. Parameter "f" is for force and "r" for recursive, deleting everything under microsoft-r. This command is destructive and irrevocable, so be sure you have the correct directory before you press Enter.


## <a name="learn-more"></a>Learn More

You can learn more with these guides:

+ [Overview of Microsoft R Client](../r-client-get-started.md) 

+ [Quickstart: Running R code in Microsoft R](../r/quickstart-run-r-code.md) (example)

+ [How-to guides in Machine Learning Server](../r/how-to-introduction.md)

+ [RevoScaleR R package reference](../r/tutorial-introduction.md)

+ [MicrosoftML R package reference](../r-reference/microsoftml/microsoftml-package.md)

+ [mrsdeploy R package reference](../r-reference/mrsdeploy/mrsdeploy-package.md)