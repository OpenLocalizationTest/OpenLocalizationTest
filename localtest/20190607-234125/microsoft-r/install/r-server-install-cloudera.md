---
title: R Server installation on Cloudera CDH
description: Install Microsoft R Server 9.1 on the Cloudera distribution of Apache Hadoop (CDH).
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 03/29/2017
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: 7b1cfa3d9cfe8c37e963162f04d029ed27231783
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="install-r-server-91-on-the-cloudera-distribution-of-apache-hadoop-cdh"></a>Install R Server 9.1 on the Cloudera distribution of Apache Hadoop (CDH)

**Looking for the latest release? See [Machine Learning Server for Cloudera installation](machine-learning-server-cloudera-install.md)**

Cloudera offers a parcel installation methodology for adding services and features to a cluster. If you prefer parcel installation over the regular install script used for deploying R Server on other Hadoop distributions, you can use functionality we provide to create the parcel.

If you've used parcel installation in previous releases of Microsoft R Server, the 9.1.0 release is enhanced in two respects. First, instead of using pre-built parcels downloaded from Microsoft, you can generate your own parcel using a new generate_mrs_parcel.sh script. Secondly, we added support for Custom Service Descriptors (CSDs), which means you can now deploy, configure, and monitor R Server in CDH as a managed service in Cloudera Manager.

The new revised workflow for parcel installation is a two-part exercise:

+ [Part 1: At the console, run script to output parcel and CSD files](r-server-install-cloudera-generate-parcel.md)
+ [Part 2: In Cloudera Manager, deploy parcels and add MRS as a managed service](r-server-install-cloudera-deploy-activate.md)

Download and unpacking the distribution remains the same. Instructions are included in Part 1.

**Feature restrictions in a parcel installation**

R Server includes two packages, `MicrosoftML` and `mrsdeploy`, that either cannot be included in the parcel, or included only if the underlying operating system is a specific platform and version.

+ `MicrosoftML` is conditionally available. The package can be included in the parcel if the underlying operating system is CentOS/RHEL 7.x. If CDH runs on any other operating system, including an earlier version of RHEL, the `MicrosoftML` package cannot be included.

+ `mrsdeploy` is excluded from a parcel installation. This package has a .NET Core dependency and cannot be added to a parcel.

The workaround is to perform a manual installation of individual packages. For instructions, see [Manual package installation](r-server-install-hadoop-manual-package.md).

## <a name="see-also"></a>See Also

[R Server Installation on Hadoop Overview](r-server-install-hadoop.md)
