<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="RxInSqlServer.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b48adf35ceddc073c562f505994cfd754a8e51e3db.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8adf35ceddc073c562f505994cfd754a8e51e3db</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\RxInSqlServer.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxInSqlServer: Generate SQL Server in-database compute context (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Creates a compute context for running revoscalepy analyses inside Microsoft SQL Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Currently only supported in Windows.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>sql</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>RxInSqlServer</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Creates a compute context for running revoscalepy analyses inside Microsoft SQL Server.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Currently only supported in Windows.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>connection_string</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>An ODBC connection string used to connect to the Microsoft SQL Server database.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>num_tasks</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Number of tasks (processes) to run for each computation.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This is the maximum number of tasks that will be used; SQL Server may start fewer processes if there is not enough data, if too many resources are already being used by other jobs, or if num_tasks exceeds the MAXDOP (maximum degree of parallelism) configuration option in SQL Server.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Each of the tasks is given data in parallel, and does computations in parallel, and so computation time may decrease as num_tasks increases.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>However, that may not always be the case, and computation time may even increase if too many tasks are competing for machine resources.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Note that RxOptions.set_option(“NumCoresToUse”, n) controls how many cores (actually, threads) are used in parallel within each process, and there is a trade-off between NumCoresToUse and NumTasks that depends upon the specific algorithm, the type of data, the hardware, and the other jobs that are running.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>wait</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Bool value, if True, the job will be blocking and will not return until it has completed or has failed.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If False, the job will be non-blocking and return immediately, allowing you to continue running other Python code.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The client connection with SQL Server must be maintained while the job is running, even in non-blocking mode.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>console_output</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Bool value, if True, causes the standard output of the Python process started by SQL Server to be printed to the user console.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>This value may be overwritten by passing a non-None bool value to the consoleOutput argument provided in rx_exec and rx_get_job_results.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>auto_cleanup</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Bool value, if True, the default behavior is to clean up the temporary computational artifacts and delete the result objects upon retrieval.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If False, then the computational results are not deleted, and the results may be acquired using rx_get_job_results, and the output via rx_get_job_output until the rx_cleanup_jobs is used to delete the results and other artifacts.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Leaving this flag set to False can result in accumulation of compute artifacts which you may eventually need to delete before they fill up your hard drive.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>execution_timeout_seconds</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Integer value, defaults to 0 which means infinite wait.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>packages_to_load</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Optional list of strings specifying additional packages to be loaded on the nodes when jobs are run in this compute context.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`RxComputeContext`</ph>, <bpt id="p1">[</bpt><ph id="ph2">`RxLocalSeq`</ph><ept id="p1">](RxLocalSeq.md)</ept>, <bpt id="p2">[</bpt><ph id="ph3">`rx_get_compute_context`</ph><ept id="p2">](rx-get-compute-context.md)</ept>, <bpt id="p3">[</bpt><ph id="ph4">`rx_set_compute_context`</ph><ept id="p3">](rx-set-compute-context.md)</ept>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>