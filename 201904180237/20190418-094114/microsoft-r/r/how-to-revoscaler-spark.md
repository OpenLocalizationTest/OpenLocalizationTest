<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-spark.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea92636b3d1e16c53adebb30a474c2b7b23259347cd5a.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">36b3d1e16c53adebb30a474c2b7b23259347cd5a</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-spark.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to use RevoScaleR with Apache Spark (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Get started with RevoScaleR and Spark on Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to use RevoScaleR in a Spark compute context</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>This article provides a step-by-step introduction to using the <bpt id="p1">[</bpt>RevoScaleR functions<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept> in Apache Spark running on a Hadoop cluster.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>You can use a small built-in sample dataset to complete the walkthrough, and then step through tasks again using a larger dataset.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Download sample data</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Start Revo64</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Create a compute context for Spark</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Copy a data set into HDFS</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Create a data source</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Summarize your data</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Fit a linear model to the data</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Fundamentals</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>In a Spark cluster, you typically connect to Machine Learning Server on the edge node for most of your work, writing and running script in a local <bpt id="p1">[</bpt>compute context<ept id="p1">](concept-what-is-compute-context.md)</ept>, using client tools and the RevoScaleR engine on that machine.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Your script calls the RevoScaleR functions to execute scalable and high-performance data management, analysis, and visualization functions.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>As with any script using RevoScaleR, you can call base R functions, as well as other functions available in packages you have installed separately.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The RevoScaleR engine is built on the R interpreter, extending but not breaking any core functions you are accustomed to using.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>To load data and run analyses on worker nodes, you set the compute context in your script to <bpt id="p1">[</bpt>RxSpark<ept id="p1">](../r-reference/revoscaler/rxSpark.md)</ept>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>In this context, RevoScaleR functions automatically distribute the workload across all the worker nodes, with no built-in requirement for managing jobs or the queue.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Internally, RevoScaleR in an RxSpark compute context uses the Hadoop infrastructure, including the Yarn scheduler, HDFS, and of course, Spark as the processing framework.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Alternatively, if project requirements dictate manual overrides, RevoScaleR provides functions for manual data allocation and scheduled processing across selected nodes.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>How RevoScaleR distributes jobs in Spark and Hadoop</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>In a Spark cluster, the RevoScaleR analysis functions go through the following steps:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>A master process is initiated to run the main thread of the algorithm.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The master process initiates a Spark job to make a pass through the data.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Spark worker produces an intermediate results object for each task processing a chunk of data.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>These are then combined and returned to master node.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The master process examines the results.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>For iterative algorithms, it decides if another pass through the data is required.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If so, it initiates another Spark job and repeats.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>When complete, the final results are computed and returned.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>When running on Spark, the RevoScaleR analysis functions process data contained in the Hadoop Distributed File System (HDFS).</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>HDFS data can also be accessed directly from RevoScaleR, without performing the computations within the Hadoop framework.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>An example can be found in <bpt id="p1">[</bpt>Using a Local Compute Context with HDFS Data<ept id="p1">](#bkmk_local_compute_with_hdfs)</ept>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For a comprehensive list of functions for the Spark or Hadoop compute contexts, see <bpt id="p1">[</bpt>RevoScaleR Functions for Hadoop<ept id="p1">](../r-reference/revoscaler/revoscaler-hadoop-functions.md)</ept>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>For a list of which functions support distributed computing, see <bpt id="p1">[</bpt>Running distributed analyses using RevoScaleR<ept id="p1">](how-to-revoscaler-distributed-computing-distributed-analysis.md)</ept>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>1 - Download sample data</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Sample data is required if you intend to follow the steps.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>This walkthrough starts with the AirlineDemoSmall.csv file from the local RevoScaleR SampleData directory.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Optionally, you can graduate to a second series of tasks using a larger dataset.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>Airline 2012 On-Time Data Set<ept id="p1">*</ept> consists of 12 comma-separated files containing information on flight arrival and departure details for all commercial flights within the USA, for the year 2012.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>This is a big data set with over six million observations.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>To download the larger dataset, go to <bpt id="p1">[</bpt><ph id="ph1">https://packages.revolutionanalytics.com/datasets/</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698896&amp;clcid=0x409)</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>2 - Start Revo64</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Machine Learning Server for Hadoop runs on Linux.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>On the edge node, start an R session by typing <ph id="ph1">`Revo64`</ph> at the shell prompt: $ <ph id="ph2">`Revo64`</ph></source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>3 - Spark compute context</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The Spark compute context is established through RxSpark or rxSparkConnect() to create the Spark compute context, and uses rxSparkDisconnect() to return to a local compute context.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The rxSparkConnect() function maintains a persistent Spark session and results in more efficient execution of RevoScaleR functions for this context.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>In the Revo64 command line, define a Spark compute context using default values:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The default settings include a specification of <bpt id="p1">*</bpt>/var/RevoShare/$USER<ept id="p1">*</ept> as the <bpt id="p2">*</bpt>shareDir<ept id="p2">*</ept> and <bpt id="p3">*</bpt>/user/RevoShare/$USER<ept id="p3">*</ept> as the <bpt id="p4">*</bpt>hdfsShareDir<ept id="p4">*</ept>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>These are the default locations for writing files to the native local file system and HDFS file system, respectively.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>These directories must be writable for your cluster jobs to succeed.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>You must either create these directories or specify suitable writable directories for these parameters.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If you are working on a node of the cluster, the default specifications for the shared directories are:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>You can have multiple compute context objects available for use, but you can only use one at a time.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Specify the active compute context using the <bpt id="p1">[</bpt>rxSetComputeContext<ept id="p1">](../r-reference/revoscaler/rxsetcomputecontext.md)</ept> function: <ph id="ph1">`rxSetComputeContext(myHadoopCluster2)`</ph></source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Defining a Compute Context on a High-Availability Cluster</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>On a Hadoop cluster configured for high-availability, you must specify the node providing the name service using the <bpt id="p1">*</bpt>nameNode<ept id="p1">*</ept> argument to <bpt id="p2">*</bpt>RxSpark<ept id="p2">*</ept>, and also specify the Hadoop port with the <bpt id="p3">*</bpt>port<ept id="p3">*</ept> argument:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>4 - Copy data to HDFS</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Start with the built-in data set, <bpt id="p1">*</bpt>AirlineDemoSmall.csv<ept id="p1">*</ept> provided with RevoScaleR.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>You can verify that it is on your local system as follows:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>To use this file in our distributed computations, it must first be copied to Hadoop Distributed File System (HDFS).</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>For our examples, we make extensive use of the HDFS shared directory, /share:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>First, check to see what directories and files are already in your shared file directory.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>You can use the <bpt id="p1">*</bpt>rxHadoopListFiles<ept id="p1">*</ept> function, which will automatically check your active compute context for information:</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>If the AirlineDemoSmall subdirectory does not exist and you have write permission, you can use the following functions to copy the data there:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>We can then verify that it exists as follows:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>5 - Create a data source</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>In a Spark compute context, you can create data sources using the following functions:</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>A comma-delimited text data source.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Data in the XDF data file format.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>In RevoScaleR, the XDF file format is modified for Hadoop to store data in a composite set of files rather than a single file.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Generates a Hive Data Source object.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Generates a Parquet Data Source object.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Generates an Orc Data Source object.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>In this step, create an RxTextData object using the text file you just copied to HDFS.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>First, create a file system object that uses the default values:</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>The input .csv file uses the letter M to represent missing values, rather than the default NA, so we specify this with the <bpt id="p1">*</bpt>missingValueString<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>We will explicitly set the factor levels for <bpt id="p1">*</bpt>DayOfWeek<ept id="p1">*</ept> in the desired order using the <bpt id="p2">*</bpt>colInfo<ept id="p2">*</ept> argument:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>6 - Summarize data</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">*</bpt>rxSummary<ept id="p1">*</ept> function to obtain descriptive statistics for your data.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxSummary<ept id="p1">*</ept> function takes a formula as its first argument, and the name of the data set as the second.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Summary statistics are computed on the variables in the formula, removing missing values for all rows in the included variables:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Notice that the summary information shows cell counts for categorical variables, and appropriately does not provide summary statistics such as <bpt id="p1">*</bpt>Mean<ept id="p1">*</ept> and <bpt id="p2">*</bpt>StdDev<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Also notice that the <bpt id="p1">*</bpt>Call:<ept id="p1">*</ept> line shows the actual call you entered or the call provided by <bpt id="p2">*</bpt>summary<ept id="p2">*</ept>, so appear differently in different circumstances.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>You can also compute summary information by one or more categories by using interactions of a numeric variable with a factor variable.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>For example, to compute summary statistics on Arrival Delay by Day of Week:</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>The output shows the summary statistics for <bpt id="p1">*</bpt>ArrDelay<ept id="p1">*</ept> for each day of the week:</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>7 - Fit a linear model</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">*</bpt>rxLinMod<ept id="p1">*</ept> function to fit a linear model using your <bpt id="p2">*</bpt>airDS<ept id="p2">*</ept> data source.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Use a single dependent variable, the factor <bpt id="p1">*</bpt>DayOfWeek<ept id="p1">*</ept>:</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>The resulting output is:</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>More Spark scenarios</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Use Machine Learning Server as a Hadoop Client</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>A common practice is to do exploratory analysis on your laptop, then deploy the same analytics code on a Hadoop cluster.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>The underlying RevoScaleR engine in Machine Learning Server handles the distribution of the computations across cores and nodes automatically.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>If you are running Machine Learning Server from Linux or from a Windows computer equipped with PuTTY <bpt id="p1">*</bpt>and/or<ept id="p1">*</ept> both the Cygwin shell and Cygwin OpenSSH packages, you can create a compute context that runs <bpt id="p2">**</bpt>RevoScaleR<ept id="p2">**</ept> functions from your local client in a distributed fashion on your Hadoop cluster.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>You use <bpt id="p1">*</bpt>RxSpark<ept id="p1">*</ept> to create the compute context, but use additional arguments to specify your user name, the file-sharing directory where you have read and write access, the publicly facing host name, or IP address of your Hadoop cluster’s name node or an edge node that run the master processes, and any additional switches to pass to the ssh command (such as the -i flag if you are using a pem or ppk file for authentication, or -p to specify a non-standard ssh port number).</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>if you are using a pem or ppk file for authentication the permissions of the file must be modified to ensure that only the owner has full read and write access (that is, chmod go-rwx user1.pem).</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>If you are using PuTTY, you may incorporate the publicly facing host name and any authentication requirements into a PuTTY saved session, and use the name of that saved session as the sshHostname.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>The above assumes that the directory containing the ssh and scp commands (Linux/Cygwin) or plink and pscp commands (PuTTY) is in your path (or that the Cygwin installer has stored its directory in the Windows registry).</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>If not, you can specify the location of these files using the sshClientDir argument:</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>In some cases, you may find that environment variables needed by Hadoop are not set in the remote sessions run on the sshHostname computer.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>This may be because a different profile or startup script is being read on ssh login.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>You can specify the appropriate profile script by specifying the sshProfileScript argument to RxSpark; this should be an absolute path:</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Now that you have defined your compute context, make it the active compute context using the <bpt id="p1">*</bpt>rxSetComputeContext<ept id="p1">*</ept> function:</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Use RxSpark Compute Context in Persistent Mode</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>By default, with RxSpark Compute Context, a new Spark application is launched when a job starts and is terminated when the job completes.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>To avoid the overhead of Spark initialization on launching time, the persistentRun mode (experimental) is introduced.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>If you set persistentRun as “TRUE”, the Spark application (and associated processes) persists across jobs until idleTimeout or the rxStopEngine is called explicitly:</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>The idleTimeout is the number of seconds of being idle before the system kills the Spark process.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>If persistentRun mode is enabled, then the RxSpark compute context cannot be a Non-Waiting Compute Context.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>Non-Waiting Compute Context<ept id="p1">](#NonWaitingComputeContext)</ept>.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Use a local compute context</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>At times, it may be more efficient to perform smaller computations on the local node rather than using Spark.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>You can easily do this, accessing the same data from the HDFS file system.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>When working with the local compute context, you need to specify the name of a specific data file.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>The same basic code is then used to run the analysis; simply change the compute context to a local context.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>(Note that this will not work if you are accessing the Hadoop cluster via a client.)</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>The results are the same as doing the computations across the nodes with the RxSpark compute context:</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Now set the compute context back to the Hadoop cluster for further analyses:</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Create a Non-Waiting Compute Context</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>When running all but the shortest analyses in Hadoop, it can be convenient to let Hadoop do its processing while returning control of your R session to you immediately.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>You can do this by specifying <bpt id="p1">*</bpt>wait = FALSE<ept id="p1">*</ept> in your compute context definition.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>By using our existing compute context as the first argument, all of the other settings will be carried over to the new compute context:</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Once you have set your compute context to non-waiting, distributed <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions return relatively quickly with a <bpt id="p2">*</bpt>jobInfo<ept id="p2">*</ept> object, which you can use to track the progress of your job, and, when the job is complete, obtain the results of the job.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>For example, we can rerun our linear model in the non-waiting case as follows:</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Right after submission, the job status will typically return <bpt id="p1">*</bpt>"running"<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>When the job status returns <bpt id="p1">*</bpt>"finished"<ept id="p1">*</ept>, you can obtain the results using <bpt id="p2">*</bpt>rxGetJobResults<ept id="p2">*</ept> as follows:</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>You should always assign the <bpt id="p1">*</bpt>jobInfo<ept id="p1">*</ept> object so that you can easily track your work, but if you forget, the most recent <bpt id="p2">*</bpt>jobInfo<ept id="p2">*</ept> object is saved in the global environment as the object <bpt id="p3">*</bpt>rxgLastPendingJob<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>(By default, after you’ve retrieved your job results, the results are removed from the cluster.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>To have your job results remain, set the <bpt id="p1">*</bpt>autoCleanup<ept id="p1">*</ept> argument to <bpt id="p2">*</bpt>FALSE<ept id="p2">*</ept> in <bpt id="p3">*</bpt>RxSpark<ept id="p3">*</ept>.)</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>If after submitting a job in a non-waiting compute context, you decide you don’t want to complete the job, you can cancel the job using the <bpt id="p1">*</bpt>rxCancelJob<ept id="p1">*</ept> function:</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxCancelJob<ept id="p1">*</ept> function returns <bpt id="p2">*</bpt>TRUE<ept id="p2">*</ept> if the job is successfully canceled, <bpt id="p3">*</bpt>FALSE<ept id="p3">*</ept> otherwise.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>For the remainder of this tutorial, we return to a waiting compute context:</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Analyze a Large Data Set</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Set up the sample airline dataset</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>We will now move to examples using a much larger version of the airline data set.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>airline on-time data<ept id="p1">](http://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=236)</ept> has been gathered by the Department of Transportation since 1987.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>The data through 2008 was used in the American Statistical Association Data Expo in 2009 (<ph id="ph1">&lt;http://stat-computing.org/dataexpo/2009/&gt;</ph>).</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>ASA describes the data set as follows:</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>The data consists of flight arrival and departure details for all commercial flights within the USA, from October 1987 to April 2008. This is a large dataset: there are nearly 120 million records in total, and takes up 1.6 gigabytes of space compressed and 12 gigabytes when uncompressed.<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>The airline on-time data set for 2012, consisting of 12 separate CSV files, is available <bpt id="p1">[</bpt>online<ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698896&amp;clcid=0x409)</ept>.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>We assume you have uploaded them to the /tmp directory on your edge node or a name node (although any directory visible as a native file system directory from the name node will work.)</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>As before, our first step is to copy the data into HDFS.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>We specify the location of your Hadoop-stored data for the <bpt id="p1">*</bpt>airDataDir<ept id="p1">*</ept> variable:</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>The original CSV files have rather unwieldy variable names, so we supply a colInfo list to make them more manageable (we won’t use all of these variables in this manual, but you use the data sources created in this manual as you continue to explore distributed computing in the <bpt id="p1">[</bpt>RevoScaleR Distributed Computing Guide<ept id="p1">](how-to-revoscaler-distributed-computing.md)</ept>:</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>We create a data source using these definitions as follows:</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Estimate a linear model with a big data set</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>We fit our first model to the large airline data much as we created the linear model for the AirlineDemoSmall data, and we time it to see how long it takes to fit the model on this large data set:</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>To see a summary of your results:</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>You should see the following results:</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>DayOfWeek=Sun   2.82780    0.03829   73.84 2.22e-16 ***</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>858366</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Notice that the results indicate we have processed all the data, six million observations, using all the .csv files in the specified directory.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Notice also that because we specified <bpt id="p1">*</bpt>cube = TRUE<ept id="p1">*</ept>, we have an estimated coefficient for each day of the week (and not the intercept).</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Import data as composite XDF files</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>As we have seen, you can analyze CSV files directly with RevoScaleR on Hadoop, but the analysis can be done more quickly if the data is stored in a more efficient format.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>The RevoScaleR .xdf format is extremely efficient, but is modified somewhat for HDFS so that individual files remain within a single HDFS block.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>(The HDFS block size varies from installation to installation but is typically either 64 MB or 128 MB.) When you use rxImport on Hadoop, you specify an RxTextData data source such as bigAirDS as the inData and an RxXdfData data source with fileSystem set to an HDFS file system as the outFile argument to create a set of <bpt id="p1">*</bpt>composite .xdf files<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>The RxXdfData object can then be used as the data argument in subsequent RevoScaleR analyses.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>For our airline data, we define our RxXdfData object as follows (the second “user” should be replaced by your actual user name on the Hadoop cluster):</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>We set a block size of 250000 rows and specify that we read all the data by specifying</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>We then import the data using rxImport:</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Write to CSV in HDFS</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>If you <bpt id="p1">[</bpt>converted your CSV to XDF<ept id="p1">](#importingDataAsCompositeXdfFiles)</ept> to take advantage of the efficiency while running analyses, but now wish to convert your data back to CSV you can do so using <bpt id="p2">*</bpt>rxDataStep<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>To create a folder of CSV files, first create an RxTextData object using a directory name as the file argument; this represents the folder in which to create the CSV files.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>This directory is created when you run the <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>Then, point to this <bpt id="p1">*</bpt>RxTextData<ept id="p1">*</ept> object in the <bpt id="p2">*</bpt>outFile<ept id="p2">*</ept> argument of the <bpt id="p3">*</bpt>rxDataStep<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Each CSV created will be named based on the directory name and followed by a number.</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>Suppose we want to write out a folder of CSV in HDFS from our airData composite XDF after we performed the logistic regression and prediction, so that the new CSV files contain the predicted values and residuals.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>We can do this as follows:</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>You notice that the <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept> wrote out one CSV for every .xdfd file in the input composite XDF file.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>This is the default behavior for writing CSV from composite XDF to HDFS when the compute context is set to RxSpark.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>Alternatively, you could switch your compute context back to “local” when you are done performing your analyses and take advantage of two arguments within <bpt id="p1">*</bpt>RxTextData<ept id="p1">*</ept> that give you slightly more control when writing out CSV files to HDFS: <bpt id="p2">*</bpt>createFileSet<ept id="p2">*</ept> and <bpt id="p3">*</bpt>rowsPerOutFile<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>When <bpt id="p1">*</bpt>createFileSet<ept id="p1">*</ept> is set to TRUE a folder of CSV files is written to the directory you specify.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>When <bpt id="p1">*</bpt>createFileSet<ept id="p1">*</ept> is set to FALSE a single CSV file is written.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>The second argument, <bpt id="p1">*</bpt>rowsPerOutFile<ept id="p1">*</ept>, can be set to an integer to indicate how many rows to write to each CSV file when <bpt id="p2">*</bpt>createFileSet<ept id="p2">*</ept> is TRUE.</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>Returning to the example above, suppose we wanted to write out a folder of CSVs but we wanted to write out the airData but into only six CSV files.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>When using an RxSpark compute context, createFileSet defaults to TRUE and rowsPerOutFile has no effect.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>Thus if you wish to create a single CSV or customize the number of rows per file you must perform the rxDataStep in a local compute context (data can still be in HDFS).</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>Estimate a linear model using composite XDF files</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>Now we can re-estimate the same linear model, using the new, faster data source:</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>To see a summary of your results:</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>You should see the following results (which should match the results we found for the CSV files above):</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>DayOfWeek=Sun   2.82780    0.03829   73.84 2.22e-16 ***</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>858366</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>Handling larger linear models</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>The data set contains a variable <bpt id="p1">*</bpt>UniqueCarrier<ept id="p1">*</ept>, which contains airline codes for 15 carriers.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>Because the RevoScaleR Compute Engine handles factor variables so efficiently, we can do a linear regression looking at the Arrival Delay by Carrier.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>This takes a little longer than the previous analysis, because we are estimating 15 instead of 7 parameters.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>Next, sort the coefficient vector so that  we can see the airlines with the highest and lowest values.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>Next, see how the airlines rank in arrival delays:</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>The result is:</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>Notice that Alaska Airlines comes in as the best in on-time arrivals, while Frontier is at the bottom of the list.</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>We can see the difference by subtracting the coefficients:</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>which results in:</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>A Large Data Logistic Regression</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>Our airline data includes a logical variable, ArrDel15, that tells whether a flight is 15 or more minutes late.</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>We can use this as the response for a logistic regression to model the likelihood that a flight will be late given the day of the week:</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>which results in:</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>Prediction on Large Data</source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>You can predict (or score) from a fitted model on Hadoop using <bpt id="p1">*</bpt>rxPredict<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>In this example, we compute predicted values and their residuals for the logistic regression in the previous section.</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source>These new prediction variables are output to a new composite XDF in HDFS.</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>(As in an earlier example, the second “user” in the airDataPredDir path should be changed to the actual user name of your Hadoop user.)</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>By putting in a call to <bpt id="p1">*</bpt>rxGetVarInfo<ept id="p1">*</ept> we see that two variables, <bpt id="p2">*</bpt>ArrDel15<ph id="ph1">\_</ph>Pred<ept id="p2">*</ept> and <bpt id="p3">*</bpt>ArrDel15<ph id="ph2">\_</ph>Resid<ept id="p3">*</ept> were written to the <bpt id="p4">*</bpt>airDataPred<ept id="p4">*</ept> composite XDF.</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>If in addition to the prediction variables, we wanted to have the variables used in the model written to our <bpt id="p1">*</bpt>outData<ept id="p1">*</ept> we would need to add the <bpt id="p2">*</bpt>writeModelVars=TRUE<ept id="p2">*</ept> to our <bpt id="p3">*</bpt>rxPredict<ept id="p3">*</ept> call.</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>Alternatively, we can update the <bpt id="p1">*</bpt>airData<ept id="p1">*</ept> to include the predicted values and residuals by not specifying an <bpt id="p2">*</bpt>outData<ept id="p2">*</ept> argument, which is <bpt id="p3">*</bpt>NULL<ept id="p3">*</ept> by default.</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>Since the <bpt id="p1">*</bpt>airData<ept id="p1">*</ept> composite XDF already exists, we would need to add <bpt id="p2">*</bpt>overwrite=TRUE<ept id="p2">*</ept> to the <bpt id="p3">*</bpt>rxPredict<ept id="p3">*</ept> call.</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>An <bpt id="p1">*</bpt>RxTextData<ept id="p1">*</ept> object can be used as the input data for <bpt id="p2">*</bpt>rxPredict<ept id="p2">*</ept> on Hadoop, but only XDF can be written to HDFS.</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source>When using a CSV file or directory of CSV files as the input data to <bpt id="p1">*</bpt>rxPredict<ept id="p1">*</ept> the <bpt id="p2">*</bpt>outData<ept id="p2">*</ept> argument must be set to an <bpt id="p3">*</bpt>RxXdfData<ept id="p3">*</ept> object.</source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>Performing Data Operations on Large Data</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source>To create or modify data in HDFS on Hadoop, we can use the <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept> function.</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>Suppose we want to repeat the analyses with a “cleaner” version of the large airline dataset.</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source>To do this we keep only the flights having arrival delay information and flights that did not depart more than one hour early.</source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source>We can put a call to <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept> to output a new composite XDF to HDFS.</source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source>(As in an earlier example, the second “user” in the newAirDir path should be changed to the actual user name of your Hadoop user.)</source>
        </trans-unit><trans-unit id="324" translate="yes" xml:space="preserve">
          <source>To modify an existing composite XDF using <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept> set the <bpt id="p2">*</bpt>overwrite<ept id="p2">*</ept> argument to <bpt id="p3">*</bpt>TRUE<ept id="p3">*</ept> and either omit the <bpt id="p4">*</bpt>outFile<ept id="p4">*</ept> argument or set it to the same data source specified for <bpt id="p5">*</bpt>inData<ept id="p5">*</ept>.</source>
        </trans-unit><trans-unit id="325" translate="yes" xml:space="preserve">
          <source>Parallel Partial Decision Forests</source>
        </trans-unit><trans-unit id="326" translate="yes" xml:space="preserve">
          <source>As mentioned earlier, both <bpt id="p1">*</bpt>rxDForest<ept id="p1">*</ept> and <bpt id="p2">*</bpt>rxBTrees<ept id="p2">*</ept> are available on Hadoop--these provide two different methods for fitting classification and regression decision forests.</source>
        </trans-unit><trans-unit id="327" translate="yes" xml:space="preserve">
          <source>In the default case, both algorithms generate multiple stages in the Spark job, and thus can tend to incur significant overhead, particularly with smaller data sets.</source>
        </trans-unit><trans-unit id="328" translate="yes" xml:space="preserve">
          <source>However, the <bpt id="p1">*</bpt>scheduleOnce<ept id="p1">*</ept> argument to both functions allows the computation to be performed via <bpt id="p2">*</bpt>rxExec<ept id="p2">*</ept>, which generates only a single stage in the Spark job, and thus incurs significantly less overhead.</source>
        </trans-unit><trans-unit id="329" translate="yes" xml:space="preserve">
          <source>When using the <bpt id="p1">*</bpt>scheduleOnce<ept id="p1">*</ept> argument, you can specify the number of trees to be grown within each <bpt id="p2">*</bpt>rxExec<ept id="p2">*</ept> task using the forest function’s <bpt id="p3">*</bpt>nTree<ept id="p3">*</ept> argument together with <bpt id="p4">*</bpt>rxExec’s<ept id="p4">*</ept> <bpt id="p5">*</bpt>rxElemArgs<ept id="p5">*</ept> function, as in the following regression example using the built-in claims data:</source>
        </trans-unit><trans-unit id="330" translate="yes" xml:space="preserve">
          <source>Equivalently, you can use nTree together with rxExec’s timesToRun argument:</source>
        </trans-unit><trans-unit id="331" translate="yes" xml:space="preserve">
          <source>In this example, using <bpt id="p1">*</bpt>scheduleOnce<ept id="p1">*</ept> can be up to 45 times faster than the default, and so we recommend it for decision forests with small to moderate-sized data sets.</source>
        </trans-unit><trans-unit id="332" translate="yes" xml:space="preserve">
          <source>Similarly, the <bpt id="p1">*</bpt>rxPredict<ept id="p1">*</ept> methods for <bpt id="p2">*</bpt>rxDForest<ept id="p2">*</ept> and <bpt id="p3">*</bpt>rxBTrees<ept id="p3">*</ept> objects include the <bpt id="p4">*</bpt>scheduleOnce<ept id="p4">*</ept> argument, and should be used when using these methods on small to moderate-sized data sets.</source>
        </trans-unit><trans-unit id="333" translate="yes" xml:space="preserve">
          <source>Using Hive data</source>
        </trans-unit><trans-unit id="334" translate="yes" xml:space="preserve">
          <source>There are multiple ways to access and use data from Hive for analyses with RevoScaleR.</source>
        </trans-unit><trans-unit id="335" translate="yes" xml:space="preserve">
          <source>Here are some general recommendations, assuming in each case that the data for analysis is defined by the results of a Hive query.</source>
        </trans-unit><trans-unit id="336" translate="yes" xml:space="preserve">
          <source>If running from a remote client or edge node, and the data is modest, then use RxOdbcData to stream results, or land them as XDF in the local file system, for subsequent analysis in a local compute context.</source>
        </trans-unit><trans-unit id="337" translate="yes" xml:space="preserve">
          <source>If the data is large, then use the Hive command-line interface (hive or beeline) from an edge node to run the Hive query with results spooled to a text file on HDFS for subsequent analysis in a distributed fashion using the HadoopMR or Spark compute contexts.</source>
        </trans-unit><trans-unit id="338" translate="yes" xml:space="preserve">
          <source>Here’s how to get started with each of these approaches.</source>
        </trans-unit><trans-unit id="339" translate="yes" xml:space="preserve">
          <source>Accessing Hive data via ODBC</source>
        </trans-unit><trans-unit id="340" translate="yes" xml:space="preserve">
          <source>Start by following your Hadoop vendor’s recommendations for accessing Hive via ODBC from a remote client or edge node.</source>
        </trans-unit><trans-unit id="341" translate="yes" xml:space="preserve">
          <source>Once you have the prerequisite software installed and have run a smoke test to verify connectivity, then accessing data in Hive from Machine Learning Server is just like accessing data from any other data source.</source>
        </trans-unit><trans-unit id="342" translate="yes" xml:space="preserve">
          <source>Accessing Hive data via an Export to Text Files</source>
        </trans-unit><trans-unit id="343" translate="yes" xml:space="preserve">
          <source>This approach uses the Hive command-line interface to first spool the results to text files in the local or HDFS file systems and then analyze them in a distributed fashion using local or HadoopMR/Spark compute contexts.</source>
        </trans-unit><trans-unit id="344" translate="yes" xml:space="preserve">
          <source>First, check with your Hadoop system administrator find out whether the ‘hive’ or ‘beeline’ command should be used to run a Hive query from the command line, and obtain the needed credentials for access.</source>
        </trans-unit><trans-unit id="345" translate="yes" xml:space="preserve">
          <source>Next, try out your hive/beeline command from the Linux command line to make sure it works and that you have the proper authentication and syntax.</source>
        </trans-unit><trans-unit id="346" translate="yes" xml:space="preserve">
          <source>Finally, run the command from within R using R’s system command.</source>
        </trans-unit><trans-unit id="347" translate="yes" xml:space="preserve">
          <source>Here are some sample R statements that output a Hive query to the local and HDFS file systems:</source>
        </trans-unit><trans-unit id="348" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Run a Hive query and dump results to a local text file (edge node)<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="349" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Run the same query using beeline’s csv2 output format<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="350" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Run the same query but dump the results to CSV in HDFS<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="351" translate="yes" xml:space="preserve">
          <source>After you’ve exported the query results to a text file, it can be streamed directly as input to a RevoScaleR analysis routine via use of the RxTextdata data source, or imported to XDF for improved performance upon repeated access.</source>
        </trans-unit><trans-unit id="352" translate="yes" xml:space="preserve">
          <source>Here’s an example assuming output was spooled as text to HDFS:</source>
        </trans-unit><trans-unit id="353" translate="yes" xml:space="preserve">
          <source>Clean up Data</source>
        </trans-unit><trans-unit id="354" translate="yes" xml:space="preserve">
          <source>You can run the following commands to clean up data in this tutorial:</source>
        </trans-unit></group></body></file></xliff>