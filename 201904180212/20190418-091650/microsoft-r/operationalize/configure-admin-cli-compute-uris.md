<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="configure-admin-cli-compute-uris.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4b60c23c486cf02d18210144672b483738371ad96.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">b60c23c486cf02d18210144672b483738371ad96</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\configure-admin-cli-compute-uris.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Manage and declare compute node URIs - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Declare the compute node URIs so that Machine Learning Server web nodes know to which compute nodes they can send requests.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Manage and declare compute nodes</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Machine Learning Server, Microsoft R Server<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>In order for the Machine Learning Server web nodes to know to which compute nodes it can send requests, you must maintain a complete list of compute node URIs.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This list of compute node URIs is shared across all web nodes automatically and is managed through the Admin CLI (v9.3) or, for earlier versions, in the Administration Utility.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>R Server 9.1 administrators must declare URIs manually for each web node in their respective appsettings.json file.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>If the <bpt id="p1">[</bpt>'owner' role is defined<ept id="p1">](configure-roles.md)</ept>, then the administrator must belong to the 'Owner' role in order to manage compute nodes.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>If you declared URIs in R Server and have upgraded to Machine Learning Server, the URIs are copied from the old appsettings.json to the database so they can be shared across all web nodes.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If you remove a URI with the utility, it is deleted from the appsettings.json file as well for consistency.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Machine Learning Server 9.3</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server 9.3, you can use <ph id="ph1">`admin`</ph> extension of the Azure Command Line Interface (<bpt id="p1">[</bpt>Azure CLI<ept id="p1">](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest)</ept>) to set up and manage your configuration, including the declaration and management of compute nodes with your web nodes.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>You must first <bpt id="p1">[</bpt>set up your compute nodes<ept id="p1">](configure-machine-learning-server-enterprise.md)</ept> before doing anything else with the <ph id="ph1">`admin`</ph> extension of the CLI.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>You do not need an Azure subscription to use this CLI.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>It is installed as part of Machine Learning Server and runs locally.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>On the machine hosting the node, launch a command-line window or terminal  with administrator (Windows) or root/sudo (Linux) privileges.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If you are not yet authenticated in the CLI, do so now.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>This is an administrator task only, so you must have the Owner role to declare or manage URIs.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The account name is <ph id="ph1">`admin`</ph> unless LDAP or AAD is configured.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Use the CLI to declare the IP address of each compute node you configured.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>You can specify a single URI, several URIs, or even an IP range:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>For multiple compute nodes, separate each URI with a comma.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The following example shows a single URI and a range of IPs (1.0.1.1, 1.0.1.2, 1.0.2.1, 1.0.2.2, 1.0.3.1, 1.0.3.2):</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&lt;http://1.1.1.1:12805&gt;</ph>, <ph id="ph2">http://1.0.1-3.1-2:12805</ph></source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Machine Learning Server 9.2</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>To declare or manage URIs in Machine Learning Server 9.2:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Log in to the machine on which one of your web nodes is installed.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](configure-admin-cli-launch.md)</ept> with administrator privileges (Windows) or root/sudo privileges (Linux).</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option <bpt id="p1">**</bpt>Manage compute nodes<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>From the submenu, choose <bpt id="p1">**</bpt>Add URIs<ept id="p1">**</ept> to declare one or more compute node URIs.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>When prompted, enter the IP address of each compute node you configured.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>You can specify a specific URI or  specify IP ranges.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>For multiple compute nodes, separate each URI with a comma.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>For example: <ph id="ph1">http://1.1.1.1:12805</ph>, <ph id="ph2">http://1.0.1-3.1-2:12805</ph></source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>In this example, the range represents six IP values: 1.0.1.1, 1.0.1.2, 1.0.2.1, 1.0.2.2, 1.0.3.1,  1.0.3.2.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>You can also choose to remove URIs or view the list of URIs.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Return the main menu of the utility.</source>
        </trans-unit></group></body></file></xliff>