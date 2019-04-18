<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxcleanup.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea9264a2d49e67ca36b40562d8233b0fbc88205af8785.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">4a2d49e67ca36b40562d8233b0fbc88205af8785</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxcleanup.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxCleanupJobs function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Removes artifacts created while executing a distributed computing job.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxCleanupJobs, IO</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxCleanupJobs:  Cleanup of a Distributed Computing Job or Jobs.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Removes artifacts created while executing a distributed computing job.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxJobInfo`</ph> object or a list of job objects that can be obtained  from <bpt id="p1">[</bpt>rxGetJobs<ept id="p1">](rxGetJobs.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, forces removal of job directories even if  there are retrievable results or if the current job state is undetermined.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, will print the directories/records being deleted.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`jobInfoList`</ph> is a <ph id="ph2">`jobInfo`</ph> object, <ph id="ph3">`rxCleanupJobs`</ph> attempts to remove the artifacts.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>However, if the job has successfully completed and <ph id="ph1">`force=FALSE`</ph>, <ph id="ph2">`rxCleanupJobs`</ph> issues a warning saying to either set <ph id="ph3">`force=TRUE`</ph> or use <bpt id="p1">[</bpt>rxGetJobResults<ept id="p1">](rxGetJobResults.md)</ept> to get the results and delete the artifacts.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`jobInfoList`</ph> is a list of jobs, <ph id="ph2">`rxCleanupJobs`</ph> attempts to apply the cleanup rules for a single job to each element in the list.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>This function is called for its side effects (removing job artifacts); it does not have a useful return value.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxGetJobs<ept id="p1">](rxGetJobs.md)</ept>, <bpt id="p2">[</bpt>rxGetJobOutput<ept id="p2">](rxGetJobOutput.md)</ept>, <bpt id="p3">[</bpt>RxSpark<ept id="p3">](RxSpark.md)</ept>, <bpt id="p4">[</bpt>RxHadoopMR<ept id="p4">](RevoScaleR-deprecated.md)</ept>, <bpt id="p5">[</bpt>rxGetJobResults<ept id="p5">](rxGetJobResults.md)</ept></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>