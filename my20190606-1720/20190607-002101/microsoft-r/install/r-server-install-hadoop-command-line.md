<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-hadoop-command-line.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c376cb621e27f58946db5bc3c6b16cbb59ea928dd94.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">6cb621e27f58946db5bc3c6b16cbb59ea928dd94</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-hadoop-command-line.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Server 9.1 Command line installation (CDH, HDP, MapR)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Hadoop installation and configuration guide for Microsoft R Server version 9.x</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Command-line installation for R Server 9.1 on Hadoop (CDH, HDP, MapR)</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Looking for the latest release?</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>Machine Learning Server for Hadoop installation<ept id="p1">](machine-learning-server-hadoop-install.md)</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>R Server for Hadoop is supported on Hadoop distributions provided by Cloudera, HortonWorks, and MapR.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>For most users, installing R Server on a cluster involves running the same series of steps on each data node of the cluster.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>A summary of setup tasks is as follows:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Download the installer</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Unpack the distribution</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Run the install script with a -p parameter (for Hadoop)</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Verify the installation</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Repeat on the next data node.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The install script uses an internet connection to download and install missing dependencies, Microsoft R Open (MRO), and the .NET Core for Linux.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If internet connections are restricted, use the alternate <bpt id="p1">[</bpt>offline instructions<ept id="p1">](r-server-install-hadoop-offline.md)</ept> instead.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If you previously installed version 9.0.1, it will be replaced with the 9.1 version.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>An 8.x version can run side-by-side 9.x, unaffected by the new installation.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Recommendations for installation</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>We recommend installing R Server on all data nodes of the cluster to avoid Hadoop queuing up jobs on nodes that don't actually have R Server.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Although the task will eventually get reassigned to a node that has R Server, you will see errors from the worker node and experience unnecessary delay while waiting for the error to resolve.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Microsoft Azure offers virtual machines with Hadoop templates.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If you don't have a Hadoop cluster, you can purchase and provision virtual machines on Azure using templates provided by several vendors.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Sign in to <bpt id="p1">[</bpt>Azure portal<ept id="p1">](https://ms.portal.azure.com)</ept>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>New<ept id="p1">**</ept> in the top left side bar.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>In the search box, type the name of one of these vendors: Cloudera, HortonWorks, and MapR.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Several of these vendors offer sandbox deployments that make it easier to get started.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Installation requirements</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Installation requires administrator permissions and must be performed as a <ph id="ph1">`root`</ph> installation.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Non-root installations are not supported.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>R Server must be installed on at least one master or client node which will serve as the submit node; it should be installed on as many workers as is practical to maximize the available compute resources.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Nodes must have the same version of R Server within the cluster.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Setup checks the operating system and detects the Hadoop cluster, but it doesn't check for specific distributions.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Microsoft R Server works with the Hadoop distributions listed here: <bpt id="p1">[</bpt>Supported platforms<ept id="p1">](r-server-install-supported-platforms.md)</ept></source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Microsoft R Server requires Hadoop MapReduce, the Hadoop Distributed File System (HDFS), and Apache YARN.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Optionally, Spark version 1.6-2.0 is supported for Microsoft R Server 9.x.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>System requirements</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Minimum system configuration requirements for Microsoft R Server are as follows:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Processor:<ept id="p1">**</ept> 64-bit CPU with x86-compatible architecture (variously known as AMD64, Intel64, x86-64, IA-32e, EM64T, or x64 CPUs).</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Itanium-architecture CPUs (also known as IA-64) are not supported.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Multiple-core CPUs are recommended.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Memory:<ept id="p1">**</ept> A minimum of 8 GB of RAM is required for Microsoft R Server; 16 GB or more are recommended.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Hadoop itself has substantial memory requirements; see your Hadoop distribution’s documentation for specific recommendations.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Disk Space:<ept id="p1">**</ept> A minimum of 500 MB of disk space is required on each node for R Server.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Hadoop itself has substantial disk space requirements; see your Hadoop distribution’s documentation for specific recommendations.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Download R Server installer</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Get the zipped RServerSetup installer file from one of the following download sites.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Site</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Edition</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Visual Studio Dev Essentials</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Developer (free)</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>This option provides a zipped file, free when you sign up for Visual Studio Dev Essentials.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Developer edition has the same features as Enterprise, except it is licensed for development scenarios.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Volume Licensing Service Center (VLSC)</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Enterprise</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Sign in, search for R Server for Hadoop.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>A selection for <bpt id="p1">**</bpt>R Server 9.1.0 for Hadoop<ept id="p1">**</ept> is provided on this site.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>For downloads from <bpt id="p1">[</bpt>Visual Studio Dev Essentials<ept id="p1">](https://www.visualstudio.com/dev-essentials/)</ept>:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Join or access now<ept id="p1">**</ept> to sign up for download benefits.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Check the URL to verify it changed to <bpt id="p1">*</bpt><ph id="ph1">https://my.visualstudio.com/</ph><ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> to search for R Server.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> for a specific version to select the platform.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Download page on Visual Studio benefits page</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Unpack the distribution</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Download the software to a writable directory, such as <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept>, unpack the distribution and then run the installation script.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>The distribution includes one installer for Microsoft R Server.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>For a gzipped TAR file, you should unpack the file as follows (be sure you have downloaded the file to a writable directory, such as <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept>):</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Log in as root or a user with super user privileges (<ph id="ph1">`sudo su`</ph>).</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Switch to the <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept> directory (assuming it's the download location)</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Unpack the file:      <ph id="ph1">`[tmp] $ tar zxvf en_microsoft_r_server_910_for_hadoop_x64_10323951.tar.gz`</ph></source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Run the install script</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>The Hadoop component is deployed by running the install script with the <bpt id="p1">**</bpt>-p<ept id="p1">**</ept> parameter, which you can install at the root, or as super user via <ph id="ph1">`sudo`</ph>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Log in as root or as a user with super user privileges (<ph id="ph1">`sudo -s`</ph>).</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Verify system repositories are up-to-date:      [username] $ <ph id="ph1">`sudo yum clean all`</ph></source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Change to the directory to which you mounted or unpacked the installer (for example, /tmp/MRS91Hadoop if you unpacked the tar.gz file):      [username] $ <ph id="ph1">`cd /tmp`</ph> [username tmp] $ <ph id="ph2">`cd MRS91Hadoop`</ph></source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Run the script with the <bpt id="p1">**</bpt>-p<ept id="p1">**</ept> parameter, specifying the Hadoop component.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Optionally, add the pre-trained machine learning models: [username tmp MRS91Hadoop] $</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>When prompted to accept the license terms for Microsoft R Open, click Enter to read the EULA, click <bpt id="p1">**</bpt>q<ept id="p1">**</ept> when you are finished reading, and then click <bpt id="p2">**</bpt>y<ept id="p2">**</ept> to accept the terms.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Repeat the key sequence to accept license terms for Microsoft R Server.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Installer output shows the packages and location of the log file.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Unattended install options</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>You can perform a silent install to bypass prompts during setup.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>In MRS91Hadoop, run the install script with the following parameters:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Additional flags are available, as follows:</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>flag</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Option</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>-a</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>--accept-eula</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Accept all end user license agreements.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>-d</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>--download-mro</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Download microsoft r open for distribution to an offline system.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>-m</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>--models</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Install Microsoft pre-trained machine learning models.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>-p</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>--hadoop</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Install the Hadoop component.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>-r</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>--no-dotnet-core</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Opt out of installing .NET Core (required for mrsdeploy and MicrosoftML)</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>-s</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>--silent</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Perform a silent, unattended install.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>-u</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>--unattended</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Perform an unattended install.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>-h</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>--help</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Print this help text.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Verify installation</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>List installed packages and get package names:      <ph id="ph1">`[MRS91Hadoop] $ yum list \*microsoft\*`</ph></source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Check the version of Microsoft R Open using <ph id="ph1">`rpm -qi`</ph>:      <ph id="ph2">`[MRS91Hadoop] $ rpm -qi microsoft-r-open-mro-3.3.3.x86_64`</ph></source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Check the version of Microsoft R Server:      <ph id="ph1">`[MRS91Hadoop] $ rpm -qi microsoft-r-server-packages-9.1.x86_64`</ph></source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Partial output is as follows (note version 9.1.0):</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>For further verification, check folders and permissions.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Following that, you should run the Revo64 program, a sample Hadoop job, and if applicable, a sample Spark job.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Check folders and permissions</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Each user should ensure that the appropriate user directories exist, and if necessary, create them with the following shell commands:</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>The HDFS directory can also be created in a user’s R session (provided the top-level /user/RevoShare has the appropriate permissions) using the following RevoScaleR commands (substitute your actual user name for "username").</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Run the RevoScaleR commands in a Revo64 session.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Output for each command should be <ph id="ph1">`[1] TRUE`</ph>.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>As part of this process, make sure the base directories /user and /user/RevoShare have <ph id="ph1">`uog+rwx`</ph> permissions as well.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Run programs and sample jobs using sample data</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>The next procedure loads sample data and runs the Revo64 program to further verify the installation.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Send sample data to HDFS.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Start Revo64.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Run a simple local computation.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>This step uses the proprietary Microsoft libraries.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Partial output is as follows (showing the first 4 lines).</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Run a sample local job.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>This step uses the sample dataset and downloads data from HDFS, confirming that your local session can access HDFS.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Paste the following code into your Revo64 session.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Partial output is as follows (showing the last 8 lines).</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Run a sample Hadoop job.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>This step uses the sample dataset to run a Hadoop job.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Paste the following code into your Revo64 session.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>This snippet differs from the previous snippet by the first line.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Partial output is as follows (showing the first 10 lines).</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Run a sample Spark job.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>To quit the program, type <ph id="ph1">`q()`</ph> at the command line with no arguments.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Automate a distributed installation</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>If you have multiple nodes, you can automate the installation across nodes using any distributed shell.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Examples include the following</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>dsh ("Dancer’s shell")</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>pdsh (Parallel Distributed Shell)</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>PyDSH (the Python Distributed Shell)</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>fabric</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Each distributed shell has its own methods for specifying hosts, authentication, and so on, but ultimately all that is required is the ability to run a shell command on multiple hosts.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>If possible, use a distributed shell that provides a top-level copy command, such as the pdcp command that is part of pdsh.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Download Microsoft R Open rpm and the Microsoft R Server installer tar.gz file and copy all to /tmp.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>Mount the IMG file.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>The following commands create a mount point and mount the file to that mount point:</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>For RHEL/CENTOS systems;      tar zxvf MRS80RHEL.tar.gz</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>For SLES systems;      tar zxvf MRS80SLES.tar.gz</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Copy the installer gzipped tar file to a writable directory, such as /tmp:</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>From the mounted img file:      cp /mnt/mrsimage/Microsoft-R-Server-<ph id="ph1">`*`</ph>.tar.gz /tmp</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>From the unpacked tar file:      cp /tmp/MRS80<ph id="ph1">&lt;em&gt;</ph>/Microsoft-R-Server-<ph id="ph2">`&lt;/em&gt;`</ph>.tar.gz /tmp</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>The following commands use pdsh and pdcp to distribute and install Microsoft R Server (ensure that each command is run on a single logical line, even if it spans two lines below due to space constraints; lines beginning with “<ph id="ph1">&amp;gt;</ph>” indicate commands typed into an interactive pdsh session):</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>The following commands use pdsh and pdcp to distribute and install Microsoft R Server:</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Each command must run on a single logical line, even if it spans two lines below due to space constraints.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Lines beginning with <ph id="ph1">`&gt;`</ph> indicate commands typed into an interactive pdsh session.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Enable Remote Connections and Analytic Deployment</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>The server can be used as-is if you install and use an R IDE on the same box, but to benefit from the deployment and consumption of web services with Microsoft R Server, then you must configure R Server after installation to act as a deployment server and host analytic web services.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>Possible configurations are a <bpt id="p1">[</bpt>one-box setup<ept id="p1">](operationalize-r-server-one-box-config.md)</ept> or an <bpt id="p2">[</bpt>enterprise setup<ept id="p2">](operationalize-r-server-enterprise-config.md)</ept>.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Doing so also enables remote execution, allowing you to connect to R Server from an R Client workstation and execute code on the server.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Next Steps</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>Review the following walkthroughs to move forward with using R Server and the RevoScaleR package in Spark and MapReduce processing models.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Practice data import and exploration on Spark</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>Practice data import and exploration on MapReduce</source>
        </trans-unit></group></body></file></xliff>