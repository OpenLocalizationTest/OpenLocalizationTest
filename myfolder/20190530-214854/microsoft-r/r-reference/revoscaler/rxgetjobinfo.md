<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxgetjobinfo.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3ee7b0c8c576b3e7a3965c4c375bb594365540ca10.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">e7b0c8c576b3e7a3965c4c375bb594365540ca10</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxgetjobinfo.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxGetJobInfo function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Gets job information for a given distributed computing job.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxGetJobInfo, IO</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxGetJobInfo:  Get Job Information from Distributed Computing Job</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Gets job information for a given distributed computing job.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>an object containing <ph id="ph1">`jobInfo`</ph> information, such as that returned from a non-waiting, distributed computation.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The object returned from a non-waiting, distributed computation contains job information together with other information.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The job information is used internally by such functions as <ph id="ph1">`rxGetJobStatus`</ph>, <ph id="ph2">`rxGetJobOutput`</ph>, and <ph id="ph3">`rxGetJobResults`</ph>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>It is sometimes useful to extract it for its own sake, as it contains complete information on the job's compute context as well as other information needed by the distributed computing resources.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>For most users, the principal use of this function is to determine whether a given object actually contains job information.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If the return value is not <ph id="ph1">`NULL`</ph>, then the object contains job information.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Note, however, that the structure of the job information is subject to change, so code that attempts to manipulate it directly is not guaranteed to be forward-compatible.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>the job information, if present, or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept>, RxHadoopMR, <bpt id="p2">[</bpt>RxInSqlServer<ept id="p2">](RxInSqlServer.md)</ept>, <bpt id="p3">[</bpt>rxGetJobStatus<ept id="p3">](rxGetJobResults.md)</ept>, <bpt id="p4">[</bpt>rxGetJobOutput<ept id="p4">](rxGetJobOutput.md)</ept>, <bpt id="p5">[</bpt>rxGetJobResults<ept id="p5">](rxGetJobResults.md)</ept></source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>