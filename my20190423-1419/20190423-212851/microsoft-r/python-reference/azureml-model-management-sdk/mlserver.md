<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="mlserver.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a400ba4ae6ce1f43ff378a20c1c007d7c64d266b6.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">400ba4ae6ce1f43ff378a20c1c007d7c64d266b6</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\azureml-model-management-sdk\mlserver.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>MLServer class: from azureml-model-management-sdk – Machine Learning Server | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve">
          <source>Class MLServer</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>MLServer</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Bases: <bpt id="p1">[</bpt><ph id="ph1">`azureml.deploy.operationalization.Operationalization`</ph><ept id="p1">](operationalization.md)</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>This module provides a service implementation for the ML Server.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>authentication</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Override</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Authentication lifecycle method called by the framework.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Invokes the authentication entry-point for the class hierarchy.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>ML Server supports two forms of authentication contexts:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>LDAP: tuple <bpt id="p1">*</bpt>(username, password)<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Azure Active Directory (AAD): dict <bpt id="p1">*</bpt>{…}<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>access-token: str <bpt id="p1">*</bpt>=4534535<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>context</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The authentication context: LDAP, Azure Active Directory (AAD), or existing <bpt id="p1">*</bpt>access-token<ept id="p1">*</ept> string.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>HttpException</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If an HTTP fault occurred calling the ML Server.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>create_or_update_service_pool</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Creates or updates the pool for the published web service, with given initial and maximum pool sizes on the ML Server by <bpt id="p1">*</bpt>name<ept id="p1">*</ept> and <bpt id="p2">*</bpt>version<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The unique web service name.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>version</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The web service version.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>initial_pool_size</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The initial pool size for the web service.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>max_pool_size</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The max pool size for the web service.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>This cannot be less than initial_pool_size.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>requests.models.Response: HTTP Status indicating if the request was submitted successfully or not.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>HttpException</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If an HTTP fault occurred calling the ML Server.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>delete_service</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Delete a web service.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The web service name.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>opts</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The web service version (<bpt id="p1">*</bpt>version=’v1.0.1<ept id="p1">*</ept>).</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>A <ph id="ph1">`bool`</ph> indicating the service deletion was succeeded.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>HttpException</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If an HTTP fault occurred calling the ML Server.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>delete_service_pool</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Delete the pool for the published web service on the ML Server by <bpt id="p1">*</bpt>name<ept id="p1">*</ept> and <bpt id="p2">*</bpt>version<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The unique web service name.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>version</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The web service version.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>requests.models.Response: HTTP Status if the pool was deleted for the service.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>HttpException</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If an HTTP fault occurred calling the ML Server.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>deploy_realtime</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Publish a new <bpt id="p1">*</bpt>real-time<ept id="p1">*</ept> web service on the ML Server by <bpt id="p2">*</bpt>name<ept id="p2">*</ept> and <bpt id="p3">*</bpt>version<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>All input and output types are defined as a <ph id="ph1">`pandas.DataFrame`</ph>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>NOTE:<ept id="p1">**</ept> Using <bpt id="p2">*</bpt>deploy_realtime()<ept id="p2">*</ept> in this fashion is identical to publishing a service using the fluent APIS <bpt id="p3">[</bpt><ph id="ph1">`deploy()`</ph><ept id="p3">](realtime-definition.md)</ept></source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>The web service name.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>opts</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The service properties to publish as a <ph id="ph1">`dict`</ph>.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>opts<ept id="p1">*</ept> supports the following optional properties:</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>version (str) - Defines a unique alphanumeric web service version.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>If the version is left blank, a unique <bpt id="p1">*</bpt>guid<ept id="p1">*</ept> is generated in its place.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Useful during service development before the author is ready to officially publish a semantic version to share.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>description (str) - The service description.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>alias (str) - The consume function name.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Defaults to <bpt id="p1">*</bpt>consume<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>A new instance of <bpt id="p1">[</bpt><ph id="ph1">`Service`</ph><ept id="p1">](service.md)</ept> representing the real-time service <bpt id="p2">*</bpt>redeployed<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>HttpException</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>If an HTTP fault occurred calling the ML Server.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>deploy_service</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Publish a new web service on the ML Server by <bpt id="p1">*</bpt>name<ept id="p1">*</ept> and <bpt id="p2">*</bpt>version<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>NOTE:<ept id="p1">**</ept> Using <ph id="ph1">`deploy_service()`</ph> in this fashion is identical to publishing a service using the fluent APIS <bpt id="p2">[</bpt><ph id="ph2">`deploy()`</ph><ept id="p2">](service-definition.md)</ept>.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>The unique web service name.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>opts</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>The service properties to publish.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>opts<ept id="p1">*</ept> dict supports the following optional properties:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>version (str) - Defines a unique alphanumeric web service version.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>If the version is left blank, a unique <bpt id="p1">*</bpt>guid<ept id="p1">*</ept> is generated in its place.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Useful during service development before the author is ready to officially publish a semantic version to share.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>description (str) - The service description.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>code_str (str) - A block of python code to run and evaluate.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>init_str (str) - A block of python code to initialize service.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>code_fn (function) - A Function to run and evaluate.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>init_fn (function) - A Function to initialize service.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>objects (dict) - Name and value of <bpt id="p1">*</bpt>objects<ept id="p1">*</ept> to include.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>models (dict) - Name and value of <bpt id="p1">*</bpt>models<ept id="p1">*</ept> to include.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>inputs (dict) - Service input schema by <bpt id="p1">*</bpt>name<ept id="p1">*</ept> and <bpt id="p2">*</bpt>type<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>The following types are supported:</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>int</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>float</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>str</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>bool</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>numpy.array</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>numpy.matrix</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>pandas.DataFrame</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>outputs (dict) - Defines the web service output schema.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>If empty, the service will not return a response value.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>outputs<ept id="p1">*</ept> are defined as a dictionary <ph id="ph1">`{'x'=int}`</ph> or <ph id="ph2">`{'x': 'int'}`</ph> that describes the output parameter names and their corresponding data <bpt id="p2">*</bpt>types<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>The following types are supported:</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>int</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>float</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>str</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>bool</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>numpy.array</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>numpy.matrix</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>pandas.DataFrame</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>artifacts (list) - A collection of file artifacts to return.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>File content is encoded as a <bpt id="p1">*</bpt>Base64 String<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>alias (str) - The consume function name.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Defaults to <bpt id="p1">*</bpt>consume<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>code_fn<ept id="p1">*</ept> function is provided, then it will use that function name by default.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>A new instance of <bpt id="p1">[</bpt><ph id="ph1">`Service`</ph><ept id="p1">](service.md)</ept> representing the service <bpt id="p2">*</bpt>deployed<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>HttpException</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>If an HTTP fault occurred calling the ML Server.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>destructor</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Override</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Destroy lifecycle method called by the framework.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Invokes destructors for the class hierarchy.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>get_service</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Get a web service for consumption.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>The web service name.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>opts</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>The optional web service version.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`version=None`</ph> the most recent service will be returned.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>A new instance of <bpt id="p1">[</bpt><ph id="ph1">`Service`</ph><ept id="p1">](service.md)</ept>.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>HttpException</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>If an HTTP fault occurred calling the ML Server.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>get_service_pool_status</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Get status of pool on each compute node of the ML Server for the published services with the provided <bpt id="p1">*</bpt>name<ept id="p1">*</ept> and <bpt id="p2">*</bpt>version<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>The unique web service name.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>version</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>The web service version.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>str: json representing the status of pool on each compute node for the deployed service.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>HttpException</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>If an HTTP fault occurred calling the ML Server.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Override</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Init lifecycle method called by the framework, invoked during construction.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Sets up attributes and invokes initializers for the class hierarchy.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>http_client</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>The http request session to manage and persist settings across requests (auth, proxies).</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>config</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>The global configuration.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>adapters</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>A <ph id="ph1">`dict`</ph> of transport adapters by url.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>list_services</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>List the different published web services on the ML Server.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>The service <bpt id="p1">*</bpt>name<ept id="p1">*</ept> and service <bpt id="p2">*</bpt>version<ept id="p2">*</ept> are optional.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>This call allows you to retrieve service information regarding:</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>All services published</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>All versioned services for a specific named service</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>A specific version for a named service</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>Users can use this information along with the <ph id="ph1">`[get_service()](#getservice)`</ph> operation to interact with and consume the web service.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>The web service name.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>opts</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>The optional web service version.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>A <ph id="ph1">`list`</ph> of service metadata.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>HttpException</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>If an HTTP fault occurred calling the ML Server.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>realtime_service</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>Begin fluent API chaining of properties for defining a <bpt id="p1">*</bpt>real-time<ept id="p1">*</ept> web service.</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>The web service name.</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt><ph id="ph1">`RealtimeDefinition`</ph><ept id="p1">](realtime-definition.md)</ept> instance for fluent API chaining.</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>redeploy_realtime</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>Updates properties on an existing <bpt id="p1">*</bpt>real-time<ept id="p1">*</ept> web service on the Server by <bpt id="p2">*</bpt>name<ept id="p2">*</ept> and <bpt id="p3">*</bpt>version<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`version=None`</ph> the most recent service will be updated.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>All input and output types are defined as a <ph id="ph1">`pandas.DataFrame`</ph>.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>NOTE:<ept id="p1">**</ept> Using <bpt id="p2">*</bpt>redeploy_realtime()<ept id="p2">*</ept> in this fashion is identical to updating a service using the fluent APIS <bpt id="p3">[</bpt><ph id="ph1">`redeploy()`</ph><ept id="p3">](realtime-definition.md)</ept></source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>The web service name.</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>opts</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>The service properties to update as a <ph id="ph1">`dict`</ph>.</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>opts<ept id="p1">*</ept> supports the following optional properties:</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>version (str) - Defines the web service version.</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>description (str) - The service description.</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>alias (str) - The consume function name.</source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>Defaults to <bpt id="p1">*</bpt>consume<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source>A new instance of <bpt id="p1">[</bpt><ph id="ph1">`Service`</ph><ept id="p1">](service.md)</ept> representing the real-time service <bpt id="p2">*</bpt>redeployed<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>HttpException</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>If an HTTP fault occurred calling the ML Server.</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>redeploy_service</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>Updates properties on an existing web service on the ML Server by <bpt id="p1">*</bpt>name<ept id="p1">*</ept> and <bpt id="p2">*</bpt>version<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`version=None`</ph> the most recent service will be updated.</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>NOTE:<ept id="p1">**</ept> Using <bpt id="p2">*</bpt>redeploy_service()<ept id="p2">*</ept> in this fashion is identical to updating a service using the fluent APIS <bpt id="p3">[</bpt><ph id="ph1">`redeploy()`</ph><ept id="p3">](service-definition.md)</ept></source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>The web service name.</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source>opts</source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source>The service properties to update as a <ph id="ph1">`dict`</ph>.</source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>opts<ept id="p1">*</ept> supports the following optional properties:</source>
        </trans-unit><trans-unit id="324" translate="yes" xml:space="preserve">
          <source>version (str) - Defines a unique alphanumeric web service version.</source>
        </trans-unit><trans-unit id="325" translate="yes" xml:space="preserve">
          <source>If the version is left blank, a unique <bpt id="p1">*</bpt>guid<ept id="p1">*</ept> is generated in its place.</source>
        </trans-unit><trans-unit id="326" translate="yes" xml:space="preserve">
          <source>Useful during service development before the author is ready to officially publish a semantic version to share.</source>
        </trans-unit><trans-unit id="327" translate="yes" xml:space="preserve">
          <source>description (str) - The service description.</source>
        </trans-unit><trans-unit id="328" translate="yes" xml:space="preserve">
          <source>code_str (str) - A block of python code to run and evaluate.</source>
        </trans-unit><trans-unit id="329" translate="yes" xml:space="preserve">
          <source>init_str (str) - A block of python code to initialize service.</source>
        </trans-unit><trans-unit id="330" translate="yes" xml:space="preserve">
          <source>code_fn (function) - A Function to run and evaluate.</source>
        </trans-unit><trans-unit id="331" translate="yes" xml:space="preserve">
          <source>init_fn (function) - A Function to initialize service.</source>
        </trans-unit><trans-unit id="332" translate="yes" xml:space="preserve">
          <source>objects (dict) - Name and value of <bpt id="p1">*</bpt>objects<ept id="p1">*</ept> to include.</source>
        </trans-unit><trans-unit id="333" translate="yes" xml:space="preserve">
          <source>models (dict) - Name and value of <bpt id="p1">*</bpt>models<ept id="p1">*</ept> to include.</source>
        </trans-unit><trans-unit id="334" translate="yes" xml:space="preserve">
          <source>inputs (dict) - Service input schema by <bpt id="p1">*</bpt>name<ept id="p1">*</ept> and <bpt id="p2">*</bpt>type<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="335" translate="yes" xml:space="preserve">
          <source>The following types are supported: - int - float - str - bool - numpy.array - numpy.matrix - pandas.DataFrame</source>
        </trans-unit><trans-unit id="336" translate="yes" xml:space="preserve">
          <source>outputs (dict) - Defines the web service output schema.</source>
        </trans-unit><trans-unit id="337" translate="yes" xml:space="preserve">
          <source>If empty, the service will not return a response value.</source>
        </trans-unit><trans-unit id="338" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>outputs<ept id="p1">*</ept> are defined as a dictionary <ph id="ph1">`{'x'=int}`</ph> or <ph id="ph2">`{'x': 'int'}`</ph> that describes the output parameter names and their corresponding data <bpt id="p2">*</bpt>types<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="339" translate="yes" xml:space="preserve">
          <source>The following types are supported: - int - float - str - bool - numpy.array - numpy.matrix - pandas.DataFrame</source>
        </trans-unit><trans-unit id="340" translate="yes" xml:space="preserve">
          <source>artifacts (list) - A collection of file artifacts to return.</source>
        </trans-unit><trans-unit id="341" translate="yes" xml:space="preserve">
          <source>File content is encoded as a <bpt id="p1">*</bpt>Base64 String<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="342" translate="yes" xml:space="preserve">
          <source>alias (str) - The consume function name.</source>
        </trans-unit><trans-unit id="343" translate="yes" xml:space="preserve">
          <source>Defaults to <bpt id="p1">*</bpt>consume<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="344" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>code_fn<ept id="p1">*</ept> function is provided, then it will use that function name by default.</source>
        </trans-unit><trans-unit id="345" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="346" translate="yes" xml:space="preserve">
          <source>A new instance of <bpt id="p1">[</bpt><ph id="ph1">`Service`</ph><ept id="p1">](service.md)</ept> representing the service <bpt id="p2">*</bpt>deployed<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="347" translate="yes" xml:space="preserve">
          <source>HttpException</source>
        </trans-unit><trans-unit id="348" translate="yes" xml:space="preserve">
          <source>If an HTTP fault occurred calling the ML Server.</source>
        </trans-unit><trans-unit id="349" translate="yes" xml:space="preserve">
          <source>service</source>
        </trans-unit><trans-unit id="350" translate="yes" xml:space="preserve">
          <source>Begin fluent API chaining of properties for defining a <bpt id="p1">*</bpt>standard<ept id="p1">*</ept> web service.</source>
        </trans-unit><trans-unit id="351" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="352" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="353" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="354" translate="yes" xml:space="preserve">
          <source>The web service name.</source>
        </trans-unit><trans-unit id="355" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="356" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt><ph id="ph1">`ServiceDefinition`</ph><ept id="p1">](service-definition.md)</ept> instance for fluent API chaining.</source>
        </trans-unit></group></body></file></xliff>