<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-deploy-web-service-publish-manage-in-r.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc77501eb1e39cfb410602761ef67a5ef91d390548aa4c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1eb1e39cfb410602761ef67a5ef91d390548aa4c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\how-to-deploy-web-service-publish-manage-in-r.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Deploy &amp; manage web services in R with mrsdeploy - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Web service deployment functions in the mrsdeploy package in Microsoft R can be used for any arbitrary R code block.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>mrsdeploy package</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>How to publish and manage R web services in Machine Learning Server with mrsdeploy</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Applies to:  Machine Learning Server, Microsoft R Server 9.x</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This article details how you can publish and manage your <bpt id="p1">[</bpt>analytic web services<ept id="p1">](concept-what-are-web-services.md)</ept> directly in R. You can deploy your R models, scripts, and code as web services using the functions in the <bpt id="p2">[</bpt>mrsdeploy R package<ept id="p2">](../r-reference/mrsdeploy/mrsdeploy-package.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The mrsdeploy R package containing these functions is installed with both Machine Learning Server (and Microsoft R Server) and Microsoft R Client.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>These web services can be <bpt id="p1">[</bpt>consumed in R<ept id="p1">](how-to-consume-web-service-interact-in-r.md)</ept> by other authenticated users or in the <bpt id="p2">[</bpt>language of their choice via Swagger<ept id="p2">](how-to-build-api-clients-from-swagger-for-app-integration.md)</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Using the mrsdeploy R package, you can <bpt id="p1">[</bpt>publish<ept id="p1">](#publishService)</ept>, <bpt id="p2">[</bpt>update<ept id="p2">](#updateService)</ept>, and  <bpt id="p3">[</bpt>delete<ept id="p3">](#deleteService)</ept> two kinds of R web services: <bpt id="p4">[</bpt>standard R web services and real-time R web services<ept id="p4">](concept-what-are-web-services.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Additionally, you can get a <bpt id="p1">[</bpt>list of all services<ept id="p1">](how-to-consume-web-service-interact-in-r.md#listServices)</ept>, retrieve a <bpt id="p2">[</bpt>web service object<ept id="p2">](how-to-consume-web-service-interact-in-r.md#getService)</ept> for consumption, and <bpt id="p3">[</bpt>share services<ept id="p3">](how-to-consume-web-service-interact-in-r.md#consume-service)</ept> with others.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>You can also publish or interact with a web service outside of R using the <bpt id="p1">[</bpt>RESTful APIs<ept id="p1">](concept-api.md)</ept>, which provide direct programmatic access to a service's lifecycle.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Requirements</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Before you can use the web service management functions in the mrsdeploy R package, you must:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Have access to a Machine Learning Server instance that was  <bpt id="p1">[</bpt>properly configured<ept id="p1">](../r-reference/mrsdeploy/mrsdeploy-package.md#configure)</ept> to host web services.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Authenticate with Machine Learning Server using the remoteLogin() or remoteLoginAAD() functions in the mrsdeploy package as described in "<bpt id="p1">[</bpt>Connecting to Machine Learning Server to use mrsdeploy<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept>."</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Permissions for managing web services</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Any authenticated user can:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Update and delete web services they have published</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Retrieve any web service object for consumption</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Retrieve a list of any or all web services</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>While any authenticated user can also publish a web service by default, roles can be used to further control permissions.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Beginning in version 9.1, your administrator can also <bpt id="p1">**</bpt><bpt id="p2">[</bpt>assign role-based authorization<ept id="p2">](configure-roles.md)</ept><ept id="p1">**</ept> to further restrict the permissions around web services to give some users more control over web services than others.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Ask your administrator for details on your role.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Publish and update web services</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>To deploy your analytics, you must publish them as web services in Machine Learning Server.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Once hosted on Machine Learning Server, you can update and manage them.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>They can also be consumed by other users.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Versioning</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Every time a web service is published, a version is assigned to the web service.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Versioning enables users to better manage the release of their web services.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Versions help the users consuming your service to easily identify it.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>At publish time, you can specify an alphanumeric string that is meaningful to the users who consume the service in your organization.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>For example, you could use '2.0', 'v1.0.0', 'v1.0.0-alpha', or 'test-1'.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Meaningful versions are helpful when you intend to share services with others.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>We highly recommend a <bpt id="p1">**</bpt>consistent and meaningful versioning convention<ept id="p1">**</ept> across your organization or team such as <bpt id="p2">[</bpt>semantic versioning<ept id="p2">](http://semver.org/)</ept>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If you do not specify a version, a globally unique identifier (GUID) is automatically assigned by Machine Learning Server.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>These GUID version numbers are harder to remember by the users consuming your services and are therefore less desirable.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Publish service</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>To deploy your analytics, you must publish them as web services in Machine Learning Server.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Once hosted on Machine Learning Server, you can update and manage them.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>They can also be consumed by other users.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>After you've authenticated, use the publishService() function in the mrsdeploy package to publish a web service.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>package reference for publishService()<ept id="p1">](../r-reference/mrsdeploy/publishservice.md)</ept> for the full description of all arguments.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Response</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>R Help</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>publishService(...)</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Returns an <bpt id="p1">[</bpt>API instance<ept id="p1">](how-to-consume-web-service-interact-in-r.md#api-client)</ept> client stub for consuming that service and viewing its service holdings) as an <bpt id="p2">[</bpt>R6<ept id="p2">](https://cran.r-project.org/web/packages/R6/index.html)</ept> class.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>View</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>You can publish web services to a local Machine Learning Server from your command line.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If you <bpt id="p1">[</bpt>create a remote session<ept id="p1">](../r/how-to-execute-code-remotely.md#publish-remote-session)</ept>, you can also publish a web service to a remote Machine Learning Server from your local command line.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Standard web services</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Standard web services<ept id="p1">](concept-what-are-web-services.md)</ept>, like all web services, are identified by their name and version.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Additionally, a standard web service is also defined by any code, models, and any necessary model assets.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>When deploying, you should also define the required inputs and any output the application developers use to integrate the service in their applications.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Additional arguments are possible -- many of which are shown in the following example.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Example of standard web service:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>For a full example, you can also follow the quickstart article "<bpt id="p1">[</bpt>Deploying an R model as a web service<ept id="p1">](quickstart-publish-r-web-service.md)</ept>."</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>You can also see the Workflow examples at the end of this article.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>R source</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Can come from</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>R code</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>- A filepath to a local R script, such as:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph></source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>- A block of R code as a character string, such as:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph></source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>- A function handle, such as:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph></source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph>  <ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph>  <ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph>  <ph id="ph7">&amp;nbsp;</ph><ph id="ph8">&amp;nbsp;</ph></source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph>  <ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph>  <ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph>  <ph id="ph7">&amp;nbsp;</ph><ph id="ph8">&amp;nbsp;</ph></source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph></source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>R model</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>The R model can come from an object or a file-path to an external representation of R objects to be loaded and used with the code, including:</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>- A filepath to an RData file holding the external R objects to be loaded and used with the code, such as:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph></source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>- A filepath to an R file that is evaluated into an environment and loaded, such as:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph></source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>- A model object, such as:</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph></source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Real-time web services</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Real-time web services offer even lower latency to produce results faster and score more models in parallel.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Real-time web services are also identified by their name and version.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>However, unlike standard web services, you cannot specify the following for real-time web services:</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>inputs and outputs (dataframes are assumed)</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>code (only <bpt id="p1">[</bpt>certain models are supported<ept id="p1">](concept-what-are-web-services.md#realtime)</ept>)</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Real-time web services only accept model objects created with the <bpt id="p1">[</bpt>supported functions<ept id="p1">](concept-what-are-web-services.md#realtime)</ept> from packages installed with the product.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Example of real-time service (supported since R Server 9.1):</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">[</bpt>full examples<ept id="p1">](#workflow)</ept>, see the end of this article.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Learn how to get a <bpt id="p1">[</bpt>list of all services<ept id="p1">](how-to-consume-web-service-interact-in-r.md#listServices)</ept>, retrieve a <bpt id="p2">[</bpt>web service object<ept id="p2">](how-to-consume-web-service-interact-in-r.md#getService)</ept> for consumption, and <bpt id="p3">[</bpt>share services<ept id="p3">](how-to-consume-web-service-interact-in-r.md#consume-service)</ept> with others.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Update service</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>To change a web service after you've published it, while retaining the same name and version, use the updateService() function.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>For arguments, specify what needs to change, such as the R code, model, and inputs.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>When you update a service, it overwrites that named version.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>After you've authenticated, use the updateService() function in the mrsdeploy package to update a web service.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>package reference help page for updateService()<ept id="p1">](../r-reference/mrsdeploy/updateservice.md)</ept> for the full description of all arguments.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Response</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>R Help</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>updateService(...)</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Returns an <bpt id="p1">[</bpt>API instance<ept id="p1">](how-to-consume-web-service-interact-in-r.md#api-client)</ept> client stub for consuming that service and viewing its service holdings) as an <bpt id="p2">[</bpt>R6<ept id="p2">](https://cran.r-project.org/web/packages/R6/index.html)</ept> class.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>View</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>If you want to change the name or version number, use the publishService() function instead and specify the new name or version number.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Supported I/O data types</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>The following table lists the supported data types for the <bpt id="p1">[</bpt>publishService<ept id="p1">](#publishService)</ept> and <bpt id="p2">[</bpt>updateService<ept id="p2">](#updateService)</ept> function input and output schemas.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>I/O data types</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Full support?</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>numeric</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Yes</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>integer</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Yes</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>logical</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Yes</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>character</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Yes</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>vector</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Yes</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>matrix</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Partial</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>(Not for logical &amp; character matrices)</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>data.frame</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Yes</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Note: Coercing an object during</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>I/O is a user-defined task</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Delete web services</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>When you no longer want to keep a web service, you can delete it.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Only the user who initially created the web service can use this function.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>After you've authenticated, use the deleteService() function in the mrsdeploy package to delete a web service.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Each web service is uniquely defined by a name and version.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>package reference help page for deleteService()<ept id="p1">](../r-reference/mrsdeploy/deleteservice.md)</ept> for the full description of all arguments.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Response</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>R Help</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>deleteService(...)</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>If it is successful, it returns a success status and message such as <bpt id="p1">_</bpt>"Service mtService version v1.0.0 deleted."<ept id="p1">_</ept></source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>If it fails for any reason, then it stops execution with error message.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>View</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Standard workflow examples</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>The following workflow examples demonstrate how to publish a web service, interact with it, and then consume it.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Each standard web service example uses the same code and models and returns the same results.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>However the code and model are represented in different formats each time, such as R scripts, objects, and files.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>To learn more about standard web services, <bpt id="p1">[</bpt>see here<ept id="p1">](#standard)</ept>.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Before you begin</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Replace the connection details in the remoteLogin() function in each example with the details for your configuration.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Connecting to R Server using the mrsdeploy package is covered <bpt id="p1">[</bpt>in this article<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept>.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>The base path for files is set to your working directory, but you can change that using ServiceOption as follows:</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Specify a different base path for code and model arguments:</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Clear the path and expect the code and model files to be in the current working directory during publishService():</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Clear the path and require a FULLY QUALIFIED path for code and model parameters in publishService():</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>1. R code and model are objects</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>In this example, the code comes from an object (<ph id="ph1">`code = manualTransmission`</ph>) and the model comes from a model object (<ph id="ph2">`model = carsModel`</ph>).</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>For an example of inputs/outputs as dataframes, see <bpt id="p1">[</bpt>"Example 5"<ept id="p1">](#dataframe)</ept>.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>2. R code as object and RData as file</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>In this example, the code is still an object (<ph id="ph1">`code = manualTransmission`</ph>), but the model now comes from a Rdata file (<ph id="ph2">`model = "transmission.RData"`</ph>).</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>The result is still the same as in the first example.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>3. Code and model as R scripts</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>In this example, the code (<ph id="ph1">`code = transmission-code.R,`</ph>) and the model comes from R scripts (<ph id="ph2">`model = "transmission.R"`</ph>).</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>The result is still the same as in the first example.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>4. Code as script and model as a RData file</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>In this example, the code (<ph id="ph1">`code = transmission-code.R,`</ph>) comes from an R script, and the model from an RData file (<ph id="ph2">`model = "transmission.RData"`</ph>).</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>The result is still the same as in the first example.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>5. R code &amp; model as objects, inputs/outputs as dataframes</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>In this example, the code comes from an object (<ph id="ph1">`code = manualTransmission`</ph>) and the model comes from a model object (<ph id="ph2">`model = carsModel`</ph>) as it was in example 1.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>However, in this example, the inputs and outputs are provided in the form of dataframes.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Real-time workflow example</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>In this example, the local model object (<ph id="ph1">`model = kyphosisModel`</ph>) is generated using the <ph id="ph2">`rxLogit`</ph> modeling function in the RevoScaleR package.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>Real-time web services were introduced in R Server 9.1.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>To learn more about the supported model formats, supported product versions, and supported platforms for real-time web services, <bpt id="p1">[</bpt>see here<ept id="p1">](#realtime)</ept>.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>What is operationalization?</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>What are web services?</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>mrsdeploy function overview</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Quickstart: Deploying an R model as a web service</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Connecting to R Server from mrsdeploy<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept>.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>How to interact with and consume web services in R</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>How to integrate web services and authentication into your application</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Asynchronous batch execution of web services in R</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>Execute on a remote Microsoft R Server</source>
        </trans-unit></group></body></file></xliff>