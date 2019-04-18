<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-consume-web-service-interact-in-r.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4a195b9ea05e96df5a2c9867a5be6dc5723e5ef9a.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a195b9ea05e96df5a2c9867a5be6dc5723e5ef9a</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\how-to-consume-web-service-interact-in-r.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Get &amp; consume web services in R with mrsdeploy - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Web service interaction and consumption functions in the mrsdeploy package.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>mrsdeploy package</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>How to interact with and consume web services in R with mrsdeploy</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Machine Learning Server, Microsoft R Server 9.x<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>After a web service has been published or updated, any authenticated user can list, examine, and consume that web service.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>You can do so directly in R using the functions in the <bpt id="p1">[</bpt>mrsdeploy R package<ept id="p1">](../r-reference/mrsdeploy/mrsdeploy-package.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The mrsdeploy R package is installed with both Machine Learning Server and Microsoft R Client.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Also note that application developers can also consume a web service in the <bpt id="p1">[</bpt>language of their choice via Swagger<ept id="p1">](how-to-build-api-clients-from-swagger-for-app-integration.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If you do not want to list, examine, or consume the web service in R, a set of <bpt id="p1">[</bpt>RESTful APIs<ept id="p1">](concept-api.md)</ept> are also available to provide direct programmatic access to a service's lifecycle directly.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>To list, examine, or consume the web service outside of R, use the <bpt id="p1">[</bpt>RESTful APIs<ept id="p1">](concept-api.md)</ept>, which provide direct programmatic access to a service's lifecycle.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Requirements</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Before you can use the functions in the mrsdeploy R package to manage your web services, you must:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Have access to a Machine Learning Server instance that was  <bpt id="p1">[</bpt>properly configured<ept id="p1">](../r-reference/mrsdeploy/mrsdeploy-package.md#configure)</ept> to host web services.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Authenticate with Machine Learning Server using the remoteLogin() or remoteLoginAAD() functions in the mrsdeploy package as described in the article "<bpt id="p1">[</bpt>Connecting to Machine Learning Server to use mrsdeploy<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept>."</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Find and list web services</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Any authenticated user can retrieve a list of web services using the listServices() function in the mrsdeploy package.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Use function arguments to return a specific web service or all labeled versions of a given web service.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>package reference help page for listServices()<ept id="p1">](../r-reference/mrsdeploy/listservices.md)</ept> for the full description of all arguments.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Your ability to see the code inside the web service depends on your permissions.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Did you publish the web service or do you have the "Owner" role?</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If yes, then the code in the service is returned along with other metadata.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If no, then the code in the service is never returned in the metadata.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>To learn more about the roles in your organization, contact your Machine Learning Server administrator.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Response</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>R Function Help</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>listServices(...)</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>R list containing service metadata.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>View<ept id="p1">](../r-reference/mrsdeploy/listservices.md)</ept></source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Once you find the service you want, use <bpt id="p1">[</bpt>the getService() function<ept id="p1">](#getService)</ept> to retrieve the service object for consumption.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Example code:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>For a detailed example with listServices, check out these <bpt id="p1">[</bpt>"Workflow" examples<ept id="p1">](how-to-deploy-web-service-publish-manage-in-r.md#workflow)</ept>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Example output:</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>R Server 9.1+</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>R Server 9.0</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>9.1 output</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>9.0 output</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Retrieve and examine service objects</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Any authenticated user can retrieve a web service object for consumption.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>After the object is returned, you can look at its capabilities to see what the service can do and how it should be consumed.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>After you've authenticated, use the getService() function in the mrsdeploy package to retrieve a service object.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>package reference help page for getService()<ept id="p1">](../r-reference/mrsdeploy/getservice.md)</ept> for the full description of all arguments.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Response</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>R Function Help</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>getService(...)</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Returns an <bpt id="p1">[</bpt>API instance<ept id="p1">](#api-client)</ept> client stub for consuming that service and viewing its service holdings) as an <bpt id="p2">[</bpt>R6<ept id="p2">](https://cran.r-project.org/web/packages/R6/index.html)</ept> class.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>View<ept id="p1">](../r-reference/mrsdeploy/getservice.md)</ept></source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>For a detailed example with getService, check out these <bpt id="p1">[</bpt>"Workflow" examples<ept id="p1">](how-to-deploy-web-service-publish-manage-in-r.md#workflow)</ept>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Interact with API clients</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>When you publish, update, or get a web service, an API instance is returned as an <bpt id="p1">[</bpt>R6<ept id="p1">](https://cran.r-project.org/web/packages/R6/index.html)</ept> class.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>This instance is a client stub you can use to consume that service and view its service holdings.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>You can use the following supported public functions to interact with the API client instance.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>print</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Print method that lists all members of the object</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>capabilities</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Report on the service features such as I/O schema, name, version</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>consume</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Consume the service based on I/O schema</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>consume <bpt id="p1">_</bpt>alias<ept id="p1">_</ept></source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Alias to the consume function for convenience (see alias argument for the <bpt id="p1">[</bpt>publishService function<ept id="p1">](../r-reference/mrsdeploy/publishservice.md)</ept>).</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>swagger</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Displays the service's swagger specification</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>batch</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Define the data records to be batched.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>There are additional publish functions used to <bpt id="p1">[</bpt>consume a service asynchronously via batch execution<ept id="p1">](how-to-consume-web-service-asynchronously-batch.md#public-fx-batch)</ept>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>For a detailed example, check out these <bpt id="p1">[</bpt>"Workflow" examples<ept id="p1">](how-to-deploy-web-service-publish-manage-in-r.md#workflow)</ept>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Consume web services</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Web services are published to facilitate the consumption and integration of the operationalized models and code.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Whenever the web service is published or updated, a Swagger-based JSON file is generated automatically that define the service.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>When you publish a service, you can let people know that it is ready for consumption.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Users can get the Swagger file they need to consume the service directly in R or via the API.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>To make it easy for others to find your service, provide them with the service name and version number (or they can use <bpt id="p1">[</bpt>the listServices() function<ept id="p1">](#listServices)</ept>).</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Users can consume the service directly using a single consumption call.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>This approach is referred to as a "Request Response" approach and is described in the following section.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Another approach is the <bpt id="p1">[</bpt>asynchronous "Batch" consumption approach<ept id="p1">](how-to-consume-web-service-asynchronously-batch.md)</ept>, where users send as a single request to Machine Learning Server, which then makes multiple asynchronous API calls on your behalf.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Collaborate with data scientists</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Other data scientists may want to explore, test, and consume Web services directly in R using the functions in the mrsdeploy package.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Quality engineers might want to bring the models in these web services into validation and monitoring cycles.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>You can share the name and version of a web service with fellow data scientists so they can call that service in R using the functions in the mrsdeploy package.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>After authenticating, data scientists can use the getService() function in R to call the service.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Then, they can get details about the service and start consuming it.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>You can also <bpt id="p1">[</bpt>build a client library directly in R using the httr package<ept id="p1">](https://blogs.msdn.microsoft.com/rserver/2017/07/20/using-r-to-generate-api-client-from-swagger/)</ept>.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>It is also possible to perform batch consumption as <bpt id="p1">[</bpt>described here<ept id="p1">](how-to-consume-web-service-asynchronously-batch.md)</ept>.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>In this example, replace the following remoteLogin() function with the correct login details for your configuration.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Connecting to Machine Learning Server using the mrsdeploy package is covered <bpt id="p1">[</bpt>in this article<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept>.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Collaborate with application developers</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Application developers can call and integrate a web service into their applications using the service-specific Swagger-based JSON file and by providing any required inputs to that service.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Using the Swagger-based JSON file, application developers can generate client libraries for integration.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Read "<bpt id="p1">[</bpt>How to integrate web services and authentication into your application<ept id="p1">](how-to-build-api-clients-from-swagger-for-app-integration.md)</ept>" for more details.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Application developers can get the Swagger-based JSON file in one of these ways:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>A data scientist, probably the one who published the service, can send you the Swagger-based JSON file.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>This approach is often faster than the following one.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>They can get the file in R with the following code and send it to the application developer:</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Or, the application developer can request the file  <bpt id="p1">**</bpt>as an authenticated user with an <bpt id="p2">[</bpt>active bearer token<ept id="p2">](how-to-build-api-clients-from-swagger-for-app-integration.md#authentication)</ept> in the request header<ept id="p1">**</ept> (since all API calls must be authenticated).</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>The URL is formed as follows:</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>What is operationalization?<ept id="p1">](../what-is-operationalization.md)</ept></source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>What are web services?<ept id="p1">](../operationalize/concept-what-are-web-services.md)</ept></source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>mrsdeploy function overview<ept id="p1">](../r-reference/mrsdeploy/mrsdeploy-package.md)</ept></source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to publish and manage web services in R<ept id="p1">](how-to-deploy-web-service-publish-manage-in-r.md)</ept></source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Quickstart: Deploying an R model as a web service<ept id="p1">](quickstart-publish-r-web-service.md)</ept></source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Connecting to Machine Learning Server from mrsdeploy<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept>.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to integrate web services and authentication into your application<ept id="p1">](how-to-build-api-clients-from-swagger-for-app-integration.md)</ept></source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Asynchronous batch execution of web services in R<ept id="p1">](how-to-consume-web-service-asynchronously-batch.md)</ept></source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Execute on a remote Machine Learning Server<ept id="p1">](../r/how-to-execute-code-remotely.md)</ept></source>
        </trans-unit></group></body></file></xliff>