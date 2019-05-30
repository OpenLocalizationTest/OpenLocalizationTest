<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-teradata-805.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e194c94a08f4a800b9648d8465e9d553595f786b7.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">194c94a08f4a800b9648d8465e9d553595f786b7</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-teradata-805.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install Microsoft R Server 2016 (8.0.5) on Teradata Servers</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Installation and configuration for Microsoft R Server 2016 (version 8.0.5) on Teradata servers.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Server 8.05 on Teradata Servers</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>In this release, SLES 10 is no longer supported, only SLES 11 SP1.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Microsoft R Server for Teradata is an R-based analytical engine embedded in your Teradata data warehouse.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Together with a Microsoft R Server client, it provides a comprehensive set of tools for interacting with the Teradata database and performing in-database analytics.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>This article provides detailed instructions for installing Microsoft R Server for Teradata in the Teradata data warehouse.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>For configuring local workstations to submit jobs to run within your Teradata data warehouse, see <bpt id="p1">[</bpt>Microsoft R Server Client Installation for Teradata<ept id="p1">](r-server-install-teradata-client.md)</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Microsoft R Server for Teradata is required for running Microsoft R Server scalable analytics in-database.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If you do not need to run your analytics in-database, but simply need to access Teradata data via Teradata Parallel Transport or ODBC, skip installing R Server in your Teradata data warehouse, but do configure your local workstations per <bpt id="p1">[</bpt>Microsoft R Server Client Installation for Teradata<ept id="p1">](r-server-install-teradata-client.md)</ept>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>System Requirements</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Microsoft R Server for Teradata has the following system requirements:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Processor:<ept id="p1">**</ept> 64-bit processor with x86-compatible architecture (variously known as AMD64, Intel64, x86-64, IA-32e, EM64T, or x64 chips).</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Itanium-architecture chips (also known as IA-64) are not supported.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Multiple-core processors are recommended.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Operating System:<ept id="p1">**</ept> SUSE Linux Enterprise Server 11 SP 1 (64-bit).</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Teradata Version:<ept id="p1">**</ept> Teradata 15.10, 15.00, or 14.10.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Memory:<ept id="p1">**</ept> A minimum of 1GB of RAM is required; 4GB or more are recommended.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Disk Space:<ept id="p1">**</ept> A minimum of 500MB of disk space is required</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The following specific libraries must be installed on the Teradata appliance from the SLES 11 installation DVDs:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>SLES-11-SP1-DVD-x86_64-GM-DVD1.iso/suse/x86_64/ghostscript-fonts-std-8.62-32.27.31.x86_64.rpm</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>SLES-11-SP1-DVD-x86_64-GM-DVD1.iso/suse/x86_64/libicu-4.0-7.24.11.x86_64.rpm</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>SLE-11-SP1-SDK-DVD-x86_64-GM-DVD1.iso/suse/x86_64/libstdc++45-4.5.0_20100414-1.2.7.x86_64.rpm</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>SLE-11-SP1-SDK-DVD-x86_64-GM-DVD1.iso/suse/x86_64/libgfortran43-4.3.4_20091019-0.7.35.x86_64.rpm</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>SLE-11-SP1-SDK-DVD-x86_64-GM-DVD1.iso/suse/x86_64/gcc43-fortran-4.3.4_20091019-0.7.35.x86_64.rpm</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>SLE-11-SP1-SDK-DVD-x86_64-GM-DVD1.iso/suse/x86_64/gcc-fortran-4.3-62.198.x86_64.rpm</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Download software</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>First, download the version of Microsoft R Open.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>For this release, you must have Microsoft R Open 3.3.0 for SLES 11 (found at <bpt id="p1">[</bpt>the mro repository<ept id="p1">](https://mran.microsoft.com/release-history)</ept></source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Second, download R Server 8.0.5 for Teradata from <bpt id="p1">[</bpt>Visual Studio Dev Essentials<ept id="p1">](https://www.visualstudio.com/dev-essentials/)</ept>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Join or access now<ept id="p1">**</ept> to sign up for download benefits.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Check the URL to verify it changed to <bpt id="p1">*</bpt><ph id="ph1">https://my.visualstudio.com/</ph><ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> to search for R Server.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> for a specific version to select the platform.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Download page on Visual Studio benefits page</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Installing the Microsoft R Server rpms</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Use the Teradata Parallel Update Tool (PUT) to install the Microsoft R Server rpms.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>PUT runs in a browser.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>We recommend upgrading to the latest version (3.06.01, as of this writing).</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>This version contains the <bpt id="p1">*</bpt>PUT Customer Mode<ept id="p1">*</ept>, which is the easiest way to install Microsoft R Server.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If you have an img file, you must first mount the file.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The following commands create a mount point and mount the file to that mount point:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Copy the following files to the Customer Mode directory (which you may need to create) <bpt id="p1">*</bpt>/var/opt/teradata/customermodepkgs:<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Change directory to the Customer Mode packages directory:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Unpack the Microsoft R Server installer distribution file using the tar command as follows:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Change directory to the one directory created in Step 7:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Run the install script, install.sh. This script downloads an installer from the internet.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>For non-internet connected nodes, manually place the en_microsoft_r_server_for_teradata_db_x64_8944642.tar.gz file in /var/opt/teradata/customernodepkgs/MRS80TERA directory on each Teradata node before running 'install.sh'.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>By running install.sh you are installing Microsoft-r-server-mro-tar-gz, agreeing to MRO_EULA.txt and EULA.txt license agreements.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Change directory to the Customer Mode packages directory:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Point your Java-enabled browser to <ph id="ph1">`https://&lt;HOSTIP&gt;:8443/put`</ph> where <ph id="ph2">&amp;lt;</ph>HOSTIP<ph id="ph3">&amp;gt;</ph> is the IP address of your Teradata data warehouse node and log in to Customer Mode using a <bpt id="p1">*</bpt>Linux<ept id="p1">*</ept> account such as root (<bpt id="p2">*</bpt>not<ept id="p2">*</ept> a database account).</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>To install the Microsoft R Server rpms on all the nodes, do the following:</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The initial PUT screen asks you to select an operation.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Install/Upgrade Software<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>At the <bpt id="p1">**</bpt>Install/Upgrade Software: Customer Mode<ept id="p1">**</ept> step, confirm the summary and click <bpt id="p2">**</bpt>Next<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>You may receive a dialog box saying that PUT was unable to find any packages to auto-select.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>If you see this dialog box, click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Microsoft-r-server-teradata-8.0<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Select all Groups and click <ph id="ph1">&amp;gt;</ph><ph id="ph2">&amp;gt;</ph> to install on all groups, then click <bpt id="p1">**</bpt>Next<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Review the list of dependencies and files to be installed, then click <bpt id="p1">**</bpt>Yes<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Next<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Clear the <bpt id="p1">**</bpt>Restore normal Teradata Vital Infrastructure (TVI) escalation path (recommended)<ept id="p1">**</ept> check box.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Finish<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Before proceeding, create the /tmp/revoJobs directory on each node and set the correct permissions.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Setting Up the Revolution Analytics Database</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>After you have installed the rpms, change directory to the "teradata" directory.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>There are now 3 directories that contain “revoTdSetup.sh”, one for each version of the DBS we support.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Use whichever directory applies to your Teradata version:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>/usr/lib64/microsoft-r/8.0/teradata/1410</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>/usr/lib64/microsoft-r/8.0/teradata/1500</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>/usr/lib64/microsoft-r/8.0/teradata/1510</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Next, run the revoTdSetup.sh script:</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Enter the parent user database name and password at the prompts.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Do not modify this script<ept id="p1">**</ept>, and in particular, do not modify the name of the revoAnalytics_Zqht2 database.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>The database administrator running the script must have specific grants, as described in the next section.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>If you have previously run Microsoft R Server on your Teradata database, restart the database before proceeding.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Adding and Configuring Users</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>All users who will interact with the database, including the database administrator, need to have specific grants.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>The following example provides an existing “sysdba” user the required grants to run the revoTdSetup.sh script:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>If you don’t already have such a user, the following example creates a database administrator user named "sysdba" with the required grants to run the revoTdSetup.sh script:</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>You will often want to allow a user account to run jobs on data in other databases also.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>The lines shown below are examples of the types of permissions your Revolution users may require.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>(For convenience, these steps are organized according to the purpose of the permissions granted.)</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>First, you will need to grant permissions for the user account to work with the Revolution database.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source> Logon to bteq with your admin account, and run the following lines.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source> Substitute the new user account name for 'ut1' in the sample lines below.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Next you will need to grant permissions for the user account and the revolution database to work with data in the user account database.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source> Run the following lines, substituting your user account name for 'ut1'.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Finally, you will want to grant permissions on any other databases you wish that account to have access to.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source> Run the following lines, substituting your user account name for 'ut1', and your other database name for 'RevoTestDB'.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Managing Memory in In-Teradata Computations</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Because a Teradata cluster node typically has many worker processes (AMPs) running constantly, it is important to limit how much memory a distributed analysis consumes.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Microsoft R Server provides stored procedures in the revoAnalytics<ph id="ph1">\_</ph>Zqht2 scheduler database that allow a database administrator to set the memory limits for master and worker processes working on a RevoScaleR job.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>By default, the master process memory limit is 2000 MB (approximately 2GB) and the worker process memory limit is 1000MB (approximately 1GB).</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>These limits may be customized by a database administrator using the SetMasterMemoryLimitMB() and SetWorkerMemoryLimitMB() stored procedures, defined in the revoAnalytics<ph id="ph1">\_</ph>Zqht2 database created on installation.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>For example, to set the master memory limit to 3000MB:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>To set the worker memory limit to 1500MB:</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>The current memory limits can be viewed in the revoAnalytics<ph id="ph1">\_</ph>Zqht2.Properties table.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Note that memory limits that have been changed are in effect immediately, and no restart of the database is required.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Maintaining the Revolution Database</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Two tables in the revoAnalytics<ph id="ph1">\_</ph>Zqht2 database may require periodic cleanup:</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoJobs<ept id="p1">**</ept> – one row is added to this table for each job.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Each job is assigned a job ID between 1 and 2,147,483,647.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>The table is not automatically cleaned up.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>If never cleaned up, it can grow to up to 2,147,483,647 rows.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>In version 8.0.0 and earlier, values did not recycle unless old rows were deleted, and the next ID was always computed as the max ID in the table plus 1, which could result in integer overflow.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>In version 8.0.1 and later, after reaching the maximum value, the job IDs cycle back to 1 (or a relatively low number) harmlessly.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoAnalyticsJobResults<ept id="p1">**</ept> – multiple rows are added for each job.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>It is automatically cleaned up if wait = TRUE in RxInTeradata(), but not if wait = FALSE.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>In version 8.0.1 and later, if the job IDs have cycled, then any rows matching a recycled ID are deleted before the ID is reused.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Installing Additional R Packages</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>The R community is an active, open-source community, and new packages extending R’s capacity for statistics, data analysis, graphics, and interconnectivity are added frequently.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>The most up-to-date source for these third-party packages is the Comprehensive R Archive Network (CRAN), a network of servers around the world that store open-source R distributions, extensions, documentation and binaries.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>The repository (<ph id="ph1">&lt;https://cran.r-project.org/&gt;</ph>) has grown from only 12 packages in 1997 to over 5300 packages currently.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>However, CRAN does not maintain source packages by R version, and Microsoft R Server for Teradata is seldom the latest R version, so packages from CRAN may be incompatible with Microsoft R Server for Teradata.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Microsoft’s MRAN archive (<ph id="ph1">&lt;https://mran.microsoft.com&gt;</ph>), however, maintains daily snapshots of the CRAN repository.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Users may take advantage of this repository and download the chosen packages from any specific date, but notice that they are completely external to Teradata.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>In most cases, the natural place to install additional R packages is to the client workstation.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Installation to the Teradata data warehouse is required only if you plan to use the package’s functions as transform functions inside RevoScaleR functions, in which case the packages will actually need to be loaded in-database.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>If you need a package for this purpose, you can do so as follows:</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>To manually distribute and install the package:</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Download the package and any required dependencies from <ph id="ph1">&lt;https://mran.microsoft.com/&gt;</ph>.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Copy the downloaded packages to each node of your data warehouse.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>For each package, run the command “R CMD INSTALL <ph id="ph1">`*`</ph>package.<ph id="ph2">`*`</ph>tar.gz” on each node.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>(If your data warehouse is equipped with the psh command, you can use that to run the command on all the nodes in parallel.)</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Removing Microsoft R Server</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>To remove Microsoft R Server from your computer, run the following commands:</source>
        </trans-unit></group></body></file></xliff>