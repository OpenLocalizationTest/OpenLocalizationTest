<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxgetjoboutput.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e000fb50094dd51095ca408c50effc35391999168.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">000fb50094dd51095ca408c50effc35391999168</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxgetjoboutput.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxGetJobOutput function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Gets the console output from the various nodes in a non-waiting distributed computing job.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxGetJobOutput, IO</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxGetJobOutput:  Get Console Output from Distributed Computing Job</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Gets the console output from the various nodes in a non-waiting distributed computing job.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>a job information object, such as that returned from a non-waiting,  distributed computation, for example, the <ph id="ph1">`rxgLastPendingJob`</ph> object, if available.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>During a job run, the state of the output is non-deterministic (that is, it may or may not be on disk, and what is on disk at any given point in time may not reflect the actual completion state of a job).</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`autoCleanup`</ph> has been set to <ph id="ph2">`TRUE`</ph>, the console output will not persist after the job completes.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Unlike <bpt id="p1">[</bpt>rxGetJobResults<ept id="p1">](rxGetJobResults.md)</ept>, this function does not remove any job information upon retrieval.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>This function is called for its side effect of printing console output; it does not have a useful return value.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept>, RxHadoopMR, <bpt id="p2">[</bpt>RxInSqlServer<ept id="p2">](RxInSqlServer.md)</ept>, <bpt id="p3">[</bpt>rxGetJobs<ept id="p3">](rxGetJobs.md)</ept>, <bpt id="p4">[</bpt>rxCleanupJobs<ept id="p4">](rxCleanup.md)</ept>, <bpt id="p5">[</bpt>rxGetJobResults<ept id="p5">](rxGetJobResults.md)</ept>, <bpt id="p6">[</bpt>rxExec<ept id="p6">](rxExec.md)</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>