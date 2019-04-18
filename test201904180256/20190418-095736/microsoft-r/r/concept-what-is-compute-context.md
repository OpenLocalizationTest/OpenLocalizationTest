<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="concept-what-is-compute-context.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18cce289cb5d98738908fe3b3b7008101ba1e8fba4c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">ce289cb5d98738908fe3b3b7008101ba1e8fba4c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\concept-what-is-compute-context.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Compute context for script execution on Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Compute context for local, distributed, and parallel processing on Machine Learning Server using revoscalepy or RevoScaleR packages.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Compute context for script execution in Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server, a <bpt id="p1">*</bpt>compute context<ept id="p1">*</ept> refers to the physical location of the computational engine handling a given workload.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The default is local.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>However, if you have multiple machines, you can switch from local to remote, pushing execution of data-centric <bpt id="p1">[</bpt>RevoScaleR (R)<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept>, <bpt id="p2">[</bpt>revoscalepy (Python)<ept id="p2">](../python-reference/revoscalepy/revoscalepy-package.md)</ept>, <bpt id="p3">[</bpt>MicrosoftML (R)<ept id="p3">](../r-reference/microsoftml/microsoftml-package.md)</ept> and <bpt id="p4">[</bpt>microsoftml (Python)<ept id="p4">](../python-reference/microsoftml/microsoftml-package.md)</ept> functions to a computational engine on another system.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>For example, script running locally in R Client can shift execution to a remote Machine Learning Server in a Spark cluster to process data there.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The primary reason for shifting compute context is to eliminate data transfer over your network, bringing computations to where the data resides.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>This is particularly relevant for big data platforms like Hadoop, where data is distributed over multiple nodes, or for data sets that are simply too large for a client workstation.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Compare "local" to "remote"</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Context</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Local</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Default, supported by all products (including R Client), on all platforms.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Script executes on local interpreters using local machine resources.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Remote</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Specifically targets a Machine Learning Server on selected data platforms: Spark over the Hadoop Distributed File System (HDFS) and SQL Server.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Clients, or servers acting in the capacity of a client, can initiate a remote compute context, but the target remote machine itself must be a Machine Learning Server installation.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Compare "remote execution" to "remote compute context"</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Although similarly named, remote execution is distinct from a remote compute context.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Concept</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Language</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Configuration</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Remote compute context</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>R and Python</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Data-centric and function-specific.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Script or code that runs in a remote compute context can include functions from our proprietary libraries: RevoScaleR (R), MicrosoftML (R), revoscalepy (Python), and microsoftml (Python).</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>None required.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If you have server or client installs at the same functional level, you can write script that shifts the compute context.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Remote execution</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>R only</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Machine-oriented, using two or more Machine Learning Server instances interchangeably, or shifting execution from R Client to a more powerful Machine Learning Server on Windows or Linux.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Remote execution is data and library agnostic: you can call functions from any library, including base R and third-party vendors.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>An operationalization feature, enabled as a post-installation task.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>remote execution<ept id="p1">](how-to-execute-code-remotely.md)</ept>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>RevoScaleR compute context</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Remote computing is available for specific data sources on selected platforms.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The following tables document the supported combinations.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Context name</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Alias</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>local</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>All server and client configurations support a local compute context.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>spark</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Remote compute context.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Target is a Spark cluster on Hadoop.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>sqlserver</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Remote compute context.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Target server is a single database node (SQL Server 2016 R Services or SQL Server 2017 Machine Learning Services).</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Computation is parallel, but not distributed.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>localpar</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Compute context is often used to enable controlled, distributed computations relying on instructions you provide rather than a built-in scheduler on Hadoop.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>You can use compute context for manual distributed computing.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>dopar</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Use for manual distributed computing.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Data sources per compute context</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Given a compute context, the following table shows which data sources are available (x indicates available):</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Data Source</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Within a data source type, you might find differences depending on the file system type and compute context.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>For example, the .xdf files created on the Hadoop Distributed File System (HDFS) are somewhat different from .xdf files created in a non-distributed file system such as Windows or Linux.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>How to use RevoScaleR on Spark<ept id="p1">](how-to-revoscaler-spark.md)</ept>.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>revoscalepy compute context</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Remote computing is available for specific data sources on selected platforms.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The following tables document the supported combinations for revoscalepy.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Context name</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Alias</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>local</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>All server and client configurations support a local compute context.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>spark</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Remote compute context.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Target is a Spark 2.0-2.1 cluster over Hadoop Distributed File System (HDFS).</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>sqlserver</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Remote compute context.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Target server is a single database node (SQL Server 2017 Machine Learning with Python support).</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Computation is parallel, but not distributed.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Data sources per compute context</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Given a compute context, the following table shows which data sources are available (x indicates available):</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Data Source</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>X</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>When to switch context</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>The primary use case for switching the compute context is to bring calculations and analysis to the data itself.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>As such, the use cases for a remote compute context leverage database platforms, such as SQL Server, or data located on the Hadoop Distributed File System (HDFS) using Spark or MapReduce for processing layer.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Use case</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Client to Server</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Write and run script locally in R Client, pushing specific computations to a remote Machine Learning Server instance.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>You can shift calculations to systems with more powerful processing capabilities or database assets.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Server to Server</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Push platform-specific computations to a server on a different platform.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Supported platforms include SQL Server,  Hadoop (Spark).</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>You can implement a distributed processing architecture: RxLocalSeq, RxSpark, RxInSqlServer.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Context and distributed computing</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Many analytical functions in RevoScaleR, MicrosoftML, revoscalepy, and microsoftml can execute in parallel.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>On a multi-core computer, such functions run multi-threaded.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>On a distributed platform like Hadoop, the functions distribute workload execution to all available cores and nodes.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>This capability translates into high-performance computing for predictive and statistical analysis of big data, and is a major motivation for pushing a compute context to a remote Hadoop cluster.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Distributed and parallel computing in Machine Learning Server<ept id="p1">](how-to-revoscaler-distributed-computing.md)</ept>.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Step-by-step instructions on how to get, set, and manage compute context in <bpt id="p1">[</bpt>How to set and manage compute context in Machine Learning Server<ept id="p1">](how-to-revoscaler-distributed-computing-compute-context.md)</ept>.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Introduction to Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Machine Learning Server on Windows<ept id="p1">](../install/machine-learning-server-windows-install.md)</ept></source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Machine Learning Server on Linux<ept id="p1">](../install/machine-learning-server-linux-install.md)</ept></source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Machine Learning Server on Hadoop<ept id="p1">](../install/machine-learning-server-hadoop-install.md)</ept></source>
        </trans-unit></group></body></file></xliff>