<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-build-api-clients-from-swagger-for-app-integration.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86bdf7b796719c2b1cce51677dcaa645d0474bd032.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">bdf7b796719c2b1cce51677dcaa645d0474bd032</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\how-to-build-api-clients-from-swagger-for-app-integration.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Integrate web services &amp; authentication into applications - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Use Swagger to help integrate your R and Python analytics into your applications.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to add web services and authentication to applications</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies to:  Machine Learning Server, Microsoft R Server 9.x</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Learn how to build and use API Client libraries from Swagger to integrate into your applications.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Swagger is a machine-readable representation of a RESTful API that enables support for interactive documentation, client SDK generation, and discoverability.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>While data scientists can work with R / Python directly in a console window or IDE, application developers often need a different set of tools to leverage R inside applications.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>As an application developer integrating with these web services, typically your interest is in executing R / Python code, not writing it.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Data scientists with the R programming skills write the R / Python code.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Then, using some core APIs, this code can be published as a Machine Learning Server-hosted analytics Web service.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>To simplify the integration of your R / Python analytics web services, Machine Learning Server (formerly R Server) provides <bpt id="p1">[</bpt>Swagger templates<ept id="p1">](http://swagger.io/)</ept> for operationalization.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>These Swagger-based JSON files define the list of calls and resources available in the REST <bpt id="p1">[</bpt>APIs<ept id="p1">](concept-api.md)</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>To access these RESTful APIs outside of R / Python, generate an API client library in your preferred programming language, such as .NET, C#, Java, JS, Python, or node.js.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This library is built with a Swagger tool.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The resulting API client library simplifies the making of calls, encoding of data, and markup response handling on the API.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Swagger workflow</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Swagger Workflow: build api clients from swagger for app integration</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Get the Swagger file</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Machine Learning Server provides a Swagger template to simplify the integration.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>This template defines the available resources in the REST API and defines the operations you can call on those resources.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>A standard set of core operationalization APIs is <bpt id="p1">[</bpt>available and defined<ept id="p1">](https://microsoft.github.io/deployr-api-docs/)</ept> in <ph id="ph1">`mlserver-swagger-&lt;version&gt;.json`</ph>, where <ph id="ph2">&lt;version&gt;</ph> is the 3-digit product version number.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Additionally, another Swagger-based JSON file is generated for each web service version.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>For R Server users, replace mlserver-swagger with rserver-swagger in the filename.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>API<ph id="ph1">&amp;nbsp;</ph>Types</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Corresponding Swagger-based JSON File</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Core<ph id="ph1">&amp;nbsp;</ph>APIs</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Download Swagger file containing the set of core operationalization APIs from <ph id="ph1">`https://microsoft.github.io/deployr-api-docs/&lt;version&gt;/swagger/mlserver-swagger-&lt;version&gt;.json`</ph>, where <ph id="ph2">`&lt;version&gt;`</ph> is the 3-digit product version number.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;bull;</ph> For 9.2.1: <ph id="ph2">https://microsoft.github.io/deployr-api-docs/9.2.1/swagger/mlserver-swagger-9.2.1.json</ph></source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;bull;</ph> For 9.1.0 <ph id="ph2">https://microsoft.github.io/deployr-api-docs/9.1.0/swagger/rserver-swagger-9.1.0.json</ph></source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Service-specific<ph id="ph1">&amp;nbsp;</ph>APIs</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Get the service-specific APIs defined in <ph id="ph1">`swagger.json`</ph> so you can consume that service.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Obtain it directly from the user that published the service or retrieve yourself using 'GET /api/{service}/{version}/swagger.json'.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Build the core client library</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Option 1.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Build using a Swagger code generator</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>To build a client library, run the file through the Swagger code generator, and specify the language you want.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Popular Swagger code generation tools include <bpt id="p1">[</bpt>Azure AutoRest<ept id="p1">](https://github.com/Azure/autorest)</ept> (requires node.js) and <bpt id="p2">[</bpt>Swagger Codegen<ept id="p2">](https://github.com/swagger-api/swagger-codegen)</ept>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Generate Swagger</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Familiarize yourself with the tool so you can generate the API client libraries in your preferred programming language.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If you use AutoRest to generate a C# client library, it might look like the following command:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>where <ph id="ph1">`&lt;version&gt;`</ph> is the 3-digit product version number.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>You can now provide some custom headers and make other changes before using the generated client library stub.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">&lt;a href="https://github.com/Azure/autorest/blob/master/docs/user/cli.md" target="_blank"&gt;</bpt>Command Line Interface<ept id="p1">&lt;/a&gt;</ept> documentation for details regarding different configuration options and preferences.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Option 2.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Build using an online Swagger editor</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>You are not required to install a Swagger code generator on your machine.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Instead, you can  build the client library in your preferred language using an online Swagger editor.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Go to <ph id="ph1">http://editor.swagger.io/</ph>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The editor appears with default contents.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Delete the default contents so the editor is empty.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Open the Swagger file on your local machine in a text editor of your choice.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Copy the Swagger contents to your clipboard.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Switch back to the Swagger site and paste the contents into the online editor.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Click the <bpt id="p1">**</bpt>Generate Client<ept id="p1">**</ept> button on the toolbar.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Choose the language for the client.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>The client library is generated.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Swagger Generate Client Library</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Option 3.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Build using httr package in R</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>You can also build a client library directly in R using the httr package.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Like option 2, this option does not require you to install a Swagger code generator on your machine.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>This is very convenient when you want to publish a web service and immediately generate a client library from the resulting Swagger file.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Learn more in <bpt id="p1">[</bpt>this blog post<ept id="p1">](https://blogs.msdn.microsoft.com/rserver/2017/07/20/using-r-to-generate-api-client-from-swagger/)</ept>.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Add Authentication Workflow Logic</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Keep in mind that all APIs require authentication.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Therefore, all users must authenticate when making an API call using the <ph id="ph1">`POST /login`</ph> API or through Azure Active Directory (AAD).</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>To simplify this process, bearer access tokens are issued so that users need not provide their credentials for every single call.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>This bearer token is a lightweight security token that grants the “bearer” access to a protected resource, in this case, Machine Learning Server's operationalization APIs.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>After a user has provided authentication credentials, the application must validate the user’s bearer token to ensure that authentication was successful.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Learn more about managing these tokens.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Before you interact with the core APIs, you must authenticate, get the bearer access token, and then include the token in each header for each subsequent request.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Azure Active Directory (AAD)</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Add code to pass the AAD credentials, authority, and client ID.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>In turn, AAD issues the token.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Here is an example of Azure Active Directory authentication in CSharp:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Active Directory LDAP or Local Admin</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>For these authentication methods, you must call the <ph id="ph1">`POST /login`</ph> API in order to authenticate.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Now you can pass in the  <ph id="ph1">`username`</ph> and <ph id="ph2">`password`</ph> for the local administrator, or if Active Directory is enabled, pass the LDAP account information.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>In turn, Machine Learning Server issues you a <bpt id="p1">[</bpt>bearer/access token<ept id="p1">](how-to-manage-access-tokens.md)</ept>.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>After authenticated, the user does not need to provide credentials again as long as the token is still valid.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Here is an example of Active Directory/LDAP authentication in CSharp:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Interact with the APIs</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Now that you have generated the client library and added authentication logic to your application, you can interact with the core operationalization APIs.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Example: Core Client Library from Swagger (in CSharp)</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>This example shows how you can use the <ph id="ph1">`mlserver-swagger-9.2.1.json`</ph> swagger file to build a client library to interact with the core operationalization APIs from your application.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>For other versions, get the file from <ph id="ph1">`https://microsoft.github.io/deployr-api-docs/&lt;version&gt;/swagger/mlserver-swagger-&lt;version&gt;.json`</ph> where <ph id="ph2">&lt;version&gt;</ph> is the server product version.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Build and use a core Machine Learning Server 9.2.1 client library from swagger in CSharp and Azure Active Directory authentication:</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Download <ph id="ph1">`mlserver-swagger-9.2.1.json`</ph> from <ph id="ph2">https://microsoft.github.io/deployr-api-docs/9.2.1/swagger/mlserver-swagger-9.2.1.json</ph>.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Build the statically generated client library files for CSharp from the <ph id="ph1">`mlserver-swagger-9.2.1.json`</ph> swagger.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Notice the language is <ph id="ph1">`CSharp`</ph> and the namespace is <ph id="ph2">`IO.Swagger.Client`</ph>.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>In Visual Studio, add the following <ph id="ph1">`NuGet`</ph> package dependencies to your VS project.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Open the Package Manager Console for NuGet and add them with this command:</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Use the statically generated client library files to call the operationalization APIs.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>In your application code, import the required namespace types and create an API client to manage the API calls:</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Add the authentication workflow to your application.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>In this example, the organization has Azure Active Directory.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Since all APIs require authentication, we first need to obtain our <ph id="ph1">`Bearer`</ph> access token such that it can be included in every request header like this:</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>In your application code, insert the following:</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Begin consuming the core operationalization APIs.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Example: Service Consumption Client Library from Swagger (in CSharp)</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>This example shows how you can use the <ph id="ph1">`swagger.json`</ph> swagger file for version 1.0.0 of a service named <ph id="ph2">`transmission`</ph> to build a client library to interact with published service from your application.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Build and use a service consumption client library from swagger in CSharp and Active Directory LDAP authentication:</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Get the <ph id="ph1">`swagger.json`</ph> for the service you want to consume named <ph id="ph2">`transmission`</ph>:</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Build the statically generated client library files for CSharp from the <ph id="ph1">`swagger.json`</ph> swagger.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Notice the language is <ph id="ph1">`CSharp`</ph> and the namespace is <ph id="ph2">`Transmission`</ph>.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>In Visual Studio, add the following <ph id="ph1">`NuGet`</ph> package dependencies to your VS project.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Open the Package Manager Console for NuGet and add them with this command:</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Use the statically-generated client library files to call the operationalization APIs.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>In your application code, import the required namespace types and create an API client to manage the API calls:</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Add the authentication workflow to your application.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>In this example, the organization has Active Directory/LDAP.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Since all APIs require authentication, first get the <ph id="ph1">`Bearer`</ph> access token so it can be included in every request header.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>In your application code, insert the following code:</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Begin consuming the service consumption APIs.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Example in Java</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>The following blog article shows how to create a Java client.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Blog article: REST Calls using PostMan</source>
        </trans-unit></group></body></file></xliff>