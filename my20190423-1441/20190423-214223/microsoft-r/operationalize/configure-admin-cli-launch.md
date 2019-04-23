<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="configure-admin-cli-launch.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca860f2f83b884ad8cd2fcf448bb400cda117ab72834.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">0f2f83b884ad8cd2fcf448bb400cda117ab72834</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\configure-admin-cli-launch.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Launch the Administration CLI - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Launch the Admin CLI and utility used to manage the operationalization configuration for Machine Learning Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Launch the administration tool/CLI to manage the operationalization configuration</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies to:  Machine Learning Server, Microsoft R Server</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>This article describes how to launch the tool used to manage the web and compute nodes for Machine Learning Server.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>These nodes enable you to operationalize your analytics with Machine Learning Server.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The tool you use to set up and manage your configuration depends on your version:</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server 9.3, use the command-line interface (CLI).</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>In versions 9.0 - 9.2, use the Administration Utility.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>With this tool, you can:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Configure web and compute nodes to enable operationalizing with Machine Learning Server</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Encrypt credentials</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Stop and restart nodes</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Run diagnostic tests</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Declare compute nodes</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Update the node ports</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Update the local admin password</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Evaluate the capacity of your configuration</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Machine Learning Server 9.3: Administration with Azure CLI</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>In this release, use the <ph id="ph1">`admin`</ph> extension of the <bpt id="p1">[</bpt>Azure CLI<ept id="p1">](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest)</ept> to set up and manage your Machine Learning Server node configuration.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>You do not need an Azure subscription to use this CLI.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This CLI is installed with Machine Learning Server and runs locally.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Launch a DOS command line, powershell window, or terminal window with administrator privileges.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Call the help function to verify that Administration CLI is working properly.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>At the command prompt, enter:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>You must first <bpt id="p1">[</bpt>set up your nodes<ept id="p1">](configure-machine-learning-server-one-box.md)</ept> before running any other <ph id="ph1">`admin`</ph> extension commands in the CLI.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>For a speedy setup of a one-box configuration, use <ph id="ph1">`az ml admin bootstrap`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Machine Learning Server 9.2: Administration utility</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>These instructions describe how to launch the Administrator Utility on Machine Learning Server 9.2.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>To launch the 9.2 Administration Utility:</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On Windows,<ept id="p1">**</ept> right-click the "Administration Utility" program icon in the Start menu, and then click "Run as Administrator".</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If the default powershell execution policy for your organization is "Restricted", the shortcut may not work.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>To get around this issue, either change the execution policy to "Unrestricted", or run the following in a command-line window with administrator privileges:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On Linux,<ept id="p1">**</ept> run the following commands with <ph id="ph1">`root`</ph> or <ph id="ph2">`sudo`</ph> privileges:</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Also read about the <bpt id="p1">[</bpt>command-line switches<ept id="p1">](#switch)</ept>  to the administration utility.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>R Server 9.1: Administration utility</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>These instructions describe how to launch the Administrator Utility on Machine Learning Server 9.1.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>To launch the 9.1 Administration Utility:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On Windows,<ept id="p1">**</ept> right-click the "Administration Utility" program icon in the Start menu, and then click "Run as Administrator".</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>If the default powershell execution policy for your organization is "Restricted", the shortcut may not work.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>To get around this issue, either change the execution policy to "Unrestricted", or run the following in a command-line window with administrator privileges:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Find r-home by running <ph id="ph1">`normalizePath(R.home())`</ph> in the R console.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On Linux,<ept id="p1">**</ept> run the following commands with <ph id="ph1">`root`</ph> or <ph id="ph2">`sudo`</ph> privileges:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Also read about the <bpt id="p1">[</bpt>command-line switches<ept id="p1">](#switch)</ept>  to the administration utility.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>R Server 9.0: Administration utility</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>These instructions describe how to launch the Administrator Utility on Machine Learning Server 9.0.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>To launch the 9.0 Administration Utility:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On Windows,<ept id="p1">**</ept> right-click the "Administration Utility" program icon in the Start menu, and then click "Run as Administrator".</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>If the default powershell execution policy for your organization is "Restricted", the shortcut may not work.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>To get around this issue, either change the execution policy to "Unrestricted", or run the following in a command-line window with administrator privileges:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Find r-home by running <ph id="ph1">`normalizePath(R.home())`</ph> in the R console.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On Linux,<ept id="p1">**</ept> run the following commands with <ph id="ph1">`root`</ph> or <ph id="ph2">`sudo`</ph> privileges:</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Command-line switches</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The following command-line switches are available for the administration utility installed with R Server 9.0 - 9.1 and Machine Learning Server 9.2.1.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Switch</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Introduced in version</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>-silentoneboxinstall password uris</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>-silentinstall  password uris</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Sets up a <bpt id="p1">[</bpt>one-box configuration<ept id="p1">](configure-start-for-administrators.md#configure-server-for-operationalization)</ept> silently, sets an admin password, and in 9.2 allows you to <bpt id="p2">[</bpt>specify compute node URIs<ept id="p2">](configure-admin-cli-compute-uris.md)</ept> or IP ranges.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>A password is required.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>-silentinstall myPass123 <ph id="ph1">http://1.1.1.1:12805</ph>,<ph id="ph2">http://1.0.1.1-3:12805</ph></source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>9.1,</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>URIs in 9.2</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>-silentwebnodeinstall password uris</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Configures a <bpt id="p1">[</bpt>web node<ept id="p1">](configure-start-for-administrators.md#configure-server-for-operationalization)</ept> silently, sets an admin password, and in 9.2 allows you to <bpt id="p2">[</bpt>specify compute node URIs<ept id="p2">](configure-admin-cli-compute-uris.md)</ept> or IP ranges.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>A password is required.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>-silentwebnodeinstall myPass123 <ph id="ph1">http://1.1.1.1:12805</ph>,<ph id="ph2">http://1.0.1.1-3:12805</ph></source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>9.1,</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>URIs in 9.2</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>-silentcomputenodeinstall</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Configures a <bpt id="p1">[</bpt>compute node<ept id="p1">](configure-start-for-administrators.md#configure-server-for-operationalization)</ept> silently.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>-silentcomputenodeinstall</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>9.1</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>-setpassword password</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Sets the password.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Cannot be used</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>if LDAP or AAD was configured.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>-setpassword myPass123</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>9.1</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>-preparedbmigration filePath</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Migrates the data from current database to a different database schema.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Takes the <bpt id="p1">[</bpt>path to the web node’s appsetting.json file<ept id="p1">](../operationalize/configure-find-admin-configuration-file.md)</ept> as an argument.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>This is uncommonly needed as a step when upgrading.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>-preparedbmigration <ph id="ph1">\&lt;</ph>web-node-dir&gt;/appsettings.json</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>9.1</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>-encryptsecret Secret CertificateStoreName CertificateStoreLocation CertificateSubjectName</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Silently <bpt id="p1">[</bpt>encrypts secrets<ept id="p1">](configure-admin-cli-encrypt-credentials.md)</ept>.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>-encryptsecret<ph id="ph1">&amp;nbsp;</ph>theSecret<ph id="ph2">&amp;nbsp;</ph>Store<ph id="ph3">&amp;nbsp;</ph>Location Subject</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>9.1</source>
        </trans-unit></group></body></file></xliff>