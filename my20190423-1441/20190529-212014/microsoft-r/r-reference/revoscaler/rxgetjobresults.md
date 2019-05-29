<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxgetjobresults.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3898757e3d4f17f423569accaf7429a2f18c5d52b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">898757e3d4f17f423569accaf7429a2f18c5d52b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxgetjobresults.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxGetJobResults function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Obtain distributed computing results and processing status.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxGetJobResults, rxGetJobStatus, IO</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxGetJobResults:  Obtain Distributed Computing Job Status and Results</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Obtain distributed computing results and processing status.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>a <ph id="ph1">`jobInfo`</ph> object as returned by <bpt id="p1">[</bpt>rxExec<ept id="p1">](rxExec.md)</ept> or a <bpt id="p2">**</bpt>RevoScaleR<ept id="p2">**</ept>analysis function, for example, the <ph id="ph2">`rxgLastPendingJob`</ph> object, if available.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>or logical value.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the console output from  all of the processes is printed to the user console.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>,  no console output is displayed.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Output can be retrieved with the function  <bpt id="p1">[</bpt>rxGetJobOutput<ept id="p1">](rxGetJobOutput.md)</ept> for a non-waiting job.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If not <ph id="ph1">`NULL`</ph>,  this flag overrides the  value set in the compute context when the job was submitted.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>,  the setting in the compute context will be used.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>or logical value.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the default behavior is to clean up  any artifacts created by the distributed computing job.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, then the  artifacts are not deleted, and the results may be acquired using <bpt id="p1">[</bpt>rxGetJobResults<ept id="p1">](rxGetJobResults.md)</ept>,  and the console output via <bpt id="p2">[</bpt>rxGetJobOutput<ept id="p2">](rxGetJobOutput.md)</ept> until the <bpt id="p3">[</bpt>rxCleanupJobs<ept id="p3">](rxCleanup.md)</ept> is used to delete the artifacts.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If not <ph id="ph1">`NULL`</ph>, this flag overwrites the value set in the compute context when the job was submitted.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If you routinely set <ph id="ph1">`autoCleanup=FALSE`</ph>, you will eventually fill your hard disk with compute artifacts.If you set <ph id="ph2">`autoCleanup=TRUE`</ph>and experience performance degradation on a Windows XP client, consider setting <ph id="ph3">`autoCleanup=FALSE`</ph>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The possible job status strings returned by <ph id="ph1">`rxGetJobStatus`</ph> are:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>information no longer retained by job scheduler.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>May still retrieve results  and output when available.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>job has successfully completed.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>job has failed.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>job has been canceled and the cancel process is completed.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>job is no longer available on the cluster.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>job is either running or completing it's run (finishing, flushing buffers, etc.), or it is in the process of being canceled.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>job is in one of the following states:   it is being configured, has been submitted but has not started, is being validated, or is in the job queue.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>On LSF clusters, job information by default is held for only one hour (although this is configurable using the LSF parameter CLEAN_PERIOD); jobs older than the CLEAN_PERIOD setting will have status <ph id="ph1">`"undetermined"`</ph>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>: either the results of the run (prepended with console output if the <ph id="ph1">`consoleOutput`</ph> argument is set to <ph id="ph2">`TRUE`</ph>) or a message saying that the results are not available because the job has not finished, has failed, or was deleted.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>: a character string denoting the job status.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept>, RxHadoopMR, <bpt id="p2">[</bpt>RxInSqlServer<ept id="p2">](RxInSqlServer.md)</ept>, <bpt id="p3">[</bpt>rxGetJobs<ept id="p3">](rxGetJobs.md)</ept>, <bpt id="p4">[</bpt>rxCleanupJobs<ept id="p4">](rxCleanup.md)</ept>, <bpt id="p5">[</bpt>rxGetJobStatus<ept id="p5">](rxGetJobResults.md)</ept>, <bpt id="p6">[</bpt>rxExec<ept id="p6">](rxExec.md)</ept>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>