<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-install-on-windows.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335b3eec7c4914c195e93c21c47a17c133d21a015eb.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">b3eec7c4914c195e93c21c47a17c133d21a015eb</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-install-on-windows.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install DeployR for Microsoft R Server 2016 on Windows - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to install, migrate, and configure DeployR</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>install, installation, DeployR, configuration, configure</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Installing DeployR for Microsoft R Server 2016 (8.0.5) on Windows</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Before You Begin</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Read and follow these points before you begin the installation process.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If you already have a version of DeployR installed, follow the <bpt id="p1">[</bpt>migration instructions<ept id="p1">](#migrate)</ept> first.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>We highly recommend installing DeployR on a dedicated machine.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Always install the DeployR main server first before any grid nodes.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>While it is technically possible to run instances of two different versions of DeployR side-by-side on a single machine, we strongly recommend that you dedicate one machine for each server instance that is <bpt id="p1">*</bpt>in production<ept id="p1">*</ept> so as to avoid resource contention.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>System Requirements</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Verify that the computer meets the following minimum hardware and software requirements.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><bpt id="p1">_</bpt>Table: System Requirements<ept id="p1">_</ept></source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>System<ph id="ph1">&amp;nbsp;</ph>Requirement</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Operating Systems</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Windows Server 2012, Windows Server 2016</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;small&gt;</bpt>(64-bit processor only)<ept id="p1">&lt;/small&gt;</ept></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Hardware</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Intel Pentium®-class processor; 3.0 GHz recommended</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Free disk space</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>250+ GB recommended</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>RAM</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>4+ GB recommended</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Java JVM heap size</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>1+ GB in production</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Swap space</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>8+ GB for larger data sets</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Internet access</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>To download DeployR and any dependencies, interact with the Repository Manager, Administration Console, API Explorer Tool.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Installing Dependencies</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The following dependencies are required before you can install the DeployR main server machine or any additional grid node.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>DeployR Enterprise depends on the manual installation and configuration of these dependencies.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Dependency Name</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>DeployR Server</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>DeployR Grid Node</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Microsoft R Server 2016 and its dependencies</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Yes</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Yes</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>DeployR Rserve 8.0.5 (installed for you)</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Yes</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Yes</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Java™ Runtime Environment 8 (64-bit)</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Yes</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>No</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To install the required dependencies for DeployR Enterprise:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>On the DeployR server, <bpt id="p1">[</bpt>download<ept id="p1">](http://go.microsoft.com/fwlink/?LinkId=789397)</ept> and install <bpt id="p2">**</bpt>Java™ Runtime Environment 8<ept id="p2">**</ept>, <ph id="ph1">`jre-8u&lt;NUMBER&gt;-windows-x64.exe`</ph>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Java is only required on the DeployR server, not on any grid node machines.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Download <bpt id="p1">**</bpt><bpt id="p2">[</bpt>SQL Server 2016 and R Server (standalone)<ept id="p2">](https://aka.ms/eval-sql-server-2016 )</ept><ept id="p1">**</ept>, which includes ScaleR for multi-processor and big data support.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Then, follow <bpt id="p1">[</bpt>the instructions<ept id="p1">](https://msdn.microsoft.com/en-us/library/mt695941.aspx)</ept> provided with R Server to install it as well as any of its dependencies.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source><bpt id="p1">_</bpt>If you have internet access<ept id="p1">_</ept> while installing DeployR, the DeployR installation setup will attempt to install the DeployR Rserve dependency for you.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source><bpt id="p1">_</bpt>If you are installing while offline<ept id="p1">_</ept>, you will have to <bpt id="p2">[</bpt>download and install DeployR Rserve 8.0.5<ept id="p2">](https://github.com/Microsoft/deployr-rserve/releases)</ept> manually as <bpt id="p3">[</bpt>described here<ept id="p3">](deployr-admin-diagnostics-troubleshooting.md#manual-package-install)</ept>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Installing DeployR Server</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The basic installation of DeployR will install the DeployR main server after which you can also install additional <bpt id="p1">[</bpt>grid nodes<ept id="p1">](#gridnodes)</ept> for optimized workload distribution.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>After installing the <bpt id="p1">[</bpt>prerequisites<ept id="p1">](#depend)</ept> above, install DeployR as follows:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To install the DeployR Server:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>If you need to disable your anti-virus software to complete the DeployR installation process, then turn it back on as soon as you are finished.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Log in as a user with administrator rights.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Get the DeployR installer file.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>From Microsoft Volume Licensing Service Center (VLSC):</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Once you've signed the license purchase agreement with Microsoft, you'll get your credentials.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Log in and search for <bpt id="p1">**</bpt>SQL Server 2016 Enterprise Edition<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>In the product page, click <bpt id="p1">**</bpt>Continue<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Download the <bpt id="p1">**</bpt>SQL Server Enterprise Edition 2016 DeployR 64-Bit<ept id="p1">**</ept> ISO file.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Double-click the ISO file to mount it as a DVD drive.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Then, select and run <ph id="ph1">`DeployR-Enterprise-8.0.5.exe`</ph>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>From MSDN:</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Log into <bpt id="p1">[</bpt>MSDN subscriptions<ept id="p1">](http://msdn.microsoft.com/subscriptions/downloads)</ept> or <bpt id="p2">[</bpt>Technet<ept id="p2">]( 
http://technet.microsoft.com/subscriptions/downloads)</ept>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Search for <bpt id="p1">**</bpt>DeployR<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Download the ZIP file.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Extract the files.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>From Visual Studio Dev Essentials:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Log into <bpt id="p1">[</bpt>Visual Studio Dev Essentials<ept id="p1">](https://myprodscussu1.app.vssubscriptions.visualstudio.com/Downloads)</ept>.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Search for <bpt id="p1">**</bpt>Microsoft R Server<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Download the DeployR for SQL Server Enterprise Edition ZIP file.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Extract the files.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Launch the <ph id="ph1">`DeployR-Enterprise-8.0.5.exe`</ph> installer and follow the onscreen prompts to complete the installation.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Troubleshooting:<ept id="p1">**</ept> During installation, certain details (and/or errors) are written to the following log files under the <ph id="ph1">`%temp%`</ph> directory: <ph id="ph2">`DeployR-configuration.log`</ph>, <ph id="ph3">`DeployR-dependencies.log`</ph>, and <ph id="ph4">`DeployR-Enterprise-8.0.5.log`</ph>.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>You can also learn about other diagnostic and troubleshooting topics <bpt id="p1">[</bpt>here<ept id="p1">](deployr-admin-diagnostics-troubleshooting.md#troubleshooting)</ept>.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Review and follow these critical <bpt id="p1">[</bpt>post-installation steps<ept id="p1">](#postinstall)</ept>.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>You will not be able to log into the server until you set a password.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Post Installation Steps</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>The following steps outline what you need to do after running the DeployR installer.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Set the administrator's password<ept id="p1">**</ept> so you can log into the server and its landing page.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Launch the DeployR Administrator Utility script with <bpt id="p1">**</bpt>administrator privileges<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option to set a password for the local DeployR <ph id="ph1">`admin`</ph> account.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Enter a password for this account.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Passwords must be <bpt id="p1">**</bpt>8-16 characters<ept id="p1">**</ept> long and contain at least 1 or more uppercase character(s), 1 or more lowercase character(s), 1 or more number(s), <bpt id="p2">**</bpt>and<ept id="p2">**</ept> 1 or more special character(s).</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Confirm the password.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Log into the DeployR landing page<ept id="p1">**</ept> as <ph id="ph1">`admin`</ph> to test your newly defined password at <ph id="ph2">`http://&lt;DEPLOYR_SERVER_IP&gt;:8050/deployr/landing`</ph>.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>At this point, you will only be able to login locally using <ph id="ph1">`localhost`</ph>.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>You will be able to login remotely only once you've <bpt id="p1">[</bpt>configure public access<ept id="p1">](#configuring-public-access)</ept> in a later step in this section.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>[Optional] <bpt id="p1">**</bpt>Set up any grid nodes.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>If desired, install and configure any <bpt id="p1">[</bpt>additional grid nodes<ept id="p1">](#gridnodes)</ept>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>[Optional] If you want to <bpt id="p1">[</bpt>use non-default port numbers for DeployR<ept id="p1">](deployr-admin-diagnostics-troubleshooting.md#changeport)</ept>, manually update them now.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>[Optional] If you want to <bpt id="p1">**</bpt>use a SQL Server database<ept id="p1">**</ept> locally or remotely instead of the default local H2 database, configure that as <bpt id="p2">[</bpt>described here<ept id="p2">](#sqlserver)</ept>.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>[Optional] If you need to <bpt id="p1">**</bpt>provision DeployR on Azure or AWS<ept id="p1">**</ept> as described in <bpt id="p2">[</bpt>these steps<ept id="p2">](deployr-admin-install-in-cloud.md)</ept>.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>To <bpt id="p1">**</bpt>make DeployR accessible to remote users<ept id="p1">**</ept>, <bpt id="p2">[</bpt>update the inbound firewall rules<ept id="p2">](#updating-your-firewall)</ept>.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Run diagnostic tests<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Test the install by running the full <bpt id="p1">[</bpt>DeployR diagnostic tests<ept id="p1">](deployr-admin-diagnostics-troubleshooting.md#diagnostic-testing)</ept>.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>If there are any issues, you must solve them before continuing.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Consult the <bpt id="p1">[</bpt>Troubleshooting section<ept id="p1">](deployr-admin-diagnostics-troubleshooting.md)</ept> for additional help or post questions to our <bpt id="p2">[</bpt>DeployR Forum<ept id="p2">](http://go.microsoft.com/fwlink/?LinkID=708535)</ept>.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Review security documentation<ept id="p1">**</ept> and consider <bpt id="p2">**</bpt>enabling HTTPs<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Learn more by reading the <bpt id="p1">[</bpt>Security Introduction<ept id="p1">](deployr-security.md)</ept> and the <bpt id="p2">[</bpt>Enabling HTTPs<ept id="p2">](../operationalize/configure-https.md)</ept> topic.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>We strongly recommended that SSL/HTTPS be enabled in <bpt id="p1">**</bpt><bpt id="p2">_</bpt>all production environments<ept id="p2">_</ept><ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Check the web context<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>If the wrong IP was detected during installation, <bpt id="p1">[</bpt>update that Web context<ept id="p1">](#configuring-public-access)</ept> now.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Get DeployR client-side developer tools<ept id="p1">**</ept>, including the <bpt id="p2">[</bpt>RBroker framework and client libraries<ept id="p2">](deployr-tools-and-samples.md)</ept>.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Create accounts for your users<ept id="p1">**</ept> in the <bpt id="p2">[</bpt>Administration Console<ept id="p2">](deployr-admin-console-user-accounts.md)</ept>.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Then, provide each user with their username and password as well as the address of the DeployR landing page.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Learn more<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Read the <bpt id="p1">[</bpt>Administrator Getting Started<ept id="p1">](deployr-administrator-getting-started.md)</ept> guide.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>You can also read and share the <bpt id="p1">[</bpt>Data Scientist Getting Started<ept id="p1">](deployr-data-scientist-getting-started.md)</ept> and the <bpt id="p2">[</bpt>Application Developer Getting Started<ept id="p2">](deployr-application-developer-getting-started.md)</ept> guides.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Configuring DeployR</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>For the best results, complete these configuration topics in the order in which they are presented.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Updating Your Firewall</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>During installation, the Windows firewall was automatically updated with several new inbound rules for  inbound communications to DeployR.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>For your security, those inbound rules are disabled by default and set to a <ph id="ph1">`Private`</ph> profile.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To make DeployR accessible to remote users:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Edit the inbound rules in the Windows Firewall.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>In the Properties dialog, enable each rule.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>In the Advanced tab of that dialog, set the profile to <ph id="ph1">`Public`</ph> or <ph id="ph2">`Domain`</ph>.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Machine</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Default Ports</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Open Ports</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>DeployR server machine</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Tomcat ports:</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source><ph id="ph1">- </ph><ph id="ph2">`8050`</ph> (Tomcat default port)</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source><ph id="ph1">- </ph><ph id="ph2">`8051`</ph> (Tomcat HTTPS port)</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>To the outside</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>DeployR server machine</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Event Console port:</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source><ph id="ph1">-</ph><ph id="ph2"> `8056`</ph><ph id="ph3"> </ph>(DeployR event console port)</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>To the public IP of DeployR server AND to the public IP of <bpt id="p1">*</bpt>each<ept id="p1">*</ept> grid node machine</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Remote grid node machines</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>RServe ports:</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source><ph id="ph1">- </ph><ph id="ph2">`8054`</ph> (RServe connection port)</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source><ph id="ph1">- </ph><ph id="ph2">`8055`</ph> (RServe cancel port)</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>To the public IP of the DeployR server</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>If any of the following cases exist, update your firewall manually:</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Whenever you want DeployR to be accessible from another machine, edit the rules as described above in this topic.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Whenever you use <bpt id="p1">**</bpt>non-default port numbers<ept id="p1">**</ept> for communications between DeployR and its dependencies, add those port numbers instead of those in the table above.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>If connecting to a <bpt id="p1">**</bpt>remote database<ept id="p1">**</ept>, be sure to open the database port to the public IP of the DeployR server.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>If defining NFS ports for <bpt id="p1">**</bpt>external directory support<ept id="p1">**</ept>, see the Configuration section of the <bpt id="p2">[</bpt>Managing External Directories for Big Data<ept id="p2">](deployr-admin-manage-big-data.md#setting-up-nfs-setup)</ept> guide.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>If provisioning DeployR on a <bpt id="p1">**</bpt>cloud service<ept id="p1">**</ept>, configure endpoints for these ports on your <bpt id="p2">[</bpt>Azure or AWS EC2 instance<ept id="p2">](deployr-admin-install-in-cloud.md)</ept>, or enable port-forwarding for VirtualBox.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>You can change any DeployR ports<ept id="p1">](deployr-admin-diagnostics-troubleshooting.md#changeport)</ept>.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Configuring Public Access</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>When the wrong IP is defined, you will not be able to access to the DeployR landing page or other DeployR components after installation or reboot.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>In some cases, the wrong IP address may be automatically assigned during installation or when the machine is rebooted, and that address may not be the only IP address for this machine or may not be publicly accessible.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>If this case, you must update the server Web context address.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>To fix this issue, you must define the appropriate external server IP address and port number for the <bpt id="p1">**</bpt>Server web context<ept id="p1">**</ept> and disable the autodetection of the IP address.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To make changes to the IP address:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Launch the DeployR administrator utility script with administrator privileges:</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option to configure the Web Context and Security options for DeployR.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>From the sub-menu, enter <ph id="ph1">`A`</ph> to specify a different IP or fully qualified domain name (FQDN).</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Specify the new IP or FQDN.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">[</bpt>Azure or AWS EC2 instances<ept id="p1">](deployr-admin-install-in-cloud.md)</ept> services, set it to the external <bpt id="p2">**</bpt>Public IP<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Confirm the new value.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Note that the IP autodetection will be turned off when you update the IP/FQDN.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Return to the main menu.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>To apply the changes, restart the DeployR server using option <ph id="ph1">`2`</ph> from the main menu.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>Installing DeployR Grid Nodes</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>When you install the DeployR server, one local grid node is installed automatically for you.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>DeployR Enterprise offers the ability to expand your Grid framework for load distribution by installing and configuring additional grid nodes.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>For help in determining the right number of grid nodes for you, refer to the <bpt id="p1">[</bpt>Scale &amp; Throughput<ept id="p1">](deployr-admin-scale-and-throughput.md#tuning-grid-capacity)</ept> document.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Once you have installed and configured one grid node, you can copy the files over from the server that has already been set up over to the next one.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>Always install the main DeployR server first.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>Install each grid node on a separate host machine.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To install DeployR grid nodes:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source><bpt id="p1">_</bpt>After installing<ept id="p1">_</ept> the <bpt id="p2">[</bpt>main DeployR Enterprise server<ept id="p2">](#installserver)</ept>, install each grid node on a separate machine as follows:</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Log into the machine on which you will install the grid node with administrator rights.</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Server 2016 <bpt id="p1">[</bpt>as described here<ept id="p1">](#depend)</ept> on the grid node machine.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>Download the DeployR node installer file, <ph id="ph1">`DeployR-Enterprise-Node-8.0.5.exe`</ph>, which can be found in the Microsoft R Server 2016 package.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Contact technical support<ept id="p1">](https://support.microsoft.com/)</ept> if you cannot find this file.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Launch the installer, <ph id="ph1">`DeployR-Enterprise-Node-8.0.5.exe`</ph>.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>If a message appears onscreen during installation asking whether you want to <bpt id="p1">*</bpt>“allow the following program to make changes to this computer”<ept id="p1">*</ept>, click <bpt id="p2">**</bpt>Continue<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>When the script is complete, press the <bpt id="p1">**</bpt>Enter<ept id="p1">**</ept> key to exit the window.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>Repeat these steps on each machine that will host a remote grid node.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;strong&gt;</bpt>To configure <ph id="ph1">&amp;amp;</ph> validate nodes:<ept id="p1">&lt;/strong&gt;</ept></source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>After installing DeployR Enterprise server and any grid node machines, you must configure these grid nodes as follows:</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Set the proper firewall rules<ept id="p1">](#firewall)</ept> to open the RServe ports ONLY to the public IP of the DeployR server.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>Log into the DeployR landing page as <ph id="ph1">`admin`</ph> at <ph id="ph2">`http://&lt;DEPLOYR_SERVER_IP&gt;:8050/deployr/landing`</ph> where <ph id="ph3">`&lt;DEPLOYR_SERVER_IP&gt;`</ph> is the IP of the main DeployR server.</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>Go to the <bpt id="p1">**</bpt>Administration Console<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>The Grid<ept id="p1">**</ept> in the main menu.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>For each remote grid node you installed earlier, do the following: (You do not need to configure the DeployR Default Node.)</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>New Grid Node<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>Configure the <bpt id="p1">**</bpt>Name<ept id="p1">**</ept>, <bpt id="p2">**</bpt>Host<ept id="p2">**</ept>, <bpt id="p3">**</bpt>Operating Type<ept id="p3">**</ept> and <bpt id="p4">**</bpt>External Directory<ept id="p4">**</ept> <ph id="ph1">&amp;nbsp;</ph><bpt id="p5">[</bpt>using these instructions<ept id="p5">](deployr-admin-managing-the-grid.md#creating-new-nodes)</ept>.</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>When you try to add that new grid node configuration, DeployR will attempt to validate your settings.</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more...<ept id="p1">](deployr-admin-managing-the-grid.md#node-validation-and-errors)</ept></source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>Run a diagnostic test of each grid node individually as follows:</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>Enable <bpt id="p1">**</bpt>only<ept id="p1">**</ept> that node in the main <bpt id="p2">**</bpt>The Grid<ept id="p2">**</ept> tab.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>Return to the landing page to run the <bpt id="p1">[</bpt>diagnostic check<ept id="p1">](deployr-admin-diagnostics-troubleshooting.md#diagnostic-testing)</ept>.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>Consult the <bpt id="p1">[</bpt>Troubleshooting section<ept id="p1">](deployr-admin-diagnostics-troubleshooting.md)</ept> for help.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>Repeat these steps for each grid node.</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>Remember to go back and enable all the grid nodes you want to use when you are done testing.</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>Using a SQL Server Database</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>During the installation of DeployR, a local H2 database is automatically installed and configured for you.</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>After installing DeployR, <bpt id="p1">**</bpt>but before using it<ept id="p1">**</ept>, you can configure DeployR to use a database in <bpt id="p2">**</bpt>SQL Server Professional, Standard, or Express Version 2012 or greater<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>If you want to use a local or remote SQL Server database for DeployR instead of the default local H2 database, you'll need to:</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>Install and configure SQL Server as described for that product.</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>Log into the SQL Server Management Studio.</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>Create a database with the name <ph id="ph1">`deployr`</ph> and an instance called <ph id="ph2">`DEPLOYREXPRESS`</ph>.</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>For help with creating that database, visit: <ph id="ph1">https://technet.microsoft.com/en-us/library/ms186312(v=sql.130).aspx</ph></source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>The JDBC drivers are installed with DeployR.</source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>If you are using Windows Authentication for login:</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source>In SQL Server Management Studio and grant permissions to the user <ph id="ph1">`NT SERVICE\Apache-Tomcat-for-DeployR-&lt;X.Y.Z._VERSION_NUMBER&gt;`</ph>.</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>In the Object Explorer pane, right click <bpt id="p1">**</bpt>Security <ph id="ph1">&amp;gt;</ph> Logins<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>Login</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Login - New<ept id="p1">**</ept> dialog, enter <ph id="ph1">`NT SERVICE\Apache-Tomcat-for-DeployR-&lt;X.Y.Z._VERSION_NUMBER&gt;`</ph>, where <ph id="ph2">`&lt;X.Y.Z._VERSION_NUMBER&gt;`</ph> is the three digit number DeployR version number, such as <ph id="ph3">`NT SERVICE\Apache-Tomcat-for-DeployR-8.0.5`</ph> into the <bpt id="p2">**</bpt>Login name<ept id="p2">**</ept> field.</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>Login</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>Choose the <bpt id="p1">**</bpt>Server Roles<ept id="p1">**</ept> page on the left and select the checkboxes for <ph id="ph1">`public`</ph>.</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>Choose the <bpt id="p1">**</bpt>User Mapping<ept id="p1">**</ept> page on the left and select the checkbox for the database for DeployR, which in our example is called <ph id="ph1">`deployr`</ph> and for the Database role member, select <ph id="ph2">`db_owner`</ph> and <ph id="ph3">`public`</ph>.</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source>Choose the <bpt id="p1">**</bpt>Status<ept id="p1">**</ept> page on the left and <bpt id="p2">**</bpt>Grant<ept id="p2">**</ept> permission to connect to database engine and choose <bpt id="p3">**</bpt>Enabled<ept id="p3">**</ept> login.</source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept> to create the new login.</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Stop the DeployR server<ept id="p1">](deployr-common-administration-tasks.md#startstop)</ept>.</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>Update the database properties to point to the new database as follows:</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source>Open the <ph id="ph1">`$DEPLOYR_HOME\deployr\deployr.groovy`</ph> file, which is the DeployR server external configuration file.</source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source>Locate the <ph id="ph1">`dataSource`</ph> property block.</source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source>Replace <bpt id="p1">**</bpt>the entire contents<ept id="p1">**</ept> of the <ph id="ph1">`dataSource`</ph> block with these for your authentication method:</source>
        </trans-unit><trans-unit id="324" translate="yes" xml:space="preserve">
          <source>For Windows authentication:</source>
        </trans-unit><trans-unit id="325" translate="yes" xml:space="preserve">
          <source>For basic authentication:</source>
        </trans-unit><trans-unit id="326" translate="yes" xml:space="preserve">
          <source>If you are unsure of your SQL instance name, please consult with your SQL administrator.</source>
        </trans-unit><trans-unit id="327" translate="yes" xml:space="preserve">
          <source>The default instance name for:</source>
        </trans-unit><trans-unit id="328" translate="yes" xml:space="preserve">
          <source>SQL Server Express is <ph id="ph1">`SQLEXPRESS`</ph></source>
        </trans-unit><trans-unit id="329" translate="yes" xml:space="preserve">
          <source>SQL Server Standard or Professional is <ph id="ph1">`MSSQLEXPRESS`</ph></source>
        </trans-unit><trans-unit id="330" translate="yes" xml:space="preserve">
          <source>If you are using a remote database, use the IP address or FQDN of the remote machine rather than <ph id="ph1">`localhost`</ph>.</source>
        </trans-unit><trans-unit id="331" translate="yes" xml:space="preserve">
          <source>If you are connecting to a remote SQL Server database, be sure to <bpt id="p1">[</bpt>open the database port to the public IP of the DeployR server<ept id="p1">](#firewall)</ept>.</source>
        </trans-unit><trans-unit id="332" translate="yes" xml:space="preserve">
          <source>Test the connection to the database and restart the server as follows:</source>
        </trans-unit><trans-unit id="333" translate="yes" xml:space="preserve">
          <source>Launch the DeployR administrator utility script with administrator privileges:</source>
        </trans-unit><trans-unit id="334" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option <bpt id="p1">**</bpt>Test Database Connection<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="335" translate="yes" xml:space="preserve">
          <source>If there are any issues, you must solve them before continuing.</source>
        </trans-unit><trans-unit id="336" translate="yes" xml:space="preserve">
          <source>Once the connection test passes, return the main menu.</source>
        </trans-unit><trans-unit id="337" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option <bpt id="p1">**</bpt>Start/Stop Server<ept id="p1">**</ept> to restart DeployR-related services.</source>
        </trans-unit><trans-unit id="338" translate="yes" xml:space="preserve">
          <source>Once the DeployR server has been successfully restarted, return the main menu.</source>
        </trans-unit><trans-unit id="339" translate="yes" xml:space="preserve">
          <source>From the main menu, choose option to run the <bpt id="p1">[</bpt>DeployR diagnostic tests<ept id="p1">](deployr-admin-diagnostics-troubleshooting.md#diagnostic-testing)</ept>.</source>
        </trans-unit><trans-unit id="340" translate="yes" xml:space="preserve">
          <source>If there are any issues, you must solve them before continuing.</source>
        </trans-unit><trans-unit id="341" translate="yes" xml:space="preserve">
          <source>Consult the <bpt id="p1">[</bpt>Troubleshooting section<ept id="p1">](deployr-admin-diagnostics-troubleshooting.md)</ept> for additional help or post questions to our <bpt id="p2">[</bpt>DeployR Forum<ept id="p2">](http://go.microsoft.com/fwlink/?LinkID=708535)</ept>.</source>
        </trans-unit><trans-unit id="342" translate="yes" xml:space="preserve">
          <source>Exit the utility.</source>
        </trans-unit><trans-unit id="343" translate="yes" xml:space="preserve">
          <source>Setting Password on Testuser Account</source>
        </trans-unit><trans-unit id="344" translate="yes" xml:space="preserve">
          <source>In addition to the <ph id="ph1">`admin`</ph> account, DeployR is delivered with the <ph id="ph2">`testuser`</ph> account you can use to interact with our examples.</source>
        </trans-unit><trans-unit id="345" translate="yes" xml:space="preserve">
          <source>This account is disabled by default.</source>
        </trans-unit><trans-unit id="346" translate="yes" xml:space="preserve">
          <source>Log in as <ph id="ph1">`admin`</ph> to the DeployR landing page.</source>
        </trans-unit><trans-unit id="347" translate="yes" xml:space="preserve">
          <source>If you haven't set a password for <ph id="ph1">`admin`</ph> user yet, <bpt id="p1">[</bpt>do so now<ept id="p1">](#installserver)</ept>.</source>
        </trans-unit><trans-unit id="348" translate="yes" xml:space="preserve">
          <source>After installing DeployR for Microsoft R Server 2016  and setting the password for the <ph id="ph1">`admin`</ph> user account, you can log into the DeployR landing page.</source>
        </trans-unit><trans-unit id="349" translate="yes" xml:space="preserve">
          <source>The landing page is accessible at <ph id="ph1">`http://&lt;DEPLOYR_SERVER_IP&gt;:8050/deployr/landing`</ph>, where <ph id="ph2">`&lt;DEPLOYR_SERVER_IP&gt;`</ph> is the IP address of the DeployR main server machine.</source>
        </trans-unit><trans-unit id="350" translate="yes" xml:space="preserve">
          <source>Go to the <bpt id="p1">**</bpt>Administration Console<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="351" translate="yes" xml:space="preserve">
          <source>Go to the <bpt id="p1">**</bpt>Users<ept id="p1">**</ept> tab and <bpt id="p2">[</bpt>use these instructions<ept id="p2">](deployr-admin-console-user-accounts.md)</ept> to:</source>
        </trans-unit><trans-unit id="352" translate="yes" xml:space="preserve">
          <source>Enable the <ph id="ph1">`testuser`</ph> account.</source>
        </trans-unit><trans-unit id="353" translate="yes" xml:space="preserve">
          <source>Set a new password for this account.</source>
        </trans-unit><trans-unit id="354" translate="yes" xml:space="preserve">
          <source>Migrating to DeployR for Microsoft R Server 2016</source>
        </trans-unit><trans-unit id="355" translate="yes" xml:space="preserve">
          <source>Please carefully follow these migration instructions to migrate users, R Scripts, projects, other DeployR data as well as to learn how to update/preserve client application files.</source>
        </trans-unit><trans-unit id="356" translate="yes" xml:space="preserve">
          <source>If you want to upgrade or reinstall your version or R or Microsoft R Server 2016, please <bpt id="p1">[</bpt>follow these instructions<ept id="p1">](deployr-admin-configure-reinstall-r.md)</ept>.</source>
        </trans-unit><trans-unit id="357" translate="yes" xml:space="preserve">
          <source>From Previous DeployR Version to DeployR for Microsoft R Server 2016</source>
        </trans-unit><trans-unit id="358" translate="yes" xml:space="preserve">
          <source>The following instructions will walk you through a migration of DeployR 8.0.0 or earlier to DeployR for Microsoft R Server 2016.</source>
        </trans-unit><trans-unit id="359" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Do not uninstall<ept id="p1">**</ept> your older version of DeployR until you have backed up the data you want to keep and completed the data migration.</source>
        </trans-unit><trans-unit id="360" translate="yes" xml:space="preserve">
          <source>Ensure your previous version of DeployR is running and that all users are logged out of the version.</source>
        </trans-unit><trans-unit id="361" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install and configure<ept id="p1">](#installserver)</ept> DeployR for Microsoft R Server 2016 and all its dependencies.</source>
        </trans-unit><trans-unit id="362" translate="yes" xml:space="preserve">
          <source>Ensure that all users are logged out of DeployR for Microsoft R Server 2016 as well.</source>
        </trans-unit><trans-unit id="363" translate="yes" xml:space="preserve">
          <source><bpt id="p1">_</bpt>If the MongoDB database is on a different machine than the one on which you installed DeployR for Microsoft R Server 2016<ept id="p1">_</ept>, then you must copy both <ph id="ph1">`MongoMigration.jar`</ph> and the MongoDB migration tool, <ph id="ph2">`exportMongoDB.bat`</ph>:</source>
        </trans-unit><trans-unit id="364" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>from<ept id="p1">*</ept>: <ph id="ph1">&amp;nbsp;</ph> <ph id="ph2">`C:\Program Files\Microsoft\DeployR-8.0.5\deployr\tools\mongoMigration`</ph></source>
        </trans-unit><trans-unit id="365" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>to<ept id="p1">*</ept>: <ph id="ph1">&amp;nbsp;</ph> <ph id="ph2">`$DEPLOYR_HOME_OLD_VERSION\deployr\tools\mongoMigration`</ph> on the machine running MongoDB</source>
        </trans-unit><trans-unit id="366" translate="yes" xml:space="preserve">
          <source>On the <bpt id="p1">**</bpt>machine running MongoDB<ept id="p1">**</ept>, run <ph id="ph1">`exportMongoDB.bat`</ph>, the DeployR MongoDB migration tool:</source>
        </trans-unit><trans-unit id="367" translate="yes" xml:space="preserve">
          <source>Where <ph id="ph1">`&lt;MongoDB_Database_Password&gt;`</ph> is the password defined in the <ph id="ph2">`grails/mongo/password`</ph> parameter in the <ph id="ph3">`deployr.groovy`</ph> file.</source>
        </trans-unit><trans-unit id="368" translate="yes" xml:space="preserve">
          <source>Download <ph id="ph1">`db_backup.zip`</ph>.</source>
        </trans-unit><trans-unit id="369" translate="yes" xml:space="preserve">
          <source>Restore that data into the DeployR for Microsoft R Server 2016 Administration Console.</source>
        </trans-unit><trans-unit id="370" translate="yes" xml:space="preserve">
          <source>Log into the DeployR for Microsoft R Server 2016 landing page, <ph id="ph1">`http://&lt;DEPLOYR_SERVER_IP&gt;:8050/deployr/landing`</ph>.</source>
        </trans-unit><trans-unit id="371" translate="yes" xml:space="preserve">
          <source>From the landing page, open the Administration Console.</source>
        </trans-unit><trans-unit id="372" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Database<ept id="p1">**</ept> tab, click <bpt id="p2">**</bpt>Restore DeployR Database<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="373" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Database restore<ept id="p1">**</ept> window, select <ph id="ph1">`db_backup.zip`</ph>, the backup file you created a few steps back.</source>
        </trans-unit><trans-unit id="374" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Restore<ept id="p1">**</ept> to restore the database.</source>
        </trans-unit><trans-unit id="375" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>The Grid<ept id="p1">**</ept> tab in the console menu.</source>
        </trans-unit><trans-unit id="376" translate="yes" xml:space="preserve">
          <source>Delete any of the old node configurations since those are version-specific and cannot be reused.</source>
        </trans-unit><trans-unit id="377" translate="yes" xml:space="preserve">
          <source>Grid node configurations will not work after migration due to their dependence on a specific version of DeployR.</source>
        </trans-unit><trans-unit id="378" translate="yes" xml:space="preserve">
          <source>After migrating, you will notice that the old grid configuration has been carried over to the newly installed DeployR version.</source>
        </trans-unit><trans-unit id="379" translate="yes" xml:space="preserve">
          <source>However, since those grid nodes are not compatible with the DeployR server, they appear highlighted in the Administration Console when you first start the server.</source>
        </trans-unit><trans-unit id="380" translate="yes" xml:space="preserve">
          <source>This highlighting indicates that a node is unresponsive.</source>
        </trans-unit><trans-unit id="381" translate="yes" xml:space="preserve">
          <source>We recommend deleting these old grid nodes in the Administration Console the first time you log into the console.</source>
        </trans-unit><trans-unit id="382" translate="yes" xml:space="preserve">
          <source>Preserve and update any JavaScript client application files.</source>
        </trans-unit><trans-unit id="383" translate="yes" xml:space="preserve">
          <source>Before you deploy any JavaScript client application files to DeployR for Microsoft R Server 2016, update the client files so that they use the current version of <ph id="ph1">`jsDeployR`</ph> <bpt id="p1">[</bpt>client library<ept id="p1">](deployr-tools-and-samples.md)</ept>.</source>
        </trans-unit><trans-unit id="384" translate="yes" xml:space="preserve">
          <source>After installation, update your application files to use the latest <bpt id="p1">[</bpt>JavaScript API calls<ept id="p1">](https://microsoft.github.io/js-client-library)</ept>.</source>
        </trans-unit><trans-unit id="385" translate="yes" xml:space="preserve">
          <source>From DeployR for Microsoft R Server 2016 to Another Instance of This Version</source>
        </trans-unit><trans-unit id="386" translate="yes" xml:space="preserve">
          <source>Log into the landing page for the DeployR instance containing the data you wish to migrate.</source>
        </trans-unit><trans-unit id="387" translate="yes" xml:space="preserve">
          <source>After installing DeployR for Microsoft R Server 2016 and setting the password for the <ph id="ph1">`admin`</ph> user account, you can log into the DeployR landing page.</source>
        </trans-unit><trans-unit id="388" translate="yes" xml:space="preserve">
          <source>The landing page is accessible at <ph id="ph1">`http://&lt;DEPLOYR_SERVER_IP&gt;:8050/deployr/landing`</ph>, where <ph id="ph2">`&lt;DEPLOYR_SERVER_IP&gt;`</ph> is the IP address of the DeployR main server machine.</source>
        </trans-unit><trans-unit id="389" translate="yes" xml:space="preserve">
          <source>From the landing page, open the Administration Console.</source>
        </trans-unit><trans-unit id="390" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Database<ept id="p1">**</ept> tab, click <bpt id="p2">**</bpt>Backup DeployR Database<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="391" translate="yes" xml:space="preserve">
          <source>A zip file is created and downloaded to your local machine.</source>
        </trans-unit><trans-unit id="392" translate="yes" xml:space="preserve">
          <source>Then, log into the landing page for the DeployR instance to which you want to migrate the data.</source>
        </trans-unit><trans-unit id="393" translate="yes" xml:space="preserve">
          <source>From the landing page, open the Administration Console.</source>
        </trans-unit><trans-unit id="394" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Database<ept id="p1">**</ept> tab, click <bpt id="p2">**</bpt>Restore DeployR Database<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="395" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Database restore<ept id="p1">**</ept> window, select the backup file you created and downloaded a few steps back.</source>
        </trans-unit><trans-unit id="396" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Restore<ept id="p1">**</ept> to restore the database.</source>
        </trans-unit><trans-unit id="397" translate="yes" xml:space="preserve">
          <source>Uninstalling DeployR</source>
        </trans-unit><trans-unit id="398" translate="yes" xml:space="preserve">
          <source>The following instructions describe how to uninstall DeployR on Windows.</source>
        </trans-unit><trans-unit id="399" translate="yes" xml:space="preserve">
          <source>Remember to uninstall DeployR on both the main server and any other grid node machines.</source>
        </trans-unit><trans-unit id="400" translate="yes" xml:space="preserve">
          <source>Stop the Tomcat and RServe services as <bpt id="p1">[</bpt>described here<ept id="p1">](deployr-common-administration-tasks.md#startstop)</ept>.</source>
        </trans-unit><trans-unit id="401" translate="yes" xml:space="preserve">
          <source>If you are using a SQL Server database for DeployR, then stop the process as described in the documentation for that database.</source>
        </trans-unit><trans-unit id="402" translate="yes" xml:space="preserve">
          <source>Remove DeployR using the Windows instructions for uninstalling a program specific to your version of Windows.</source>
        </trans-unit><trans-unit id="403" translate="yes" xml:space="preserve">
          <source>For example, on Windows 8, choose <bpt id="p1">**</bpt>Control Panel <ph id="ph1">&amp;gt;</ph> Programs &amp; Features <ph id="ph2">&amp;gt;</ph> Uninstall<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="404" translate="yes" xml:space="preserve">
          <source>Look for <bpt id="p1">**</bpt>DeployR for Microsoft R Server 2016<ept id="p1">**</ept> on the main server  and <bpt id="p2">**</bpt>DeployR Node for Microsoft R Server 2016<ept id="p2">**</ept> on the grid node machine.</source>
        </trans-unit><trans-unit id="405" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Manually remove the DeployR install directory<ept id="p1">**</ept>, by default <ph id="ph1">`C:\Program Files\Microsoft\DeployR-8.0.5\`</ph>.</source>
        </trans-unit></group></body></file></xliff>