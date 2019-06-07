---
title: Troubleshoot Microsoft R installation problems on Hadoop
description: Troubleshoot Microsoft R installation on a Hadoop cluster.
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 01/19/2017
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: d06c296f4213e12480b35ccebf9722f4549d6763
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="troubleshoot-microsoft-r-installation-problems-on-hadoop"></a>Troubleshoot Microsoft R installation problems on Hadoop

No two Hadoop installations are exactly alike, but most are quite similar. This article brings together a number of common errors seen in attempting to run Microsoft R Server commands on Hadoop clusters, and the most likely causes of such errors from our experience.

## <a name="missing-dependencies"></a>Missing dependencies

Linux and Hadoop servers that are locked down prevent the installation script from downloading any required dependencies that are missing on your system. For a list of all dependencies required by Microsoft R, see [Package Dependencies for Microsoft R Server installations on Linux and Hadoop](r-server-install-linux-hadoop-packages.md).

## <a name="no-valid-credentials"></a>No Valid Credentials

If you see a message such as “No valid credentials provided”, this means you do not have a valid Kerberos ticket. Quit Microsoft R Server, obtain a Kerberos ticket using kinit, and then restart Microsoft R Server.

## <a name="unable-to-load-class-revoscaler"></a>Unable to Load Class RevoScaleR

If you see a message about being unable to find or load main class RevoScaleR, this means that the jar file scaleR-hadoop-0.1-SNAPSHOT.jar could not be found. This jar file must be in a location where it can be found by the getHadoopEnvVars.py script, or its location must be explicitly added to the CLASSPATH.

## <a name="classpath-errors"></a>Classpath Errors

If you see other errors related to Java classes, these are likely related to the settings of the following environment variables:

- PATH
- CLASSPATH
- JAVA\_LIBRARY\_PATH

Of these, the most commonly misconfigured is the CLASSPATH.

## <a name="unable-to-load-shared-library"></a>Unable to Load Shared Library

If you see a message about being unable to load libhdfs.so, you may need to create a symbolic link from your installed version of libhdfs.so to the system library, such as the following command:

    ln -s /path/to/libhdfs.so /usr/lib64/libhdfs.so

Or, update your LD\_LIBRARY\_PATH environment variable to include the path to the libjvm shared object:

    export LD\_LIBRARY\_PATH=$LD_LIBRARY_PATH:/path/to/libhdfs.so

(This step is normally performed automatically during the RRE install. If you continue to see errors about libhdfs.so, you may need to both create the preceding symbolic link and set LD_LIBRARY_PATH.)

Similarly, if you see a message about being unable to load libjvm.so, you may need to create a symbolic link from your installed version of libjvm.so to the system library, such as the following command:

    ln -s /path/to/libjvm.so /usr/lib64/libjvm.so

Or, update your LD\_LIBRARY\_PATH environment variable to include the path to the libjvm shared object:

export LD\_LIBRARY\_PATH=$LD\_LIBRARY\_PATH:/path/to/libjvm.so


## <a name="hive-odbc-connection-problems-on-edge-nodes"></a>Hive ODBC Connection Problems on Edge Nodes

An ODBC connection to Hive from an edge node can be useful for both importing the results of Hive queries, and directly streaming results into ScaleR algorithms for analysis. 

Prior to using `RxOdbcData` against Hive, we recommend that you begin by installing and configuring the ODBC drivers provided by your Hadoop vendor for your installed distro. Next, work with your Hadoop vendor to debug the ODBC setup until you are able to successfully run Hive queries using a Hive command-line tool such as ‘beeline’. Lastly, take one of those queries that you ran from the command line and try running it from within R Server on the edge node via `RxOdbcData`.

## <a name="check-hadoop-cluster-health"></a>Check Hadoop cluster health

Hadoop includes example programs that help verify the health of your cluster. One exmaple is the jar file hadoop-mapreduce-examples.jar. The following command should display a list of the available examples:

    hadoop jar /usr/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar

On MapR, the quick installation installs the Hadoop files to /opt/mapr by default; the path to the examples jar file is */opt/mapr/hadoop/hadoop-0.20.2/hadoop-0.20.2-dev-examples.jar*. 

On Cloudera Manager parcel installs, the default path to the examples is */opt/cloudera/parcels/CDH/lib/hadoop-mapreduce-examples.jar*.)

The following command runs the pi example, which uses Monte Carlo sampling to estimate pi. The 5 tells Hadoop to use 5 mappers, the 300 says to use 300 samples per map:

    hadoop jar /usr/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar pi 5 300

If you can successfully run one or more of the Hadoop examples, your Hadoop installation was successful and you are ready to install Microsoft R Server.
