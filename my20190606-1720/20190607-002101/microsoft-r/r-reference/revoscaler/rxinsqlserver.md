<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxinsqlserver.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c376139ead4b9219bbcf4997c094627a05cc40ffac0.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">6139ead4b9219bbcf4997c094627a05cc40ffac0</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxinsqlserver.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxInSqlServer function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Creates a compute context for running RevoScaleR analyses inside Microsoft SQL Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Currently only supported in Windows.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), RxInSqlServer, IO</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>RxInSqlServer: Generate SQL Server In-Database Compute Context</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Creates a compute context for running RevoScaleR analyses inside Microsoft SQL Server.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Currently only supported in Windows.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>An optional RxInSqlServer object.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>An ODBC connection string used to connect to the Microsoft SQL Server database.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Number of tasks (processes) to run for each computation.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This is the maximum number of tasks that will be used; SQL Server  may start fewer processes if there is not enough data, if too many resources are already being used by other jobs, or if  numTasks exceeds the MAXDOP (maximum degree of parallelism) configuration option in SQL Server.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Each of the tasks is given data in parallel, and does computations in parallel, and so computation time may decrease as <ph id="ph1">`numTasks`</ph> increases.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>However, that may not always be the case, and computation time may even increase if too many tasks are competing for machine resources.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Note that <ph id="ph1">`rxOptions(numCoresToUse=n)`</ph> controls how many cores (actually, threads) are used in parallel within each process,  and there is a trade-off between <ph id="ph2">`numCoresToUse`</ph> and <ph id="ph3">`numTasks`</ph> that depends upon the specific algorithm,  the type of data, the hardware, and the other jobs that are running.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the job will be blocking and will not return until   it has completed or has failed.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, the job will be non-blocking and return immediately,  allowing you to continue running other R code.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The object <ph id="ph1">`rxgLastPendingJob`</ph> is created with the job information.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The client connection with SQL Server must be maintained while the job is running, even in non-blocking mode.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>logical scalar.If <ph id="ph1">`TRUE`</ph>, causes the standard output  of the R process started by SQL Server to be printed to the user console.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>This value may be  overwritten by passing a non-<ph id="ph1">`NULL`</ph> logical value to the <ph id="ph2">`consoleOutput`</ph> argument  provided in <bpt id="p1">[</bpt>rxExec<ept id="p1">](rxExec.md)</ept> and <bpt id="p2">[</bpt>rxGetJobResults<ept id="p2">](rxGetJobResults.md)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the default behavior is to clean up the  temporary computational artifacts and delete the result objects upon retrieval.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>,  then the computational results are not deleted, and the results may be acquired using  <bpt id="p1">[</bpt>rxGetJobResults<ept id="p1">](rxGetJobResults.md)</ept>, and the output via <bpt id="p2">[</bpt>rxGetJobOutput<ept id="p2">](rxGetJobOutput.md)</ept> until the  <bpt id="p3">[</bpt>rxCleanupJobs<ept id="p3">](rxCleanup.md)</ept> is used to delete the results and other artifacts.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Leaving this flag set to <ph id="ph1">`FALSE`</ph> can result in accumulation of compute artifacts which you may eventually need to delete before they fill up your hard drive.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>numeric scalar.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Defaults to 0 which means infinite wait.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>optional character vector specifying additional packages to be  loaded on the nodes when jobs are run in this compute context.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>character string specifying the temporary directory on the client that is  used to serialize the R objects back and forth.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If not specified, a subdirectory under  Absolute or paths relative to current directory can be specified.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Target SQL Server instance.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Can also be specified in the connection string with the <ph id="ph1">`Server`</ph> keyword.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Database on the target SQL Server instance.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Can also be specified in the connection string with the <ph id="ph1">`Database`</ph> keyword.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>SQL login to connect to the SQL Server instance.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>SQL login can also be specified in the connection string with the <ph id="ph1">`uid`</ph> keyword.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Password associated with the SQL login.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Can also be specified in the connection  string with the <ph id="ph1">`pwd`</ph> keyword.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed to the underlying function.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Two useful additional arguments are <ph id="ph1">`traceEnabled=TRUE`</ph> and <ph id="ph2">`traceLevel=7`</ph>, which taken together enable run-time tracing of your in-SQL Server computations.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>and <ph id="ph1">`traceLevel`</ph> are deprecated as of MRS 9.0.2 and will be removed from this compute context in the next major release.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Please use <ph id="ph1">`rxOptions(traceLevel=7)`</ph> to enable run-time tracing in-SQL Server.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>, <bpt id="p2">[</bpt>RxInSqlServer-class<ept id="p2">](RxInSqlServer-class.md)</ept>, <bpt id="p3">[</bpt>RxSqlServerData<ept id="p3">](RxSqlServerData.md)</ept>, <bpt id="p4">[</bpt>rxOptions<ept id="p4">](rxOptions.md)</ept>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>