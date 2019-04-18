<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxcanceljob.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea9269fa46686ed52694aa6c6d10ea6c2c361ac66b098.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9fa46686ed52694aa6c6d10ea6c2c361ac66b098</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxcanceljob.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxCancelJob function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Causes R to cancel an existing distributed computing job.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxCancelJob, rxCancelJob,list-method, rxCancelJob,RxDistributedJob-method, rxCancelJob,RxDistributedHadoopMRJob-method, rxCancelJob,RxDistributedSqlServerJob-method, rxCancelJob,RxDistributedTeradataJob-method, rxCancelJob,ANY-method, IO</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxCancelJob:  Cancel Distributed Computing Job</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Causes R to cancel an existing distributed computing job.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>a jobInfo object, such as that returned by <bpt id="p1">[</bpt>rxExec<ept id="p1">](rxExec.md)</ept> or one of the  RevoScaleR analysis functions in a non-waiting compute context, or the current contents of the <ph id="ph1">`rxgLastPendingJob`</ph> object.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the <ph id="ph2">`consoleOutput`</ph> value assigned to  the job by the compute context at launch is used.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, any console output present at the time the job is canceled is displayed.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, no console output  is displayed.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This function does not attempt to retrieve any output objects; if the output is desired, the <ph id="ph1">`consoleOutput`</ph> flag can be used to display it.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>This function does, however, remove all job-related artifacts from the distributed computing resources, including any job results.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>On Windows, if you press ESC to interrupt a job and then call <ph id="ph1">`rxCancelJob`</ph>, you may get an error message if the job was not completely submitted before you pressed ESC.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`TRUE`</ph> if the job is successfully canceled; <ph id="ph2">`FALSE`</ph> otherwise.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxGetJobs<ept id="p1">](rxGetJobs.md)</ept>, RxHadoopMR.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>