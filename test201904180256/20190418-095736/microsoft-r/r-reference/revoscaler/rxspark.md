<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxspark.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18ce9d1de985164b3b18f8e9f00ee696fcfac6cf273.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">e9d1de985164b3b18f8e9f00ee696fcfac6cf273</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxspark.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxSpark function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxSpark creates a Spark compute context.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxSparkConnect creates the compute context object with RxSpark and then immediately starts the remote Spark application.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxSparkDisconnect shuts down the remote Spark application with rxStopEngine and switches to a local compute context.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>All rx* function calls after this will run in a local compute context.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), RxSpark, rxSparkConnect, rxSparkDisconnect, IO</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>RxSpark: Create Spark compute context, connect and disconnect a Spark application</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`RxSpark`</ph> creates a Spark compute context.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxSparkConnect`</ph> creates the compute context object with <ph id="ph2">`RxSpark`</ph> and then immediately starts the remote Spark application.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxSparkDisconnect`</ph> shuts down the remote Spark application with <ph id="ph2">`rxStopEngine`</ph> and switches to a local compute context.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>All <ph id="ph1">`rx*`</ph> function calls after this will run in a local compute context.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>object of class RxSpark.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>This argument is optional.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If supplied, the values of  the other specified arguments are used to replace those of <ph id="ph1">`object`</ph> and the modified object is returned.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>character string specifying the file sharing location within HDFS.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>You must  have permissions to read and write to this location.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>When you are running in Spark local mode, this parameter will be ignored and it will be forced to be equal to the parameter shareDir.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>character string specifying the directory on the master (perhaps edge) node that is  shared among all the nodes of the cluster and any client host.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>You must have permissions to read and write  in this directory.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>character string specifying the absolute path of the temporary directory on the client.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Defaults to /tmp for POSIX-compliant non-Windows clients.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>For Windows and non-compliant POSIX clients,  defaults to the value of the TEMP environment variable if defined, else to the TMP environment variable  if defined, else to <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If the default directory does not exist, defaults to NULL.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>UNC paths ("<ph id="ph1">`\\host\dir`</ph>") are not supported.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>character string specifying the username for making an ssh connection to the Spark cluster.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>This is not needed if you are running your R client directly on the cluster.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Defaults to the username of the user running the R client (that is, the value of <ph id="ph1">`Sys.info()[["user"]]`</ph>).</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>character string specifying the hostname or IP address of the Spark cluster  node or edge node that the client will log into for launching Spark jobs and for copying files  between the client machine and the Spark cluster.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Defaults to the hostname of the machine running  the R client (that is, the value of <ph id="ph1">`Sys.info()[["nodename"]]`</ph>)  This field is only used if  <ph id="ph2">`onClusterNode`</ph> is <ph id="ph3">`NULL`</ph> or <ph id="ph4">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If you are using PuTTY on a Windows system, this can be the name of a saved PuTTY session that can include the user name and authentication file to use.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>character string specifying any switches needed for making an ssh connection to the Spark cluster.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>This is not needed if one is running one's R client directly on the cluster.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Optional character string specifying the absolute path to a profile script on the sshHostname host.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>This is used when the target ssh host does not automatically read in a .bash_profile, .profile or other shell environment configuration file for the definition of requisite variables.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>character string specifying the Windows directory where Cygwin's ssh.exe  and scp.exe or PuTTY's plink.exe and pscp.exe executables can be found.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Needed only for Windows.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Not needed if these executables are on the Windows Path or if Cygwin's location can be found in  the Windows Registry.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Defaults to the empty string.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>character string specifying the Spark name node hostname or IP address.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Typically you can leave this at its default value.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>If set to a value other than "default" or the empty string (see below), this must be an address that can be resolved by the data nodes and used by them to contact the  name node.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Depending on your cluster, it may need to be set to a private network address  such as <ph id="ph1">`"master.local"`</ph>.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If set to the empty string, "", then the master process will set  this to the name of the node on which it is running, as returned by <ph id="ph1">`Sys.info()[["nodename"]]`</ph>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>This is likely to work when the sshHostname points to the name node or the sshHostname is not  specified and the R client is running on the name node.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If you are running in Spark local mode, this paramter defaults to "file:///"; otherwise it defaults to rxGetOption("hdfsHost").</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Character string specifying the master URL passed to Spark.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The value of this parameter could be "yarn", "standalone" and "local".</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The formats of Spark's master URL (except for mesos) specified in this website <bpt id="p1">[</bpt><ph id="ph1">`https://spark.apache.org/docs/latest/submitting-applications.html`</ph><ept id="p1">](https://spark.apache.org/docs/latest/submitting-applications.html)</ept>  is also supported.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>character scalar specifying the full URL for the jobtracker web interface.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>This is used only for the purpose of loading the job tracker web page from the <ph id="ph1">`rxLaunchClusterJobManager`</ph> convenience function.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>It is never used for job control, and its specification in the compute context is completely optional.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>rxLaunchClusterJobManager<ept id="p1">](rxLaunchClusterTaskManager.md)</ept> page for more information.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>numeric scalar specifying the port used by the name node for HDFS.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Needs to be able to be cast to an integer.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Defaults to rxGetOption("hdfsPort").</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>logical scalar or NULL specifying whether the user is initiating the job from a client that will connect to either an edge node or an actual cluster node, directly from either an edge node or node within the cluster.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>If set to  <ph id="ph1">`FALSE`</ph> or <ph id="ph2">`NULL`</ph>, then <ph id="ph3">`sshHostname`</ph> must be a valid host.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> or if <ph id="ph2">`persistentRun`</ph> is <ph id="ph3">`TRUE`</ph>, the job will be blocking and the invoking function will not return until the job has completed or has failed.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Otherwise, the job will be non-blocking and the invoking function will return, allowing you to continue running other R code.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>The object <ph id="ph1">`rxgLastPendingJob`</ph> is created with the job information.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>You can pass this object to the  <bpt id="p1">[</bpt>rxGetJobStatus<ept id="p1">](rxGetJobResults.md)</ept> function to check on the processing status of the job.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxWaitForJob<ept id="p1">](rxWaitForJob.md)</ept> will change a non-waiting job  to a waiting job.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Conversely, pressing ESC changes a waiting job to a non-waiting job, provided that the scheduler has accepted the job.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>If you press ESC before the job has been accepted, the job is canceled.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>numeric scalar specifying the number of executors in Spark, which is  equivalent to parameter --num-executors in spark-submit app.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>If not specified,  the default behavior is to launch as many executors as possible, which may use up all resources and prevent other users from sharing the cluster.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>numeric scalar specifying the number of cores per executor, which is  equivalent to parameter --executor-cores in spark-submit app.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>character string specifying memory per executor (e.g., 1000M, 2G), which is  equivalent to parameter --executor-memory in spark-submit app.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>character string specifying memory for driver (e.g., 1000M, 2G), which is  equivalent to parameter --driver-memory in spark-submit app.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>character string specifying memory overhead per executor (e.g. 1000M, 2G), which is  equivalent to setting spark.yarn.executor.memoryOverhead in YARN.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Increasing this value will allocate more memory for the R process and the ScaleR engine process in the YARN executors, so it may help resolve job failure or executor lost issues.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>character string specifying extra arbitrary Spark properties  (e.g., <ph id="ph1">`"--conf spark.speculation=true --conf spark.yarn.queue=aQueue"`</ph>), which is equivalent to additional parameters passed into spark-submit app.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>EXPERIMENTAL.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the Spark application (and associated processes) will persist across jobs until the idleTimeout is reached or the <bpt id="p1">[</bpt>rxStopEngine<ept id="p1">](rxStopEngine.md)</ept> function is called explicitly.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>This avoids the overhead of  launching a new Spark application for each job.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, a new Spark application will be launched  when a job starts and will be terminated when the job completes.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Spark job collects all parallel tasks' results to reduce as final result.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>This parameter decides reduce strategy: oneStage/twoStage/auto. oneStage: reduce parallel tasks to one result with one reduce function; twoStage: reduce paralllel tasks to square root size with the first reduce function, then reduce to final result with the second reduce function; auto: spark will smartly select oneStage or twoStage.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>numeric scalar specifying the number of seconds of being idle (i.e., not running any Spark job) before system kills the Spark process.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Setting a value greater than 600 is recommended.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Setting a negative value will not timeout.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>sparklyr interoperation will have no timeout.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, suppress warning message regarding missing Spark application parameters.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, causes the standard output  of the R processes to be printed to the user console.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, causes the standard output  of the remote primary R and Spark job process to be printed to the user console while waiting for (blocking on)  a job.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the default behavior is to clean up the  temporary computational artifacts and delete the result objects upon retrieval.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>,  then the computational results are not deleted, and the results may be acquired using  <bpt id="p1">[</bpt>rxGetJobResults<ept id="p1">](rxGetJobResults.md)</ept>, and the output via <bpt id="p2">[</bpt>rxGetJobOutput<ept id="p2">](rxGetJobOutput.md)</ept> until the  <bpt id="p3">[</bpt>rxCleanupJobs<ept id="p3">](rxCleanup.md)</ept> is used to delete the results and other artifacts.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Leaving this flag set to <ph id="ph1">`FALSE`</ph> can result in accumulation of compute artifacts which you may eventually need to delete before they fill up your hard drive.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>character string specifying a working directory for the processes  on the master node.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>NOT YET IMPLEMENTED.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>character vector defining the search path(s) for the data source(s).</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>NOT YET IMPLEMENTED.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or character vector defining the search path(s) for   new output data file(s).</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>If not <ph id="ph1">`NULL`</ph>, this overrides any specification for <ph id="ph2">`outDataPath`</ph> in <bpt id="p1">[</bpt>rxOptions<ept id="p1">](rxOptions.md)</ept></source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or an <bpt id="p1">[</bpt>RxHdfsFileSystem<ept id="p1">](RxHdfsFileSystem.md)</ept> to use as the default file system for data sources when created when this compute context is active.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>optional character vector specifying additional packages to be  loaded on the nodes when jobs are run in this compute context.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>A numeric value indicating for how long attempts should be made  to retrieve results from the cluster.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Under normal conditions, results are available immediately.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>However, under certain high load conditions, the processes on the nodes have reported as completed, but the results have not been fully committed to disk by the operating system.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Increase this parameter if results retrieval is failing on high load clusters.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>character string specifying the temporary working directory in worker nodes.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>It defaults to /dev/shm to utilize in-memory temporary file system for performance gain, when the size of /dev/shm is less than 1G, the default value would switch to /tmp for guarantee sufficiency You can specify a different location if the size of /dev/shm is insufficient.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Please make sure that YARN run-as user has permission to read and write to this location</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>if <ph id="ph1">`TRUE`</ph> all cached Spark Data Frames will be freed and all existing Spark applications that belong to the current user will be shut down.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or a character string or vector of package names for RevoScaleR interoperation.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Currently, the "sparklyr" package is supported.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Spark compute context to be terminated by <ph id="ph1">`rxSparkDisconnect`</ph>.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Microsoft R Services Compute Engine.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>This compute context is supported for Cloudera, Hortonworks, and MapR Hadoop distributions.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>object of class RxSpark.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxGetJobStatus<ept id="p1">](rxGetJobResults.md)</ept>, <bpt id="p2">[</bpt>rxGetJobOutput<ept id="p2">](rxGetJobOutput.md)</ept>, <bpt id="p3">[</bpt>rxGetJobResults<ept id="p3">](rxGetJobResults.md)</ept>, <bpt id="p4">[</bpt>rxCleanupJobs<ept id="p4">](rxCleanup.md)</ept>, RxHadoopMR, <bpt id="p5">[</bpt>RxInSqlServer<ept id="p5">](RxInSqlServer.md)</ept>,</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>, <bpt id="p2">[</bpt>rxSetComputeContext<ept id="p2">](rxSetComputeContext.md)</ept>, <bpt id="p3">[</bpt>RxSpark-class<ept id="p3">](RxSpark-class.md)</ept>.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>