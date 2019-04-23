<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-consume-web-service-asynchronously-batch.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86ec9787cfd47c98fe962e14ce108934325bda22ae.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">ec9787cfd47c98fe962e14ce108934325bda22ae</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\how-to-consume-web-service-asynchronously-batch.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Consume web services asynchronously with batch scoring with mrsdeploy  - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Asynchronous web service consumption via batch processing in Machine Learning Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>batch processing of web services</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Asynchronous web service consumption via batch processing with mrsdeploy</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Applies to:  Machine Learning Server, Microsoft R Server 9.1</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>In this article, you can learn how to consume  a web service asynchronously, which is especially useful with large input data sets and long-running computations.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The typical approach to consuming web services, <bpt id="p1">[</bpt>"Request Response" consumption<ept id="p1">](how-to-consume-web-service-interact-in-r.md#consume-service)</ept>, involves a single API call to execute the code in that web service once.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The "Asynchronous Batch" approach involves the execution of code without manual intervention using multiple asynchronous API calls on a specific web service sent as a single request to Machine Learning Server.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Then, Machine Learning Server immediately executes those operations once for every row of data provided.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Asynchronous batch workflow</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Generally speaking, the process for asynchronous batch consumption of a web service involves the following:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Call the web service on which the batch execution should be run</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Define the data records for the batch execution task</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Start (or cancel) the batch execution task</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Monitor task and interact with results</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Use these following <bpt id="p1">[</bpt>public API functions<ept id="p1">](#public-fx-batch)</ept>  to define, start, and interact with your batch executions.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Asynchronous batch execution in R with Machine Learning Server</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>End-to-end workflow example</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Use this sample code to follow along with the workflow described in greater detail in the following sections.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Be sure to replace the remoteLogin() function with the correct login details for your configuration.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Connecting to Machine Learning Server using the mrsdeploy package is covered <bpt id="p1">[</bpt>in this article<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Public functions for batch</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>You can use the following supported public functions to consume a service asynchronously.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Batch functions performed on the service object</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Once you get the service object, use these public functions on that object.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>view</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Define the data records to be batched and the thread count</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>view</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Get the list of batch execution identifiers</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>view</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Get batch object using its unique execution identifier</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Batch functions performed on the batch object</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Once you have the batch object, use these public functions to interact with it.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>view</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Starts the execution of a batch scoring operation</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>view</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Cancel the named batch execution</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>view</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Get the execution identifier for the named batch process</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>view</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Poll for the state of the batch execution (failed, complete, ...)</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>view</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Poll for batch execution results, partial or full results as defined</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>view</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Get results for a given index row returned as an array</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>view</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>List of every artifact files that was generated by this execution index</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>view</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Print the contents of the named artifact file generated by the batch execution</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>view</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Download one or all artifact files from execution index</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>1. Get the web service</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Once you have authenticated, retrieve the web service from the server, assign it to a variable, and define the inputs to it as record data in a data frame, CSV, or TSV.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Batching begins by retrieving the web service containing the code against which you score the data records you define next.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>You can get a service using its name and version with the getService() function from <ph id="ph1">`mrsdeploy`</ph>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The result is a service object, which in our example is called <ph id="ph1">`txService`</ph>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`getService`</ph> function is covered in detail in the article "<bpt id="p1">[</bpt>How to interact with and consume web services in R<ept id="p1">](how-to-consume-web-service-interact-in-r.md)</ept>."</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Syntax:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>2. Define the data records to be batched</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Next, use the public api function <ph id="ph1">`batch`</ph> to define the input record data for the batch and set the number of concurrent threads for processing.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Syntax:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Argument</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Specify the R data.frame name directly, or specify a flat list filename and convert it to a data.frame using the base R function, <ph id="ph1">`read.csv`</ph>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Default value is 10.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Specify the number of concurrent threads that can be dedicated to processing records in the batch.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Take care not to set a number so high that it negatively impacts performance.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Returns:<ept id="p1">**</ept> The batch object</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>3. Start, find, or cancel the batch execution</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Next, use the public api functions to start the asynchronous batch execution on the batch object, monitor the execution, or even cancel it.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Start batch execution task</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Start the batch task with <ph id="ph1">`start()`</ph>.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Machine Learning Server starts the batch execution and assigns an ID to the execution and returns the batch object.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Syntax:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>No arguments.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Returns:<ept id="p1">**</ept> The batch object</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>We recommend you always use the <ph id="ph1">`id`</ph> function after you start the execution so that you can find it easily with this id later such as:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Get batch ID</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Get the batch task's identifier from the service object so you can reference it during or after its execution using <ph id="ph1">`id()`</ph>.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Syntax:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>No arguments.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Returns:<ept id="p1">**</ept> The ID for the named batch object.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Get batch by ID</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Syntax:</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Argument</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>The batch execution identifiers</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Returns:<ept id="p1">**</ept> The <ph id="ph1">`Batch`</ph> object</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>List the Batch execution identifiers</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Syntax:</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>No arguments</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Returns:<ept id="p1">**</ept> List of batch execution identifiers</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Cancel execution</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Cancel the batch execution using <ph id="ph1">`cancel()`</ph>.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Syntax:</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>No arguments.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Returns:<ept id="p1">**</ept> The batch object</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>4. Monitor, retrieve, and interact with results</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>While the batch task is running, you can monitor and poll the results.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Once the batch task has completed, you can get the web service consumption output by index from the batch results object, including:</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Monitor execution results and status</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Get results for a given index row returned as an array</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Get a list of every file that was generated by this execution index</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Print the contents of a specific artifact or all artifacts returned</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Download artifacts from execution index</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Monitor execution results and status</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>There are several public functions you can use to get the results and status of a batch execution.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;ndash;</ph> Monitor or get the batch execution results</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Syntax:</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Argument</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>This argument returns the already processed results of the batch execution even if it has not been fully completed.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`showPartialResults = FALSE`</ph>, then returns only the results if the execution has completed.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Returns:<ept id="p1">**</ept> A batch result object is returned, which in our example is called <ph id="ph1">`batchRes`</ph>.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;ndash;</ph> Get the status of the batch execution.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Syntax:</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph> no arguments</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Returns:<ept id="p1">**</ept> The status of the batch execution.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Example:<ept id="p1">**</ept> In this example, we return partial results every three seconds until the batch execution fails or completes.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Then, we return results for a given index row returned as an array.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Get execution results as an array</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Get the execution results for a given index row.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Syntax:</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Argument</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Index value for a given batch data record</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Returns:<ept id="p1">**</ept> The execution results for a given index row as an array.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Example:<ept id="p1">**</ept> In this example, we return partial results every three seconds until the batch execution fails or completes.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Then, we return results for a given index row returned as an array.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Get list of generated artifacts</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Retrieve a list of every artifact that was generated during the batch execution for a given data record, or index, with <ph id="ph1">`listArtifacts()`</ph>.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>This function can be made part of a loop to get the list of the artifacts for every data record (see workflow example for a loop).</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Syntax:</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Argument</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Index value for a given batch data record</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Returns:<ept id="p1">**</ept> A list of every artifact that was generated during the batch execution for a given data record</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Display artifact contents</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>Display the contents of a named artifact returned in the preceding list with <ph id="ph1">`artifact()`</ph>.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Machine Learning Server returns the ID for the named batch object.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Syntax:</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>Argument</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Index value for a given batch data record</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Name of file artifact created during batch execution</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Returns:<ept id="p1">**</ept> The ID for the named batch object</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Download generated artifacts</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Download any artifacts from a specific execution index using <ph id="ph1">`download()`</ph>.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>By default, artifacts are downloaded to the current working directory <ph id="ph1">`getwd()`</ph> unless a different <ph id="ph2">`dest = "&lt;path&gt;"`</ph> is specified.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>You can choose to download a specific artifact or all artifacts.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>Syntax:</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Argument</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>Index value for a given batch data record</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Name of specific artifact generated during batch execution.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>If omitted, all artifacts are downloaded for that index.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>The download directory on your local machine.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>The default is the current R working directory.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>The directory must already exist on the local machine.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Returns:<ept id="p1">**</ept> The path to each downloaded artifact.</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>In this example, we download a named artifact for the fifth index to a specified directory, and then download all artifacts to the default working directory.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>mrsdeploy function overview</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>Connecting to Machine Learning Server with mrsdeploy</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>What is operationalization?</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>What are web services?</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>Working with web services in R</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>Execute on a remote Machine Learning Server</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>How to integrate web services and authentication into your application</source>
        </trans-unit></group></body></file></xliff>