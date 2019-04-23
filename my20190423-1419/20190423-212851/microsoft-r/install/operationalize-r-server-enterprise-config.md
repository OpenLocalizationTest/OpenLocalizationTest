<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="operationalize-r-server-enterprise-config.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a9b734345bd85238e9a601f09d20d3d0ec2035107.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9b734345bd85238e9a601f09d20d3d0ec2035107</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\operationalize-r-server-enterprise-config.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Configure R Server to operationalize analytics (enterprise) - Microsoft R Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Configure Operationalization for Microsoft R Server, load balancer,</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>setup r server for deployment; install r server for deploying</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Configure R Server to operationalize analytics (Enterprise)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Microsoft R Server 9.x<ept id="p1">**</ept>  <ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph><ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph><ph id="ph7">&amp;nbsp;</ph><ph id="ph8">&amp;nbsp;</ph><ph id="ph9">&amp;nbsp;</ph><ph id="ph10">&amp;nbsp;</ph><ph id="ph11">&amp;nbsp;</ph><ph id="ph12">&amp;nbsp;</ph><ph id="ph13">&amp;nbsp;</ph><ph id="ph14">&amp;nbsp;</ph><ph id="ph15">&amp;nbsp;</ph><ph id="ph16">&amp;nbsp;</ph><bpt id="p2">[</bpt>(Looking for the Machine Learning Server article)<ept id="p2">](../operationalize/configure-machine-learning-server-enterprise.md)</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This article explains how to configure R Server after installation to act as a deployment server and to host analytic web services for operationalization.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>This article describes how to perform an enterprise configuration of these features.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>With an enterprise configuration, you can work with your production-grade data within a scalable, multi-machine setup, and benefit from enterprise-grade security.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Enterprise architecture</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>This configuration includes one or more web nodes, one or more compute nodes, and a database.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Web nodes act as HTTP REST endpoints with which users can interact directly to make API calls.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>These nodes also access the data in the database and send requests to the compute node for processing.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Web nodes are stateless, and therefore, session persistence ("stickiness") is not required.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A single web node can route multiple requests simultaneously.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>However, you must have multiple web nodes to load balance your requests across multiple compute nodes.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Compute nodes are used to execute R code as a session or service.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Each compute node has its own <bpt id="p1">[</bpt>pool of R shells<ept id="p1">](../operationalize/configure-evaluate-capacity.md#pool)</ept> and can therefore execute multiple requests at the same time.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Scaling up compute nodes enables you to have more R execution shells and benefit from load balancing across these compute nodes.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The database.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>While an SQLite 3.7+ database is installed by default, we strongly recommend that you set up a <bpt id="p1">[</bpt>SQL Server (Windows) or PostgreSQL (Linux)<ept id="p1">](../operationalize/configure-remote-database-to-operationalize.md)</ept> database instead.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>In an enterprise configuration, these nodes can be scaled independently.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Scaling up web nodes enables an active-active configuration that allows you to load balance the incoming API requests.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Additionally, if you have multiple web nodes, you must use a <bpt id="p1">[</bpt>SQL Server or PostgreSQL database<ept id="p1">](../operationalize/configure-remote-database-to-operationalize.md)</ept> to share data and web services across web node services.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>For added security, you can <bpt id="p1">[</bpt>configure SSL<ept id="p1">](../operationalize/configure-https.md)</ept> and authenticate against <bpt id="p2">[</bpt>Active Directory (LDAP) or Azure Active Directory<ept id="p2">](../operationalize/configure-authentication.md)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Another configuration, referred to as "one-box", consists of a single web node and a single compute node installed on the same machine.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Learn more about this configuration, <bpt id="p1">[</bpt>here<ept id="p1">](operationalize-r-server-one-box-config.md)</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Enterprise Configuration</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Supported platforms</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The web nodes and compute nodes are supported on:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Windows Server 2012 R2, Windows Server 2016</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Ubuntu 14.04, Ubuntu 16.04,</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>CentOS/RHEL 7.x</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>How to upgrade</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>To replace an older version, you can uninstall the older distribution before installing the new version (there is no in-place upgrade).</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Carefully review the following steps:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Upgrade a compute node</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Before you begin, back up the appsettings.json file on each node.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>You can use this backup if there is an issue during the upgrade.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Uninstall Microsoft R Server 9.0 using the instructions in the article <bpt id="p1">[</bpt>Uninstall Microsoft R Server to upgrade to a newer version<ept id="p1">](r-server-install-uninstall-upgrade.md)</ept>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The uninstall process stashes away a copy of your 9.0 configuration files under this directory so you can seamlessly upgrade to R Server 9.1 in the next step:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>On Windows:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>On Linux:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Server:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>On Windows: follow these instructions <bpt id="p1">[</bpt>Installation steps<ept id="p1">](r-server-install-windows.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](r-server-install-windows-offline.md)</ept></source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>For SQL Server Machine Learning Services, you must also:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Manually install .NET Core 2.0.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Add a registry key called <ph id="ph1">`H_KEY_LOCAL_MACHINE\SOFTWARE\R Server\Path`</ph> with a value of the parent path to the <ph id="ph2">`R_SERVER`</ph> folder (for example, <ph id="ph3">`C:\Program Files\Microsoft SQL Server\140`</ph>).</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>On Linux: follow these instructions <bpt id="p1">[</bpt>Installation steps<ept id="p1">](r-server-install-linux-server.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](r-server-install-linux-offline.md)</ept></source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](../operationalize/configure-admin-cli-launch.md)</ept> with administrator privileges.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The utility checks for any 9.0 configuration files present under the <ph id="ph1">`current`</ph> folder mentioned previously.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option to <bpt id="p1">**</bpt>Configure server<ept id="p1">**</ept> (or in previously releases, Configure R Server for Operationalization).</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>From the submenu, choose the option to <bpt id="p1">**</bpt>Configure a compute node<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>When the script asks you if you'd like to upgrade, enter <ph id="ph1">`y`</ph>.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The node is automatically set up using the configuration you had for R Server 9.0.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>The compute node is now configured.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Repeat these steps for each compute node.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Upgrade a web node</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Before you begin, back up the appsettings.json file on each node.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>You can use this backup if there is an issue during the upgrade.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Uninstall Microsoft R Server 9.0 using the instructions in the article <bpt id="p1">[</bpt>Uninstall Microsoft R Server to upgrade to a newer version<ept id="p1">](r-server-install-uninstall-upgrade.md)</ept>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The uninstall process stashes away a copy of your 9.0 configuration files under this directory so you can seamlessly upgrade to R Server 9.1 in the next step:</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>On Windows:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>On Linux:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Server:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>On Windows: follow these instructions <bpt id="p1">[</bpt>Installation steps<ept id="p1">](r-server-install-windows.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](r-server-install-windows-offline.md)</ept></source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>For SQL Server Machine Learning Services, manually install .NET Core 2.0 and add a registry key called <ph id="ph1">`H_KEY_LOCAL_MACHINE\SOFTWARE\R Server\Path`</ph> with a value of the parent path to the <ph id="ph2">`R_SERVER`</ph> folder, such as <ph id="ph3">`C:\Program Files\Microsoft SQL Server\140`</ph>.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>On Linux: follow these instructions <bpt id="p1">[</bpt>Installation steps<ept id="p1">](r-server-install-linux-server.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](r-server-install-linux-offline.md)</ept></source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](../operationalize/configure-admin-cli-launch.md)</ept> with administrator privileges.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The utility checks to see if any 9.0 configuration files are present under the <ph id="ph1">`current`</ph> folder mentioned previously.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option to <bpt id="p1">**</bpt>Configure server<ept id="p1">**</ept> (or in previously releases, Configure R Server for Operationalization).</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>From the submenu, choose the option to <bpt id="p1">**</bpt>Configure a web node<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>When the script asks you if you'd like to upgrade, enter <ph id="ph1">`y`</ph>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>The node is automatically set up using the configuration you had for R Server 9.0.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Note: You can safely ignore the Python warning during upgrade.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option to <bpt id="p1">**</bpt>Run Diagnostic Tests<ept id="p1">**</ept> to <bpt id="p2">[</bpt>test the configuration<ept id="p2">](../operationalize/configure-run-diagnostics.md)</ept>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Exit the utility.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Your web node is now configured.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Repeat these steps for each web node.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>How to configure for the enterprise</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>For your convenience, <bpt id="p1">[</bpt>Azure Resource Management templates<ept id="p1">](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-overview#template-deployment)</ept> are available to quickly deploy and configure Microsoft R Server for operationalization in Azure.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Get one of <bpt id="p1">[</bpt>these templates on GitHub<ept id="p1">](https://github.com/Microsoft/microsoft-r/tree/master/rserver-arm-templates)</ept>.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Then, learn how to use it with this <bpt id="p1">[</bpt>blog post<ept id="p1">](https://blogs.msdn.microsoft.com/rserver/2017/07/07/set-up-an-auto-scale-environment-to-operationalize-your-r-analytics-with-just-one-click/)</ept>.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>1. Configure a database</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>By default, the web node configuration sets up a local SQLite database.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>We strongly recommend that you use a SQL Server or PostgreSQL database for this configuration to achieve higher availability.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>In fact, you cannot use SQLite database at all if you have multiple web nodes or need a remote database.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>To configure that database, <bpt id="p1">[</bpt>follow these instructions<ept id="p1">](../operationalize/configure-remote-database-to-operationalize.md)</ept>.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>If you intend to configure multiple web nodes, then you <bpt id="p1">**</bpt>must<ept id="p1">**</ept> set up a <bpt id="p2">[</bpt>SQL Server or PostgreSQL database<ept id="p2">](../operationalize/configure-remote-database-to-operationalize.md)</ept> so that data can be shared across web node services.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Choose and configure your database now.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>If you configure a different database later, all data in your current database is lost.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>2. Configure compute nodes</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Side-by-side installations of R Server web nodes and compute nodes are not supported.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>In an enterprise configuration, you can set up one or more compute nodes.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>We highly recommend that you configure each node (compute or web) on its own machine for higher availability.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Server and its dependencies:</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>On Windows</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Follow these instructions: <bpt id="p1">[</bpt>R Server installation steps<ept id="p1">](r-server-install-windows.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](r-server-install-windows-offline.md)</ept></source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>For SQL Server Machine Learning Services, you must manually install .NET Core 2.0 and add a registry key called <ph id="ph1">`H_KEY_LOCAL_MACHINE\SOFTWARE\R Server\Path`</ph> with a value of the parent path to the <ph id="ph2">`R_SERVER`</ph> folder, such as <ph id="ph3">`C:\Program Files\Microsoft SQL Server\140`</ph>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>On Linux</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Follow these instructions: <bpt id="p1">[</bpt>R Server installation steps<ept id="p1">](r-server-install-linux-server.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](r-server-install-linux-offline.md)</ept></source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Additional dependencies for R Server on Linux 9.0.1.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>If you have installed R Server 9.0.1 on Linux, you must add a few symlinks:</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>R Server 9.0.1</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Linux</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>CentOS 7.x</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Ubuntu 14.04</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Ubuntu 16.04</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Symlinks</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>cd /usr/lib64</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>sudo ln -s libpcre.so.1   libpcre.so.0</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>sudo ln -s libicui18n.so.50   libicui18n.so.36</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>sudo ln -s libicuuc.so.50 libicuuc.so.36</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>sudo ln -s libicudata.so.50 libicudata.so.36</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>sudo apt-get install libicu-dev</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>cd /lib/x86_64-linux-gnu</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>ln -s libpcre.so.3 libpcre.so.0</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>ln -s liblzma.so.5 liblzma.so.0</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>cd /usr/lib/x86_64-linux-gnu</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>ln -s libicui18n.so.52 libicui18n.so.36</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>ln -s libicuuc.so.52 libicuuc.so.36</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>ln -s libicudata.so.52 libicudata.so.36</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>cd /lib/x86_64-linux-gnu</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>ln -s libpcre.so.3 libpcre.so.0</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>ln -s liblzma.so.5 liblzma.so.0</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>cd /usr/lib/x86_64-linux-gnu</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>ln -s libicui18n.so.55 libicui18n.so.36</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>ln -s libicuuc.so.55 libicuuc.so.36</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>ln -s libicudata.so.55 libicudata.so.36</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Note:<ept id="p1">**</ept> If there are issues with starting the compute node, see <bpt id="p2">[</bpt>here<ept id="p2">](../operationalize/configure-run-diagnostics.md)</ept>.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](../operationalize/configure-admin-cli-launch.md)</ept> with administrator privileges.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>You can bypass the interactive configuration steps of the node using the argument <ph id="ph1">`-silentcomputenodeinstall`</ph> when launching the administration utility.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>If you choose this method, you can skip the next two steps.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>For R Server 9.1 on Windows, for example, the syntax might be: <ph id="ph1">`dotnet Microsoft.RServer.Utils.AdminUtil\Microsoft.RServer.Utils.AdminUtil.dll -silentcomputenodeinstall`</ph>.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Learn about all command-line switches for this script, <bpt id="p1">[</bpt>here<ept id="p1">](../operationalize/configure-admin-cli-launch.md#switch)</ept>.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option to <bpt id="p1">**</bpt>Configure R Server for Operationalization<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>From the submenu, choose the option to <bpt id="p1">**</bpt>Configure a compute node<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>When the configuration  utility is finished, open port 12805:</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>On Windows: Add an exception to your firewall to open port 12805.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>And, for additional security, you can also restrict communication for a private network or domain using a profile.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>On Linux: If using IPTABLES or equivalent firewall service on Linux, then open port 12805 using <ph id="ph1">`iptables`</ph>  or the equivalent command.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>From the main utility menu, choose the option <bpt id="p1">**</bpt>Stop and start services<ept id="p1">**</ept> and restart the compute node to define it as a service.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>The compute node is now configured.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Repeat these steps for each compute node you want to add.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>3. Configure web nodes</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>In an enterprise configuration, you can set up one or more web nodes.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Note that it is possible to run the web node service from within IIS.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>We highly recommend that you configure each node (compute or web) on its own machine for higher availability.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>On each machine, install the same R Server version you installed on the compute node.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>On Windows: follow these instructions <bpt id="p1">[</bpt>Installation steps<ept id="p1">](r-server-install-windows.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](r-server-install-windows-offline.md)</ept></source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>For SQL Server Machine Learning Services, you must also:</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Manually install .NET Core 2.0.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Add a registry key called <ph id="ph1">`H_KEY_LOCAL_MACHINE\SOFTWARE\R Server\Path`</ph> with a value of the parent path to the <ph id="ph2">`R_SERVER`</ph> folder (for example, <ph id="ph3">`C:\Program Files\Microsoft SQL Server\140`</ph>).</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>On Linux: follow these instructions <bpt id="p1">[</bpt>Installation steps<ept id="p1">](r-server-install-linux-server.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](r-server-install-linux-offline.md)</ept></source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Declare the IP addresses of every compute node with each web node.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Open the configuration file, <ph id="ph1">\&lt;</ph>server-home&gt;/Microsoft.RServer.WebNode/appsettings.json.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>(Find <bpt id="p1">[</bpt><ph id="ph1">\&lt;</ph>server-home&gt;<ept id="p1">](../operationalize/configure-find-admin-configuration-file.md)</ept> for your version.)</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>In the file, search for the section starting with <ph id="ph1">`"BackEndConfiguration": {`</ph> .</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Update the <ph id="ph1">`"Uris": {`</ph> properties to declare each compute node.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>In R Server 9.1, you must specify the Uri for each compute node individually using the <ph id="ph1">`Values`</ph> property and/or specify port ranges (or IP octets) using the <ph id="ph2">`Ranges`</ph> property.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>For example, both of the following snippets result in the same specification of four compute nodes:</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>In R Server 9.0, you must specify the Uri for each compute node individually using the <ph id="ph1">`Values`</ph> property.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>For example, this snippet results in four compute nodes:</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Do not update any other properties in this file at this point.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>These other properties are updated during the compute node configuration.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>Close and save the file.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>Repeat these steps on each web node to declare each compute node.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](../operationalize/configure-admin-cli-launch.md)</ept> with administrator privileges:</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>You can bypass the interactive configuration steps of the node using the argument <ph id="ph1">`-silentwebnodeinstall`</ph> and by defining a password for <bpt id="p1">[</bpt>the local 'admin' account<ept id="p1">](../deployr/../operationalize/configure-authentication.md#local)</ept> when you launch the administration utility.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>If you choose this method, you can skip the next three steps.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>For R Server 9.1 on Windows, for example, the syntax might be: <ph id="ph1">`dotnet Microsoft.RServer.Utils.AdminUtil\Microsoft.RServer.Utils.AdminUtil.dll -silentwebnodeinstall my-password`</ph>.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>Learn about all command-line switches for this script, <bpt id="p1">[</bpt>here<ept id="p1">](../operationalize/configure-admin-cli-launch.md#switch)</ept>.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option to <bpt id="p1">**</bpt>Configure R Server for Operationalization<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>From the submenu, choose the option to <bpt id="p1">**</bpt>Configure a web node<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>When prompted, provide a password for the built-in, local operationalization administrator account called 'admin'.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Later, you can configure R Server to authenticate against  <bpt id="p1">[</bpt>Active Directory (LDAP) or Azure Active Directory<ept id="p1">](../deployr/../operationalize/configure-authentication.md#local)</ept>.</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option to <bpt id="p1">**</bpt>Run Diagnostic Tests<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>Verify the configuration by running <bpt id="p1">[</bpt>diagnostic test<ept id="p1">](../operationalize/configure-run-diagnostics.md)</ept> on each web node.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>From the main utility menu, choose the option <bpt id="p1">**</bpt>Stop and start services<ept id="p1">**</ept> and restart the web node to define it as a service.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Exit the utility.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>For IPTABLES firewall or equivalent service on Linux, allow remote machines to access the web node's public IP using <ph id="ph1">`iptables`</ph> (or the equivalent command) to open port 12800.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>Your web node is now configured.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>Repeat these steps for each web node you want to add.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>R Server uses Kestrel as the web server for its operationalization web nodes.</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>Therefore, if you expose your application to the Internet, we recommend that you review the <bpt id="p1">[</bpt>guidelines for Kestrel<ept id="p1">](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/servers/kestrel)</ept> regarding reverse proxy setup.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>4. Setup enterprise-grade security</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>In production environments, we strongly recommend the following approaches:</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure SSL/TLS<ept id="p1">](../operationalize/configure-https.md)</ept> and install the necessary certificates.</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>Authenticate against <bpt id="p1">[</bpt>Active Directory (LDAP) or Azure Active Directory<ept id="p1">](../operationalize/configure-authentication.md)</ept>.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>For added security, restrict the list of IPs that can access the machine hosting the compute node.</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>5. Provision on the cloud</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>If you are provisioning on a cloud service, then you must also <bpt id="p1">[</bpt>create inbound security rule for port 12800 in Azure<ept id="p1">](https://azure.microsoft.com/en-us/documentation/articles/virtual-machines-windows-classic-setup-endpoints/)</ept> or open the port through the AWS console.</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>This endpoint allows clients to communicate with the R Server's operationalization server.</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>6. Set up a load balancer</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>You can set up the load balancer of your choosing.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>Keep in mind that web nodes are stateless.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>Therefore, session persistence ("stickiness") is NOT required.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>For proper access token signing and verification across your configuration, ensure that the JWT certificate settings are exactly the same for every web node.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>These JWT settings are defined on each web node in the configuration file, appsetting.json.</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>7. Post configuration steps</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Update service ports<ept id="p1">](../operationalize/configure-admin-cli-ports.md)</ept>, if needed.</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Run diagnostic tests<ept id="p1">](../operationalize/configure-run-diagnostics.md)</ept>.</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Evaluate<ept id="p1">](../operationalize/configure-evaluate-capacity.md)</ept> the configuration's capacity.</source>
        </trans-unit></group></body></file></xliff>