<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-application-developer-getting-started.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a81debb937cac2040c27a61382319110445c4e82e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">81debb937cac2040c27a61382319110445c4e82e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-application-developer-getting-started.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Getting Started with DeployR for Application Developers - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Getting started for Application Developers: high level introduction to DeployR for Application Developers</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Application Developers, r programmer, DeployR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Getting Started - Application Developers</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This guide for application developers introduces DeployR, the <bpt id="p1">*</bpt>R Integration Server<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>If you are an application developer or a systems integrator, then this guide explains what DeployR can do for you.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>DeployR exists to solve a number of fundamental integration problems faced by application developers.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>For example, have you ever wondered how you might execute an R script from within a Web-based dashboard, an Excel spreadsheet, an enterprise middleware solution, or a mobile application?</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>DeployR makes it simple:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>In fact, DeployR makes it simple for <bpt id="p1">**</bpt>any application<ept id="p1">**</ept> developed in <bpt id="p2">**</bpt>any language<ept id="p2">**</ept> to:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Provision one or more dedicated R sessions on demand</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Execute R scripts on those R sessions</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Pass inputs (data, files, and so on) when executing those R scripts</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Retrieve outputs (data, files, plots, and so on) following the execution of those R scripts</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>DeployR offers these features and many more through a set of <bpt id="p1">[</bpt>Analytics Web Services<ept id="p1">](#analytics-web-services)</ept>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>These Web service interfaces isolate the application developer and the application itself from R code, from the underlying R sessions, and in fact from all the complexities typically associated with R integration.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>As an application developer, you typically leave R coding and model building to the <bpt id="p1">[</bpt>data scientists<ept id="p1">](deployr-data-scientist-getting-started.md)</ept>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>And now with DeployR, you can also leave all aspects of R session management to the DeployR server.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This frees you up to focus on simple integrations with DeployR services that deliver the <bpt id="p1">[</bpt>phenomenal power of R<ept id="p1">](https://mran.microsoft.com/documents/getting-started/)</ept> directly within your applications.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The sections that follow explain <bpt id="p1">[</bpt>Analytics Web Services<ept id="p1">](#analytics-web-services)</ept> in greater detail and also introduce the set of <bpt id="p2">[</bpt>developer tools<ept id="p2">](#developer-tools)</ept> that make it simple to consume these services within your applications.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>This document also presents a series of <bpt id="p1">[</bpt>tutorials<ept id="p1">](#tutorials)</ept> with sample source code and introduces a complete <bpt id="p2">[</bpt>example application<ept id="p2">](#real-world-example)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>This example gives a concrete demonstration of building a classic application, an R analytics real-time scoring engine.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>For a general introduction to DeployR, read the <bpt id="p1">[</bpt>About DeployR<ept id="p1">](deployr-about.md)</ept> document.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Analytics Web Services</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The DeployR R Integration server exposes a rich set of services to application developers through a public Web services API.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>These services are collectively known as DeployR Analytics Web services.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>While the complete technical specification for all available services can be found <bpt id="p1">[</bpt>here<ept id="p1">](deployr-api-reference.md)</ept>, this <bpt id="p2">*</bpt>Getting Started<ept id="p2">*</ept> guide for application developers focuses on introducing the core services.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>R Session Services</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Perhaps not surprisingly, one of the core services provided by DeployR is the ability for any application to create one or more R sessions on demand.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Once an application has created an R session, it can:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Pass data into the session</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Execute R scripts and code on the session</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Retrieve data, files and plots from the session</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>DeployR typically refers to R sessions as <ph id="ph1">`projects`</ph>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>You can read more about projects in the <bpt id="p1">[</bpt>API Reference Guide<ept id="p1">](deployr-api-reference.md)</ept>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Depending on the specific needs of your application, the R sessions created by your application can be:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Stateless, meaning they exist for the duration of a single R script execution request</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Temporary, meaning they exist for a single user session in your application</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Persistent, meaning they exist across multiple user sessions in your application</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Your application can also request the activation of an R session at a scheduled time in order to execute an R script or block of R code based on some schedule that befits your application.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>A key takeaway here is that DeployR is very flexible in the services that it offers, which makes it a compelling R integration solution for just about any application you can imagine.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Repository Services</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Having access to on-demand R sessions within your application is only useful if you have access to the R scripts, models, and data you want to manipulate within those sessions.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>For this reason, DeployR exposes a comprehensive set of file and directory management services known as DeployR repository services.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Read more about these <bpt id="p1">[</bpt>repository services in the API Reference Guide<ept id="p1">](deployr-api-reference.md)</ept>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>You can think of the DeployR repository as a file system that is owned and managed by the DeployR server.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>As an application developer, you can:</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Store files of any type in the repository</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Create and manage custom directories for those files in the repository:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>These services are available on the <bpt id="p1">[</bpt>API<ept id="p1">](deployr-api-reference.md#repository)</ept> and also through the Web-based <bpt id="p2">[</bpt>Repository Manager<ept id="p2">](deployr-repository-manager-about.md)</ept>, which ships with DeployR.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>It is also simple for your application to request files be moved from the repository to your R sessions and from your R sessions back into the repository.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Perhaps most importantly, any R script stored in the repository is automatically exposed as a live, executable Analytics Web service.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>This means your R scripts can be executed on request by your application just by referencing that script by name.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Auth Services</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The fact that repository-managed R scripts are automatically exposed as live, executable Web services raises an important question:</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>"How can you enforce access controls on this type of Web service?"</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>The answer is simple.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>DeployR supports a broad set of access controls ranging from <bpt id="p1">[</bpt>user authentication and authorization<ept id="p1">](deployr-api-reference.md#users)</ept> to a set of <bpt id="p2">[</bpt>access controls enforced on a file-by-file basis<ept id="p2">](deployr-repository-manager-files.md#about-file-properties)</ept> in the repository.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The access control options available on repository files are:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>, allows access only to the file's owner.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>, allows access only to those users who were granted at least one of the associated roles</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>, allows access only to authenticated users</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>, allows access to any authenticated or anonymous user</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>These repository access controls can be manipulated directly by the file owner on the <bpt id="p1">[</bpt>API<ept id="p1">](deployr-api-reference.md)</ept> or by using the Web-based <bpt id="p2">[</bpt>Repository Manager<ept id="p2">](deployr-repository-manager-about.md)</ept> that ships with DeployR.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Developer Tools</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>It's time to move from theory into practice.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>And for an application developer, that means writing code.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>The best place to begin is with the <bpt id="p1">[</bpt>RBroker Framework<ept id="p1">](deployr-rbroker-framework.md)</ept>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>This framework exposes a simple yet powerful integration model that requires only a little code in order to deliver significant analytics capabilities within your application.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>RBroker Framework</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>What is the RBroker Framework?</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Let's start with a small code snippet that delivers big results.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>The above snippet demonstrates how, in just a few lines of code, your application can create one or more R sessions on which it can immediately start executing R tasks.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The framework handles all of the low-level details, including:</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>R session provisioning</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Client-side task queuing</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Server-side task execution</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Asynchronous callbacks to your application on task completion</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>If you are a Java, JavaScript or .NET developer, start with the official <bpt id="p1">[</bpt>RBroker Framework tutorial<ept id="p1">](deployr-rbroker-framework.md)</ept>.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>It introduces everything you need to know to get up and running, including framework download links.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>If developing in another language, go directly <bpt id="p1">[</bpt>here<ept id="p1">](#api-specification)</ept>.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Client Library</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>What if the <bpt id="p1">[</bpt>RBroker Framework<ept id="p1">](#rbroker-framework)</ept> doesn't give me everything I need?</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>They may be times when you need direct access to some of the lower-level services on DeployR, which are not exposed by the RBroker Framework.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>In such cases, if you are a Java, JavaScript or .NET developer, then you can work directly with the DeployR client libraries.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Learn more in the official <bpt id="p1">[</bpt>Client Library tutorial<ept id="p1">](deployr-client-library.md)</ept>, which introduces everything you need to know to get up and running, including library download links.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>If developing in another language, go directly <bpt id="p1">[</bpt>here<ept id="p1">](#api-specification)</ept>.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>API Specification</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>What if I'm not a Java, JavaScript or .NET developer?</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>What if I simply want to understand more about what's going on 'under the hood'?</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Then, the answer is the <bpt id="p1">[</bpt>underlying technical specification<ept id="p1">](https://microsoft.github.io/deployr-api-docs/8.0.5/)</ept> for DeployR.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>That specification details every API call, associated call parameters, encodings, error handling, and more on the DeployR API.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>As long as your development environment can establish HTTP(S) connections and consumes JSON, then you can integrate directly with DeployR services using the public <bpt id="p1">[</bpt>API<ept id="p1">](deployr-api-reference.md)</ept>.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Tutorials</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">[</bpt>Developer Tools<ept id="p1">](#developer-tools)</ept> section, you began your move from theory into practice through the introduction of the core tools and some initial fragments of sample code.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>To further bootstrap the learning process, we've written some more code for you.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>In fact, we've written a lot of code for you in the form of tutorials with which you can see the key concepts put into practice.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>To run these tutorials, you will need access to a live instance of the DeployR server.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>RBroker Framework Tutorials</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>The following tutorials are available:</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>RBroker Framework Basics<ept id="p1">](https://github.com/Microsoft/java-example-rbroker-basics)</ept> code tutorial demonstrates the basic programming model and capabilities of the RBroker Framework.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Each code example brings to life the ideas introduced by the basic <bpt id="p1">[</bpt>RBroker Tutorial<ept id="p1">](deployr-rbroker-framework.md)</ept>.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>RBroker Framework Data I/O<ept id="p1">](https://github.com/Microsoft/java-example-rbroker-data-io)</ept> code tutorial demonstrates how different types of data inputs and outputs can be sent to and retrieved from DeployR-managed R sessions when you execute tasks using the framework.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Client Library Tutorials</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>The following tutorials are available:</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>Client Library Basics<ept id="p1">](https://github.com/Microsoft/java-example-client-basics)</ept> code tutorial demonstrates a wide range of basic functionalities available on the DeployR client library.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Each code example brings to life the ideas introduced by the basic <bpt id="p1">[</bpt>Client Library Tutorial<ept id="p1">](deployr-client-library.md)</ept>.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>Client Library Data I/O<ept id="p1">](https://github.com/Microsoft/java-example-client-data-io)</ept> code tutorial demonstrates how different types of data inputs and outputs can be sent to and retrieved from DeployR-managed R sessions when you execute R scripts or code using the client library.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Command Line Interface</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>While each of the DeployR code tutorials found on GitHub provides their own complete set of instructions for downloading and running the code, we also provide the <bpt id="p1">[</bpt>DeployR CLI<ept id="p1">](https://github.com/Microsoft/deployr-cli)</ept> to make running these tutorials even easier.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>The DeployR CLI is a <bpt id="p1">[</bpt>Command Line Tool (CLI)<ept id="p1">](https://en.wikipedia.org/wiki/Command-line_interface)</ept> for running useful DeployR utilities, such as the automated installation and execution of any <bpt id="p2">[</bpt>DeployR code tutorial<ept id="p2">](#tutorials)</ept> found on GitHub.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Install and use the CLI as follows:</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Install the CLI using <bpt id="p1">[</bpt>npm<ept id="p1">](https://www.npmjs.com/)</ept>.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>At your terminal prompt, type:</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>You now have the <ph id="ph1">`di`</ph> command in your system path, thereby allowing the CLI to be run from any location.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Start the CLI.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>At your terminal prompt, type:</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>DeployR CLI</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>From the CLI main menu, choose <bpt id="p1">**</bpt>Install an example<ept id="p1">**</ept> to see the complete list of available examples, including all of the latest DeployR code tutorials found on GitHub.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Select the example to install.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>That example is automatically downloaded, installed and launched in your terminal window.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Real World Example</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>Developer Tools<ept id="p1">](#developer-tools)</ept> section introduced the available tool set and some initial fragments of sample code.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">[</bpt>Tutorials<ept id="p1">](#tutorials)</ept> section, you were introduced to more complete sample code that highlighted some important design patterns when working with DeployR.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>In this section you will be introduced to a complete sample application that demonstrates one approach to building an end-to-end solution using DeployR.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>The sample application is a classic application in the analytics space, a real-time scoring engine powered by DeployR.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>The example scenario mimics a real world application where employees at a fictitious bank can request fraud scores for one or more bank account records on-demand in order to help detect fraudulent account activity:</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Fraud Score Example Application</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Note, as this is a sample application the Web browser UI component has been implemented to display profiling information on the <bpt id="p1">[</bpt>RBroker's real-time performance<ept id="p1">](deployr-rbroker-framework.md#client-application-profiling)</ept>.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>This functionality is provided as an aid to application developers, but is not something that would typically be included in a true production application.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>In keeping with the recommended approach to building DeployR-enabled solutions, a data scientist developed the scoring function and predictive model used by this application <bpt id="p1">[</bpt>data scientist<ept id="p1">](deployr-data-scientist-getting-started.md)</ept> and an application developer wrote the application itself.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>The application design overview, source code in both Java and JavaScript, and the associated instructions needed to run the fraud score application can be found <bpt id="p1">[</bpt>on GitHub<ept id="p1">](https://github.com/Microsoft/java-example-fraud-score)</ept>.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Check it out, and post any questions you have directly to the <bpt id="p1">[</bpt>DeployR Forum<ept id="p1">](https://social.msdn.microsoft.com/Forums/en-US/home?forum=microsoftr)</ept>.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>More Resources</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Use the table of contents to find all of the guides and documentation needed by Application Developers.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>API Docs, Tools, and Samples</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>RBroker Framework and Client Library</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>API Reference Guide</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Other Getting Started Guides</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Administrators</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Data Scientists</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Helper Tools</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>DeployR Command Line Tool (CLI)</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Repository Manager<ept id="p1">](deployr-repository-manager-about.md)</ept>, available on the DeployR landing page following an install.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>API Interactive Explorer<ept id="p1">](deployr-api-explorer-tool.md)</ept>, available on the DeployR landing page following an install.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Support Channels</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>Microsoft R Server (and DeployR) Forum</source>
        </trans-unit></group></body></file></xliff>