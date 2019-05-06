<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="configure-machine-learning-server-enterprise-9-2.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc77503ec647d1839156f92ffbf1f1c4e4e4a304d2acb8.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">3ec647d1839156f92ffbf1f1c4e4e4a304d2acb8</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\configure-machine-learning-server-enterprise-9-2.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Configure Machine Learning Server 9.2.1 to operationalize analytics (Enterprise)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Configure Machine Learning Server 9.2.1 to operationalize analytics (Enterprise setup) with load balancing</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>setup machine learning server for deployment; install machine learning server for deploying</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Configure Machine Learning Server 9.2.1 to operationalize analytics (Enterprise)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: Machine Learning Server 9.2.1<ept id="p1">**</ept> <ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph><ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph><ph id="ph7">&amp;nbsp;</ph><ph id="ph8">&amp;nbsp;</ph><ph id="ph9">&amp;nbsp;</ph><ph id="ph10">&amp;nbsp;</ph><ph id="ph11">&amp;nbsp;</ph><ph id="ph12">&amp;nbsp;</ph><ph id="ph13">&amp;nbsp;</ph><ph id="ph14">&amp;nbsp;</ph><ph id="ph15">&amp;nbsp;</ph><ph id="ph16">&amp;nbsp;</ph><ph id="ph17">&amp;nbsp;</ph><ph id="ph18">&amp;nbsp;</ph><ph id="ph19">&amp;nbsp;</ph><ph id="ph20">&amp;nbsp;</ph><ph id="ph21">&amp;nbsp;</ph><ph id="ph22">&amp;nbsp;</ph><ph id="ph23">&amp;nbsp;</ph>(See instructions for <bpt id="p2">[</bpt>latest release.)<ept id="p2">](configure-machine-learning-server-enterprise.md)</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>You can configure Microsoft Learning Server after installation to act as a deployment server and to host analytic web services for operationalization.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Machine Learning Server offers two types of configuration for operationalizing analytics and remote execution: <bpt id="p1">**</bpt>One-box and Enterprise<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This article describes the enterprise configuration.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>For more on one-box configurations, <bpt id="p1">[</bpt>see here<ept id="p1">](configure-machine-learning-server-one-box.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>An enterprise configuration involves multiple <bpt id="p1">[</bpt>web and compute nodes<ept id="p1">](../operationalize/configure-start-for-administrators.md#configure-server-for-operationalization)</ept> that  are configured on multiple machines along with other enterprise features.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>These nodes can be scaled independently.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Scaling out web nodes enables an active-active configuration that allows you to load balance the incoming API requests.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Additionally, with multiple web nodes, you must use a <bpt id="p1">[</bpt>SQL Server or PostgreSQL database<ept id="p1">](../operationalize/configure-remote-database-to-operationalize.md)</ept> to share data and web services across web node services.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The web nodes are stateless therefore there is no need for session stickiness if you use a load balancer.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>For added security, you can <bpt id="p1">[</bpt>configure SSL<ept id="p1">](../operationalize/configure-https.md)</ept> and authenticate against <bpt id="p2">[</bpt>Active Directory (LDAP) or Azure Active Directory<ept id="p2">](../operationalize/configure-authentication.md)</ept> in this configuration.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Configure Machine Learning Server on enterprise architecture</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>How to configure</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>For a speedy setup in Azure, try one of <bpt id="p1">[</bpt>our Azure Resource Management templates<ept id="p1">](https://github.com/Microsoft/microsoft-r/tree/master/mlserver-arm-templates)</ept> stored in GitHub.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>This <bpt id="p1">[</bpt>blog post<ept id="p1">](https://blogs.msdn.microsoft.com/rserver/2017/05/14/configuring-r-server-to-operationalize-analytics-using-arm-templates/)</ept> explains how.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>1. Configure a database</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>While the web node configuration sets up a local SQLite database by default, you must use a SQL Server or PostgreSQL database for this configuration for any of the following situations:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Have multiple web nodes (so data can be shared across web nodes)</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Want to achieve higher availability</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Need a remote database for your web node</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>To configure that database, <bpt id="p1">[</bpt>follow these instructions<ept id="p1">](../operationalize/configure-remote-database-to-operationalize.md)</ept>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Choose and configure your database now.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If you configure a different database later, all data in your current database is lost.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>2. Configure compute nodes</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Configure one or more compute nodes as needed.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>We highly recommend that you configure each node (compute or web) on its own machine for higher availability.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>In the Enterprise configuration, side-by-side installations of a web and compute node are not supported.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server and its dependencies as follows.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Learn about supported platforms for this configuration.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Windows instructions: <bpt id="p1">[</bpt>Installation steps<ept id="p1">](../install/machine-learning-server-windows-install.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](../install/machine-learning-server-windows-offline.md)</ept></source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">_</bpt>SQL Server Machine Learning Services<ept id="p1">_</ept>, you must also manually install .NET Core 1.1 and add a registry key called 'H_KEY_LOCAL_MACHINE\SOFTWARE\R Server\Path' with a value of the parent path to the R<ph id="ph1">\_</ph>SERVER or PYTHON<ph id="ph2">\_</ph>SERVER folder (for example, C:\Program Files\Microsoft SQL Server\140).</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Linux instructions: <bpt id="p1">[</bpt>Installation steps<ept id="p1">](../install/machine-learning-server-linux-install.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](../install/machine-learning-server-linux-offline.md)</ept></source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](../operationalize/configure-admin-cli-launch.md)</ept> with administrator privileges.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>From the main utility menu, choose <bpt id="p1">**</bpt>Configure server<ept id="p1">**</ept> and then choose <bpt id="p2">**</bpt>Configure a compute node<ept id="p2">**</ept> from the submenu.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If you plan on configuring SSL/TLS and <bpt id="p1">[</bpt>install the necessary certificates<ept id="p1">](../operationalize/configure-https.md)</ept> on the compute node, do so now.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Open the port 12805 <bpt id="p1">_</bpt>on every compute node<ept id="p1">_</ept>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If you plan to configure SSL/TLS, you must do so BEFORE opening this port.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>On Windows: Add a firewall exception to open the port number.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>On Linux: Use 'iptables' or the equivalent command to open the port number.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>You can now <bpt id="p1">**</bpt>repeat these steps<ept id="p1">**</ept> for each compute node you want to add.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>3. Configure web nodes</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>In an enterprise configuration, you can set up one or more web nodes.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>It is possible to run the web node service from within IIS.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server and its dependencies as follows.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Learn about supported platforms for this configuration.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Windows instructions: <bpt id="p1">[</bpt>Installation steps<ept id="p1">](../install/machine-learning-server-windows-install.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](../install/machine-learning-server-windows-offline.md)</ept></source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">_</bpt>SQL Server Machine Learning Services<ept id="p1">_</ept>, you must also manually install .NET Core 1.1 and add a registry key called 'H_KEY_LOCAL_MACHINE\SOFTWARE\R Server\Path' with a value of the parent path to the R<ph id="ph1">\_</ph>SERVER or PYTHON<ph id="ph2">\_</ph>SERVER folder (for example, C:\Program Files\Microsoft SQL Server\140).</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Linux instructions: <bpt id="p1">[</bpt>Installation steps<ept id="p1">](../install/machine-learning-server-linux-install.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](../install/machine-learning-server-linux-offline.md)</ept></source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](../operationalize/configure-admin-cli-launch.md)</ept> with administrator privileges to configure a web node:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Bypass these interactive steps to install the node and set an admin password using these command-line switches: -silentwebnodeinstall mypassword uri1,uri2 Learn more about command-line switches for this utility <bpt id="p1">[</bpt>here<ept id="p1">](../operationalize/configure-admin-cli-launch.md#switch)</ept>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>From the main menu, choose <bpt id="p1">**</bpt>Configure server<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Then, choose <bpt id="p1">**</bpt>Configure a web node<ept id="p1">**</ept> from the submenu.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>When prompted, provide a password for the built-in, local operationalization administrator account called 'admin'.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Later, you can configure the server to authenticate against  <bpt id="p1">[</bpt>Active Directory (LDAP) or Azure Active Directory<ept id="p1">](../deployr/../operationalize/configure-authentication.md#local)</ept>.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>When prompted, enter the IP address of each compute node you configured.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>You can specify a specific URI or  specify IP ranges.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>For multiple compute nodes, separate each URI with a comma.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>For example: <ph id="ph1">http://1.1.1.1:12805</ph>, <ph id="ph2">http://1.0.1-3.1-2:12805</ph></source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>In this example, the range represents six IP values: 1.0.1.1, 1.0.1.2, 1.0.2.1, 1.0.2.2, 1.0.3.1,  1.0.3.2.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Return the main menu of the utility.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>When configuring your web node, you might see the following message:  "Web Node was not able to start because it is not configured."</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Typically, this is not really an issue since the web node is automatically restarted within 5 minutes by an auto-recovery mechanism.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>In the same utility, test the configuration.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>From the main utility menu, choose <bpt id="p1">**</bpt>Run Diagnostic Tests<ept id="p1">**</ept> and choose a <bpt id="p2">[</bpt>diagnostic test<ept id="p2">](../operationalize/configure-run-diagnostics.md)</ept>.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Exit the utility.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>If you plan on configuring SSL/TLS and <bpt id="p1">[</bpt>install the necessary certificates<ept id="p1">](../operationalize/configure-https.md)</ept> on the compute node, do so now.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Open the port 12800 <bpt id="p1">_</bpt>on every web node<ept id="p1">_</ept>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>If you plan to configure SSL/TLS, you must do so BEFORE opening this port.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>On Windows: Add a firewall exception to open the port number.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>On Linux: Use 'iptables' or the equivalent command to open the port number.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>You can now <bpt id="p1">**</bpt>repeat these steps<ept id="p1">**</ept> for each web node you want to add.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Machine Learning Server uses Kestrel as the web server for its operationalization web nodes.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Therefore, if you expose your application to the Internet, we recommend that you review the <bpt id="p1">[</bpt>guidelines for Kestrel<ept id="p1">](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/servers/kestrel)</ept> regarding reverse proxy setup.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>4. Setup enterprise-grade security</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>In production environments, we strongly recommend the following approaches:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure SSL/TLS<ept id="p1">](../operationalize/configure-https.md)</ept> and install the necessary certificates.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Authenticate against <bpt id="p1">[</bpt>Active Directory (LDAP) or Azure Active Directory<ept id="p1">](../operationalize/configure-authentication.md)</ept>.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>For added security, restrict the list of IPs that can access the machine hosting the compute node.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Important!</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>For proper access token signing and verification across your configuration, ensure that the JWT certificate settings are exactly the same for every web node.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>These JWT settings are defined on each web node in the configuration file, appsetting.json.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>5. Provision on the cloud</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>If you are provisioning on a cloud service, then you must also <bpt id="p1">[</bpt>create inbound security rule for port 12800 in Azure<ept id="p1">](https://azure.microsoft.com/en-us/documentation/articles/virtual-machines-windows-classic-setup-endpoints/)</ept> or open the port through the AWS console.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>This endpoint allows clients to communicate with the  Machine Learning Server's operationalization server.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>6. Set up a load balancer</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>You can set up the load balancer of your choosing.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Keep in mind that web nodes are stateless.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Therefore, session persistence ("stickiness") is NOT required.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>7. Post configuration steps</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Update service ports<ept id="p1">](../operationalize/configure-admin-cli-ports.md)</ept>, if needed.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Run diagnostic tests<ept id="p1">](../operationalize/configure-run-diagnostics.md)</ept>.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Evaluate<ept id="p1">](../operationalize/configure-evaluate-capacity.md)</ept> the configuration's capacity.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>How to upgrade</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>To replace an older version, you can uninstall the older distribution before installing the new version (there is no in-place upgrade).</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Carefully review the steps in the following sections.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Upgrade a compute node</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Before you begin, back up the appsettings.json file on each node in case of an issue during the upgrade process.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Uninstall Microsoft R Server 9.0 or 9.1 using the instructions in the article <bpt id="p1">[</bpt>Uninstall Microsoft R Server to upgrade to a newer version<ept id="p1">](../install/r-server-install-uninstall-upgrade.md)</ept>.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>The uninstall process stashes away a copy of your 9.0 or 9.1 configuration files under this directory so you can seamlessly upgrade to Machine Learning Server 9.2.1 in the next step:</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Windows: C:\Users\Default\AppData\Local\DeployR\current</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Linux: /etc/deployr/current</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server and its dependencies as follows.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Learn about supported platforms for this configuration.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Windows instructions: <bpt id="p1">[</bpt>Installation steps<ept id="p1">](../install/machine-learning-server-windows-install.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](../install/machine-learning-server-windows-offline.md)</ept></source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">_</bpt>SQL Server Machine Learning Services<ept id="p1">_</ept>, you must also manually install .NET Core 1.1 and add a registry key called 'H_KEY_LOCAL_MACHINE\SOFTWARE\R Server\Path' with a value of the parent path to the R<ph id="ph1">\_</ph>SERVER or PYTHON<ph id="ph2">\_</ph>SERVER folder (for example, C:\Program Files\Microsoft SQL Server\140).</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Linux instructions: <bpt id="p1">[</bpt>Installation steps<ept id="p1">](../install/machine-learning-server-linux-install.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](../install/machine-learning-server-linux-offline.md)</ept></source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](../operationalize/configure-admin-cli-launch.md)</ept> with administrator/root/sudo privileges.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>The utility checks to see if any configuration files from past releases are present under the <ph id="ph1">`current`</ph> folder mentioned previously.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Choose <bpt id="p1">**</bpt>Configure server<ept id="p1">**</ept> from the menu and then <bpt id="p2">**</bpt>Configure a compute node<ept id="p2">**</ept> from the submenu.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>When the script asks you if you want to upgrade, enter <ph id="ph1">`y`</ph>.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>The node is automatically set up using the configuration you had for R Server 9.0 or 9.1.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>You can now <bpt id="p1">**</bpt>repeat these steps<ept id="p1">**</ept> for each compute node.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Upgrade a web node</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Before you begin, back up the appsettings.json file on each node in case of an issue during the upgrade process.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Uninstall Microsoft R Server 9.0 or 9.1 using the instructions in the article <bpt id="p1">[</bpt>Uninstall Microsoft R Server to upgrade to a newer version<ept id="p1">](../install/machine-learning-server-linux-uninstall.md)</ept>.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>The uninstall process stashes away a copy of your 9.0 or 9.1 configuration files under this directory so you can seamlessly upgrade to Machine Learning Server 9.2.1 in the next step:</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Windows: C:\Users\Default\AppData\Local\DeployR\current</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Linux: /etc/deployr/current</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server and its dependencies as follows.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Learn about supported platforms for this configuration.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Windows instructions: <bpt id="p1">[</bpt>Installation steps<ept id="p1">](../install/machine-learning-server-windows-install.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](../install/machine-learning-server-windows-offline.md)</ept></source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">_</bpt>SQL Server Machine Learning Services<ept id="p1">_</ept>, you must also manually install .NET Core 1.1 and add a registry key called 'H_KEY_LOCAL_MACHINE\SOFTWARE\R Server\Path' with a value of the parent path to the R<ph id="ph1">\_</ph>SERVER or PYTHON<ph id="ph2">\_</ph>SERVER folder (for example, C:\Program Files\Microsoft SQL Server\140).</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Linux instructions: <bpt id="p1">[</bpt>Installation steps<ept id="p1">](../install/machine-learning-server-linux-install.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](../install/machine-learning-server-linux-offline.md)</ept></source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](../operationalize/configure-admin-cli-launch.md)</ept> with administrator/root/sudo privileges.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>The utility checks to see if any configuration files from past releases are present under the <ph id="ph1">`current`</ph> folder mentioned previously.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Choose <bpt id="p1">**</bpt>Configure server<ept id="p1">**</ept> from the menu and then <bpt id="p2">**</bpt>Configure a web node<ept id="p2">**</ept> from the submenu.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>When the script asks you if you'd like to upgrade, enter <ph id="ph1">`y`</ph>.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>The node is automatically set up using the configuration you had for R Server 9.0 or 9.1.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option to <bpt id="p1">**</bpt>Run Diagnostic Tests<ept id="p1">**</ept> to <bpt id="p2">[</bpt>test the configuration<ept id="p2">](../operationalize/configure-run-diagnostics.md)</ept>.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>You can now <bpt id="p1">**</bpt>repeat these steps<ept id="p1">**</ept> for each node.</source>
        </trans-unit></group></body></file></xliff>