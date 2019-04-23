<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-hadoop-offline.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338aa354aaf40f4e892afa78e40ed908cd7b23009503.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a354aaf40f4e892afa78e40ed908cd7b23009503</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-hadoop-offline.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Offline install for Microsoft R Server 9.1.0 for Hadoop</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to install R Server on Hadoop without an internet connection</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Offline installation of R Server 9.1 for Hadoop</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>By default, installers connect to Microsoft download sites to get required and updated components.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>If firewall restrictions or limits on internet access prevent the installer from reaching these sites, you can download individual components on a computer that has internet access, copy the files to another computer behind the firewall, manually install prerequisites and packages, and then run setup.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>If you previously installed version 9.0.1, it will be replaced with the 9.1.0 version.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>An 8.x version can run side-by-side 9.x, unaffected by the new installation.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Download R Server dependencies</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>From an internet-connected computer, download Microsoft R Open (MRO) and .NET Core for Linux.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>MRO provides the R distribution (base R language and script support) used by R Server.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>R Server setup checks for this specific distribution and won't use alternative distributions.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>MRO can co-exist with other distributions of R on your machine, but additional configuration could be required to make a particular version the default.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Manage an R Server installation on Linux<ept id="p1">](r-server-install-linux-manage-install.md)</ept>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The .NET Core component is required for MicrosoftML (machine learning).</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>It is also required for mrsdeploy, used for remote execution, web service deployment, and configuration of R Server as web node and compute node instances.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Component</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Version</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Download Link</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Notes</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Microsoft R Open</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>3.3.3</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Direct link to microsoft-r-open-3.3.3.tar.gz</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Use the link provided to get the required component.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Do NOT go to MRAN and download the latest or you could end up with the wrong version.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Microsoft .NET Core</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>1.1</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>.NET Core download site</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Multiple versions of .NET Core are available.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Be sure to choose from the 1.1.1 (Current) list.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The .NET Core download page for Linux provides gzipped tar files for supported platforms.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>In the Runtime column, click <bpt id="p1">**</bpt>x64<ept id="p1">**</ept> to download a tar.gz file for the operating system you are using.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The file name for .NET Core is <ph id="ph1">`dotnet-&lt;linux-os-name&gt;-x64.1.1.1.tar.gz`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Download R Server installer</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>You can get Microsoft R Server (MRS) 9.1.0 for Hadoop from one of the following download sites.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Site</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Edition</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Visual Studio Dev Essentials</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Developer (free)</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>This option provides a zipped file, free when you sign up for Visual Studio Dev Essentials.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Developer edition has the same features as Enterprise, except it is licensed for development scenarios.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Volume Licensing Service Center (VLSC)</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Enterprise</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Sign in, search for "SQL Server 2016 Enterprise edition", and then choose a per-core or CAL licensing option.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>A selection for <bpt id="p1">**</bpt>R Server for Hadoop 9.1.0<ept id="p1">**</ept> is provided on this site.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>For downloads from <bpt id="p1">[</bpt>Visual Studio Dev Essentials<ept id="p1">](https://www.visualstudio.com/dev-essentials/)</ept>:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Join or access now<ept id="p1">**</ept> to sign up for download benefits.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Check the URL to verify it changed to <bpt id="p1">*</bpt><ph id="ph1">https://my.visualstudio.com/</ph><ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> to search for R Server.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> for a specific version to select the platform.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Download page on Visual Studio benefits page</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Download package dependencies</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>R Server has package dependencies for various platforms.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The list of required packages can be found at <bpt id="p1">[</bpt>Package dependencies for Microsoft R Server<ept id="p1">](r-server-install-linux-hadoop-packages.md)</ept>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If the target system is missing any, download the ones you will need.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>You can list existing packages in /usr/lib64 to see what is currently installed.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>It's common to have a very large number of packages.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>You can do a partial string search to filter on specific filenames (such as lib* for files starting with lib.):</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>It's possible your Linux machine already has package dependencies installed.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>By way of illustration, on a few systems, only libpng12 had to be installed.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Transfer files</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Use a tool like <bpt id="p1">[</bpt>SmarTTY<ept id="p1">](http://smartty.sysprogs.com/download/)</ept> or <bpt id="p2">[</bpt>PuTTY<ept id="p2">](http://www.putty.org)</ept> or another mechanism to upload or transfer files to a writable directory, such as <bpt id="p3">**</bpt>/tmp<ept id="p3">**</ept>, on your internet-restricted server.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Files to be transferred include the following:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>any missing packages from the dependency list</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Install package dependencies</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>On the target system which is disconnected from the internet, run <ph id="ph1">`rpm -i &lt;package-name&gt;`</ph> to install any packages that are missing from your system (for example, <ph id="ph2">`rpm -i libpng12-1-2-50-10.el7.x86_64.rpm`</ph>).</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Unpack .NET Core and set symbolic link</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>For an offline installation of .NET Core, manually create its directory path, unpack the distribution, and then set references so that the component can be discovered by other applications.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Log in as root or as a user with super user privileges (<ph id="ph1">`sudo -s`</ph>).</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Switch to the <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept> directory (assuming it's the download location) and execute <ph id="ph1">`ls`</ph> to list the files as a verification step.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>You should see the tar.gz files you transferred earlier.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Make a directory for .NET Core:</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Unpack the .NET Core redistribution into the /opt/dotnet directory:</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Set the symbolic link for .NET Core to user directories:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Unpack MRS distribution and copy MRO</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Next, unpack the R Server distribution and copy the gzipped MRO distribution to the MRS91Hadoop folder.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Do not unpack MRO yourself.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The installer looks for a gzipped tar file for MRO.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Unpack the MRS gzipped file.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>A new folder called MRS91Hadoop is created under /tmp.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>This folder contains files and packages used during setup.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Copy the gzipped MRO tar file to the new MRS91Hadoop folder containing the installation script (install.sh).</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Run the MRS install script</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>R Server for Hadoop is deployed by running the install script with no parameters.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>At this point, you could opt for <bpt id="p1">[</bpt>unattended install<ept id="p1">](#unattended)</ept> to bypass EULA prompts.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Switch to the <ph id="ph1">`MRS91Hadoop`</ph> directory containing the installation script:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Run the script with the <bpt id="p1">**</bpt>-p<ept id="p1">**</ept> parameter, specifying the Hadoop component.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Optionally, add the pre-trained machine learning models.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>When prompted to accept the license terms for Microsoft R Open, click Enter to read the EULA, click <bpt id="p1">**</bpt>q<ept id="p1">**</ept> when you are finished reading, and then click <bpt id="p2">**</bpt>y<ept id="p2">**</ept> to accept the terms.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Repeat EULA acceptance for Microsoft R Server.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Installer output shows the packages and location of the log file.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Verify installation</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>List installed packages and get package names:</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Check the version of Microsoft R Open using <ph id="ph1">`rpm -qi`</ph>:</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Check the version of Microsoft R Server:</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Partial output is as follows (note version 9.1.0):</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Name        : microsoft-r-server-packages-9.0     Relocations: /usr/lib64 Version     : 9.1.0                               Vendor: Microsoft .</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Start Revo64</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>As a verification step, run the Revo64 program.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Switch to the directory containing the executable:</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Start the program:</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Run an R function, such as <bpt id="p1">**</bpt>rxSummary<ept id="p1">**</ept> on a dataset.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Many sample datasets, such as the iris dataset, are ready to use because they are installed with the software:</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Output from the iris dataset should look similar to the following:</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>To quit the program, type <ph id="ph1">`q()`</ph> at the command line with no arguments.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Enable Remote Connections and Analytic Deployment</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>The server can be used as-is if you install and use an R IDE on the same box, but to benefit from the deployment and consumption of web services with Microsoft R Server, then you must configure R Server after installation to act as a deployment server and host analytic web services.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Possible configurations are a <bpt id="p1">[</bpt>one-box setup<ept id="p1">](operationalize-r-server-one-box-config.md)</ept> or an <bpt id="p2">[</bpt>enterprise setup<ept id="p2">](operationalize-r-server-enterprise-config.md)</ept>.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Doing so also enables remote execution, allowing you to connect to R Server from an R Client workstation and execute code on the server.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Next Steps</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Review the following walkthroughs to move forward with using R Server and the RevoScaleR package in Spark and MapReduce processing models.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Practice data import and exploration on Spark</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Practice data import and exploration on MapReduce</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Review the best practices in <bpt id="p1">[</bpt>Manage your R Server for Linux installation<ept id="p1">](r-server-install-linux-manage-install.md)</ept> for instructions on how to set up a local package repository using MRAN or miniCRAN, change file ownership or permissions, set Revo64 as the de facto R script engine on your server.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Supported platforms</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>What's new in R Server</source>
        </trans-unit></group></body></file></xliff>