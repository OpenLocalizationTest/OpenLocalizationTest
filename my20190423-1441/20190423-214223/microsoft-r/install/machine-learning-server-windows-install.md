<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="machine-learning-server-windows-install.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86e747e90eea7c47d24f180aae912c6aaae1727137.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">e747e90eea7c47d24f180aae912c6aaae1727137</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\machine-learning-server-windows-install.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install Machine Learning Server for Windows</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to install, connect to, and use Machine Learning Server on computers running the Windows operating system.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server for Windows</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies to:  Machine Learning Server 9.2.1 | 9.3</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Machine Learning Server for Windows runs machine learning and data mining solutions written in R or Python in standalone and clustered topologies.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This article explains how to install Machine Learning Server on a standalone Windows server with an internet connection.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>If your server has restrictions on internet access, see <bpt id="p1">[</bpt>offline installation<ept id="p1">](machine-learning-server-windows-offline.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>System requirements</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Operating system must be a <bpt id="p1">[</bpt>supported version of 64-bit Windows<ept id="p1">](r-server-install-supported-platforms.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Operationalization features<ept id="p1">](../what-is-operationalization.md)</ept> (administrator utility, web service deployment, remote sessions (R), web and compute node designations) are supported on Windows Server 2012 R2 or 2016.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>This functionality is not available on a Windows client.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Memory must be a minimum of 2 GB of RAM is required; 8 GB or more are recommended.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Disk space must be a minimum of 500 MB.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>.NET Framework 4.5.2 or later.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The installer checks for this version of the .NET Framework and provides a download link if it's missing.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>A computer restart is required after a .NET Framework installation.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The following additional components are included in Setup and required for Machine Learning Server on Windows.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Microsoft R Open 3.4.3 (if you add R)</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Anaconda 4.2 with Python 3.5 (if you add Python)</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Azure CLI</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Microsoft Visual C++ 2015 Redistributable</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Microsoft MPI 8.1</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>AS OLE DB (SQL Server 2016) provider</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Licensing</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Machine Learning Server is licensed as a SQL Server supplemental feature, even though SQL Server itself is not installed or required on a standalone Machine Learning Server installation.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>On development workstations, you can install the developer edition at no charge.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>For example, if you are learning how to use the RevoScaleR libraries, or developing a solution that is not in production, you would use this edition.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>On production servers where code supports ongoing business operations or is part of a solution you are selling commercially, you will need the enterprise edition.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The enterprise edition of Machine Learning Server for Windows is licensed by the core.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Enterprise licenses are sold in 2-core packs, and you must have a license for every core on the machine.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>For example, on an 8-core server, you would need four 2-core packs.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If you have questions, <bpt id="p1">[</bpt>review the pricing page or contact Microsoft<ept id="p1">](https://www.microsoft.com/sql-server/sql-server-2017-pricing)</ept> for more information.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>When you purchase an enterprise license of Machine Learning Server for Windows, you can install <bpt id="p1">[</bpt>Machine Learning Server for Hadoop<ept id="p1">](machine-learning-server-hadoop-install.md)</ept> for free (5 nodes for each core licensed under enterprise licensing).</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Upgrade existing installations</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If your existing server was configured for <bpt id="p1">[</bpt>operationalization<ept id="p1">](../what-is-operationalization.md)</ept>, follow these alternative steps for upgrade:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Configure Machine Learning Server to operationalize analytics (One-box) &gt; How to upgrade</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure Machine Learning Server to operationalize analytics (Enterprise) &gt; How to upgrade<ept id="p1">](../operationalize/configure-machine-learning-server-enterprise.md#how-to-upgrade)</ept>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>For all other configurations, Setup performs an in-place upgrade over existing installations.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Although the installation path is new (\Program Files\Microsoft\ML Server), when R Server 9.x is present, setup finds R Server at the old path and upgrades it to the new version.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>There is no support for side-by-side installations of older and newer versions, nor is there support for hybrid versions (such as R Server 9.1 and Python 9.3).</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>An installation is either entirely 9.3 or an earlier version.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Download Machine Learning Server installer</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>You can get the zipped installation file from one of the following download sites.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Site</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Edition</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Volume Licensing Service Center (VLSC)</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Enterprise</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Sign in, search for "SQL Server 2017", and then choose a per-core licensing option.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>A selection for <bpt id="p1">**</bpt>Machine Learning Server 9.3<ept id="p1">**</ept> is provided on this site.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Visual Studio Dev Essentials</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Developer (free)</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>This option provides a zipped file, free when you sign up for Visual Studio Dev Essentials.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Developer edition has the same features as Enterprise, except it is licensed for development scenarios.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>For downloads from <bpt id="p1">[</bpt>Visual Studio Dev Essentials<ept id="p1">](https://www.visualstudio.com/dev-essentials/)</ept>:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Join or access now<ept id="p1">**</ept> to sign up for download benefits.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>The Visual Studio page title should include "My Benefits".</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The URL should be changed to <bpt id="p1">*</bpt><ph id="ph1">https://my.visualstudio.com/</ph><ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> and search for <bpt id="p2">*</bpt>Machine Learning Server<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Find the version and click <bpt id="p1">**</bpt>Download<ept id="p1">**</ept> to get the Machine Learning Server installer for Windows.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Download page on Visual Studio benefits page</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>How to install</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>This section walks you through a Machine Learning Server deployment using the standalone Windows installer.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Run Setup</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The setup wizard installs, upgrades, and uninstalls all in one workflow.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Extract the contents of the zipped file.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>On your computer, go to the Downloads folder, right-click <bpt id="p1">**</bpt>en_machine_learning_server_for_windows_x64_.zip<ept id="p1">**</ept> to extract the contents.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Double-click <bpt id="p1">**</bpt>ServerSetup.exe<ept id="p1">**</ept> to start the wizard.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>In Configure installation, choose components to install.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Clearing a checkbox removes the component.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Selecting a checkbox adds or upgrades a component.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Core components<ept id="p1">**</ept> are listed for visibility, but are not configurable.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Core components are required.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>R<ept id="p1">**</ept> adds R Open and the R libraries.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Python<ept id="p1">**</ept> adds Anaconda and the Python libraries.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><bpt id="p2">**</bpt>Pre-trained Models<ept id="p2">**</ept><ept id="p1">](microsoftml-install-pretrained-models.md)</ept> are used for image classification and sentiment detection.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>You can install the models with R or Python, but not as a standalone component.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Accept the license agreement for Machine Learning Server, as well as the license agreements for Microsoft R Open and Anaconda.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>At the end of the wizard, click <bpt id="p1">**</bpt>Install<ept id="p1">**</ept> to run setup.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>By default, telemetry data is collected during your usage of Machine Learning Server.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>To turn this feature on or off, see <bpt id="p1">[</bpt>Opting out of data collection<ept id="p1">](../resources-opting-out.md)</ept>.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Check log files</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>If there were errors during Setup, check the log files located in the system temp directory.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>An easy way to get there is typing <ph id="ph1">`%temp%`</ph> as a Run command or search operation in Windows.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>If you installed all components, your log file list looks similar to this screenshot:</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Machine Learning Server setup log files</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Set environment variables</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Create an <bpt id="p1">**</bpt>MKL_CBWR<ept id="p1">**</ept> environment variable to <bpt id="p2">[</bpt>ensure consistent output<ept id="p2">](https://software.intel.com/articles/introduction-to-the-conditional-numerical-reproducibility-cnr)</ept> from Intel Math Kernel Library (MKL) calculations.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>In Control Panel, click <bpt id="p1">**</bpt>System and Security<ept id="p1">**</ept><ph id="ph1"> &gt; </ph><bpt id="p2">**</bpt>System<ept id="p2">**</ept><ph id="ph2"> &gt; </ph><bpt id="p3">**</bpt>Advanced System Settings<ept id="p3">**</ept><ph id="ph3"> &gt; </ph><bpt id="p4">**</bpt>Environment Variables<ept id="p4">**</ept>.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Create a new User or System variable.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Set variable name to</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Set the variable value to</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>This step requires a server restart.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Connect and validate</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Machine Learning Server executes on demand as R Server or as a Python application.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>As a verification step, connect to each application and run a script or function.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>For R</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>R Server runs as a background process, as <bpt id="p1">**</bpt>Microsoft ML Server Engine<ept id="p1">**</ept> in Task Manager.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Server startup occurs when a client application like <bpt id="p1">[</bpt>R Tools for Visual Studio<ept id="p1">](https://docs.microsoft.com/visualstudio/rtvs/installation)</ept> or Rgui.exe connects to the server.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Go to C:\Program Files\Microsoft\ML Server\R_SERVER\bin\x64.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Double-click <bpt id="p1">**</bpt>Rgui.exe<ept id="p1">**</ept> to start the R Console application.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>At the command line, type <ph id="ph1">`search()`</ph> to show preloaded objects, including the <bpt id="p1">[</bpt>RevoScaleR package<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept>.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`print(Revo.version)`</ph> to show the software version.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`rxSummary(~., iris)`</ph> to return summary statistics on the built-in iris sample dataset.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxSummary`</ph> function is from RevoScaleR.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>For Python</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Python runs when you execute a .py script or run commands in a Python console window.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Go to C:\Program Files\Microsoft\ML Server\PYTHON_SERVER.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Double-click <bpt id="p1">**</bpt>Python.exe<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>At the command line, type <ph id="ph1">`help()`</ph> to open interactive help.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">` revoscalepy`</ph> at the help prompt to print the package contents.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Paste in the following revoscalepy script to return summary statistics from the built-in AirlineDemo demo data:</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Output from the sample dataset should look similar to the following:</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>To quit the program, type <ph id="ph1">`quit()`</ph> at the command line with no arguments.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Verify CLI</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Before you continue, reboot the machine.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Open an Administrator command prompt.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Enter the following command to check availability of the CLI: <ph id="ph1">`az ml admin --help`</ph>.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>If you receive the following error: <ph id="ph1">`az: error argument _command_package: invalid choice: ml`</ph>, follow the <bpt id="p1">[</bpt>instructions to re-add the extension to the CLI<ept id="p1">](https://docs.microsoft.com/en-us/machine-learning-server/resources-known-issues#1-missing-azure-ml-admin-cli-extension-on-dsvm-environments
)</ept>.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Enable web service deployment and remote connections</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>If you installed Machine Learning Server on Windows Server 2012 R2 or Windows Server 2016, <bpt id="p1">[</bpt>configure the server for operationalization<ept id="p1">](../operationalize/configure-start-for-administrators.md#configure-server-for-operationalization)</ept> to enable additional functionality, including logging, diagnostics, and web service hosting.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>You can use the <ph id="ph1">`bootstrap`</ph> command for this step.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>This command enables operationalization features on a standalone server.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>It creates and starts a web node and compute node, and runs a series of diagnostic tests against the configuration to confirm the internal data storage is functional and that web services can be successfully deployed.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>If you have multiple servers, you can designate each one as either a web node or compute node, and then link them up.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>For instructions, see <bpt id="p1">[</bpt>Configure Machine Learning Server (Enterprise)<ept id="p1">](../operationalize/configure-machine-learning-server-enterprise.md)</ept>.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Open an Administrator command prompt.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Enter the following command to configure the server:</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>CLI screenshot</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>This command invokes the Administrator Command Line Interface (CLI), installed by Machine Learning Server and added as a system environment variable to your path so that you can run it anywhere.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Set a password used to protect your configuration settings.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Later, after configuration is finished, anyone who wants to use the CLI to modify a configuration must provide this password to gain access to settings and operations.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>The password must meet these requirements: 8-16 characters long, with at least one upper-case letter, one lower-case letter, one number, and one special character.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>After you provide the password, the tool does the rest.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Your server is fully operationalized once the process is complete.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>For more information about the benefits of operationalization:</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Deploy Python and R script as a web service</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Connect to a remote R server for code execution<ept id="p1">](../r/how-to-execute-code-remotely.md)</ept>.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Remote execution makes the server accessible to client workstations running <bpt id="p1">[</bpt>R Client<ept id="p1">](../r-client/install-on-linux.md)</ept> or other Machine Learning Server nodes on your network.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Python support is new and there are a few limitations in remote computing scenarios.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Remote execution is not supported on Windows or Linux in Python code.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Additionally, you cannot set a <bpt id="p1">[</bpt>remote compute context<ept id="p1">](../r/concept-what-is-compute-context.md)</ept> to HadoopMR in Python.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>What's installed</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>An installation of Machine Learning Server includes some or all of the following components.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Component</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Microsoft R Open (MRO)</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>An open-source distribution of the base R language, plus the Intel Math Kernel library (int-mkl).</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>The distribution includes standard libraries, documentation, and tools like R.exe and RGui.exe.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Tools for the standard base R (RTerm, Rgui.exe, and RScript) are under <ph id="ph1">`&lt;install-directory&gt;\bin`</ph>.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Documentation is under <ph id="ph1">`&lt;install-directory&gt;\doc`</ph> and in <ph id="ph2">`&lt;install-directory&gt;\doc\manual`</ph>.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>One easy way to open these files is to open <ph id="ph1">`RGui`</ph>, click <bpt id="p1">**</bpt>Help<ept id="p1">**</ept>, and select one of the options.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>R proprietary libraries and script engine</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Proprietary libraries are co-located with R base libraries in the <ph id="ph1">`&lt;install-directory&gt;\library`</ph> folder.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Libraries include RevoScaleR, MicrosoftML, mrsdeploy, olapR, RevoPemaR, and others listed in <bpt id="p1">[</bpt>R Package Reference<ept id="p1">](../r-reference/introducing-r-server-r-package-reference.md)</ept>.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>On Windows, the default R installation directory is <ph id="ph1">`C:\Program Files\Microsoft\ML Server\R_SERVER`</ph>.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>RevoScaleR is engineered for distributed and parallel processing of all multi-threaded functions, utilizing available cores and disk storage of the local machine.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>RevoScaleR also supports the ability to transfer computations to other RevoScaleR instances on other platforms and computers through compute context instructions.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Python proprietary libraries</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Proprietary packages provide modules of class objects and static functions.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Python libraries are in the <ph id="ph1">`&lt;install-directory&gt;\lib\site-packages`</ph> folder.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Libraries include revoscalepy, microsoftml, and azureml-model-management-sdk.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>On Windows, the default installation directory is <ph id="ph1">`C:\Program Files\Microsoft\ML Server\PYTHON_SERVER`</ph>.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Anaconda 4.2 with Python 3.5.2</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>An open-source distribution of Python.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>Admin CLI</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Used for enabling remote execution and web service deployment, operationalizing analytics, and configuring web and compute nodes.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Pre-trained models</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>Used for sentiment analysis and image detection.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Consider adding a development tool on the server to build script or solutions using R Server features:</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Visual Studio 2017<ept id="p1">](https://www.visualstudio.com/downloads/)</ept> followed by the <bpt id="p2">[</bpt>R Tools for Visual Studio (RTVS) add-in<ept id="p2">](https://docs.microsoft.com/visualstudio/rtvs/installation)</ept> and the <bpt id="p3">[</bpt>Python for Visual Studio (PTVS)<ept id="p3">](https://www.visualstudio.com/vs/python/)</ept>.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>We recommend starting with any Quickstart tutorial listed in the contents pane.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>What's new in Machine Learning Server</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>Supported platforms</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>Known Issues</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Configure Machine Learning Server to operationalize your analytics</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>R Function Reference</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>Python Function Reference</source>
        </trans-unit></group></body></file></xliff>