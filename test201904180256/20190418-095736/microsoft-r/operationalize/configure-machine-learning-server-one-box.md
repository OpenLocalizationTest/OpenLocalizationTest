<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="configure-machine-learning-server-one-box.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c6f85c48a60701e0e608433b4b63bff393f90504f.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">6f85c48a60701e0e608433b4b63bff393f90504f</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\configure-machine-learning-server-one-box.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Configure Machine Learning Server 9.3 to operationalize analytics (one-box)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Configure Machine Learning Server 9.3 to operationalize analytics on a single machine (One-box)</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>setup machine learning server for deployment; install machine learning server for deploying</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Configure Machine Learning Server 9.3 to operationalize analytics on a single machine (One-box)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: Machine Learning Server 9.3<ept id="p1">**</ept> <ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph><ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph><ph id="ph7">&amp;nbsp;</ph><ph id="ph8">&amp;nbsp;</ph><ph id="ph9">&amp;nbsp;</ph><ph id="ph10">&amp;nbsp;</ph><ph id="ph11">&amp;nbsp;</ph><ph id="ph12">&amp;nbsp;</ph><ph id="ph13">&amp;nbsp;</ph><ph id="ph14">&amp;nbsp;</ph><ph id="ph15">&amp;nbsp;</ph><ph id="ph16">&amp;nbsp;</ph>For older versions: <bpt id="p2">[</bpt>ML Server 9.2.1<ept id="p2">](configure-machine-learning-server-one-box-9-2.md)</ept><ph id="ph17"> | </ph><bpt id="p3">[</bpt>R Server 9.x<ept id="p3">](../install/operationalize-r-server-one-box-config.md)</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>You can configure Microsoft Learning Server after installation to act as a deployment server and to host analytic web services for operationalization.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Machine Learning Server offers two types of configuration for operationalizing analytics and remote execution: <bpt id="p1">**</bpt>One-box and Enterprise<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This article describes the one-box configuration.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>For more on enterprise configurations, <bpt id="p1">[</bpt>see here<ept id="p1">](configure-machine-learning-server-enterprise.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>A one-box configuration, as the name suggests, involves a single <bpt id="p1">[</bpt>web node and compute node<ept id="p1">](../operationalize/configure-start-for-administrators.md#configure-server-for-operationalization)</ept> run on a single machine along with a database.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Set-up is a breeze.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>This configuration is useful when you want to explore what it is to operationalize R and Python analytics using Machine Learning Server.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>It is perfect for testing, proof-of-concepts, and small-scale prototyping, but might not be appropriate for production usage.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Configure Machine Learning Server on one-box architecture</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>How to configure</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>You can create a ready-to-use server with just a few clicks using Azure Marketplace VM <bpt id="p1">[</bpt>Machine Learning Server Operationalization<ept id="p1">](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/deploy-r.operationalization?tab=Overview)</ept>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Navigate to the virtual machine listing on <bpt id="p1">[</bpt>Azure portal<ept id="p1">](https://portal.azure.com/#create/deploy-r.operationalizationonebox)</ept>, select the <bpt id="p2">**</bpt>Create<ept id="p2">**</ept> button at the bottom, provide necessary inputs to create the Operationalization Server.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Azure Resource Management templates<ept id="p1">](https://github.com/Microsoft/microsoft-r/tree/master/mlserver-arm-templates)</ept> are also provided in GitHub.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>This <bpt id="p1">[</bpt>blog post<ept id="p1">](https://blogs.msdn.microsoft.com/mlserver/2018/02/27/configuring-microsoft-machine-learning-server-9-3-to-operationalize-analytics-using-arm-templates/)</ept> provides more information.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To configure on a single machine:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server and its dependencies as follows.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Learn about <bpt id="p1">[</bpt>supported platforms<ept id="p1">](../operationalize/configure-start-for-administrators.md#supported-platforms)</ept>  for this configuration.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Linux instructions: <bpt id="p1">[</bpt>Installation steps<ept id="p1">](../install/machine-learning-server-linux-install.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](../install/machine-learning-server-linux-offline.md)</ept></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Windows instructions: <bpt id="p1">[</bpt>Installation steps<ept id="p1">](../install/machine-learning-server-windows-install.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](../install/machine-learning-server-windows-offline.md)</ept><ph id="ph2">    </ph></source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">_</bpt>SQL Server Machine Learning Services<ept id="p1">_</ept>, you must also manually install .NET Core 2.0 and add a registry key called 'H_KEY_LOCAL_MACHINE\SOFTWARE\R Server\Path' with a value of the parent path to the R<ph id="ph1">\_</ph>SERVER or PYTHON<ph id="ph2">\_</ph>SERVER folder (for example, C:\Program Files\Microsoft SQL Server\140<ph id="ph3">\)</ph>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>In a command-line window or terminal that was launched with administrator (Windows) or root/sudo (Linux) privileges, run the following <bpt id="p1">[</bpt>CLI commands<ept id="p1">](configure-admin-cli-launch.md)</ept> to:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Set up a web node and compute node on the same machine.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Define a password for the default 'admin' account.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Replace <ph id="ph1">&lt;Password&gt;</ph> with a password of your choice.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The admin password must be 8-16 characters long and contain 1+ uppercase character, 1+ lowercase character, 1+ one number, and 1+ special characters:</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Authenticate with Machine Learning Server.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Test the configuration<ept id="p1">](../operationalize/configure-run-diagnostics.md)</ept>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>You can always configure the server to authenticate against  <bpt id="p1">[</bpt>Active Directory (LDAP) or Azure Active Directory<ept id="p1">](../deployr/../operationalize/configure-admin-cli-local-password.md)</ept> later.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If you need help with CLI commands, run the command but add <ph id="ph1">`--help`</ph> to the end.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If on Linux and using the IPTABLES firewall or equivalent service, then use the <ph id="ph1">`iptables`</ph> command (or the equivalent) to open port 12800 to the public IP of the web node so that remote machines can access it.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Machine Learning Server uses Kestrel as the web server for its operationalization web nodes.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Therefore, if you expose your application to the Internet, we recommend that you review the <bpt id="p1">[</bpt>guidelines for Kestrel<ept id="p1">](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/servers/kestrel)</ept> regarding reverse proxy setup.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>You are now ready to begin operationalizing your R and Python analytics with Machine Learning Server.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>How to upgrade</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Carefully review the following steps.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Before you begin, back up the appsettings.json file on each node in case of an issue during the upgrade process.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>R Server 9.x users only: If you used the default SQLite database, <ph id="ph1">`deployrdb_9.0.0.db`</ph> or <ph id="ph2">`deployrdb_9.1.0.db`</ph> in R Server and want to persist the data, then you must <bpt id="p1">**</bpt>back up the SQLite database before uninstalling Microsoft R Server<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Make a copy of the database file and put it outside of the Microsoft R Server directory structure.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>(If you are using a SQL Server or PostgreSQL database, you can skip this step.)</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>If you skip this SQLite database backup step, your database data will be lost.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Uninstall the old version.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The uninstall process stashes away a copy of your configuration files for a seamlessly upgrade to Machine Learning Server 9.3.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>For Machine Learning Server 9.2.1, read these instructions: <bpt id="p1">[</bpt>Windows<ept id="p1">](../install/machine-learning-server-windows-uninstall.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Linux<ept id="p2">](../install/machine-learning-server-linux-uninstall.md)</ept>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>For Microsoft R Server 9.x, read this <bpt id="p1">[</bpt>Uninstall Microsoft R Server to upgrade to a newer version<ept id="p1">](../install/r-server-install-uninstall-upgrade.md)</ept>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>If you are using a SQL Server or PostgreSQL database, you can skip this step.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If you backed up a SQLite database in Step 1, manually move the .db file under this directory so it can be found during the upgrade:</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Windows: C:\Users\Default\AppData\Local\DeployR\current\frontend</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Linux: /etc/deployr/current/frontend</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server and its dependencies as follows.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Learn about <bpt id="p1">[</bpt>supported platforms<ept id="p1">](../operationalize/configure-start-for-administrators.md#supported-platforms)</ept>  for this configuration.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Linux instructions: <bpt id="p1">[</bpt>Installation steps<ept id="p1">](../install/machine-learning-server-linux-install.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](../install/machine-learning-server-linux-offline.md)</ept></source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Windows instructions: <bpt id="p1">[</bpt>Installation steps<ept id="p1">](../install/machine-learning-server-windows-install.md)</ept><ph id="ph1"> | </ph><bpt id="p2">[</bpt>Offline steps<ept id="p2">](../install/machine-learning-server-windows-offline.md)</ept></source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">_</bpt>SQL Server Machine Learning Services<ept id="p1">_</ept>, you must also manually install .NET Core 2.0 and add a registry key called 'H_KEY_LOCAL_MACHINE\SOFTWARE\R Server\Path' with a value of the parent path to the R<ph id="ph1">\_</ph>SERVER or PYTHON<ph id="ph2">\_</ph>SERVER folder (for example, C:\Program Files\Microsoft SQL Server\140<ph id="ph3">\)</ph>.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>In a command-line window or terminal that was launched with administrator (Windows) or root/sudo (Linux) privileges, run <bpt id="p1">[</bpt>CLI commands<ept id="p1">](configure-admin-cli-launch.md)</ept> to:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Set up a web node and compute node on the same machine.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Define a password for the default 'admin' account.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Replace <ph id="ph1">&lt;Password&gt;</ph> with a password of your choice.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>The admin password must be 8-16 characters long and contain 1+ uppercase character, 1+ lowercase character, 1+ one number, and 1+ special characters:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Authenticate with Machine Learning Server.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Test the configuration<ept id="p1">](../operationalize/configure-run-diagnostics.md)</ept>.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>You can always configure the server to authenticate against  <bpt id="p1">[</bpt>Active Directory (LDAP) or Azure Active Directory<ept id="p1">](../deployr/../operationalize/configure-admin-cli-local-password.md)</ept> later.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>If you need help with CLI commands, run the command but add <ph id="ph1">`--help`</ph> to the end.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>If on Linux and using the IPTABLES firewall or equivalent service, then use the <ph id="ph1">`iptables`</ph> command (or the equivalent) to open port 12800 to the public IP of the web node so that remote machines can access it.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Machine Learning Server uses Kestrel as the web server for its operationalization web nodes.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Therefore, if you expose your application to the Internet, we recommend that you review the <bpt id="p1">[</bpt>guidelines for Kestrel<ept id="p1">](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/servers/kestrel)</ept> regarding reverse proxy setup.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>You are now ready to begin operationalizing your R and Python analytics with Machine Learning Server.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>The entities created by users, specifically web services, and <bpt id="p1">[</bpt>snapshots<ept id="p1">](../r/how-to-execute-code-remotely.md#snapshot)</ept>, are tied to their usernames.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>For this reason, you must be careful to prevent changes to the user identifier over time.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Otherwise, pre-existing web services and snapshots cannot be mapped to the users who created them.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>For this reason, we strongly recommend that you DO NOT change the unique LDAP identifier in appsettings.json once users start publishing service or creating snapshots.</source>
        </trans-unit></group></body></file></xliff>