<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-distributed-computing.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca865024696be5892f25edad11df7427b248544dcbce.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5024696be5892f25edad11df7427b248544dcbce</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-distributed-computing.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Distributed and parallel execution for high-performance computing (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>High performance computing (HPC) for distributed workloads using SQL Server in-database and Hadoop clusters computing RevoScaleR package for R and revoscalepy for Python.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Distributed and parallel computing in Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Machine Learning Server's computational engine is built for distributed and parallel processing, automatically partitioning a workload across multiple nodes in a cluster, or on the available threads on multi-core machine.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Access to the engine is through functions in our proprietary packages: <bpt id="p1">[</bpt>RevoScaleR (R)<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept>, <bpt id="p2">[</bpt>revoscalepy (Python)<ept id="p2">](../python-reference/revoscalepy/revoscalepy-package.md)</ept>, and machine learning algorithms in <bpt id="p3">[</bpt>MicrosoftML (R)<ept id="p3">](../r-reference/microsoftml/microsoftml-package.md)</ept> and <bpt id="p4">[</bpt>microsoftml (Python)<ept id="p4">](../python-reference/microsoftml/microsoftml-package.md)</ept>, respectively.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>RevoScaleR and revoscalepy provide data structures and data operations used in downstream analyses and predictions.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Both libraries are designed to process large data one chunk at a time, independently and in parallel.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Each computing resource needs access only to that portion of the total data source required for its particular computation.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>This capability is amplified on distributed computing platforms like Spark.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Instead of passing large amounts of data from node to node, the computations are farmed out to nodes in the cluster, executing on the node providing the data.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Architectures supporting workload distribution</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>On a single server with multiple cores, jobs run in parallel, assuming the workload can be divided into smaller pieces and executed on multiple threads.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>On a distributed platform like Hadoop, you might write script that runs locally on one node, such as an edge node in the cluster, but shift execution to worker nodes for bigger jobs.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>When executed on a distributed platform like Spark over Hadoop Distributed File System (HDFS), both revoscalepy and RevoScaleR automatically use all available cores on all nodes in a cluster.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Distributed and parallel processing is revo-managed, where the engine assigns a job to an available computing resource (a node in cluster, or a thread on a multi-core machine), thereby becoming the logical master node for that job.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The master node is responsible for the following operations:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Distributes the computation to itself and the other computing resources</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Gathers the results of the independent, parallel computations</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Finalizes and returns the results</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>To shift execution to the worker nodes in a cluster, you have to set the <bpt id="p1">[</bpt>compute context<ept id="p1">](concept-what-is-compute-context.md)</ept> to the platform.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>For example, you might use the local compute context on an edge node to prepare data or set up variables, and then shift context  to RxSpark or RxHadoopMR to run data analysis on worker nodes.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Shifting to a Spark or HadoopMR compute context comes with a list of supported data sources for that platform.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Assuming the data inputs you want to analyze are supported in a Spark or Hadoop compute context, your scripts for distributed analysis can include any of the functions noted in this article.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>For a list of supported data sources by compute context, see <bpt id="p1">[</bpt>Compute context for script execution in Machine Learning Server<ept id="p1">](concept-what-is-compute-context.md)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Distributed computing is conceptually similar to parallel computing, but in Machine Learning Server, it specifically refers to workload distribution across multiple physical servers.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Distributed platforms contribute the following infrastructure used for managing the entire operation: a job scheduler for allocating jobs, data nodes to run the jobs, and a master node for tracking the work and coordinating the results.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>In practical terms, you can think of distributed computing as a capability provided by <bpt id="p1">[</bpt>Machine Learning Server for Hadoop and Spark<ept id="p1">](../install/machine-learning-server-hadoop-install.md)</ept>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Functions for multi-threaded data operations</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Import, merge, and step transformations are multi-threaded on a parallel architecture.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>RevoScaleR (R)</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>revoscalepy (Python)</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>RxImport</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>rx-import</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>RxDataStep</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>rx-data-step</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>RxMerge</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>not available</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Functions for distributed analysis</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The following analytical functions execute in parallel, with the results unified as a single response in the return object:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>RevoScaleR (R)</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>revoscalepy (Python)</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>rxSummary</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>rx-summary</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>rxLinMod</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>rx-lin-mod</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>rxLogit</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>rx-logit</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>rxGlm</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>not available</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>rxCovCor</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>not available</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>rxCube</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>not available</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>rxCrossTabs</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>not available</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>rxKmeans</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>not available</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>rxDTree</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>rx-dtree</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>rxDForest</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>rx-dforest</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>rxBTrees</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>rx-btrees</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>rxNaiveBayes</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>not available</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>For examples and practical tips on working with high-performance analytical functions, see <bpt id="p1">[</bpt>Running distributed analyses using RevoScaleR<ept id="p1">](how-to-revoscaler-distributed-computing-distributed-analysis.md)</ept>.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>User-defined distributed analysis</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>An alternative approach is to use the <bpt id="p1">[</bpt>rxExec (R)<ept id="p1">](../r-reference/revoscaler/rxexec.md)</ept> or <bpt id="p2">[</bpt>rx-exec (Python)<ept id="p2">](../python-reference/revoscalepy/rx-exec.md)</ept>function, which can run arbitrary R functions in a distributed fashion on available cores, and all available nodes in a cluster.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>You can create new functions or call existing functions in sequence, packaged as a single execution performed by rxExec.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>When using rxExec, you largely control how the computational tasks are distributed and you are responsible for any aggregation and final processing of results.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Running distributed analyses using RevoScaleR</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Compute context</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>What is RevoScaleR</source>
        </trans-unit></group></body></file></xliff>