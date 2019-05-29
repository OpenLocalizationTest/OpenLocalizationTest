<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="whats-new-in-machine-learning-server.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3a79be6d83e377aa4ca7a4e757982ac4461553637.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a79be6d83e377aa4ca7a4e757982ac4461553637</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\whats-new-in-machine-learning-server.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>New in Machine Learning Server 9.3</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>New features, improvements, and changes in release 9.3 of Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>What's new in Machine Learning Server 9.3</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Machine Learning Server provides powerful R and Python function libraries for data science and machine learning on small-to-massive data sets, in parallel on local or distributed systems, with modern algorithms for predictive analytics, supervised learning, and data mining.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Functionality is delivered through proprietary R and Python packages, internal computational engines built on open-source R and Python, tools, solutions, and samples.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>In this article, learn about the new capabilities introduced in the latest packages and tools.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>If you develop in R, you might also want to review feature announcements from recent past releases.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>For updates to R Client, see <bpt id="p1">[</bpt>What's New for Microsoft R Client<ept id="p1">](r-client/what-is-microsoft-r-client.md#r-client-whats-new)</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>For known issues and workarounds, see <bpt id="p1">[</bpt>Known issues in 9.3<ept id="p1">](resources-known-issues.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Announced in 9.3</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The 9.3 release marks the beginning of a faster release cadence, with fewer features delivered more frequently.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>New capabilities introduced in 9.3 are listed in the following table.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Feature</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Area</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Administration command line interface</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Operationalization</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Refactored tooling for Machine Learning Server configuration.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The new command-line interface is similar to Azure CLIs and offers full parity with the previous utility.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Use the tool to enable web service deployment, web and compute node designations, and remote execution (R only).</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>You can also manage ports, nodes, credentials; run diagnostic reports; and test the capacity and throughput of web services you create.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Dedicated session pools</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Operationalization</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>You can construct a dedicated session pool for a specific web service to provide ready-to-use connections with preloaded dependencies for fast access to production code.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>This capability is in addition to the <bpt id="p1">[</bpt>generic session pools<ept id="p1">](operationalize/configure-evaluate-capacity.md#pool)</ept> that you can establish server-wide as a shared resource for all web services.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure in R<ept id="p1">](operationalize/how-to-create-manage-session-pools.md)</ept> &amp;#124; <bpt id="p2">[</bpt>Configure in Python<ept id="p2">](operationalize/python/how-to-create-manage-session-pools.md)</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>For R script, the <bpt id="p1">[</bpt>mrsdeploy<ept id="p1">](r-reference/mrsdeploy/mrsdeploy-package.md)</ept> function library provides three new functions for managing dedicated sessions: <bpt id="p2">[</bpt>configureServicePool<ept id="p2">](r-reference/mrsdeploy/configureServicePool.md)</ept>, <bpt id="p3">[</bpt>getPoolStatus<ept id="p3">](r-reference/mrsdeploy/getPoolStatus.md)</ept>, <bpt id="p4">[</bpt>deleteServicePool<ept id="p4">](r-reference/mrsdeploy/deleteServicePool.md)</ept>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>For Python, the <bpt id="p1">[</bpt>azureml-model-management-sdk<ept id="p1">](python-reference/azureml-model-management-sdk/azureml-model-management-sdk.md)</ept> provides the following methods in the mlserver class: <bpt id="p2">[</bpt>create_or_update_service_pool<ept id="p2">](python-reference/azureml-model-management-sdk/mlserver.md#create_or_update_service_pool)</ept>, <bpt id="p3">[</bpt>delete_service_pool<ept id="p3">](python-reference/azureml-model-management-sdk/mlserver.md#delete_service_pool)</ept>, <bpt id="p4">[</bpt>get_service_pool_status<ept id="p4">](python-reference/azureml-model-management-sdk/mlserver.md#get_service_pool_status)</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>CDH 5.12</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Supported platforms</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Version 5.12 of Cloudera distribution of Apache Hadoop (CDH) is now supported for <bpt id="p1">[</bpt>Machine Learning Server for Hadoop<ept id="p1">](install/machine-learning-server-hadoop-install.md)</ept>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Announced in 9.2.1</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The 9.2.1 release was the first release of Machine Learning Server - based on R Server - expanded with Python libraries for developers and analysts who code in Python.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The following table summarizes the Python and R features that were introduced in the 9.2.1 release.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>release announcement for Machine Learning Server 9.2.1<ept id="p1">](https://aka.ms/mlserver92)</ept>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Feature</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Language</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>revoscalepy</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Python</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The first release of this library, used for distributed computing, local compute context, remote compute context for SQL Server and Spark 2.0-2.1 over the Hadoop Distributed File System (HDFS), and high-performance algorithms for Python.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>This library is similar to <bpt id="p1">[</bpt>RevoScaleR<ept id="p1">](r-reference/revoscaler/revoscaler.md)</ept> for R.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>microsoftml</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Python</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The first release of this library, used for machine learning algorithms and data mining.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>This library is similar to <bpt id="p1">[</bpt>MicrosoftML<ept id="p1">](r-reference/microsoftml/microsoftml-package.md)</ept> for R.)</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Pre-trained models</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Python</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Ready-to-use machine learning models for image classification and sentiment detection articulated in Python.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>azureml-model-management-sdk library</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Python</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The first release of this library, used to programmatically build web services encapsulating your Python script.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Standard web service support</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Python</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Contains Python code, models, and model assets.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Accepts specific inputs and provides specific outputs for integration with other services and applications.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Real-time web service support</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Python</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>A fully encapsulated web service with no inputs or outputs (operates on dataframes).</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Real-time model scoring</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>R</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Now supported on Linux.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Role-based access control<ept id="p1">](operationalize/configure-roles.md)</ept> (RBAC)</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Both</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>RBAC was extended with a new explicit Reader role.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Administration utility update</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Both</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The utility simplifies registration of compute nodes with web nodes.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Python development</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server, Python libraries used in script execute locally, or remotely in either Spark over Hadoop Distributed File System (HDFS) or in a SQL Server compute context.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Libraries are built on Anaconda 4.2 over Python 3.5.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>You can run any 3.5-compatible library on a Python interpreter included in Machine Learning Server.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Remote execution is not available for Python scripts.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>For information about to do this in R, see <bpt id="p1">[</bpt>Remote execution in R<ept id="p1">](r/how-to-execute-code-remotely.md)</ept>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>R development</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>R function libraries are built on <bpt id="p1">[</bpt>Microsoft R Open (MRO)<ept id="p1">](https://mran.microsoft.com/open/)</ept>, Microsoft's distribution of open-source R 3.4.1.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The last several releases of R Server added substantial capability for R developers.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>To review recent additions to R functionality, see <bpt id="p1">[</bpt>feature announcements<ept id="p1">](whats-new-in-r-server.md)</ept> for previous versions.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Previous versions</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Visit <bpt id="p1">[</bpt>Feature announcements in R Server<ept id="p1">](whats-new-in-r-server.md)</ept> version 9.1 and earlier, for descriptions of features added in recent past releases.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Welcome to Machine Learning Server</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server on Windows</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server on Linux</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server on Hadoop</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Configure Machine Learning Server to operationalize your analytics</source>
        </trans-unit></group></body></file></xliff>