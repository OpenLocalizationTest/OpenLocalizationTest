<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="service.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef0690673352016121891e2cfdbdaad01e644d65325b10cb467.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">2016121891e2cfdbdaad01e644d65325b10cb467</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\azureml-model-management-sdk\service.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Service class: from azureml-model-management-sdk Python module in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve">
          <source>Class Service</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Service</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Dynamic object for service consumption and batching based on service metadata attributes.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>batch</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Register a set of input records for batch execution on this service.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>records</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>data.frame<ept id="p1">*</ept> or <bpt id="p2">*</bpt>list<ept id="p2">*</ept> of input records to execute.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>parallel_count</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Number of threads used to process entries in the batch.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Default value is 10.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Please make sure not to use too high of a number because it might negatively impact performance.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt><ph id="ph1">`Batch`</ph><ept id="p1">](batch.md)</ept> instance to control this service’s batching lifecycle.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>capabilities</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Provides the following information describing the holdings of this service:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>api<ept id="p1">*</ept> -  The API REST endpoint.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>name<ept id="p1">*</ept> - The service name.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>version<ept id="p1">*</ept> - The service version.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>published_by<ept id="p1">*</ept> - The service publishing author.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>runtime<ept id="p1">*</ept> - The service runtime context <bpt id="p2">_</bpt>R|Python<ept id="p2">_</ept>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>description<ept id="p1">*</ept> - The service description.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>creation_time<ept id="p1">*</ept> - The service publish timestamp.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>snapshot_id<ept id="p1">*</ept> - The snapshot identifier this service is bound with.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>inputs<ept id="p1">*</ept> - The input schema name/type definition.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>outputs<ept id="p1">*</ept> - The output schema name/type definition.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>inputs_encoded<ept id="p1">*</ept> - The input schema name/type encoded to python.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>outputs_encoded<ept id="p1">*</ept> - The output schema name/type encoded to python.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>artifacts<ept id="p1">*</ept> - The supported generated files.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>operation_id<ept id="p1">*</ept> - The function <ph id="ph1">`alias`</ph>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>swagger<ept id="p1">*</ept> - The API REST endpoint to this service’s <bpt id="p2">*</bpt>swagger.json<ept id="p2">*</ept> document.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>A <ph id="ph1">`dict`</ph> of key/values describing the service.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>get_batch</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Retrieves the service batch based on an execution identifier.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>execution_id</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The identifier of the batch execution.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt><ph id="ph1">`Batch`</ph><ept id="p1">](batch.md)</ept> instance to control this service’s batching lifecycle.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>list_executions</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Gets all batch execution identifiers currently queued for this service.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>A <ph id="ph1">`list`</ph> of execution identifiers.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>swagger</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Retrieves the <bpt id="p1">*</bpt>swagger.json<ept id="p1">*</ept> for this service (see <bpt id="p2">[</bpt><ph id="ph1">http://swagger.io/</ph><ept id="p2">](http://swagger.io/)</ept>).</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The swagger document for this service as a json <ph id="ph1">`str`</ph>.</source>
        </trans-unit></group></body></file></xliff>