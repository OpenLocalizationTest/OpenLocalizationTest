<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxinteradata.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37a1f89afda06311e263a92ad6e1efe1334ca898a2.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a1f89afda06311e263a92ad6e1efe1334ca898a2</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxinteradata.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Generate Teradata In-Database Compute Context</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Creates a compute context for running RevoScaleR analyses inside a Teradata database.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>, RxInTeradata, IO</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RxInTeradata: Generate Teradata In-Database Compute Context</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>DEPRECATED: Creates a compute context for running RevoScaleR analyses inside a Teradata database.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>An optional RxInTeradata object.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The share directory in Teradata.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>An ODBC connection string used to connect to the Teradata database.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The share directory.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>This directory must exist on the client with write permission.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The path where Microsoft R Server is installed on Teradata.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The control database name a user can specify for supporting user isolation to enhance security.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>This requires that stored procedures, stored functions and tables are properly created and initialized in the control database, and access permissions are granted to users.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the job will be blocking and will not return until   it has completed or has failed.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, the job will be non-blocking and return immediately,  allowing you to continue running other R code.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The object <ph id="ph1">`rxgLastPendingJob`</ph> is created with the job information.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The client connection with Teradata must be maintained while the job is running, even in non-blocking mode.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>logical scalar.If <ph id="ph1">`TRUE`</ph>, causes the standard output  of the R processes on the AMPS to be printed to the user console.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>This value may be  overwritten by passing a non-<ph id="ph1">`NULL`</ph> logical value to the <ph id="ph2">`consoleOutput`</ph> argument  provided in <bpt id="p1">[</bpt>rxExec<ept id="p1">](rxExec.md)</ept> and <bpt id="p2">[</bpt>rxGetJobResults<ept id="p2">](rxGetJobResults.md)</ept>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the default behavior is to clean up the  temporary computational artifacts and delete the result objects upon retrieval.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>,  then the computational results are not deleted, and the results may be acquired using  <bpt id="p1">[</bpt>rxGetJobResults<ept id="p1">](rxGetJobResults.md)</ept>, and the output via <bpt id="p2">[</bpt>rxGetJobOutput<ept id="p2">](rxGetJobOutput.md)</ept> until the  <bpt id="p3">[</bpt>rxCleanupJobs<ept id="p3">](rxCleanup.md)</ept> is used to delete the results and other artifacts.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Leaving this flag set to <ph id="ph1">`FALSE`</ph> can result in accumulation of compute artifacts which you may eventually need to delete before they fill up your hard drive.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>NOT YET IMPLEMENTED.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Optional character vector specifying additional packages to be  loaded on the nodes when jobs are run in this compute context.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed to the underlying function.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Two useful additional arguments are <ph id="ph1">`traceEnabled=TRUE`</ph> and <ph id="ph2">`traceLevel=7`</ph>, which taken together enable run-time tracing of your in-Teradata computations.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>and <ph id="ph1">`traceLevel`</ph> are deprecated as of MRS 9.0.2 and will be removed from this Compute Context in the next major release.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Please use <ph id="ph1">`rxOptions(traceLevel=7)`</ph> to enable run-time tracing in-Teradata</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>, <bpt id="p2">[</bpt>RxInTeradata-class<ept id="p2">](RxInTeradata-class.md)</ept>, <bpt id="p3">[</bpt>RxTeradata<ept id="p3">](RxTeradata.md)</ept>, <bpt id="p4">[</bpt>RxInSqlServer<ept id="p4">](RxInSqlServer.md)</ept>, <bpt id="p5">[</bpt>rxOptions<ept id="p5">](rxOptions.md)</ept>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>