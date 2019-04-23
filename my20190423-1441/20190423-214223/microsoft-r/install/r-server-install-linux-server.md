<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-linux-server.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca862e474641fa0c899f47b466c63be9c43847f2d145.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">2e474641fa0c899f47b466c63be9c43847f2d145</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-linux-server.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Server 9.1 installation for Linux systems</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install Microsoft R Server 9.1.0 on Linux.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>R Server 9.1 Installation for Linux Systems</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Looking for the latest release?</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>Machine Learning Server for Linux installation<ept id="p1">](machine-learning-server-linux-install.md)</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Microsoft R Server is an enterprise class server for hosting and managing parallel and distributed workloads of R processes on servers and clusters.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The server runs on a wide range of computing platforms, including Linux.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This article explains how to install Microsoft R Server 9.1.0 on a standalone Linux server that has an internet connection.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>If your server has restrictions on internet access, see the instructions for an <bpt id="p1">[</bpt>offline installation<ept id="p1">](r-server-install-linux-offline.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If you previously installed version 9.0.1, it will be replaced with the 9.1.0 version.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>An 8.x version can run side-by-side 9.x, unaffected by the new installation.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>System requirements</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Operating system must be a <bpt id="p1">[</bpt>supported version of Linux<ept id="p1">](r-server-install-supported-platforms.md)</ept> on a 64-bit with x86-compatible architecture (variously known as AMD64, Intel64, x86-64, IA-32e, EM64T, or x64 chips).</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Itanium chips (also known as IA-64) are not supported.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Multiple-core chips are recommended.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Memory must be a minimum of 2 GB of RAM is required; 8 GB or more are recommended.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Disk space must be a minimum of 500 MB.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>An internet connection.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If you do not have an internet connection, for the instructions for an <bpt id="p1">[</bpt>offline installation<ept id="p1">](r-server-install-linux-offline.md)</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>A package manager (yum for RHEL systems, apt for Ubuntu, zypper for SLES systems)</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Root or super user permissions</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The following additional components are included in Setup and required for R Server.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Microsoft R Open 3.3.3</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Microsoft .NET Core 1.1 for Linux (required for mrsdeploy and MicrosoftML use cases)</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>How to install</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>This section walks you through an R Server 9.1.0 deployment using the <ph id="ph1">`install.sh`</ph> script.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Under these instructions, your installation will be serviced under the <bpt id="p1">[</bpt>Modern Lifecycle policy<ept id="p1">](https://support.microsoft.com/en-us/help/447912)</ept> and includes the ability to <bpt id="p2">[</bpt>operationalize your analytics<ept id="p2">](../what-is-operationalization.md)</ept> and use the MicrosoftML package.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Review <bpt id="p1">[</bpt>recommendations and best practices<ept id="p1">](r-server-install-linux-manage-install.md)</ept> for deployments in locked down environments.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Download R Server installer</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>You can get the gzipped installation file from one of the following download sites.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Site</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Edition</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Visual Studio Dev Essentials</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Developer (free)</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>This option provides a zipped file, free when you sign up for Visual Studio Dev Essentials.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Developer edition has the same features as Enterprise, except it is licensed for development scenarios.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Volume Licensing Service Center (VLSC)</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Enterprise</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Sign in, search for R Server for Linux.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>A selection for <bpt id="p1">**</bpt>R Server 9.1.0 for Linux<ept id="p1">**</ept> is provided on this site.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>For downloads from <bpt id="p1">[</bpt>Visual Studio Dev Essentials<ept id="p1">](https://www.visualstudio.com/dev-essentials/)</ept>:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Join or access now<ept id="p1">**</ept> to sign up for download benefits.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Check the URL to verify it changed to <bpt id="p1">*</bpt><ph id="ph1">https://my.visualstudio.com/</ph><ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> to search for R Server.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> for a specific version to select the platform.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Download page on Visual Studio benefits page</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Unpack the distribution</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Download the software to a writable directory, such as <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept>, unpack the distribution and then run the installation script.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The distribution includes one installer for Microsoft R Server.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>For a gzipped TAR file, you should unpack the file as follows (be sure you have downloaded the file to a writable directory, such as <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept>):</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Log in as root or a user with super user privileges (<ph id="ph1">`sudo su`</ph>).</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Switch to the <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept> directory (assuming it's the download location).</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Unpack the file:</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>The distribution is unpacked into an <ph id="ph1">`MRS91Linux`</ph> folder at the download location.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The distribution includes the following files:</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>File</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Script for installing R Server.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Script for generating a parcel used for <bpt id="p1">[</bpt>installing R Server on CDH<ept id="p1">](r-server-install-cloudera.md)</ept>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>End user license agreements for each separately licensed component.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>DEB folder</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Contains Microsoft R packages for deployment on Ubuntu.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>RPM folder</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Contains Microsoft R packages for deployment on CentOS/RHEL and SUSE.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Parcel folder</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Contains files used to generate a parcel for installation on CDH.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>MRS packages include an admin utility, core engine and function libraries, compute node and web node configuration options, platform packages, and machine learning.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Package names in the R Server distribution have changed in the 9.1 release.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Instead of DeployrR-themed package names, the new names are aligned to base packages.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>If you have script or tooling for manual R Server package installation, be sure to note the name change.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Run the MRS install script</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>R Server for Linux is deployed by running the install script with no parameters.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Log in as root or as a user with super user privileges (<ph id="ph1">`sudo -s`</ph>).</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>The following instructions assume root install.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Clean cached data so that the installer can get updated packages.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>On RHEL use <bpt id="p1">[</bpt>yum<ept id="p1">](https://access.redhat.com/documentation/Red_Hat_Enterprise_Linux/6/html/Deployment_Guide/sec-Working_with_Yum_Cache.html)</ept>:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>On Ubuntu use <bpt id="p1">[</bpt>apt-get<ept id="p1">](https://help.ubuntu.com/community/AptGet/Howto)</ept>:</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Change to the <ph id="ph1">`MRS91Linux`</ph> directory containing the installation script:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Run the script.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>To include the <bpt id="p1">[</bpt>pre-trained machine learning models for MicrosoftML<ept id="p1">](microsoftml-install-pretrained-models.md)</ept>, append the <ph id="ph1">`-m`</ph> switch.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>When prompted to accept the license terms for Microsoft R Open, click Enter to read the EULA, click <bpt id="p1">**</bpt>q<ept id="p1">**</ept> when you are finished reading, and then click <bpt id="p2">**</bpt>y<ept id="p2">**</ept> to accept the terms.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Repeat for the R Server license agreement: click Enter, click <bpt id="p1">**</bpt>q<ept id="p1">**</ept> when finished reading, click <bpt id="p2">**</bpt>y<ept id="p2">**</ept> to accept the terms.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Installation begins immediately.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Installer output shows the packages and location of the log file.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Verify installation</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>List installed MRS packages:</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>On RHEL:</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>On Ubuntu:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Once you have a package name, you can obtain verbose version information.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>On RHEL:</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>On Ubuntu:</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Partial output is as follows (note version 9.1.0):</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Start Revo64</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>As another verification step, run the Revo64 program.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>By default, Revo64 is linked to the /usr/bin directory, available to any user who can log in to the machine:</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>From /Home or any other working directory:</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Run a RevoScaleR function, such as <bpt id="p1">**</bpt>rxSummary<ept id="p1">**</ept> on a dataset.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Many sample datasets, such as the iris dataset, are ready to use because they are installed with the software:</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Output from the iris dataset should look similar to the following:</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>To quit the program, type <ph id="ph1">`q()`</ph> at the command line with no arguments.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Enable Remote Connections and Analytic Deployment</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>The server can be used as-is if you install and use an R IDE on the same box, but to benefit from the deployment and consumption of web services with Microsoft R Server, then you must configure R Server after installation to act as a deployment server and host analytic web services.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Possible configurations are a <bpt id="p1">[</bpt>one-box setup<ept id="p1">](operationalize-r-server-one-box-config.md)</ept> or an <bpt id="p2">[</bpt>enterprise setup<ept id="p2">](operationalize-r-server-enterprise-config.md)</ept>.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Doing so also enables remote execution, allowing you to connect to R Server from an R Client workstation and execute code on the server.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Unattended install options</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>You can perform a silent install to bypass prompts during setup.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>In /tmp/MRS91Linux, run the install script with the following parameters:</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Additional flags are available, as follows:</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>flag</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Option</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>-a</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>--accept-eula</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Accept all end user license agreements.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>-d</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>--download-mro</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Download microsoft r open for distribution to an offline system.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>-m</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>--models</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Install Microsoft ML models.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>-r</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>--no-dotnet-core</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Opt out of installing .NET Core (required for mrsdeploy and MicrosoftML)</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>-s</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>--silent</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Perform a silent, unattended install.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>-u</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>--unattended</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Perform an unattended install.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>-h</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>--help</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Print this help text.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>What's Installed with R Server</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>The Microsoft R Server setup installs the R base packages and a set of enhanced and proprietary R packages that support parallel processing, improved performance, and connectivity to data sources including SQL Server and Hadoop.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>In contrast with R Client, R Server supports much larger data sets and distributed workloads.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>By default, telemetry data is collected during your usage of R Server.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>To turn this feature off, use the RevoScaleR package function <ph id="ph1">`rxPrivacyControl(FALSE)`</ph>.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>To turn it back on, change the setting to <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Next Steps</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Review the best practices in <bpt id="p1">[</bpt>Manage your R Server for Linux installation<ept id="p1">](r-server-install-linux-manage-install.md)</ept> for instructions on how to set up a local package repository using MRAN or miniCRAN, change file ownership or permissions, set Revo64 as the de facto R script engine on your server.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Introduction to R Server<ept id="p1">](../what-is-microsoft-r-server.md)</ept> <bpt id="p2">[</bpt>What's New in R Server<ept id="p2">](../whats-new-in-r-server.md)</ept> <bpt id="p3">[</bpt>Supported platforms<ept id="p3">](r-server-install-supported-platforms.md)</ept></source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Known Issues</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Install R on Hadoop overview</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Uninstall Microsoft R Server to upgrade to a newer version<ept id="p1">](r-server-install-linux-uninstall.md)</ept> <bpt id="p2">[</bpt>Troubleshoot R Server installation problems on Hadoop<ept id="p2">](r-server-install-hadoop-troubleshoot.md)</ept></source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Configure R Server to operationalize analytics</source>
        </trans-unit></group></body></file></xliff>