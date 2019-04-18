<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-client-library.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c63592f4602df6353a7e4c249c737061246dfc94f.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">63592f4602df6353a7e4c249c737061246dfc94f</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-client-library.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>DeployR Client Library Tutorial - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>DeployR Client Library Tutorial</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Client Library Tutorial</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Introduction</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The DeployR API exposes a wide range of R analytics services to client application developers.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>These services are exposed using standards-based JSON and are delivered as Web services over HTTP(s).</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>This standards-based approach makes it possible to integrate DeployR services within just about any client application environment.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>To further simplify the integration of DeployR services within client applications, several client libraries are provided for Java, JavaScript and .NET developers.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>These native client libraries provide a number of significant advantages over working directly with the raw API, including simplified service calls, encoding of call parameter data, and automatic handling of response markup on the API.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Try Out Our Examples!<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Explore the client library examples for <bpt id="p1">[</bpt>Java, <ept id="p1">](https://github.com/Microsoft/java-example-client-basics)</ept> <bpt id="p2">[</bpt>Javascript,<ept id="p2">](https://github.com/Microsoft/js-client-library/releases)</ept> and <bpt id="p3">[</bpt>.NET.<ept id="p3">](https://github.com/Microsoft/dotnet-client-library)</ept></source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Find them under the <ph id="ph1">`examples`</ph> directory of each Github repository.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Additionally, find more comprehensive examples for <bpt id="p1">[</bpt>Java<ept id="p1">](https://github.com/microsoft/?utf8=%E2%9C%93&amp;query=java-example)</ept> and <bpt id="p2">[</bpt>JavaScript<ept id="p2">](https://github.com/microsoft/?utf8=✓&amp;query=js-example)</ept>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Check out the <bpt id="p1">[</bpt><bpt id="p2">*</bpt>RBroker Framework<ept id="p2">*</ept><ept id="p1">](deployr-tools-and-samples.md)</ept> for a simple yet powerful alternative to working with the client libraries.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The framework handles much of the complexity in building real world client applications so you don't have to.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>API Overview</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>This section briefly introduces the top-level R analytics services exposed on the DeployR API:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>User Services @ /r/user/<ept id="p1">**</ept><ph id="ph1">*</ph></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Providing the basic authentication mechanisms for end-users and client applications that need to avail of <bpt id="p1">[</bpt><bpt id="p2">*</bpt>authenticated services<ept id="p2">*</ept><ept id="p1">](#authenticated-services)</ept> on the API.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Project Services @ /r/project/<ept id="p1">**</ept><ph id="ph1">*</ph></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Providing <bpt id="p1">[</bpt><bpt id="p2">*</bpt>authenticated services<ept id="p2">*</ept><ept id="p1">](#authenticated-services)</ept> related to stateful, and optionally persistent, R session environments and analytics Web service execution.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Background Job Services @ /r/job/<ept id="p1">**</ept><ph id="ph1">*</ph></source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Providing <bpt id="p1">[</bpt><bpt id="p2">*</bpt>authenticated services<ept id="p2">*</ept><ept id="p1">](#authenticated-services)</ept> related to persistent R session environments for scheduled or periodic analytics Web service executions.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Repository Services @ /r/repository/<ept id="p1">**</ept><ph id="ph1">*</ph></source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Providing <bpt id="p1">[</bpt><bpt id="p2">*</bpt>authenticated services<ept id="p2">*</ept><ept id="p1">](#authenticated-services)</ept> related to R script, model and data file persistence plus <bpt id="p3">*</bpt>authenticated<ept id="p3">*</ept> and <bpt id="p4">[</bpt><bpt id="p5">*</bpt>anonymous services<ept id="p5">*</ept><ept id="p4">](#anonymous-services)</ept> related to analytics Web service execution.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>All services on the DeployR API are documented in detail in the <bpt id="p1">[</bpt>API Reference Guide<ept id="p1">](deployr-api-reference.md)</ept>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Hello World Example</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The following code snippets provide the ubiquitous "Hello World" example for the client libraries, demonstrating the basic programming model used when working with the client libraries in Java and JavaScript, and C<ph id="ph1">\#</ph> respectively.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Try Out Our Examples!<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>After downloading the client library, you can find basic examples that complement this tutorial under the <ph id="ph1">`rbroker/examples`</ph> directory.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Additionally, find more comprehensive examples for <bpt id="p1">[</bpt>Java<ept id="p1">](https://github.com/microsoft/?utf8=%E2%9C%93&amp;query=java-example)</ept> and <bpt id="p2">[</bpt>JavaScript<ept id="p2">](https://github.com/microsoft/?utf8=✓&amp;query=js-example)</ept>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Getting Connected</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The first step for any client application developer using the client libraries is to establish a connection with the DeployR server.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>A connection is established as follows:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Authentication</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Once a connection to the DeployR server has been established, the next step for a client application developer is to decide if end users or the application itself needs access to <bpt id="p1">[</bpt><bpt id="p2">*</bpt>authenticated services<ept id="p2">*</ept><ept id="p1">](#api-overview)</ept> on the API.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>authenticated project<ept id="p1">*</ept>, <bpt id="p2">*</bpt>background job<ept id="p2">*</ept> or <bpt id="p3">*</bpt>repository<ept id="p3">*</ept> management services are needed by the application then the application must first authenticate.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If an application only uses <bpt id="p1">[</bpt><bpt id="p2">*</bpt>anonymous services<ept id="p2">*</ept><ept id="p1">](#anonymous-services)</ept>, then the application can operate <bpt id="p3">*</bpt>anonymously<ept id="p3">*</ept>, without ever authenticating.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate how to authenticate using the client libraries:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Authenticated users not only have access to <bpt id="p1">*</bpt>authenticated services<ept id="p1">*</ept> on the API, they also have much broader access to R scripts, models, and data files stored in the repository compared to <bpt id="p2">*</bpt>anonymous<ept id="p2">*</ept> users.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Authenticated Services</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>An <bpt id="p1">*</bpt>authenticated<ept id="p1">*</ept> user or simply an authenticated client application has access to the full range of <bpt id="p2">*</bpt>authenticated services<ept id="p2">*</ept> offered on the DeployR API.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>These services are categorized as follows:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Authenticated Project Services<ept id="p1">](#project-services)</ept></source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Background Job Services<ept id="p1">](#background-job-services)</ept></source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Repository Management Services<ept id="p1">](#repository-services)</ept></source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>The following sections introduce the services themselves and demonstrate how the client libraries make these services available.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Project Services</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>A project is simply a DeployR-managed R session.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Any project created by an authenticated user is referred to as an <bpt id="p1">[</bpt>Authenticated Project<ept id="p1">](deployr-api-reference.md#authenticated-projects)</ept>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>There are three types of <bpt id="p1">*</bpt>authenticated project<ept id="p1">*</ept>:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Temporary Project - a stateful, transient R session offering unrestricted API access that lives only for the duration of the current user HTTP session or until explicitly closed.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>User Blackbox Project - a stateful, transient R session offering restricted API access that lives only for the duration of the current user HTTP session.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Persistent Project - a stateful, persistent R session offering unrestricted API access can live indefinitely, across multiple user HTTP sessions.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Each type of <bpt id="p1">*</bpt>authenticated project<ept id="p1">*</ept> is provided to support distinct workflows within client applications.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Project Services are most easily understood when considered as a collection of related services:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Project Creation Services</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Project Execution Services</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Project Workspace Services</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Project Directory Services</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Project Package Services</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>The following sections demonstrate working with some of the key features associated with each family of services within the client libraries.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>1. Project Creation Services</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>These services support the creation of <bpt id="p1">*</bpt>authenticated projects<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate some of the ways the client libraries make these services available.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>2. Project Execution Services</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>These services support the execution of analytics Web services on <bpt id="p1">*</bpt>authenticated projects<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate some of the ways the client libraries make these services available.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>All executions services support a standard execution model defined on the DeployR API.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>3. Project Workspace Services</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>These services support the manipulation and management of R workspace objects within <bpt id="p1">*</bpt>authenticated projects<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate some of the ways the client libraries make these services available.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>4. Project Directory Services</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>These services support the manipulation and management of R working directory files within <bpt id="p1">*</bpt>authenticated projects<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate some of the ways the client libraries make these services available.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>5. Project Package Services</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>These services support the manipulation and management of R packages within <bpt id="p1">*</bpt>authenticated projects<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate some of the ways the client libraries make these services available.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Background Job Services</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>A background job is simply a request to execute an R analytics Web service in the background, possibly at some future time and date.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>By default, the result of that execution is stored as a <bpt id="p1">*</bpt>persistent project<ept id="p1">*</ept> on behalf of the <bpt id="p2">*</bpt>authenticated<ept id="p2">*</ept> user making the request.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>By default, each background job execution stores its results in a <bpt id="p1">*</bpt>persistent project<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Persistent projects are discussed in the <bpt id="p1">[</bpt><bpt id="p2">*</bpt>Authenticated Project Service<ept id="p2">*</ept><ept id="p1">](#project-services)</ept> section.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Each job moves through a simple lifecycle on the server, starting with submission, followed by queueing, running, and eventually reaching a completion state indicating success or failure.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>The status of each background job can be queried, jobs can be canceled, and when a job completes the <bpt id="p1">*</bpt>authenticated<ept id="p1">*</ept> user that submitted the job can collect the results of the execution.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate some of the ways the client libraries make these services available.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>All executions services support the standard execution model defined on the DeployR API.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Repository Services</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>Repository Manager<ept id="p1">](deployr-repository-manager-about.md)</ept> is a tool, delivered as an easy-to-use Web interface, that serves as a bridge between the R scripts, models, and data created in existing analytics tools and the deployment of that work into the DeployR repository to support the development of client applications and integrations.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>That tool uses the full range of <bpt id="p1">*</bpt>repository services<ept id="p1">*</ept> on the DeployR API to deliver its many <bpt id="p2">*</bpt>file<ept id="p2">*</ept> and *directory-related functionalities.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Your own applications can also leverage these same services as needed.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate some of the ways the client libraries make these services available.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>Working with the Repository APIs<ept id="p1">](deployr-api-reference.md#repository)</ept> chapter for detailed information regarding working with repository-managed files and directories.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Anonymous Services</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>An <bpt id="p1">*</bpt>anonymous<ept id="p1">*</ept> user, being any user that has not authenticated with the DeployR server, only has access to <bpt id="p2">*</bpt>anonymous services<ept id="p2">*</ept> offered on the DeployR API.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>There is just one single services category for <bpt id="p1">*</bpt>anonymous services<ept id="p1">*</ept>, which is <bpt id="p2">[</bpt>Anonymous Project Services<ept id="p2">](#anonymous-services)</ept></source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>A project is simply a DeployR-managed R session.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Any project created by an anonymous user is known as an <bpt id="p1">*</bpt>anonymous project<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>In practice, anonymous projects are automatically created by DeployR on behalf of anonymous users each time they execute an analytics Web service.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>There are two types of <bpt id="p1">*</bpt>anonymous project<ept id="p1">*</ept>:</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Stateless Project - a stateless, transient R session that lives only for the duration of the analytics Web service execution.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>HTTP Blackbox Project - a stateful, transient R session that lives only for the duration of the current user HTTP session.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>While <bpt id="p1">*</bpt>anonymous project services<ept id="p1">*</ept> are provided primarily for <bpt id="p2">*</bpt>anonymous<ept id="p2">*</ept> users, these same service calls are also available to <bpt id="p3">*</bpt>authenticated<ept id="p3">*</ept> users.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate how the client libraries make these services available.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>For further details, see the <bpt id="p1">[</bpt>Anonymous Projects<ept id="p1">](deployr-api-reference.md#r-for-application-developers)</ept> section.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Standard Execution Model</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>The DeployR API supports a standard set of parameters across all execution APIs that are commonly known as the standard execution model.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>A summary of those execution APIs is shown here:</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/project/execute/code<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-project-execute-code)</ept></source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/project/execute/script<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-project-execute-script)</ept></source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/repository/script/execute<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-repository-script-execute)</ept></source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/repository/script/render<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-repository-script-render)</ept></source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/job/submit<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-job-submit)</ept></source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/job/schedule<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-job-schedule)</ept></source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Conceptually this standard set of parameters can be categorized into three groups: <bpt id="p1">*</bpt>pre-execution<ept id="p1">*</ept>, <bpt id="p2">*</bpt>on-execution<ept id="p2">*</ept> and <bpt id="p3">*</bpt>post-execution<ept id="p3">*</ept> parameters.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Pre-Execution Parameters</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>pre-execution<ept id="p1">*</ept> parameters allow the caller to <bpt id="p2">*</bpt>pre-heat<ept id="p2">*</ept> the R session with DeployR-encoded R data, binary R object data, and file data taken from a number of different sources.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate how to use these parameters using the client libraries:</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>On-Execution Parameters</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>on-execution<ept id="p1">*</ept> parameters allow the caller to control certain aspects of the R session environment itself.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate how to use these parameters using the client libraries:</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Post-Execution Parameters</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>post-execution<ept id="p1">*</ept> parameters allow the caller to retrieve data from the R session on the response markup and/or store data from the R session into the repository.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>It is important to note that the <bpt id="p1">*</bpt>post-execution<ept id="p1">*</ept> parameters that support storing data into the repository are only available to <bpt id="p2">*</bpt>authenticated<ept id="p2">*</ept> users on these calls.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate how to use these parameters using the client libraries:</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>R Object Data Encoding</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>DeployR-specific encodings are used to encode R object data passing into and out of the DeployR server.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>Each of the client libraries provides support that simplifies the task of encoding R object data for sending to the DeployR server.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>Encoded R object data can be sent on the <bpt id="p1">*</bpt>inputs<ept id="p1">*</ept> parameter on the following calls:</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/project/execute/code<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-project-execute-code)</ept></source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/project/execute/script<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-project-execute-script)</ept></source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/repository/script/execute<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-repository-script-execute)</ept></source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/repository/script/render<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-repository-script-render)</ept></source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/job/submit<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-job-submit)</ept></source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/job/schedule<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-job-schedule)</ept></source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/project/workspace/push<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-project-workspace-push)</ept></source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>Standard Execution Model<ept id="p1">](#standard-execution-model)</ept> section of this documentation for details describing how DeployR-encoded R object data can be sent using the <bpt id="p2">*</bpt>inputs<ept id="p2">*</ept> parameter on these calls.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>DeployR-specific encodings are provided for the following classes of R object:</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>character, integer, numeric and logical</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>Date, POSIXct, and POSIXlt</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>vector, matrix</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>ordered, factor</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>list, data.frame.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate the mechanism for creating these types of encodings using the client libraries.</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate the mechanism for creating these types of encodings using the client libraries.</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>Web Service API Data Encodings<ept id="p1">](deployr-api-reference.md#encoding)</ept> section for further details.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>R Object Data Decoding</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>DeployR-specific encodings are used to encode R object data passing into and out of the DeployR server.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>Each of the client libraries provides support that simplifies the task of decoding R object data being returned from the DeployR server.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>One or more R objects can be returned as DeployR-encoded objects in the response markup on any of the following execution calls:</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/project/execute/code<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-project-execute-code)</ept></source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/project/execute/script<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-project-execute-script)</ept></source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/repository/script/execute<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-repository-script-execute)</ept></source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/repository/script/render<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-repository-script-render)</ept></source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate the mechanism for requesting DeployR-encoded objects to be returned on these calls:</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>When working with temporary or persistent DeployR projects, R objects can also be returned as DeployR-encoded objects in the response markup on the following workspace call:</source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>/r/project/workspace/get<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/#r-project-workspace-get)</ept></source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>The following code snippet demonstrates the mechanism for requesting DeployR-encoded objects to be returned on this call:</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>Encodings are provided for the following classes of R object:</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>character, integer, numeric and logical</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>Date, POSIXct, and POSIXlt</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>vector, matrix</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source>ordered, factor</source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>list, data.frame.</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source>The method for decoding these DeployR-encoded objects within a client application depends on the specific client library being used.</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate the mechanism for decoding R objects in order to retrieve their values using the client libraries:</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Java:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>JavaScript:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>C#:<ept id="p1">**</ept></source>
        </trans-unit></group></body></file></xliff>