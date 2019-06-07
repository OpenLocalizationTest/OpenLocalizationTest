<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-rbroker-framework.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c372bb6504222ac7fae9490f256efcae0d85c1cab5e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">2bb6504222ac7fae9490f256efcae0d85c1cab5e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-rbroker-framework.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>DeployR RBroker Framework Tutorial - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>The tutorial for DeployR's RBroker framework</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>DeployR, tutorial, RBroker, framework</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RBroker Framework Tutorial</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Introduction</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The RBroker Framework is the simplest way to integrate DeployR-enabled analytics Web services inside any Java, JavaScript or .NET application.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>This document introduces the basic building blocks exposed by the framework, explains the programming model encouraged by the framework, and demonstrates the framework in action using language-specific code samples.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The RBroker Framework is designed to support transactional, on-demand analytics, where each invocation on an analytics Web service is a standalone operation that executes on a stateless R session environment.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If your application requires a long-lived stateful R session environment, then please see the <bpt id="p1">[</bpt>DeployR Client Libraries<ept id="p1">](deployr-tools-and-samples.md)</ept>, which offer support for stateful operations on DeployR-managed Projects.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Try Out Our Examples!</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Explore the RBroker Framework examples for <bpt id="p1">[</bpt>Java,<ept id="p1">](https://github.com/deployr/java-example-rbroker-basics)</ept> <bpt id="p2">[</bpt>Javascript,<ept id="p2">](https://github.com/deployr/js-rbroker-framework)</ept> and <bpt id="p3">[</bpt>.NET.<ept id="p3">](https://github.com/deployr/dotnet-rbroker-framework)</ept></source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Find them under the <ph id="ph1">`examples`</ph> directory of each GitHub repository.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Additional sample applications are also <bpt id="p1">[</bpt>available on GitHub.<ept id="p1">](http://github.com/deployr?query=example)</ept></source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Basic Building Blocks</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The RBroker Framework defines three simple building blocks:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RBroker<ept id="p1">**</ept>: an RTask execution engine</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RTask<ept id="p1">**</ept>: an executable representing any analytics Web service</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RTaskResult<ept id="p1">**</ept>: a collection of result data for an instance of RTask</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>These building blocks are described in further detail in the following sections.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Building Block 1: RBroker</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>At its most fundamental level, an RBroker is an RTask execution engine, exposing a simple interface to be used by client application developers to submit RTask for execution.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>However, an RBroker engine handles more than simple execution.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Specifically, an RBroker engine is responsible for the following:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Queuing RTask requests on behalf of client applications</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Acquiring a dedicated R session for the purposes of executing each RTask</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Initiating optional R session pre-initialization for each RTask</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Launching the execution of each RTask</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Handling execution success or failure responses for each RTask</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Returning RTaskResult result data for each RTask to client applications</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>An RBroker takes on these responsibilities so that client application developers don't have to.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Building Block 2: RTask</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>An RTask is an executable description of any DeployR-enabled analytics Web service.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>There are three distinct styles of analytics Web service available to client application developers.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>They are based on:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Repository-managed R scripts</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Arbitrary blocks of R code</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>URL-addressable R scripts</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Each style of analytics Web service is supported when instantiating instances of RTask.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>To execute any RTask, submit the RTask to an instance of RBroker.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Building Block 3: RTaskResult</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>An RTaskResult provides the client application access to RTask result data.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Such result data may include:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>RTask generated R console output</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>RTask generated graphics device plots</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>RTask generated working directory files</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>RTask generated R object workspace data</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>RTaskResult data can be read, displayed, processed, stored, or further distributed by client applications.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Basic Programming Model</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The basic programming model when working with the RBroker framework is as follows:</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Create an instance of RBroker within your application.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Create one or more instances of RTask within your application.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Submit these RTasks to your instance of RBroker for execution.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Integrate the results of your RTasks returned by RBroker within your application.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>As this basic programming model indicates, when using the RBroker framework, your application logic can focus entirely on defining your R analytics tasks and integrating your R analytics task results.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The inherent complexity of managing both client-side DeployR API calls and server-side R session lifecycles is handled entirely by RBroker, which greatly simplifies client application development.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Hello World Example</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The following code snippets provide the ubiquitous "Hello World" example for the RBroker framework.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Each snippet provides a brief demonstration of how the RBroker framework basic programming model is accomplished in Java, JavaScript and C<ph id="ph1">\#</ph> code respectively.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Java:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>JavaScript:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>C#:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Try Out Our Examples!</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>After downloading the RBroker Framework, you can find basic examples that complement this tutorial under the <ph id="ph1">`deployr/examples`</ph> directory.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Additionally, find more comprehensive examples for <bpt id="p1">[</bpt>Java<ept id="p1">](https://github.com/microsoft/?utf8=%E2%9C%93&amp;query=java-example)</ept> and <bpt id="p2">[</bpt>JavaScript<ept id="p2">](https://github.com/microsoft/?utf8=✓&amp;query=js-example)</ept>.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>RBroker Runtime Options</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The RBroker Framework defines three simple building blocks (RBroker, RTask and RTaskResult), which can be instantiated in a number of ways to allow client application solutions to leverage distinct runtime characteristics from the framework.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Currently, there are three RBroker runtimes available.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>These runtimes are identified as:</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Discrete Task Runtime</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Pooled Task Runtime</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Background Task Runtime</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>When contemplating any RBroker-based solution, a developer must first decide which runtime to use.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The following sections detail the characteristics of each RBroker runtime and provide guidance to help developers make the correct runtime selection based on their specific needs.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Discrete Task Runtime</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The Discrete Task Runtime acquires DeployR grid resources per RTask on-demand, which has a number of important consequences at runtime.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>These consequences are:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>If an appropriate slot on the grid can be acquired by the RBroker, then an RTask will be executed.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>If an appropriate slot on the grid cannot be acquired by the RBroker, then the RTask result will indicate an <ph id="ph1">`RGridException`</ph> failure.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Any RTask indicating an <ph id="ph1">`RGridException`</ph> failure can be resubmitted to the RBroker.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>It is the responsibility of the client application developer to decide whether such RTasks should be resubmitted to RBroker, logged by the application, and/or reported to the end-user.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>This runtime supports a <ph id="ph1">`maxConcurrency`</ph> configuration property that limits the maximum number of RTasks that the RBroker will attempt to execute in parallel.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>All RTasks submitted in excess of this limit are automatically queued by the RBroker, which ensures that no more than <ph id="ph1">`maxConcurrency`</ph> RTasks are executing on the runtime at any one time.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Tuning the <ph id="ph1">`maxConcurrency`</ph> property to reflect the real-world limits determined by grid resources provisioned by the DeployR system administrator is an important step when deploying solutions on the Discrete Task Runtime.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>Grid Resource Management<ept id="p1">](#gridprimer)</ept> section of this tutorial for guidance when setting <ph id="ph1">`maxConcurrency`</ph> for your RBroker instance.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Discrete Task Runtime Suitability</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>This type of runtime is well-suited to all forms of RBroker prototyping as well as for public facing production deployments.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>If you anticipate anonymous users making use of DeployR analytics Web services, then this runtime is for you.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Tip!</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>If that does not sound like a suitable RBroker runtime for your client application, then consider the <bpt id="p1">[</bpt>Pooled Task Runtime<ept id="p1">](#pooled-task-runtime)</ept> or the <bpt id="p2">[</bpt>Background Task Runtime<ept id="p2">](#background-task-runtime)</ept>.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Discrete Task Runtime Programming Model</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>The Discrete Task Runtime is supported by the DiscreteTaskBroker.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>This broker executes instances of DiscreteTask.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>The R session environment allocated on the grid per DiscreteTask can be pre-initialized using DiscreteTaskOptions.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Java:</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>JavaScript:</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>C#:</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Discrete Task Runtime Authentication</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>RBroker authentication is optional for this type of runtime, therefore RTask can be executed on behalf of an authenticated user or anonymously.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Whether to use authentication or not depends on your specific deployment goals.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Discrete Task Runtime Persistence</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>When RTask are executed on behalf of an authenticated user, optional persistence to the DeployR-repository post-execution is supported.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>See storageOptions on DiscreteTaskOptions as documented on the <bpt id="p1">[</bpt>RBroker Framework API<ept id="p1">](deployr-tools-and-samples.md)</ept>.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>When RTasks are executed anonymously, persistence to the DeployR-repository post-execution is unsupported.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Pooled Task Runtime</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>The Pooled Task Runtime acquires a dedicated pool of DeployR grid resources at startup, which has a number of important consequences at runtime.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>These consequences are:</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>The time taken to initialize the dedicated grid resource pool for this runtime depends on the nature of the PooledCreationOptions indicated on the PooledBrokerConfig and the size of the pool itself.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Every RTask submitted to the RBroker is guaranteed to execute eventually.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>There is no possibility of failure due to grid resource exhaustion.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>This runtime supports a <ph id="ph1">`maxConcurrency`</ph> configuration property that limits the maximum number of RTasks that the RBroker will attempt to execute in parallel.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>By definition, the <ph id="ph1">`maxConcurrency`</ph> limit determines the size of the pool.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>All RTasks submitted in excess of this limit are automatically queued, which ensures that no more than <ph id="ph1">`maxConcurrency`</ph> RTasks are executing on the runtime at any one time.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Tuning the <ph id="ph1">`maxConcurrency`</ph> property to reflect the real-world limits determined by grid resources provisioned by the DeployR system administrator is an important step when deploying solutions on the Pooled Task Runtime.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>Grid Resource Management<ept id="p1">](#grid-resource-management)</ept> section of this tutorial for guidance when setting <ph id="ph1">`maxConcurrency`</ph> for your RBroker instance.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Pooled Task Runtime Suitability</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>This type of runtime is well suited to production deployments where consistent runtime semantics are required.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>If you anticipate a high-volume RTask workload, then this runtime is for you.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Remember to size the pool in line with expected workload.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>If that does not sound like a suitable RBroker runtime for your client application, then consider the <bpt id="p1">[</bpt>Discrete Task Runtime<ept id="p1">](#discrete-task-runtime)</ept> or the <bpt id="p2">[</bpt>Background Task Runtime<ept id="p2">](#background-task-runtime)</ept>.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Pooled Task Runtime Programming Model</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>The Pooled Task Runtime is supported by the PooledTaskBroker.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>This broker executes instances of PooledTask.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>The R session environment assigned to handle the execution of each PooledTask can be pre-initialized using PooledTaskOptions.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Java:</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>JavaScript:</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>C#:</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Pooled Task Runtime Authentication</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>RBroker authentication is required for this type of runtime, therefore RTask will always execute on behalf of an authenticated user.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>In many instances, this user may represent your client application, and not individual end-users.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Pooled Task Runtime Persistence</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Since RTasks executed on this type of runtime are executing on behalf of an authenticated user, optional persistence to the DeployR-repository following an execution is supported.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>See storageOptions on PooledTaskOptions as documented on the <bpt id="p1">[</bpt>RBroker Framework API<ept id="p1">](deployr-tools-and-samples.md)</ept>.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Pooled Task Runtime Resource Management</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>While this runtime is ideal for high-volume RTask environments, it is important to proactively manage server-side resources dedicated to the pool.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>One such resource that requires special attention is the DeployR database.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Each RTask results in meta-data, and sometimes data, being persisted to the DeployR database.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>This data is preserved in the database until the PooledTaskBroker is ultimately released.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Given this runtime could theoretically service hundreds of thousands or even millions of RTask we recommend that you periodically release and rebuild your pool which allows the DeployR server to flush old RTask data from the system.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Background Task Runtime</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>The Background Task Runtime acquires DeployR grid resources per RTask based on the server-side management of asynchronous grid resources.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>This has a number of important consequences at runtime:</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Unlike the other runtimes, this runtime only schedules RTasks for execution.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>It delegates actual execution to the server-side job scheduling manager.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Every RTask submitted to the RBroker is guaranteed to execute eventually.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>There is no possibility of failure due to grid resource exhaustion.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>This runtime does not support a <ph id="ph1">`maxConcurrency`</ph> configuration property.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>The server-side job scheduling manager maintains its own queuing systems that function independently of the RBroker configuration.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Background Task Runtime Suitability</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>This type of runtime is well-suited to deployments that require periodic, scheduled or batch processing.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>If that does not sound like a suitable RBroker runtime for your client application consider the <bpt id="p1">[</bpt><bpt id="p2">*</bpt>Discrete Task Runtime<ept id="p2">*</ept><ept id="p1">](#discrete-task-runtime)</ept> or the <bpt id="p3">[</bpt><bpt id="p4">*</bpt>Pooled Task Runtime<ept id="p4">*</ept><ept id="p3">](#pooled-task-runtime)</ept>.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>2. Background Task Runtime Programming Model</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>The background task runtime is supported by the BackgroundTaskBroker.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>This broker schedules instances of BackgroundTask for execution on the server.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>The R session environment that is assigned to handle the execution of each BackgroundTask can be pre-initialized using BackgroundTaskOptions.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Java:</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>JavaScript:</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>C#:</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Background Task Runtime Authentication</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>RBroker authentication is required for this type of runtime, therefore RTask will always execute on behalf of an authenticated user.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>In many instances, that user may represent your client application, and not individual end-users.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Background Task Runtime Persistence</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>Since RTasks executed on this type of runtime are executing on behalf of an authenticated user, optional persistence to the DeployR-repository following an execution is supported.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>See storageOptions on BackgroundTaskOptions as documented on the <bpt id="p1">[</bpt>RBroker Framework API<ept id="p1">](deployr-tools-and-samples.md)</ept>.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Result data are not directly available on RTaskResult.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Instead a DeployR Job identifier is returned.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>An application developer must use an appropriate <bpt id="p1">[</bpt>DeployR Client Library<ept id="p1">](deployr-tools-and-samples.md)</ept> that supports APIs for the retrieval of results persisted by the BackgroundTask on DeployR Job.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>RBroker Resource Management</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>While each RBroker runtime automatically manages all DeployR-related client-side and server-side resources on behalf of client applications, it is the responsibility of the application developer to make an explicit call on RBroker to release any residual resources associated with the broker instance whenever a client application terminates.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate the mechanism:</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>Java:</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>JavaScript:</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>C#:</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>This step is especially important for applications that make use of the <bpt id="p1">[</bpt>Pooled Task Broker Runtime<ept id="p1">](#pooled-task-runtime)</ept> since significant DeployR grid resources associated with that runtime will remain unavailable until explicitly released.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>RTask Priority Execution</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>Each RBroker runtime maintains a basic FIFO queue for RTask.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Each RTask on that FIFO queue is eventually submitted to the DeployR server for execution.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>By default, RTask are executed in this FIFO order.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>However, there are times when FIFO semantics get in the way of desired client application semantics.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>For example, when a high priority RTask generated by the client application needs to take precedence over any existing RTasks that may already be in the FIFO queue.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>Each RBroker runtime has built-in support for high priority RTasks.</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>When RTasks are submitted as high priority, they jump the default FIFO queue and form their own priority FIFO queue.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate how this mechanism works in practice:</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>Java:</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>JavaScript:</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>C#:</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>All RTasks on the priority FIFO queue are guaranteed to be executed by the RBroker before any attempt is made to execute RTasks on the default FIFO queue.</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>Client Application Simulations</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>When evaluating any new software technology, one of the first things you are likely to come across is the ubiquitous "Hello World" sample application.</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>Not to be outdone, we provide our own <bpt id="p1">[</bpt>"Hello World" sample application<ept id="p1">](#hello-world-example)</ept> for the RBroker framework.</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>While such sample applications provide a great starting point for any new technology, they can only take you so far.</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>This section discusses client application simulations, which is one of the key tools that is built into the RBroker framework that will help you go a whole lot further.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>As a client application developer interested in integrating analytics Web services into your custom client application you really have two technical challenges that need solving:</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>How best to build or extend your custom client application to facilitate the integration of analytics Web services?</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>How best to integrate analytics Web services to ensure your application meets runtime performance goals?</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>On the first challenge, we offer no particular guidance, since you already know best in such matters.</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>However, on the second challenge, we believe there are key questions that can and should be asked and answered before full integration commences, such as:</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>What RBroker runtime should my application be using?</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>What is the best configuration for my RBroker runtime based on anticipated workload and throughput requirements?</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>How can assumptions be verified regarding throughput and overall performance of the integration?</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>If client application developers can answer these kinds of questions without first having to build a complete client application to test drive each scenario, it can make life a lot simpler.</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>It is for this reason that the RBroker framework supports client application simulations.</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>These simulations are headless client applications that are designed to drive RTask requests through an RBroker instance in order to help developers test, measure and optimize their RBroker integration.</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>To run a client application simulation simply create a simulation that implements the appropriate interface and then ask an instance of RBroker to run the simulation.</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate the mechanism.</source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>Java:</source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>JavaScript:</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source>C#:</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>Now that we have seen how the basic mechanism works for launching client application simulations, let's take a look at the simulation itself.</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate the most simple simulation imaginable, the execution of a single RTask.</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>Java:</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>JavaScript:</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>C#:</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>As you can see, asynchronous callbacks from RBroker allow you to track the progress of the simulation.</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source>Now, let's consider the building of a simulation of a real-time scoring engine, which is something a little more sophisticated.</source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>The following code snippets demonstrate what's involved.</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source>Java:</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>JavaScript:</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source>C#:</source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source>By running client application simulations, experiencing live execution result data and execution failures, and observing overall throughput, a client application developer can learn how to tune the RBroker runtime and RTask options for predictable, even optimal runtime performance.</source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source>And to aid further in the measurement of analytics Web service runtime performance, developers can take advantage of yet another feature of the RBroker framework, <bpt id="p1">[</bpt>client application profiling<ept id="p1">](#client-application-profiling)</ept>.</source>
        </trans-unit><trans-unit id="324" translate="yes" xml:space="preserve">
          <source>Client Application Profiling</source>
        </trans-unit><trans-unit id="325" translate="yes" xml:space="preserve">
          <source>As we just learned, the <bpt id="p1">[</bpt>client application simulation<ept id="p1">](#client-application-simulations)</ept> feature of the RBroker framework helps you quickly answer key integration questions by supporting rapid, iterative experimentation and testing.</source>
        </trans-unit><trans-unit id="326" translate="yes" xml:space="preserve">
          <source>The client application profiling feature extends these capabilities by helping you to accurately measure the runtime impact of each simulated test, which can greatly improve the quality of any integration.</source>
        </trans-unit><trans-unit id="327" translate="yes" xml:space="preserve">
          <source>The client application profiling features are also available beyond simulations, so production environments can also make use of this feature, for example, to maintain audit logs that detail the runtime performance details of each analytics Web service invocation.</source>
        </trans-unit><trans-unit id="328" translate="yes" xml:space="preserve">
          <source>As with most things in the RBroker framework, it is very simple to activate this feature.</source>
        </trans-unit><trans-unit id="329" translate="yes" xml:space="preserve">
          <source>First, note that each RTaskResult has built-in profiling data.</source>
        </trans-unit><trans-unit id="330" translate="yes" xml:space="preserve">
          <source>Second, each RBroker runtime generates runtime profiling events.</source>
        </trans-unit><trans-unit id="331" translate="yes" xml:space="preserve">
          <source>By registering the appropriate asynchronous listener, a client application can receive these profiling events.</source>
        </trans-unit><trans-unit id="332" translate="yes" xml:space="preserve">
          <source>The following code snippets extend the sample demonstrated in the <bpt id="p1">[</bpt>client application simulation<ept id="p1">](#client-application-simulations)</ept> section with support for handling runtime profiling events.</source>
        </trans-unit><trans-unit id="333" translate="yes" xml:space="preserve">
          <source>Java:</source>
        </trans-unit><trans-unit id="334" translate="yes" xml:space="preserve">
          <source>JavaScript:</source>
        </trans-unit><trans-unit id="335" translate="yes" xml:space="preserve">
          <source>C#:</source>
        </trans-unit><trans-unit id="336" translate="yes" xml:space="preserve">
          <source>Grid Resource Management</source>
        </trans-unit><trans-unit id="337" translate="yes" xml:space="preserve">
          <source>This short primer is provided as a note for client application developers.</source>
        </trans-unit><trans-unit id="338" translate="yes" xml:space="preserve">
          <source>The guidance presented here should prove useful when considering suitable values for <ph id="ph1">`maxConcurrency`</ph> on an RBrokerConfig or when discussing DeployR grid resources with a DeployR system administrator.</source>
        </trans-unit><trans-unit id="339" translate="yes" xml:space="preserve">
          <source>What is the DeployR Grid?</source>
        </trans-unit><trans-unit id="340" translate="yes" xml:space="preserve">
          <source>The DeployR grid is a flexible, network of collaborating nodes that contribute resources (memory, CPU, disk) to the DeployR server in order to facilitate the execution of a myriad of different types of operations, many of which are exposed by the RBroker Framework.</source>
        </trans-unit><trans-unit id="341" translate="yes" xml:space="preserve">
          <source>How is the DeployR Grid Configured?</source>
        </trans-unit><trans-unit id="342" translate="yes" xml:space="preserve">
          <source>To simplify grid management for the system administrator, the DeployR grid identifies three distinct types of operation, known as <bpt id="p1">**</bpt>anonymous<ept id="p1">**</ept>, <bpt id="p2">**</bpt>authenticated<ept id="p2">**</ept> and <bpt id="p3">**</bpt>asynchronous<ept id="p3">**</ept> operations respectively.</source>
        </trans-unit><trans-unit id="343" translate="yes" xml:space="preserve">
          <source>These names simply provide a high-level description for related sets of runtime operations that share common characteristics.</source>
        </trans-unit><trans-unit id="344" translate="yes" xml:space="preserve">
          <source>Typically, each node on the grid can be configured by the server administrator to support just one type of operation.</source>
        </trans-unit><trans-unit id="345" translate="yes" xml:space="preserve">
          <source>For example, the administrator could designate a node to asynchronous operations only.</source>
        </trans-unit><trans-unit id="346" translate="yes" xml:space="preserve">
          <source>If the administrator does not want to limit the availability of the resources on a particular grid node to a single type of operation they can assign a special <bpt id="p1">**</bpt>mixed mode<ept id="p1">**</ept> operating type to the node.</source>
        </trans-unit><trans-unit id="347" translate="yes" xml:space="preserve">
          <source>This designation permits any operation to take advantage of the grid node resources at runtime.</source>
        </trans-unit><trans-unit id="348" translate="yes" xml:space="preserve">
          <source>How Does the DeployR Grid Configuration Impact on RBroker?</source>
        </trans-unit><trans-unit id="349" translate="yes" xml:space="preserve">
          <source>Each RBroker runtime automatically acquires grid resources at runtime on behalf of the client application.</source>
        </trans-unit><trans-unit id="350" translate="yes" xml:space="preserve">
          <source>The exact nature of the resources acquired by each runtime are discussed here:</source>
        </trans-unit><trans-unit id="351" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>Discrete Task Runtime<ept id="p1">](#discrete-task-runtime)</ept> submits all tasks, whether executing on behalf of an authenticated or anonymous RBroker, to run on grid nodes configured for anonymous operations.</source>
        </trans-unit><trans-unit id="352" translate="yes" xml:space="preserve">
          <source>If the server cannot find an available slot on that subset of grid nodes, then the task may execute on a grid node configured for mixed mode operations.</source>
        </trans-unit><trans-unit id="353" translate="yes" xml:space="preserve">
          <source>If your DiscreteTaskBroker instance is returning RTaskResults that indicate RGridException, then consider speaking to your DeployR system administrator about provisioning additional resources for existing grid nodes or even additional grid nodes for  <bpt id="p1">&lt;b&gt;</bpt>anonymous<ept id="p1">&lt;/b&gt;</ept> operations.</source>
        </trans-unit><trans-unit id="354" translate="yes" xml:space="preserve">
          <source>These additional resources will support greater levels of concurrent workload.</source>
        </trans-unit><trans-unit id="355" translate="yes" xml:space="preserve">
          <source>Once provisioned, make sure to increase the <ph id="ph1">`maxConcurrency`</ph> configuration option on your instance of RBroker to take full advantage of the new resources on the grid.</source>
        </trans-unit><trans-unit id="356" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt><bpt id="p2">*</bpt>Pooled Task Runtime<ept id="p2">*</ept><ept id="p1">](#pooled-task-runtime)</ept> submits all tasks to run on grid nodes configured for authenticated operations.</source>
        </trans-unit><trans-unit id="357" translate="yes" xml:space="preserve">
          <source>If the server cannot find an available slot on that subset of grid nodes, then the task may execute on a grid node configured for mixed mode operations.</source>
        </trans-unit><trans-unit id="358" translate="yes" xml:space="preserve">
          <source>If the size of the pool allocated to your PooledTaskBroker is less than requested by your <ph id="ph1">`maxConcurrency`</ph> configuration option on your instance of RBroker, then consider speaking to your DeployR system administrator about provisioning additional resources for existing grid nodes or even additional grid nodes for <bpt id="p1">&lt;b&gt;</bpt>authenticated<ept id="p1">&lt;/b&gt;</ept> operations.</source>
        </trans-unit><trans-unit id="359" translate="yes" xml:space="preserve">
          <source>Also you may want to discuss increasing the per-authenticated user concurrent operation limit, which is a setting found under <bpt id="p1">**</bpt>Server Policies<ept id="p1">**</ept> in the Administration Console.</source>
        </trans-unit><trans-unit id="360" translate="yes" xml:space="preserve">
          <source>Ultimately, this setting determines the maximum pool size that a single instance of an authenticated PooledTaskBroker can allocate.</source>
        </trans-unit><trans-unit id="361" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt><bpt id="p2">*</bpt>Background Task Runtime<ept id="p2">*</ept><ept id="p1">](#background-task-runtime)</ept> submits all tasks to run on grid nodes configured for asynchronous operations.</source>
        </trans-unit><trans-unit id="362" translate="yes" xml:space="preserve">
          <source>If the server cannot find an available slot on that subset of grid nodes then the task may execute on a grid node configured for mixed mode operations.</source>
        </trans-unit><trans-unit id="363" translate="yes" xml:space="preserve">
          <source>If you feel that too many of your BackgroundTask are waiting on a queue pending available resources, then consider speaking with your DeployR system administrator about provisioning additional resources for existing grid nodes or even additional grid nodes for <bpt id="p1">&lt;b&gt;</bpt>asynchronous<ept id="p1">&lt;/b&gt;</ept> operations.</source>
        </trans-unit></group></body></file></xliff>