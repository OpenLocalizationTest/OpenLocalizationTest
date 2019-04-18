---
title: Install Microsoft R Server 2016 (8.0.5) on Teradata Servers
description: Installation and configuration for Microsoft R Server 2016 (version 8.0.5) on Teradata servers.
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 07/29/2016
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: 194c94a08f4a800b9648d8465e9d553595f786b7
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="install-microsoft-r-server-805-on-teradata-servers"></a>Install Microsoft R Server 8.05 on Teradata Servers

>[!NOTE]
>In this release, SLES 10 is no longer supported, only SLES 11 SP1.

Microsoft R Server for Teradata is an R-based analytical engine embedded in your Teradata data warehouse. Together with a Microsoft R Server client, it provides a comprehensive set of tools for interacting with the Teradata database and performing in-database analytics. This article provides detailed instructions for installing Microsoft R Server for Teradata in the Teradata data warehouse. For configuring local workstations to submit jobs to run within your Teradata data warehouse, see [Microsoft R Server Client Installation for Teradata](r-server-install-teradata-client.md).

>[!NOTE]
>Microsoft R Server for Teradata is required for running Microsoft R Server scalable analytics in-database. If you do not need to run your analytics in-database, but simply need to access Teradata data via Teradata Parallel Transport or ODBC, skip installing R Server in your Teradata data warehouse, but do configure your local workstations per [Microsoft R Server Client Installation for Teradata](r-server-install-teradata-client.md).

## <a name="system-requirements"></a>System Requirements

Microsoft R Server for Teradata has the following system requirements:

**Processor:** 64-bit processor with x86-compatible architecture (variously known as AMD64, Intel64, x86-64, IA-32e, EM64T, or x64 chips). Itanium-architecture chips (also known as IA-64) are not supported. Multiple-core processors are recommended.

**Operating System:** SUSE Linux Enterprise Server 11 SP 1 (64-bit).

**Teradata Version:** Teradata 15.10, 15.00, or 14.10.

**Memory:** A minimum of 1GB of RAM is required; 4GB or more are recommended.

**Disk Space:** A minimum of 500MB of disk space is required

The following specific libraries must be installed on the Teradata appliance from the SLES 11 installation DVDs:

* SLES-11-SP1-DVD-x86_64-GM-DVD1.iso/suse/x86_64/ghostscript-fonts-std-8.62-32.27.31.x86_64.rpm

* SLES-11-SP1-DVD-x86_64-GM-DVD1.iso/suse/x86_64/libicu-4.0-7.24.11.x86_64.rpm

* SLE-11-SP1-SDK-DVD-x86_64-GM-DVD1.iso/suse/x86_64/libstdc++45-4.5.0_20100414-1.2.7.x86_64.rpm

* SLE-11-SP1-SDK-DVD-x86_64-GM-DVD1.iso/suse/x86_64/libgfortran43-4.3.4_20091019-0.7.35.x86_64.rpm

* SLE-11-SP1-SDK-DVD-x86_64-GM-DVD1.iso/suse/x86_64/gcc43-fortran-4.3.4_20091019-0.7.35.x86_64.rpm

* SLE-11-SP1-SDK-DVD-x86_64-GM-DVD1.iso/suse/x86_64/gcc-fortran-4.3-62.198.x86_64.rpm


## <a name="download-software"></a>Download software

First, download the version of Microsoft R Open. For this release, you must have Microsoft R Open 3.3.0 for SLES 11 (found at [the mro repository](https://mran.microsoft.com/release-history)

Second, download R Server 8.0.5 for Teradata from [Visual Studio Dev Essentials](https://www.visualstudio.com/dev-essentials/).

1. Click **Join or access now** to sign up for download benefits.
2. Check the URL to verify it changed to *https://my.visualstudio.com/*.
3. Click **Downloads** to search for R Server.
4. Click **Downloads** for a specific version to select the platform.

![Download page on Visual Studio benefits page](./media/mlserver-install-older-versions.png)

## <a name="installing-the-microsoft-r-server-rpms"></a>Installing the Microsoft R Server rpms

Use the Teradata Parallel Update Tool (PUT) to install the Microsoft R Server rpms. PUT runs in a browser. We recommend upgrading to the latest version (3.06.01, as of this writing). This version contains the *PUT Customer Mode*, which is the easiest way to install Microsoft R Server.

1.  If you have an img file, you must first mount the file. The following commands create a mount point and mount the file to that mount point:

        mkdir /mnt/mrsimage
        mount –o loop MRS80TERA.img /mnt/mrsimage

2. Copy the following files to the Customer Mode directory (which you may need to create) */var/opt/teradata/customermodepkgs:*

        microsoft-r-server-mro-8.0.tar.gz
        en_microsoft_r_server_for_teradata_db_x64_8944642.tar.gz

3. Change directory to the Customer Mode packages directory:

        cd /var/opt/teradata/customermodepkgs

4. Unpack the Microsoft R Server installer distribution file using the tar command as follows:

        tar -zxf en_microsoft_r_server_for_teradata_db_x64_8944642.tar.gz

8. Change directory to the one directory created in Step 7:

        cd MRS80TERA

9. Run the install script, install.sh. This script downloads an installer from the internet. For non-internet connected nodes, manually place the en_microsoft_r_server_for_teradata_db_x64_8944642.tar.gz file in /var/opt/teradata/customernodepkgs/MRS80TERA directory on each Teradata node before running 'install.sh'. By running install.sh you are installing Microsoft-r-server-mro-tar-gz, agreeing to MRO_EULA.txt and EULA.txt license agreements.

        ./install.sh

10. Change directory to the Customer Mode packages directory:

        cd /var/opt/teradata/customermodepkgs

11. Point your Java-enabled browser to `https://<HOSTIP>:8443/put` where &lt;HOSTIP&gt; is the IP address of your Teradata data warehouse node and log in to Customer Mode using a *Linux* account such as root (*not* a database account).

To install the Microsoft R Server rpms on all the nodes, do the following:

1.  The initial PUT screen asks you to select an operation. Select **Install/Upgrade Software**.

2.  At the **Install/Upgrade Software: Customer Mode** step, confirm the summary and click **Next**.

3.  You may receive a dialog box saying that PUT was unable to find any packages to auto-select. If you see this dialog box, click **OK**.

4.  Select **Microsoft-r-server-teradata-8.0**.

5.  Select all Groups and click &gt;&gt; to install on all groups, then click **Next**.

6.  Review the list of dependencies and files to be installed, then click **Yes**.

7.  Click **Next**.

8.  Clear the **Restore normal Teradata Vital Infrastructure (TVI) escalation path (recommended)** check box.

9.  Click **Finish**.

Before proceeding, create the /tmp/revoJobs directory on each node and set the correct permissions.

        psh mkdir /tmp/revoJobs
        psh chmod 775 /tmp/revoJobs

## <a name="setting-up-the-revolution-analytics-database"></a>Setting Up the Revolution Analytics Database

After you have installed the rpms, change directory to the "teradata" directory. There are now 3 directories that contain “revoTdSetup.sh”, one for each version of the DBS we support. Use whichever directory applies to your Teradata version:

- /usr/lib64/microsoft-r/8.0/teradata/1410
- /usr/lib64/microsoft-r/8.0/teradata/1500
- /usr/lib64/microsoft-r/8.0/teradata/1510

Next, run the revoTdSetup.sh script:

        chmod u+x ./revoTdSetup.sh
        ./revoTdSetup.sh

Enter the parent user database name and password at the prompts. **Do not modify this script**, and in particular, do not modify the name of the revoAnalytics_Zqht2 database. The database administrator running the script must have specific grants, as described in the next section.

>[!NOTE]
>If you have previously run Microsoft R Server on your Teradata database, restart the database before proceeding.

## <a name="adding-and-configuring-users"></a>Adding and Configuring Users

All users who will interact with the database, including the database administrator, need to have specific grants. The following example provides an existing “sysdba” user the required grants to run the revoTdSetup.sh script:

    grant all on sysdba to sysdba with grant option;

If you don’t already have such a user, the following example creates a database administrator user named "sysdba" with the required grants to run the revoTdSetup.sh script:

    # Create the user who will run revoTdSetup.sh (e.g., sysdba):
    bteq .logon localhost/dbc,dbc
    create user SYSDBA from dbc as perm=25E9, spool=15E9, temporary=15E9, password=sysdba;
    grant select, execute on dbc to sysdba with grant option;
    grant all on sysdba to sysdba with grant option;
    grant select on sys_calendar to sysdba with grant option;
    grant select on dbc to public;

You will often want to allow a user account to run jobs on data in other databases also. The lines shown below are examples of the types of permissions your Revolution users may require. (For convenience, these steps are organized according to the purpose of the permissions granted.)

1.  First, you will need to grant permissions for the user account to work with the Revolution database.  Logon to bteq with your admin account, and run the following lines.  Substitute the new user account name for 'ut1' in the sample lines below.

        -- grant ut1 various permissions on revoAnalytics_Zqht2 DB
        grant execute procedure on revoAnalytics_Zqht2.InitRevoJob to ut1;
        grant execute procedure on revoAnalytics_Zqht2.StartRevoJobXsp to ut1;
        grant execute procedure on revoAnalytics_Zqht2.GetRevoJobState to ut1;
        grant execute procedure on revoAnalytics_Zqht2.RemoveRevoJobResults to ut1;
        grant execute function on revoAnalytics_Zqht2.FinishRevoJob to ut1;
        grant execute function on revoAnalytics_Zqht2.DistributeRevoJobDataUdf to ut1;
        grant execute function on revoAnalytics_Zqht2.revoAnalyticsTblOp to ut1;
        grant select on revoAnalytics_Zqht2.RevoAnalyticsJobResults to ut1;

        -- the following two create view and drop view grants are for the
        -- table operator PARTITION BY work-around
        -- for Teradata's Issue DR166609, which was fixed in 14.10.02d
        grant create view on revoAnalytics_Zqht2 to ut1;
        grant drop view on revoAnalytics_Zqht2 to ut1;

2.  Next you will need to grant permissions for the user account and the revolution database to work with data in the user account database.  Run the following lines, substituting your user account name for 'ut1'.

        -- grant ut1 rights on db with data to be analyzed -
        -- in this case itself
        grant all on ut1 to ut1;

        -- give revoAnalytics_Zqht2 rights on database with data to
        -- be analyzed - in this case ut1
        grant select on ut1 to revoAnalytics_Zqht2;
        grant create table on ut1 to revoAnalytics_Zqht2;
        grant drop table on ut1 to revoAnalytics_Zqht2;

3.  Finally, you will want to grant permissions on any other databases you wish that account to have access to.  Run the following lines, substituting your user account name for 'ut1', and your other database name for 'RevoTestDB'.

        -- grant ut1 rights on db with data to be analyzed
        grant select on RevoTestDB to ut1;

        -- give revoAnalytics_Zqht2 rights on database with data to
        -- be analyzed
        grant select on RevoTestDB to revoAnalytics_Zqht2;
        grant create table on RevoTestDB to revoAnalytics_Zqht2;

## <a name="managing-memory-in-in-teradata-computations"></a>Managing Memory in In-Teradata Computations

Because a Teradata cluster node typically has many worker processes (AMPs) running constantly, it is important to limit how much memory a distributed analysis consumes. Microsoft R Server provides stored procedures in the revoAnalytics\_Zqht2 scheduler database that allow a database administrator to set the memory limits for master and worker processes working on a RevoScaleR job. By default, the master process memory limit is 2000 MB (approximately 2GB) and the worker process memory limit is 1000MB (approximately 1GB).

These limits may be customized by a database administrator using the SetMasterMemoryLimitMB() and SetWorkerMemoryLimitMB() stored procedures, defined in the revoAnalytics\_Zqht2 database created on installation.

For example, to set the master memory limit to 3000MB:

        call revoAnalytics_Zqht2.SetMasterMemoryLimitMB(3000);

To set the worker memory limit to 1500MB:

        call revoAnalytics_Zqht2.SetWorkerMemoryLimitMB(1500);

The current memory limits can be viewed in the revoAnalytics\_Zqht2.Properties table.

Note that memory limits that have been changed are in effect immediately, and no restart of the database is required.

## <a name="maintaining-the-revolution-database"></a>Maintaining the Revolution Database

Two tables in the revoAnalytics\_Zqht2 database may require periodic cleanup:

- **RevoJobs** – one row is added to this table for each job. Each job is assigned a job ID between 1 and 2,147,483,647. The table is not automatically cleaned up. If never cleaned up, it can grow to up to 2,147,483,647 rows. In version 8.0.0 and earlier, values did not recycle unless old rows were deleted, and the next ID was always computed as the max ID in the table plus 1, which could result in integer overflow. In version 8.0.1 and later, after reaching the maximum value, the job IDs cycle back to 1 (or a relatively low number) harmlessly.

- **RevoAnalyticsJobResults** – multiple rows are added for each job. It is automatically cleaned up if wait = TRUE in RxInTeradata(), but not if wait = FALSE. In version 8.0.1 and later, if the job IDs have cycled, then any rows matching a recycled ID are deleted before the ID is reused.

## <a name="installing-additional-r-packages"></a>Installing Additional R Packages

The R community is an active, open-source community, and new packages extending R’s capacity for statistics, data analysis, graphics, and interconnectivity are added frequently. The most up-to-date source for these third-party packages is the Comprehensive R Archive Network (CRAN), a network of servers around the world that store open-source R distributions, extensions, documentation and binaries. The repository (<https://cran.r-project.org/>) has grown from only 12 packages in 1997 to over 5300 packages currently. However, CRAN does not maintain source packages by R version, and Microsoft R Server for Teradata is seldom the latest R version, so packages from CRAN may be incompatible with Microsoft R Server for Teradata. Microsoft’s MRAN archive (<https://mran.microsoft.com>), however, maintains daily snapshots of the CRAN repository. Users may take advantage of this repository and download the chosen packages from any specific date, but notice that they are completely external to Teradata.

In most cases, the natural place to install additional R packages is to the client workstation. Installation to the Teradata data warehouse is required only if you plan to use the package’s functions as transform functions inside RevoScaleR functions, in which case the packages will actually need to be loaded in-database. If you need a package for this purpose, you can do so as follows:

To manually distribute and install the package:

1.  Download the package and any required dependencies from <https://mran.microsoft.com/>.
2.  Copy the downloaded packages to each node of your data warehouse.
3.  For each package, run the command “R CMD INSTALL `*`package.`*`tar.gz” on each node. (If your data warehouse is equipped with the psh command, you can use that to run the command on all the nodes in parallel.)

## <a name="removing-microsoft-r-server"></a>Removing Microsoft R Server

To remove Microsoft R Server from your computer, run the following commands:

        psh rpm -e microsoft-r-server-teradata-8.0
        psh rpm -e microsoft-r-server-packages-8.0
        psh rpm -e microsoft-r-server-intel-mkl-8.0
        psh rpm -e microsoft-r-server-mro-8.0
