<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-admin-install-in-cloud.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926b47bf7f49adfb3fde4b3f3d53006d8f6128828b7.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">b47bf7f49adfb3fde4b3f3d53006d8f6128828b7</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-admin-install-in-cloud.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Enabling DeployR on the Cloud (Azure, AWS) - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to Enable DeployR on Azure and AWS (Cloud)</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Enabling DeployR on the Cloud</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>You can set up DeployR on <bpt id="p1">**</bpt>Microsoft Azure<ept id="p1">**</ept> or <bpt id="p2">**</bpt>AWS<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>For each instance, be sure to:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Set the server Web context to an external, public IP address and disable IP autodetection.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Open three DeployR external ports by adding <bpt id="p1">[</bpt>Azure endpoints<ept id="p1">](#configuring-azure-endpoints)</ept> or opening the ports through the AWS console to set the appropriate permissions.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Update the <bpt id="p1">[</bpt>firewall<ept id="p1">](#updating-the-firewall)</ept> to set the appropriate security permissions on the internal and external ports used by DeployR.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Have the minimum required disk space (or more) for the installation of DeployR.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Refer to the installation guide for your DeployR version and operating system.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>We highly recommended that you also <bpt id="p1">[</bpt>enable HTTPS support<ept id="p1">](../operationalize/configure-https.md)</ept> for DeployR to secure the communications to the server.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Enabling DeployR on Azure</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>You can set up DeployR on <bpt id="p1">**</bpt>Microsoft Azure<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>For each Azure instance, be sure to:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Set the <bpt id="p1">[</bpt>server Web context<ept id="p1">](#setting-the-server-web-context)</ept> to an external, public IP address.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Open three DeployR external ports by adding <bpt id="p1">[</bpt>Azure endpoints<ept id="p1">](#configuring-azure-endpoints)</ept> to set the appropriate permissions.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Update the <bpt id="p1">[</bpt>firewall<ept id="p1">](#updating-the-firewall)</ept> to set the appropriate security permissions on the internal and external ports used by DeployR.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Setting the Server Web Context</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The DeployR server Web context must be updated to the Public IP address of the virtual machine.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To update the DeployR server Web context:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>You must update the server Web context or else you will not be able to access to the DeployR landing page or other DeployR components after installation.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Log into the Azure portal and take note of the <bpt id="p1">**</bpt>Public IP address<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Public IP Address in Azure portal</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If DeployR was installed on a virtual machine, remote desktop or SSH into that machine.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">**</bpt>DeployR for Microsoft R Server 8.0.5<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Launch the DeployR administrator utility script with administrator privileges:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>On Windows, run:</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>On Linux, run:</source>
        </trans-unit></group></body></file></xliff>