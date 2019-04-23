<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="configure-cors.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca8603c29ff6e46902fbe7e6e1643c4487e29d252826.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">03c29ff6e46902fbe7e6e1643c4487e29d252826</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\configure-cors.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Cross-Origin Resource Sharing CORS in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Enterprise-Grade Security: CORS with Machine Learning Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Cross-Origin Resource Sharing</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies to:  Machine Learning Server, Microsoft R Server 9.x</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Cross-Origin Resource Sharing (CORS) enables your client application to freely communicate and make cross-site HTTP requests for resources from a domain other than where the web node is hosted.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>You can enable or disable CORS in the external configuration file, appsettings.json.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Support for CORS is disabled by default.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>To enable CORS support:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>On each web node, open the configuration file, <ph id="ph1">\&lt;</ph>web-node-install-path&gt;/appsettings.json.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>(Find the <bpt id="p1">[</bpt>install path<ept id="p1">](../operationalize/configure-find-admin-configuration-file.md)</ept> for your version.)</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Enable CORS in the <ph id="ph1">`"CORS": {`</ph> section of the  appsettings.json file:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Set CORS</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Enter a comma-separated list of allowed <ph id="ph1">`"Origins"`</ph> for your policy.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>In this example, the policy allows cross-origin requests from "<ph id="ph1">&lt;http://www.contoso.com&gt;</ph>", "<ph id="ph2">&lt;http://www.microsoft.com&gt;</ph>", and no other origins.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Launch the administrator's utility and <bpt id="p1">[</bpt>restart the web node<ept id="p1">](configure-admin-cli-stop-start.md)</ept>.</source>
        </trans-unit></group></body></file></xliff>