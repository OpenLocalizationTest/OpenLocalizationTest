<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-windows-offline.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a41891fff21af2f06ac7083098f692d33f6de2ed2.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">41891fff21af2f06ac7083098f692d33f6de2ed2</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-windows-offline.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Offline install for Microsoft R Server 9.1 for Windows</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to install R Server 9.1 without an internet connection</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Offline installation for R Server 9.1 for Windows</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Looking for the latest release?</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>Machine Learning Server for Windows installation<ept id="p1">](machine-learning-server-windows-offline.md)</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>By default, installers connect to Microsoft download sites to get required and updated components.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>If firewall restrictions or constraints on internet access prevent the installer from reaching these sites, you can use an internet-connected device to download files, transfer files to an offline server, and then run setup.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>In this release, most components required for R Server installation are embedded, which means fewer prerequisites have to be downloaded in advance.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The following components are now included in the Windows installer:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Microsoft .NET Core 1.1</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Microsoft MPI 7.1</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>AS OLE DB (SQL Server 2016) provider</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Microsoft R Open 3.3.3</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Microsoft Visual C++ 2013 Redistributable</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Microsoft Visual C++ 2015 Redistributable</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>System requirements</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Operating system must be a <bpt id="p1">[</bpt>supported version of Windows<ept id="p1">](r-server-install-supported-platforms.md)</ept> on a 64-bit with x86-compatible architecture (variously known as AMD64, Intel64, x86-64, IA-32e, EM64T, or x64 chips).</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Itanium chips (also known as IA-64) are not supported.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Multiple-core chips are recommended.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Memory must be a minimum of 2 GB of RAM is required; 8 GB or more are recommended.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Disk space must be a minimum of 500 MB.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>.NET Framework 4.5.2 or later.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Download required components</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Without an internet connection, the following components must be downloaded to a separate device and transferred to the target machine.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Component</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Download Link</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>SRO_3.3.3.0_1033.cab</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Microsoft R Open</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>MLM_9.1.0.0_1033.cab</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Machine learning models</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Download R Server installer</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>You can get the zipped installation file from one of the following download sites.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Site</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Edition</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Visual Studio Dev Essentials</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Developer (free)</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>This option provides a zipped file, free when you sign up for Visual Studio Dev Essentials.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Developer edition has the same features as Enterprise, except it is licensed for development scenarios.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Volume Licensing Service Center (VLSC)</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Enterprise</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Sign in, search for "SQL Server 2016 Enterprise edition", and then choose a per-core or CAL licensing option.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>A selection for <bpt id="p1">**</bpt>R Server for Windows 9.0.1<ept id="p1">**</ept> is provided on this site.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>From <bpt id="p1">[</bpt>Visual Studio Dev Essentials<ept id="p1">](https://www.visualstudio.com/dev-essentials/)</ept>:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Join or access now<ept id="p1">**</ept> to sign up for download benefits.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Check the URL to verify it changed to <bpt id="p1">*</bpt><ph id="ph1">https://my.visualstudio.com/</ph><ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> to search for R Server.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> for a specific version to select the platform.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Download page on Visual Studio benefits page</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Transfer files</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Use a flash drive or another mechanism to transfer the following to the offline server.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>SRO_3.3.3.0_1033.cab</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>MLM_9.1.0.0_1033.cab</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>en_microsoft_r_server_910_for_windows_x64_10324119.zip</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Put the CAB files in the setup user's temp folder: <ph id="ph1">`C:\Users\&lt;user-name&gt;\AppData\Local\Temp`</ph>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Run RServerSetup</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If you previously installed version 9.0.1, it will be replaced with the 9.1 version.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>An 8.x version can run side-by-side 9.x, unaffected by the new installation.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Unzip the installation file en_microsoft_r_server_910_for_windows_x64_10324119.zip, navigate to the folder containing RServerSetup.exe, and then run setup.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Double-click <bpt id="p1">**</bpt>RServerSetup.exe<ept id="p1">**</ept> to start the wizard.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>In Configure installation, choose optional components.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Required components are listed, but not configurable.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Optional components include:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>R Server (Standalone)</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Pre-trained Models<ept id="p1">](microsoftml-install-pretrained-models.md)</ept> used for machine learning.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>In an offline installation scenario, you are notified about missing requirements, given a URL for obtaining the CAB files using an internet-connected device, and a folder path for placing the files.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Accept the SQL Server license agreement for R Server <bpt id="p1">&lt;sup&gt;</bpt>1<ept id="p1">&lt;/sup&gt;</ept>, as well as the license agreement for Microsoft R Open.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Optionally, change the home directory for R Server.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>At the end of the wizard, click <bpt id="p1">**</bpt>Install<ept id="p1">**</ept> to run setup.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;sup&gt;</bpt>1<ept id="p1">&lt;/sup&gt;</ept> R Server is licensed as a SQL Server enterprise feature, even though it can be installed independently of SQL Server on a Windows operating system.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>View log files</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Post-installation, you can review log files (RServerSetup_<ph id="ph1">&lt;timestamp&gt;</ph>.log) located in the system temp directory.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>An easy way to get there is typing <ph id="ph1">`%temp%`</ph> as a Run command or search operation in Windows.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Connect and validate</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>R Server runs on demand as a background process, as <bpt id="p1">**</bpt>Microsoft R Engine<ept id="p1">**</ept> in Task Manager.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Server startup occurs when a client application like RTVS or Rgui.exe connects to the server.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>As a verification step, you can connect to the server and execute a few ScaleR functions to validate the installation.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Go to C:\Program Files\Microsoft\R Server\R_SERVER\bin\x64.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Double-click Rgui.exe to start the R Console application.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>At the command line, type <ph id="ph1">`search()`</ph> to show preloaded objects, including the <ph id="ph2">`RevoScaleR`</ph> package.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`print(Revo.version)`</ph> to show the software version.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`rxSummary(~., iris)`</ph> to return summary statistics on the built-in iris sample dataset.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxSummary`</ph> function is from <ph id="ph2">`RevoScaleR`</ph>.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Additionally, run the <bpt id="p1">[</bpt>Administrator Utility<ept id="p1">](../operationalize/configure-use-admin-utility.md)</ept> to configure your R Server for remote access and execution, web service deployment, or multi-server installation.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Enable Remote Connections and Analytic Deployment</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>The server can be used as-is if you install and use an R IDE on the same box, but to benefit from the deployment and consumption of web services with Microsoft R Server, then you must configure R Server after installation to act as a deployment server and host analytic web services.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Possible configurations are a <bpt id="p1">[</bpt>one-box setup<ept id="p1">](operationalize-r-server-one-box-config.md)</ept> or an <bpt id="p2">[</bpt>enterprise setup<ept id="p2">](operationalize-r-server-enterprise-config.md)</ept>.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Doing so also enables remote execution, allowing you to connect to R Server from an R Client workstation and execute code on the server.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>What's Installed with R Server</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>An installation of Microsoft R Server includes the following components.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Component</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Microsoft R Open (MRO)</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>An open-source distribution of the base R language, plus the Intel Math Kernel library (int-mkl).</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>The distribution includes standard libraries, documentation, and tools like R.exe and RGui.exe.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Tools for the standard base R (RTerm, Rgui.exe, and RScript) are under <ph id="ph1">`&lt;install-directory&gt;\bin`</ph>.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Documentation is under <ph id="ph1">`&lt;install-directory&gt;\doc`</ph> and in <ph id="ph2">`&lt;install-directory&gt;\doc\manual`</ph>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>One easy way to open these files is to open <ph id="ph1">`RGui`</ph>, click <bpt id="p1">**</bpt>Help<ept id="p1">**</ept>, and select one of the options.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Microsoft R Server proprietary libraries and script engine</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>MRS packages provide libraries of functions.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>MRS libraries are co-located with R libraries in the <ph id="ph1">`&lt;install-directory&gt;\library`</ph> folder.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Libraries include RevoScaleR, MicrosoftML, mrsdeploy, olapR, RevoPemaR, and others listed in <bpt id="p1">[</bpt>Package Reference<ept id="p1">](../r-reference/introducing-r-server-r-package-reference.md)</ept>.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>On Windows, the default R Server installation directory is <ph id="ph1">`C:\Program Files\Microsoft\R Server\R_SERVER`</ph>.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>R Server is engineered for distributed and parallel processing for all multi-threaded functions, utilizing available cores and disk storage of the local machine.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>R Server also supports the ability to transfer computations to other R Server instances on other platforms through compute context instructions.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Admin tool</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Used for enabling remote execution and web service deployment, operationalizing analytics, and configuring web and compute nodes.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Pretrained models</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Used for sentiment analysis and image featurization.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Consider adding a development tool on the server to build script or solutions using R Server features:</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Visual Studio 2015<ept id="p1">](https://www.visualstudio.com/downloads/)</ept> followed by the <bpt id="p2">[</bpt>R Tools for Visual Studio (RTVS) add-in<ept id="p2">](https://docs.microsoft.com/visualstudio/rtvs/installation)</ept></source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>By default, telemetry data is collected during your usage of R Server.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>To turn this feature off, use the RevoScaleR package function <ph id="ph1">`rxPrivacyControl(FALSE)`</ph>.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>To turn it back on, change the setting to <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Introduction to R Server<ept id="p1">](../what-is-microsoft-r-server.md)</ept> <bpt id="p2">[</bpt>What's New in R Server<ept id="p2">](../whats-new-in-r-server.md)</ept> <bpt id="p3">[</bpt>Supported platforms<ept id="p3">](r-server-install-supported-platforms.md)</ept></source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Known Issues</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Command line installation</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Microsoft R Getting Started Guide</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Configure R Server to operationalize analytics</source>
        </trans-unit></group></body></file></xliff>