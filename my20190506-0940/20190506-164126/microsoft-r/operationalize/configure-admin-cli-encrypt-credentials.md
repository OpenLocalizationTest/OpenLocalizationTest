<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="configure-admin-cli-encrypt-credentials.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc775016e81655595f20b94b2e9e00558b1b7fc6c8e9c6.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">16e81655595f20b94b2e9e00558b1b7fc6c8e9c6</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\configure-admin-cli-encrypt-credentials.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Encrypt credentials and secrets - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>You should encrypt strings in the appsettings.json configuration file.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Encrypt credentials and secrets</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies to:  Machine Learning Server, Microsoft R Server</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>For security purposes, we strongly recommend that you encrypt strings in the appsettings.json configuration file.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>For example, you should encrypt any remote database connection strings and/or LDAP/LDAP-S passwords rather than store strings in plain text.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The encryption function available in the administration utility relies on the RSA algorithm for encryption.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>To encrypt credentials or secrets:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>On the web node, install a credential encryption certificate with a private key into the default certificate store on the local machine.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>That location is in the Windows certificate store or in the Linux-based PFX file.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The length of the encryption key depends on the certificate, however, we recommend a length of at least 1048 bits.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Ensure that your certificate is secured properly.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>On Windows, for example, you can use Bitlocker to encrypt the disk.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Open the administration tool to encrypt the secret:</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>For Machine Learning Server 9.3, use <ph id="ph1">`admin`</ph> extension of the Azure Command Line Interface (<bpt id="p1">[</bpt>Azure CLI<ept id="p1">](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest)</ept>) to encrypt your credentials.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>You do not need an Azure subscription to use this CLI.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>It is installed as part of Machine Learning Server and runs locally.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>On the machine hosting the node, launch a command-line window or terminal  with administrator (Windows) or root/sudo (Linux) privileges.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Run the command to encrypt:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>CLI<ph id="ph1">&amp;nbsp;</ph>options</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>list</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Returns the list of certificates found on the machine.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>set</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Returns an encrypted string when you specify a certificate and a secret to be encrypted.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>--cert-store-name</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The certificate store name.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>In Windows, it is usually one of "My", "Root", "TrustedPeople" etc.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>--cert-store-location</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The certificate store location.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>In Windows, it is either "CurrentUser" or "LocalMachine".</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>--cert-subject_name</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The subject name of certificate.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>You could check it from "az ml admin credentials list".</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>In the above example, the subject name is "DC=Windows Azure CRP Certificate Generator".</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>For multiple entries on the subject name, escape the subject name as follows:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>--secret</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Enter information you want to encrypt.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The CLI returns an encrypted string.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>For versions 9.0 - 9.2: <bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](configure-admin-cli-launch.md)</ept> with administrator privileges (Windows) or root/sudo privileges (Linux).</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option <bpt id="p1">**</bpt>Encrypt Credentials<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Specify where is the encryption certificate installed:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Local machine (Computer account)</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Current user (My user account)</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Specify which encryption certificate to use.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Enter information you want to encrypt.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The tool returns an encrypted string.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Open the configuration file, <bpt id="p1">[</bpt><ph id="ph1">\&lt;</ph>web-node-install-path&gt;<ept id="p1">](../operationalize/configure-find-admin-configuration-file.md)</ept>/appsettings.json.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>In that file, update the appropriate section for a <bpt id="p1">[</bpt>remote database connection<ept id="p1">](configure-remote-database-to-operationalize.md)</ept> or the <bpt id="p2">[</bpt>authentication password<ept id="p2">](configure-authentication.md#encrypt)</ept> strings.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>You can bypass script interface using the argument '-encryptsecret encryptSecret encryptSecretCertificateStoreName encryptSecretCertificateStoreLocation encryptSecretCertificateSubjectName'.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>See the table at the end of this topic, <bpt id="p1">[</bpt>here<ept id="p1">](configure-admin-cli-launch.md#switch)</ept>.</source>
        </trans-unit></group></body></file></xliff>