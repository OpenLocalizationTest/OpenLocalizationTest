<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-distributed-computing-compute-context.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335bb48ac3a0edb6407097ff3872fdb12240719761b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">bb48ac3a0edb6407097ff3872fdb12240719761b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-distributed-computing-compute-context.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to set and manage compute context in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Push a compute context to Machine Learning Server on a different computer or platform for remote execution.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to set and manage compute context in Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server, every session that loads a function library has a <bpt id="p1">[</bpt>compute context<ept id="p1">](concept-what-is-compute-context.md)</ept>.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The default is <bpt id="p1">**</bpt>local<ept id="p1">**</ept>, available on all platforms.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>No action is required to use a local compute context.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>This article explains how to shift script execution to a <bpt id="p1">**</bpt>remote<ept id="p1">**</ept> Hadoop or Spark cluster, for the purpose of bring calculations to the data itself and eliminating data transfer over your network.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>For SQL Server compute contexts, see <bpt id="p1">[</bpt>Define and use a compute context<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/tutorials/deepdive-define-and-use-compute-contexts)</ept> in the SQL Server documentation.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>You can create multiple compute context objects: just use them one at a time.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Often, functions operate identically in local and remote context.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If script execution is successful locally, you can generally expect the same results on the remote server, subject to these <bpt id="p1">[</bpt>limitations<ept id="p1">](#limits-on-context-shift)</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The remote computer must be at the same functional level as the system sending the request.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A remote Machine Learning Server 9.2.1 can accept a compute context shift from another 9.2.1 interpreter on Machine Learning Server, a SQL Server 2017 Machine Learning Services instance, and for R developers on Microsoft R Client at the same functional level (3.4.1).</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The following table is a recap of platform and data source requirements for each function library.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Library</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Platforms &amp; Data Sources</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>RevoScaleR</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Spark 2.0-2.1 over HDFS, Hadoop MapReduce: Hive, Orc, Parquet, Text, XDF, ODBC</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>SQL Server: tables, views, local text and .xdf files <bpt id="p1">&lt;sup&gt;</bpt>(1)<ept id="p1">&lt;/sup&gt;</ept>, ODBC data sources</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>revoscalepy</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Spark 2.0-2.1 over HDFS: Hive, Orc, Parquet, Text, XDF, ODBC</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>SQL Server 2017 Machine Learning with Python: tables, views, local text and .xdf files <bpt id="p1">&lt;sup&gt;</bpt>(1)<ept id="p1">&lt;/sup&gt;</ept>, ODBC data sources</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;sup&gt;</bpt>(1)<ept id="p1">&lt;/sup&gt;</ept> You can load text or .xdf files locally, but be aware that code and data runs on SQL Server, which results in <bpt id="p2">[</bpt>implicit data type conversions<ept id="p2">](https://docs.microsoft.com/sql/advanced-analytics/r/r-libraries-and-data-types#r-and-sql-data-types)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>RevoScaleR is available in both Machine Learning Server and R Client.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>You can develop script in R Client for execution on the server.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>However, because R Client is limited to two threads for processing and in-memory datasets, scripts might require deeper customizations if datasets are large and come with dependencies on data chunking.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Chunking is not supported in R Client.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>In R Client, the <ph id="ph1">`blocksPerRead`</ph> argument is ignored and all data is read into memory.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Large datasets that exceed memory must be pushed to a compute context of a Machine Learning Server instance that provides data chunking.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Get a compute context</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>As a starting point, practice the syntax for returning the local compute context.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Every platform, product, and language supports the default local compute context.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>For both languages, the return object should be Return object should be <bpt id="p1">**</bpt>RxLocalSeq<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Set a remote compute context</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>This section uses examples to illustrate the syntax for setting compute context.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>For Spark</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The compute context used to distribute computations on a Hadoop Spark 2.0-2.1 cluster.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>For more information, see the <bpt id="p1">[</bpt>How to use RevoScaleR with Spark<ept id="p1">](how-to-revoscaler-spark.md)</ept>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>For MapReduce</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The compute context used to distribute computations on a Hadoop MapReduce cluster.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>This compute context can be used on a node (including an edge node) of a Cloudera or Hortonworks cluster with an RHEL operating system, or a client with an SSH connection to such a cluster.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>For details on creating and using <ph id="ph1">`RxHadoopMR`</ph> compute contexts, see the <bpt id="p1">[</bpt>How to use RevoScaleR with Hadoop<ept id="p1">](how-to-revoscaler-hadoop.md)</ept></source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>For SQL Server (in-database)</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`RxInSqlServer`</ph> compute context is a special case in that it runs computations in-database, but it runs on only a single database node, so the computation is parallel, but not distributed.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>For setting up a remote compute context to SQL Server, we provide an example below, but point you to <bpt id="p1">[</bpt>Define and use a compute context<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/tutorials/deepdive-define-and-use-compute-contexts)</ept> in the SQL Server documentation for additional instructions.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Limitations of remote compute context</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>A primary benefit of remote computing is to perform distributed analysis using the inherent capabilities of the host platform.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>For a list of analytical functions that are multithreaded and cluster aware, see <bpt id="p1">[</bpt>Running distributed analyses using RevoScaleR<ept id="p1">](how-to-revoscaler-distributed-computing-distributed-analysis.md)</ept>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>As a counter point, the concept of "remote compute context" is not optimized for data manipulation and transformation workloads.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>As such, many data-related functions come with local compute requirements.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The following table describes the exceptions to remote computing.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Limit</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Script execution of open-source routines</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Scripts use a combination of open-source and proprietary functions.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Only revoscalepy and RevoScaleR functions, with the respective interpreters, are multithreaded and distributable.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Open-source routines in your script still run locally in a single threaded process.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Single-threaded proprietary functions</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Analyses that do not run in parallel include <bpt id="p1">[</bpt>import and export functions<ept id="p1">](../r-reference/revoscaler/revoscaler.md#import-export-functions)</ept>, <bpt id="p2">[</bpt>data transformation functions<ept id="p2">](../r-reference/revoscaler/revoscaler.md#data-transform-functions)</ept>, <bpt id="p3">[</bpt>graphing functions<ept id="p3">](../r-reference/revoscaler/revoscaler.md#graphing-functions)</ept>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Date location and operational limits</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Sort and merge must be local.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Import is multithreaded, but not cluster-aware.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If you execute rxImport in a Hadoop cluster, it runs multithreaded on the current node.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Data may have to be moved back and forth between the local and remote environments during the course of overall program execution.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Except for file copying in Hadoop, RevoScaleR does not include functions for moving data.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Set a no-wait compute context</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>By default, all jobs are "waiting jobs" or "blocking jobs", where control of the command prompt is not returned until the job is complete.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>For jobs that complete quickly, this is an appropriate choice.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>For large jobs that run longer, execute the job but use a non-waiting compute context to continue working in your local session.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>In this case, you can specify the compute context to be <bpt id="p1">*</bpt>non-waiting<ept id="p1">*</ept> (or <bpt id="p2">*</bpt>non-blocking<ept id="p2">*</ept>), in which case an object containing information about the pending job is used to retrieve results later.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>To set the compute context object to run "no wait" jobs, set the argument <bpt id="p1">*</bpt>wait<ept id="p1">*</ept> to <bpt id="p2">*</bpt>FALSE<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Another use for non-waiting compute contexts is for massively parallel jobs involving multiple clusters.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>You can define a non-waiting compute context on each cluster, launch all your jobs, then aggregate the results from all the jobs once they complete.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Non-Waiting Jobs<ept id="p1">](how-to-revoscaler-distributed-computing-background-jobs.md#non-waiting-jobs)</ept>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Retrieve cluster console output</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>If you want console output from each of the cluster R processes printed to your user console, specify <bpt id="p1">*</bpt>consoleOutput=TRUE<ept id="p1">*</ept> in your compute context.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Update a compute context</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Once you have a compute context object, modify it using the same function that originally creates it.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Pass the name of the original object as its first argument, and then specify only those arguments you wish to modify as additional arguments.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>For example, to change only the <ph id="ph1">`suppressWarning`</ph> parameter of a Spark compute context <bpt id="p1">*</bpt>myHadoopCluster<ept id="p1">*</ept> from TRUE to FALSE:</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>To list parameters and default values, use the <ph id="ph1">`args`</ph> function with the name of the compute context constructor, for example:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>which gives the following output:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>You can temporarily modify an existing compute context and set the modified context as the current compute context by calling <ph id="ph1">`rxSetComputeContext`</ph>.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>For example, if you have defined <bpt id="p1">*</bpt>myHadoopCluster<ept id="p1">*</ept> to be a waiting cluster and want to set the current compute context to be non-waiting, you can call <ph id="ph1">`rxSetComputeContext`</ph> as follows:</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxSetComputeContext`</ph> function returns the previous compute context, so it can be used in constructions like the following:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>You can specify the compute context by name, as we have done here, but you can also specify it by calling a compute context constructor in the call to <ph id="ph1">`rxSetComputeContext`</ph>.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>For example, to return to the local sequential compute context after using a cluster context, you can call <ph id="ph1">`rxSetComputeContext`</ph> as follows:</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>In this case, you can also use the descriptive string "local" to do the same thing:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Create additional compute contexts</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Given a set of distributed computing resources, you might want to create multiple compute context objects to vary the configuration.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>For example, you might have one compute context for waiting or blocking jobs and another for no-wait or non-blocking jobs.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Or you might define one that uses all available nodes and another that specifies a particular set of nodes.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Because the initial specification of a compute context can be somewhat tedious, it is usually simplest to create additional compute contexts by modifying an existing compute context, in precisely the same way as we updated a compute context in the previous section.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>For example, suppose instead of simply modifying our existing compute context from <bpt id="p1">*</bpt>wait=TRUE<ept id="p1">*</ept> to <bpt id="p2">*</bpt>wait=FALSE<ept id="p2">*</ept>, we create a new compute context for non-waiting jobs:</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Store commonly used compute context objects in an R script, or add their definitions to an R startup file.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Introduction to Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Distributed computing<ept id="p1">](how-to-revoscaler-distributed-computing.md)</ept></source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Compute context<ept id="p1">](concept-what-is-compute-context.md)</ept></source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Define and use a compute context in SQL Server<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/tutorials/deepdive-define-and-use-compute-contexts)</ept></source>
        </trans-unit></group></body></file></xliff>