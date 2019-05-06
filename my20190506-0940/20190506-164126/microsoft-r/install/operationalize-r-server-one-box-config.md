<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="operationalize-r-server-one-box-config.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc77503b74fa9cdc0b2618fbca0328dd0a56e745314681.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">3b74fa9cdc0b2618fbca0328dd0a56e745314681</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\operationalize-r-server-one-box-config.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Configure Microsoft R Server to operationalize analytics (one-box)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Configuration Operationalization for Microsoft R Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>setup r server for deployment; install r server for deploying</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Configuring R Server to operationalize analytics with a one-box configuration</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Microsoft R Server 9.x<ept id="p1">**</ept>  <ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph><ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph><ph id="ph7">&amp;nbsp;</ph><ph id="ph8">&amp;nbsp;</ph><ph id="ph9">&amp;nbsp;</ph><ph id="ph10">&amp;nbsp;</ph><ph id="ph11">&amp;nbsp;</ph><ph id="ph12">&amp;nbsp;</ph><ph id="ph13">&amp;nbsp;</ph><ph id="ph14">&amp;nbsp;</ph><ph id="ph15">&amp;nbsp;</ph><ph id="ph16">&amp;nbsp;</ph><bpt id="p2">[</bpt>(Looking for the Machine Learning Server article)<ept id="p2">](../operationalize/configure-machine-learning-server-one-box.md)</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>To benefit from Microsoft R Server’s deployment and operationalization features, you can configure R Server after installation to act as a deployment server and host analytic web services.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>One-box vs enterprise architectures</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>All configurations have at least a single web node, single compute node, and a database.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Web nodes act as HTTP REST endpoints with which users can interact directly to make API calls.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>These nodes also access the data in the database and send requests to the compute node for processing.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Web nodes are stateless, and therefore, session persistence ("stickiness") is not required.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>A single web node can route multiple requests simultaneously.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>However, you must have multiple web nodes to load balance your requests to multiple compute nodes.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Compute nodes are used to execute R code as a session or service.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Each compute node has its own <bpt id="p1">[</bpt>pool of R shells<ept id="p1">](../operationalize/configure-evaluate-capacity.md#pool)</ept> and can therefore execute multiple requests at the same time.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Scaling up compute nodes enables you to have more R execution shells and benefit from load balancing across these compute nodes.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The database.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>An SQLite 3.7+ database is installed by default, but you can, and in some cases must, <bpt id="p1">[</bpt>use a SQL Server (Windows) or PostgreSQL (Linux)<ept id="p1">](../operationalize/configure-remote-database-to-operationalize.md)</ept> database instead.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>R Server offers two types of configuration for operationalizing analytics and remote execution:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>One-box configuration<ept id="p1">**</ept>: as the name suggests, one web node and one compute node run on a single machine.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Set-up is a breeze.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This configuration is useful when you want to explore what it is to operationalize R analytics using R Server.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>It is perfect for testing, proof-of-concepts, and small-scale prototyping, but might not be appropriate for production usage.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>This configuration is covered in this article.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>One-box configuration</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Enterprise configuration<ept id="p1">**</ept>: a configuration where multiple nodes are configured on multiple machines along with other enterprise features.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>This configuration can be scaled up or down by adding or removing nodes.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Learn more about this setup in the <bpt id="p1">[</bpt>enterprise configuration<ept id="p1">](operationalize-r-server-enterprise-config.md)</ept> article.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>For added security, you can <bpt id="p1">[</bpt>configure SSL<ept id="p1">](../operationalize/configure-https.md)</ept> and authenticate against <bpt id="p2">[</bpt>Active Directory (LDAP) or Azure Active Directory<ept id="p2">](../operationalize/configure-authentication.md)</ept>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Supported platforms</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The web nodes and compute nodes are supported on:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Windows Server 2012 R2, Windows Server 2016</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Ubuntu 14.04, Ubuntu 16.04,</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>CentOS/RHEL 7.x</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>How to upgrade from 9.0 to 9.1</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>To replace an older version of a one-box configuration, you can uninstall the older distribution before installing the new version (there is no in-place upgrade).</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Carefully review the following steps.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Before you begin, back up the appsettings.json file on each node you can restore in the event of an upgrade issue.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If you used the default SQLite database, <ph id="ph1">`deployrdb_9.0.0.db`</ph> in R Server 9.0 and want to persist the data, then you must <bpt id="p1">**</bpt>back up the SQLite database before uninstalling Microsoft R Server<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Make a copy of the database file and put it outside of the Microsoft R Server directory structure.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>(If you are using a SQL Server or PostgreSQL database, you can skip this step.)</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>If you skip this SQLite database backup step and uninstall Microsoft R Server 9.0 first, you cannot retrieve your database data.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Uninstall Microsoft R Server 9.0 using the instructions in the article <bpt id="p1">[</bpt>Uninstall Microsoft R Server to upgrade to a newer version<ept id="p1">](r-server-install-uninstall-upgrade.md)</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The uninstall process stashes away a copy of your 9.0 configuration files under this directory so you can seamlessly upgrade to R Server 9.1 in the next step:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>On Windows:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>On Linux:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If you backed up a SQLite database in Step 1, manually move <ph id="ph1">`deployrdb_9.0.0.db`</ph> under this directory so it can be found during the upgrade:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Windows:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Linux:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>(If you are using a SQL Server or PostgreSQL database, you can skip this step.)</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Server:</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>On Windows: follow these instructions <bpt id="p1">[</bpt>Installation steps<ept id="p1">](r-server-install-windows.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](r-server-install-windows-offline.md)</ept></source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>For SQL Server Machine Learning Services, you must also:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Add a registry key called <ph id="ph1">`H_KEY_LOCAL_MACHINE\SOFTWARE\R Server\Path`</ph> with a value of the parent path to the <ph id="ph2">`R_SERVER`</ph> folder (for example, <ph id="ph3">`C:\Program Files\Microsoft SQL Server\140`</ph>).</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Manually install .NET Core 2.0</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>On Linux: follow these instructions <bpt id="p1">[</bpt>Installation steps<ept id="p1">](r-server-install-linux-server.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](r-server-install-linux-offline.md)</ept></source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](../operationalize/configure-admin-cli-launch.md)</ept> with administrator privileges.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The utility checks to see if any 9.0 configuration files are present under the <ph id="ph1">`current`</ph> folder previously mentioned.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>From the menus, choose <bpt id="p1">**</bpt>Configure server<ept id="p1">**</ept> (or in previously releases, Configure R Server for Operationalization) and then choose <bpt id="p2">**</bpt>Configure for one box<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The configuration script begins.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>When the script asks you if you'd like to upgrade, enter <ph id="ph1">`y`</ph>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The nodes are automatically setup using the configuration you had for R Server 9.0.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Note: You can safely ignore the Python warning during upgrade.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option to <bpt id="p1">**</bpt>Run Diagnostic Tests<ept id="p1">**</ept> to <bpt id="p2">[</bpt>test the configuration<ept id="p2">](../operationalize/configure-run-diagnostics.md)</ept>.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Exit the utility.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Your web and compute nodes are now upgraded and configured as they were in version 9.0.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Repeat these steps for each node.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The entities created by users, specifically web services and <bpt id="p1">[</bpt>snapshots<ept id="p1">](../r/how-to-execute-code-remotely.md#snapshot)</ept>, are tied to their usernames.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>For this reason, you must be careful to prevent changes to the user identifier over time.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Otherwise, pre-existing web services and snapshots cannot be mapped to the users who created them.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>For this reason, we strongly recommend that you DO NOT change the unique LDAP identifier in appsettings.json once users start publishing service or creating snapshots.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>How to perform a one-box configuration</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>For your convenience, <bpt id="p1">[</bpt>Azure Management Resource (ARM) templates<ept id="p1">](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-overview#template-deployment)</ept> are available to quickly deploy and configure Microsoft R Server for operationalization in Azure.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Get one of <bpt id="p1">[</bpt>these templates on GitHub<ept id="p1">](https://github.com/Microsoft/microsoft-r/tree/master/rserver-arm-templates)</ept>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Then, learn how to use it with this <bpt id="p1">[</bpt>blog post<ept id="p1">](https://blogs.msdn.microsoft.com/rserver/2017/05/14/configuring-r-server-to-operationalize-analytics-using-arm-templates/)</ept>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>To configure on a single machine:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Server and any dependencies:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On Windows<ept id="p1">**</ept>: Follow these instructions: <bpt id="p2">[</bpt>R Server installation steps<ept id="p2">](r-server-install-windows.md)</ept><ph id="ph1"> | </ph><bpt id="p3">[</bpt>Offline steps<ept id="p3">](r-server-install-windows-offline.md)</ept></source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On Linux<ept id="p1">**</ept>:  Follow these instructions: <bpt id="p2">[</bpt>R Server installation steps<ept id="p2">](r-server-install-linux-server.md)</ept><ph id="ph1"> | </ph><bpt id="p3">[</bpt>Offline steps<ept id="p3">](r-server-install-linux-offline.md)</ept></source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Additional dependencies for R Server on Linux 9.0.1.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>If you have installed R Server 9.0.1 on Linux, you must add a few symlinks:</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>R Server 9.0.1</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Linux</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>CentOS 7.x</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Ubuntu 14.04</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Ubuntu 16.04</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Symlinks</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>cd /usr/lib64</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>sudo ln -s libpcre.so.1   libpcre.so.0</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>sudo ln -s libicui18n.so.50   libicui18n.so.36</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>sudo ln -s libicuuc.so.50 libicuuc.so.36</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>sudo ln -s libicudata.so.50 libicudata.so.36</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>sudo apt-get install libicu-dev</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>cd /lib/x86_64-linux-gnu</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>ln -s libpcre.so.3 libpcre.so.0</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>ln -s liblzma.so.5 liblzma.so.0</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>cd /usr/lib/x86_64-linux-gnu</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>ln -s libicui18n.so.52 libicui18n.so.36</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>ln -s libicuuc.so.52 libicuuc.so.36</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>ln -s libicudata.so.52 libicudata.so.36</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>cd /lib/x86_64-linux-gnu</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>ln -s libpcre.so.3 libpcre.so.0</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>ln -s liblzma.so.5 liblzma.so.0</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>cd /usr/lib/x86_64-linux-gnu</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>ln -s libicui18n.so.55 libicui18n.so.36</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>ln -s libicuuc.so.55 libicuuc.so.36</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>ln -s libicudata.so.55 libicudata.so.36</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Note:<ept id="p1">**</ept> If there are issues with starting the compute node, see <bpt id="p2">[</bpt>here<ept id="p2">](../operationalize/configure-run-diagnostics.md)</ept>.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](../operationalize/configure-admin-cli-launch.md)</ept> with administrator privileges (Windows) or <ph id="ph1">`root`</ph><ph id="ph2">/ </ph><ph id="ph3">`sudo`</ph> privileges (Linux) so you can begin to configure a one-box setup.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Bypass the interactive configuration steps using the argument <ph id="ph1">`-silentoneboxinstall`</ph> and specifying a password for <bpt id="p1">[</bpt>the local 'admin' account<ept id="p1">](../deployr/../operationalize/configure-authentication.md#local)</ept> when you launch the administration utility.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>If you choose this method, you can skip the next three substeps.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>For R Server 9.1 on Windows, for example, the syntax might be: <ph id="ph1">`dotnet Microsoft.RServer.Utils.AdminUtil\Microsoft.RServer.Utils.AdminUtil.dll -silentoneboxinstall my-password`</ph>.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Learn about all command line switches for this script, <bpt id="p1">[</bpt>here<ept id="p1">](../operationalize/configure-admin-cli-launch.md#switch)</ept>.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Choose the option to <bpt id="p1">**</bpt>Configure server<ept id="p1">**</ept> (or in previously releases, Configure R Server for Operationalization).</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Choose the option to <bpt id="p1">**</bpt>Configure for one box<ept id="p1">**</ept> to set up the web node and compute node onto the same machine.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Do not choose the suboptions <bpt id="p1">**</bpt>Configure a web node<ept id="p1">**</ept> or <bpt id="p2">**</bpt>Configure a compute node<ept id="p2">**</ept> unless you intend to have them on separate machines.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>This multi-machine configuration is described as an <bpt id="p1">[</bpt><bpt id="p2">**</bpt>Enterprise<ept id="p2">**</ept> configuration<ept id="p1">](operationalize-r-server-enterprise-config.md)</ept>.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>When prompted, provide a password for the built-in, local operationalization administrator account called 'admin'.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Return to the main menu of the utility when the configuration ends.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Run a diagnostic test of the configuration<ept id="p1">](../operationalize/configure-run-diagnostics.md)</ept>.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>If on Linux and using the IPTABLES firewall or equivalent service, then use the <ph id="ph1">`iptables`</ph> command (or the equivalent) to open port 12800 to the public IP of the web node so that remote machines can access it.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>R Server uses Kestrel as the web server for its operationalization web nodes.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Therefore, if you expose your application to the Internet, we recommend that you review the <bpt id="p1">[</bpt>guidelines for Kestrel<ept id="p1">](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/servers/kestrel)</ept> regarding reverse proxy setup.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>You are now ready to begin operationalizing your R analytics with R Server.</source>
        </trans-unit></group></body></file></xliff>