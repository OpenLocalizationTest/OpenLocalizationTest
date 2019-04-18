<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="concept-api.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b43c92426a97a7ad5bbfc74b519c28a040b0e24b22.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">3c92426a97a7ad5bbfc74b519c28a040b0e24b22</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\concept-api.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>APIs for operationalizing your models and analytics - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Operationalization APIs for authenticating, publishing, managing, and consuming web services with Machine Learning Server  or Microsoft R Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>APIs for operationalizing your models and analytics with Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: Machine Learning Server, Microsoft R Server 9.x<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The Machine Learning Server (and Microsoft R Server) <bpt id="p1">&lt;a href="https://microsoft.github.io/deployr-api-docs/" target="_blank"&gt;</bpt>REST APIs<ept id="p1">&lt;/a&gt;</ept> are exposed by the operationalization server, a standards-based server technology <bpt id="p2">[</bpt>capable of scaling to meet the needs of enterprise-grade deployments<ept id="p2">](configure-machine-learning-server-enterprise.md)</ept>.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>With the Machine Learning Server configured to operationalize, the full statistics, analytics, and visualization capabilities of R and Python can now be directly leveraged inside Web, desktop and mobile applications.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The APIs available with Machine Learning Server can be categorized into two groups: Core APIs and the Service Consumption APIs.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;big&gt;</bpt>Looking for a specific core API call? <bpt id="p2">&lt;a href="https://microsoft.github.io/deployr-api-docs/" target="_blank"&gt;</bpt>Look in this online API reference<ept id="p2">&lt;/a&gt;</ept>.<ept id="p1">&lt;/big&gt;</ept></source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Core APIs for Operationalization</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>These core REST APIs expose the R or Python platform as a service allowing the integration of Python models and R statistics, analytics, and visualizations inside Web, desktop and mobile applications.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>These APIs enable you to publish Machine Learning Server-hosted <bpt id="p1">**</bpt>R analytics web services<ept id="p1">**</ept>, making the full capabilities of R available to application developers on a simple yet powerful REST API.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>These core operationalization APIs can be grouped into several categories as shown in this table.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Core API Type</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Reference Help</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Authentication</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>These APIs provide authentication-related operations and access workflow features.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;a href="https://microsoft.github.io/deployr-api-docs/#authentication-apis" target="_blank"&gt;</bpt>Help<ept id="p1">&lt;/a&gt;</ept></source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Web Services</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>These APIs facilitate the publishing and management of user-defined analytic web services (create, delete, update, list, discover).</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Each web service is uniquely defined by a <ph id="ph1">`name`</ph> and <ph id="ph2">`version`</ph> for easy service consumption and meaningful machine-readable discovery approaches.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>When a service is published (<ph id="ph1">&lt;code&gt;POST /services/{name}/{version}&lt;/code&gt;</ph>), an endpoint is registered and a <bpt id="p1">[</bpt>custom Swagger-based JSON file is generated<ept id="p1">](how-to-build-api-clients-from-swagger-for-app-integration.md)</ept>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;a href="https://microsoft.github.io/deployr-api-docs/#services-management-apis" target="_blank"&gt;</bpt>Help<ept id="p1">&lt;/a&gt;</ept></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Session</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>These APIs provide functionality for R session management (create, delete, update, list, console output, history, and workspace and working directory files)</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;a href="https://microsoft.github.io/deployr-api-docs/#session-apis" target="_blank"&gt;</bpt>Help<ept id="p1">&lt;/a&gt;</ept></source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Snapshot</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>These APIs provide different operations to access and manage workspace snapshots.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>A snapshot is a prepared environment image of an R or Python session saved to Machine Learning Server, which includes the session's packages, objects and data files.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>This snapshot can be loaded into any subsequent remote session for the user who created it.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more about R session snapshots<ept id="p1">](../r/how-to-execute-code-remotely.md#snapshot)</ept></source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;a href="https://microsoft.github.io/deployr-api-docs/#snapshot-apis" target="_blank"&gt;</bpt>Help<ept id="p1">&lt;/a&gt;</ept></source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Status</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>This API returns a health report of the configuration, including the number of nodes, <bpt id="p1">[</bpt>pool size<ept id="p1">](configure-evaluate-capacity.md#pool)</ept>, and other details.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt>similar diagnostic report<ept id="p1">](configure-run-diagnostics.md)</ept> is available on the server.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;a href="https://microsoft.github.io/deployr-api-docs/#status-apis" target="_blank"&gt;</bpt>Help<ept id="p1">&lt;/a&gt;</ept></source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The core APIs are accessible from and described in  <ph id="ph1">`mlserver-swagger-&lt;version&gt;.json`</ph>, <bpt id="p1">**</bpt>a Swagger-based JSON document<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Download this file from <ph id="ph1">https://microsoft.github.io/deployr-api-docs/swagger/mlserver-swagger-\&lt;version&gt;.json</ph>, where <ph id="ph2">`&lt;version&gt;`</ph> is the 3-digit product version number.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Swagger is a popular specification for a JSON file that describes REST APIs.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>For R Server users, replace mlserver-swagger with rserver-swagger.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>You can access all of these core APIs using a client library built from <ph id="ph1">`rserver-swagger-&lt;version&gt;.json`</ph> using <bpt id="p1">[</bpt>these instructions and example<ept id="p1">](how-to-build-api-clients-from-swagger-for-app-integration.md)</ept>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Note: For client applications written in <bpt id="p1">**</bpt>R<ept id="p1">**</ept>, you can side-step the Swagger approach altogether and exploit <bpt id="p2">[</bpt>the mrsdeploy package<ept id="p2">](../r-reference/mrsdeploy/mrsdeploy-package.md)</ept> directly to list, discover, and consume services.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more in this article<ept id="p1">](how-to-consume-web-service-interact-in-r.md)</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Service Consumption APIs</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The service consumption REST APIs expose a wide range of Python and R analytics services to client application developers.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>After Python or R code is published and exposed by the server as a web service, an application can make API calls to pass inputs to the service, execute the service, and retrieve outputs from the service.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Whenever a web service is published (<ph id="ph1">&lt;code&gt;POST /services/{name}/{version}&lt;/code&gt;</ph>), an endpoint is registered (<ph id="ph2">&lt;code&gt;/api/{name}/{version}&lt;/code&gt;</ph>), which in turn triggers the generation of a custom Swagger-based JSON file.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>This swagger file describes each API needed to interact with that service.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>While the service consumption Swagger files are all named <ph id="ph1">`swagger.json`</ph>, you can find them each in a unique location by calling:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>To make it easier to integrate R and Python web services using these APIs, build and use an API client library stub from the <ph id="ph1">`swagger.json`</ph> file for each web service using <bpt id="p1">[</bpt>these instructions and example<ept id="p1">](how-to-build-api-clients-from-swagger-for-app-integration.md)</ept>.</source>
        </trans-unit></group></body></file></xliff>