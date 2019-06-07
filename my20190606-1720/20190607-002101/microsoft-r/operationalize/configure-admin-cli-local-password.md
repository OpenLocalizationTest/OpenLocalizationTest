<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="configure-admin-cli-local-password.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37001b4429943dfedadb3d5bda847904a8f15a5fd8.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">001b4429943dfedadb3d5bda847904a8f15a5fd8</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\configure-admin-cli-local-password.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Set or update the local administrator password - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>When no other form of authentication is used, you must define a password for the local administrator account.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Set or update the local administrator password</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies to:  Machine Learning Server, Microsoft R Server</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>When no other form of <bpt id="p1">[</bpt>authentication<ept id="p1">](configure-authentication.md)</ept> is used for Machine Learning Server, you must define a password for the local administrator account called 'admin'.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>If you enable another form of authentication, the local administrator account is automatically disabled.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The admin password must be 8-16 characters long and contain:</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>At least one uppercase character</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>At least one lowercase character</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>At least one number</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>At least one of the following special characters:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Machine Learning Server 9.3</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server 9.3, you can use <ph id="ph1">`admin`</ph> extension of the Azure Command Line Interface (<bpt id="p1">[</bpt>Azure CLI<ept id="p1">](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest)</ept>) to set up and manage your configuration, including updating the local 'admin' account password.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This password is set while you are first configuring your nodes.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>You do not need an Azure subscription to use this CLI.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>It is installed as part of Machine Learning Server and runs locally.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>To update the password:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>On the machine hosting the node, launch a command-line window or terminal  with administrator (Windows) or root/sudo (Linux) privileges.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Run the command to update the 'admin' password.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Earlier versions: 9.0 - 9.2</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>To set or update the password:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Launch the administration utility.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option to set a password for the local 'admin' account.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If a password was already defined, provide the current password.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>When prompted, enter the new password for this administrator account.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If your configuration has multiple web nodes, we recommend the same password be used.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Confirm the password.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>You can bypass script interface using the argument '-setpassword '.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Learn about all command-line switches for this script, here.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit></group></body></file></xliff>