<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-security-server-access.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea9263a0767cd8c1f84e0183e6cd42fe28484e368fb8e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">3a0767cd8c1f84e0183e6cd42fe28484e368fb8e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-security-server-access.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Security: Server Access Controls - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Security in DeployR: Authentication, HTTPS, SSL, and access controls for server, Project file and Repository File, and more.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Server Access Controls for DeployR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Learn about the following server access controls.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Working with IP Address Filters</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>While access to DeployR is typically controlled by <bpt id="p1">[</bpt>authentication mechanisms<ept id="p1">](../operationalize/configure-authentication.md)</ept>, DeployR also supports access controls based on IP address filters.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Under the <bpt id="p1">[</bpt><bpt id="p2">**</bpt>Server Policies<ept id="p2">**</ept><ept id="p1">](deployr-admin-managing-server-policies.md#server-policy-properties)</ept> tab in the DeployR Administration Console, you can configure your IP address filter policy.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Operation Policies<ept id="p1">**</ept> for authenticated, asynchronous, and anonymous operations each support an <bpt id="p2">[</bpt>IP filter<ept id="p2">](deployr-admin-managing-server-policies.md#server-policy-properties)</ept> property.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>If you assign an IP filter to this property, then any attempt by a client application to connect from outside of the IP address range on that filter will be automatically rejected.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>For example, you can make your DeployR server instance accessible only from IP addresses on the local LAN or VPN, such as <ph id="ph1">`192.168.1.xxx`</ph> or <ph id="ph2">`10.xxx.xxx.xxx`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Note that it is possible to achieve these same kinds of access controls with an appropriate configuration on your firewall and/or routers.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Cross-Origin Resource Sharing</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Cross-Origin Resource Sharing (CORS) enables your client application to freely communicate and make cross-site HTTP requests for resources from a domain other than where the DeployR is hosted.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>CORS can be enabled or disabled in the DeployR external configuration file, <ph id="ph1">`$DEPLOYR_HOME\deployr\deployr.groovy`</ph>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>In DeployR Enterprise, support for CORS is disabled by default.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To enable CORS support:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Update the relevant properties in ``$DEPLOYR_HOME\deployr\deployr.groovy<ph id="ph1">` by setting `</ph>cors.enabled = true`.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Optionally, to restrict cross-site HTTP requests to only those requests coming from a specific domain, specify a value for <ph id="ph1">`Access-Control-Allow-Origin`</ph> on the <ph id="ph2">`cors.headers`</ph> property.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Stop and restart the DeployR server<ept id="p1">](deployr-common-administration-tasks.md#startstop)</ept>.</source>
        </trans-unit></group></body></file></xliff>