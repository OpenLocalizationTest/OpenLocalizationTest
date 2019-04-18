<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-linux-offline.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b486b1667df1dd2ad3d777f98fa792551b91cd5d5e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">86b1667df1dd2ad3d777f98fa792551b91cd5d5e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-linux-offline.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Offline install for Microsoft R Server 9.1 for Linux</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to install R Server on Linux without an internet connection</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Offline installation of R Server 9.1 for Linux</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Looking for the latest release? See <bpt id="p2">[</bpt>Machine Learning Server for Linux installation<ept id="p2">](machine-learning-server-linux-offline.md)</ept><ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>By default, installers connect to Microsoft download sites to get required and updated components.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>If firewall restrictions or limits on internet access prevent the installer from reaching these sites, you can download individual components on a computer that has internet access, copy the files to another computer behind the firewall, manually install prerequisites and packages, and then run setup.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>If you previously installed version 9.0.1, it will be replaced with the 9.1 version.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>An 8.x version can run side-by-side 9.x, unaffected by the new installation.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>System requirements</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Operating system must be a <bpt id="p1">[</bpt>supported version of Linux<ept id="p1">](r-server-install-supported-platforms.md)</ept> on a 64-bit with x86-compatible architecture (variously known as AMD64, Intel64, x86-64, IA-32e, EM64T, or x64 chips).</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Itanium chips (also known as IA-64) are not supported.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Multiple-core chips are recommended.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Memory must be a minimum of 2 GB of RAM is required; 8 GB or more are recommended.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Disk space must be a minimum of 500 MB.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>An internet connection.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If you do not have an internet connection, for the instructions for an <bpt id="p1">[</bpt>offline installation<ept id="p1">](r-server-install-linux-offline.md)</ept>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>A package manager (yum for RHEL systems, zypper for SLES systems)</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Root or super user permissions</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The following additional components are included in Setup and required for R Server.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Microsoft R Open 3.3.3</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Microsoft .NET Core 1.1 for Linux (required for mrsdeploy and MicrosoftML use cases)</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Download R Server dependencies</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>From an internet-connected computer, download Microsoft R Open (MRO) and .NET Core for Linux.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>MRO provides the R distribution (base R language and script support) used by R Server.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>R Server setup checks for this specific distribution and won't use alternative distributions.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>MRO can co-exist with other distributions of R on your machine, but additional configuration could be required to make a particular version the default.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Manage an R Server installation on Linux<ept id="p1">](r-server-install-linux-manage-install.md)</ept>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The .NET Core component is required for MicrosoftML (machine learning).</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>It is also required for mrsdeploy, used for remote execution, web service deployment, and configuration of R Server as web node and compute node instances.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Component</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Version</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Download Link</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Notes</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Microsoft R Open</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>3.3.3</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Direct link to microsoft-r-open-3.3.3.tar.gz<ept id="p1">](https://go.microsoft.com/fwlink/?linkid=845297)</ept></source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Use the link provided to get the required component.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Do NOT go to MRAN and download the latest or you could end up with the wrong version.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Microsoft .NET Core</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>1.1</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>.NET Core download site<ept id="p1">](https://www.microsoft.com/net/download/linux)</ept></source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Multiple versions of .NET Core are available.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Be sure to choose from the 1.1.1 (Current) list.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The .NET Core download page for Linux provides gzipped tar files for supported platforms.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>In the Runtime column, click <bpt id="p1">**</bpt>x64<ept id="p1">**</ept> to download a tar.gz file for the operating system you are using.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The file name for .NET Core is <ph id="ph1">`dotnet-&lt;linux-os-name&gt;-x64.1.1.1.tar.gz`</ph>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Download R Server installer</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>You can get the gzipped installation file from one of the following download sites.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Site</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Edition</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Visual Studio Dev Essentials<ept id="p1">](https://go.microsoft.com/fwlink/?LinkId=717968&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Developer (free)</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>This option provides a zipped file, free when you sign up for Visual Studio Dev Essentials.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Developer edition has the same features as Enterprise, except it is licensed for development scenarios.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Volume Licensing Service Center (VLSC)<ept id="p1">](https://go.microsoft.com/fwlink/?LinkId=717966&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Enterprise</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Sign in, search for "SQL Server 2016 Enterprise edition", and then choose a per-core or CAL licensing option.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>A selection for <bpt id="p1">**</bpt>R Server for Linux 9.1<ept id="p1">**</ept> is provided on this site.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>For downloads from <bpt id="p1">[</bpt>Visual Studio Dev Essentials<ept id="p1">](https://www.visualstudio.com/dev-essentials/)</ept>:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Join or access now<ept id="p1">**</ept> to sign up for download benefits.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Check the URL to verify it changed to <bpt id="p1">*</bpt><ph id="ph1">https://my.visualstudio.com/</ph><ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> to search for R Server.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> for a specific version to select the platform.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Download page on Visual Studio benefits page</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Download package dependencies</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>R Server has package dependencies for various platforms.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The list of required packages can be found at <bpt id="p1">[</bpt>Package dependencies for Microsoft R Server<ept id="p1">](r-server-install-linux-hadoop-packages.md)</ept>.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>You can list existing packages in /usr/lib64 to see what is currently installed.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>It's common to have a very large number of packages.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>To zero in on specific packages, you can do a partial string search with this command syntax:  <ph id="ph1">`ls -l /usr/lib64/libpng*`</ph></source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>It's possible your Linux machine already has package dependencies installed.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>By way of illustration, on a few systems, only libpng12 had to be installed.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Transfer files</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Use a tool like <bpt id="p1">[</bpt>SmarTTY<ept id="p1">](http://smartty.sysprogs.com/download/)</ept> or <bpt id="p2">[</bpt>PuTTY<ept id="p2">](http://www.putty.org)</ept> or another mechanism to upload or transfer files to a writable directory, such as <bpt id="p3">**</bpt>/tmp<ept id="p3">**</ept>, on your internet-restricted server.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Files to be transferred include the following:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>any missing packages from the dependency list</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Install package dependencies</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>On the target system which is disconnected from the internet, run <ph id="ph1">`rpm -i &lt;package-name&gt;`</ph> to install any packages that are missing from your system (for example, <ph id="ph2">`rpm -i libpng12-1-2-50-10.el7.x86_64.rpm`</ph>).</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Unpack .NET Core and set symbolic link</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>For an offline installation of .NET Core, manually create its directory path, unpack the distribution, and then set references so that the component can be discovered by other applications.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Log in as root or as a user with super user privileges (<ph id="ph1">`sudo -s`</ph>).</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Switch to the <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept> directory (assuming it's the download location) and execute <ph id="ph1">`ls`</ph> to list the files as a verification step.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>You should see the tar.gz files you transferred earlier.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Make a directory for .NET Core:</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Unpack the .NET Core redistribution into the /opt/dotnet directory:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Set the symbolic link for .NET Core to user directories:</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Unpack MRS distribution and copy MRO</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Next, unpack the R Server distribution and copy the gzipped MRO distribution to the MRS91Linux folder.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Do not unpack MRO yourself.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>The installer looks for a gzipped tar file for MRO.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Unpack the MRS gzipped file.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>A new folder called MRS91Linux is created under /tmp.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>This folder contains files and packages used during setup.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Copy the gzipped MRO tar file to the new MRS91Linux folder containing the installation script (install.sh).</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Run the MRS install script</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>R Server for Linux is deployed by running the install script with no parameters.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>At this point, you could opt for <bpt id="p1">[</bpt>unattended install<ept id="p1">](#unattended)</ept> to bypass EULA prompts.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Switch to the <ph id="ph1">`MRS91Linux`</ph> directory containing the installation script:</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Run the script.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>To include the <bpt id="p1">[</bpt>pre-trained machine learning models for MicrosoftML<ept id="p1">](microsoftml-install-pretrained-models.md)</ept>, append the <ph id="ph1">`-m`</ph> switch.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>When prompted to accept the license terms for Microsoft R Open, click Enter to read the EULA, click <bpt id="p1">**</bpt>q<ept id="p1">**</ept> when you are finished reading, and then click <bpt id="p2">**</bpt>y<ept id="p2">**</ept> to accept the terms.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Repeat the key sequence for EULA acceptance for Microsoft R Server.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Installer output shows the packages and location of the log file.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Verify installation</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>List installed MRS packages:</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>On RHEL: <ph id="ph1">`rpm -qa | grep microsoft`</ph></source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>On Ubuntu: <ph id="ph1">`apt list --installed | grep microsoft`</ph></source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Once you have a package name, you can obtain verbose version information.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>On RHEL: <ph id="ph1">`$ rpm -qi microsoft-r-server-packages-9.1.x86_64`</ph></source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>On Ubuntu: <ph id="ph1">`$ dpkg --status microsoft-r-server-packages-9.1.x86_64`</ph></source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Partial output is as follows (note version 9.1.0):</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Start Revo64</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>As another verification step, run the Revo64 program.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>By default, Revo64 is linked to the /usr/bin directory, available to any user who can log in to the machine:</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>From /Home or any other working directory:</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Run an R function, such as <bpt id="p1">**</bpt>rxSummary<ept id="p1">**</ept> on a dataset.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Many sample datasets, such as the iris dataset, are ready to use because they are installed with the software:</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Output from the iris dataset should look similar to the following:</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>To quit the program, type <ph id="ph1">`q()`</ph> at the command line with no arguments.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Unattended install options</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>You can perform a silent install to bypass prompts during setup.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>In /tmp/MRS91Linux, run the install script with the following parameters:</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Additional flags are available, as follows:</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>flag</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Option</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>-a</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>--accept-eula</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Accept all end user license agreements.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>-d</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>--download-mro</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Download microsoft r open for distribution to an offline system.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>-m</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>--models</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Install Microsoft ML models.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>-r</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>--no-dotnet-core</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Opt out of installing .NET Core (required for mrsdeploy and MicrosoftML)</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>-s</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>--silent</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Perform a silent, unattended install.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>-u</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>--unattended</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Perform an unattended install.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>-h</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>--help</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Print this help text.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Enable Remote Connections and Analytic Deployment</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>The server can be used as-is if you install and use an R IDE on the same box, but to benefit from the deployment and consumption of web services with Microsoft R Server, then you must configure R Server after installation to act as a deployment server and host analytic web services.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Possible configurations are a <bpt id="p1">[</bpt>one-box setup<ept id="p1">](operationalize-r-server-one-box-config.md)</ept> or an <bpt id="p2">[</bpt>enterprise setup<ept id="p2">](operationalize-r-server-enterprise-config.md)</ept>.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>Doing so also enables remote execution, allowing you to connect to R Server from an R Client workstation and execute code on the server.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>What's Installed with R Server</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>The Microsoft R Server setup installs the R base packages and a set of enhanced and proprietary R packages that support parallel processing, improved performance, and connectivity to data sources including SQL Server and Hadoop.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>In contrast with R Client, R Server supports much larger data sets and distributed workloads.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>By default, telemetry data is collected during your usage of R Server.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>To turn this feature off, use the RevoScaleR package function <ph id="ph1">`rxPrivacyControl(FALSE)`</ph>.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>To turn it back on, change the setting to <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Next Steps</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Review the best practices in <bpt id="p1">[</bpt>Manage your R Server for Linux installation<ept id="p1">](r-server-install-linux-manage-install.md)</ept> for instructions on how to set up a local package repository using MRAN or miniCRAN, change file ownership or permissions, set Revo64 as the de facto R script engine on your server.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Introduction to R Server<ept id="p1">](../what-is-microsoft-r-server.md)</ept> <bpt id="p2">[</bpt>What's New in R Server<ept id="p2">](../whats-new-in-r-server.md)</ept> <bpt id="p3">[</bpt>Supported platforms<ept id="p3">](r-server-install-supported-platforms.md)</ept></source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Known Issues<ept id="p1">](../resources-known-issues.md)</ept></source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Microsoft R Getting Started Guide<ept id="p1">](../microsoft-r-getting-started.md)</ept></source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure R Server to operationalize analytics<ept id="p1">](operationalize-r-server-one-box-config.md)</ept></source>
        </trans-unit></group></body></file></xliff>