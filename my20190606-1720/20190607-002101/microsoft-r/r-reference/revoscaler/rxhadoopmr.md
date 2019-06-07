<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxhadoopmr.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c3703610c7c7629b7753c006d56c758a35ea6aeb231.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">03610c7c7629b7753c006d56c758a35ea6aeb231</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxhadoopmr.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxHadoopMR function (RevoScaleR)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Creates a compute context for use with a Hadoop cluster.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxHadoopMR compute context is deprecated.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Please consider using RxSpark compute context instead.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(RevoScaleR), RxHadoopMR, IO</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>RxHadoopMR: Generate Hadoop Map Reduce Compute Context</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>DEPRECATED: Creates a compute context for use with a Hadoop cluster.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>RxHadoopMR compute context is deprecated.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Please consider using RxSpark compute context instead.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>object of class RxHadoopMR.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This argument is optional.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If supplied, the values of  the other specified arguments are used to replace those of <ph id="ph1">`object`</ph> and the modified object is returned.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>character string specifying the file sharing location within HDFS.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>You must  have permissions to read and write to this location.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>character string specifying the directory on the master (perhaps edge) node that is  shared among all the nodes of the cluster and any client host.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>You must have permissions to read and write  in this directory.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>character string specifying the absolute path of the temporary directory on the client.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Defaults to /tmp for POSIX-compliant non-Windows clients.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>For Windows and non-compliant POSIX clients,  defaults to the value of the TEMP environment variable if defined, else to the TMP environment variable  if defined, else to <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If the default directory does not exist, defaults to NULL.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>UNC paths ("<ph id="ph1">`\\host\dir`</ph>") are not supported.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>character string specifying the path to the directory on the cluster  compute nodes containing the files R.exe and Rterm.exe.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The invocation of R on each  node must be identical.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>character string specifying the path to the directory on the master (perhaps edge) node  containing the files R.exe and Rterm.exe.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>character string specifying optional generic Hadoop command line switches, for example <ph id="ph1">`-conf myconf.xml`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt><ph id="ph1">`http://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-common/CommandsManual.html`</ph><ept id="p1">](http://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-common/CommandsManual.html)</ept>  for details on the Hadoop command line generic options.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>character string specifying the username for making an ssh connection to the Hadoop cluster.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>This is not needed if you are running your R client directly on the cluster.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Defaults to the username of the user running the R client (that is, the value of <ph id="ph1">`Sys.info()[["user"]]`</ph>).</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>character string specifying the hostname or IP address of the Hadoop cluster  node or edge node that the client will log into for launching Hadoop jobs and for copying files  between the client machine and the Hadoop cluster.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Defaults to the hostname of the machine running  the R client (that is, the value of <ph id="ph1">`Sys.info()[["nodename"]]`</ph>)  This field is only used if  <ph id="ph2">`onClusterNode`</ph> is <ph id="ph3">`NULL`</ph> or <ph id="ph4">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If you are using PuTTY on a Windows system, this can be the name of a saved PuTTY session that can include the user name and authentication file to use.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>character string specifying any switches needed for making an ssh connection to the Hadoop cluster.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>This is not needed if one is running one's R client directly on the cluster.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Optional character string specifying the absolute path to a profile script that will exists on the sshHostname host.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>This is used when the target ssh host does not automatically read in a .bash_profile, .profile or other shell environment configuration file for the definition of requisite variables such as HADOOP_STREAMING.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>character string specifying the Windows directory where Cygwin's ssh.exe  and scp.exe or PuTTY's plink.exe and pscp.exe executables can be found.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Needed only for Windows.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Not needed if these executables are on the Windows Path or if Cygwin's location can be found in  the Windows Registry.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Defaults to the empty string.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>logical scalar specifying whether run-as-user mode is being used on the Hadoop cluster.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>When using run-as-user mode, local R processes started by the map-reduce framework will run as the same user that started the job, and will have any allocated local permissions.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>When not using run-as-user mode (the default for many Hadoop systems), local R processes will run as user mapred.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Note that when running as user mapred, permissions for files and directories will have to be more open in order to allow hand-offs between the user and mapred.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Run-as-user mode is controlled for the Hadoop map-reduce framework by the xml setting,  <ph id="ph1">`mapred.task.tracker.task-controller`</ph>, in the <ph id="ph2">`mapred-site.xml`</ph> configuration file.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>If it is set to the value <ph id="ph1">`org.apache.hadoop.mapred.LinuxTaskController`</ph>, then  run-as-user mode is in use.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>If it is set to the value <ph id="ph1">`org.apache.hadoop.mapred.DefaultTaskController`</ph>, then  run-as-user mode is not in use.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>character string specifying the Hadoop name node hostname or IP address.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Typically you can leave this at its default value.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If set to a value other than "default" or the empty string (see below), this must be an address that can be resolved by the data nodes and used by them to contact the  name node.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Depending on your cluster, it may need to be set to a private network address  such as <ph id="ph1">`"master.local"`</ph>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If set to the empty string, "", then the master process will set  this to the name of the node on which it is running, as returned by <ph id="ph1">`Sys.info()[["nodename"]]`</ph>.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>This is likely to work when the sshHostname points to the name node or the sshHostname is not  specified and the R client is running on the name node.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Defaults to rxGetOption("hdfsHost").</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>character scalar specifying the full URL for the jobtracker web interface.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>This is used only for the purpose of loading the job tracker web page from the <ph id="ph1">`rxLaunchClusterJobManager`</ph> convenience function.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>It is never used for job control, and its specification in the compute context is completely optional.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>rxLaunchClusterJobManager<ept id="p1">](rxLaunchClusterTaskManager.md)</ept> page for more information.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>numeric scalar specifying the port used by the name node for hadoop jobs.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Needs to be able to be cast to an integer.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Defaults to rxGetOption("hdfsPort").</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>logical scalar or NULL specifying whether the user is initiating the job from a client that will connect to either an edge node or an actual cluster node, directly from either an edge node or node within the cluster.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>If set to  <ph id="ph1">`FALSE`</ph> or <ph id="ph2">`NULL`</ph>, then <ph id="ph3">`sshHostname`</ph> must be a valid host.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the job will be blocking   and will not return until it has completed or has failed.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>,   the job will be non-blocking return immediately,  allowing you to continue running other R code.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The object <ph id="ph1">`rxgLastPendingJob`</ph> is created with the job information.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>You can pass this object to the   <bpt id="p1">[</bpt>rxGetJobStatus<ept id="p1">](rxGetJobResults.md)</ept> function to check on the processing status of the job.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxWaitForJob<ept id="p1">](rxWaitForJob.md)</ept> will change a non-waiting job  to a waiting job.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Conversely, pressing ESC changes a waiting job to a non-waiting job, provided that the HPC scheduler has accepted the job.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>If you press ESC before the job has been accepted, the job is canceled.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, causes the standard output  of the R processes to be printed to the user console.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, causes the standard output  of the remote primary R and hadoop job process to be printed to the user console while waiting for (blocking on)  a job.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the default behavior is to clean up the  temporary computational artifacts and delete the result objects upon retrival.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>,  then the computational results are not deleted, and the results may be acquired using  <bpt id="p1">[</bpt>rxGetJobResults<ept id="p1">](rxGetJobResults.md)</ept>, and the output via <bpt id="p2">[</bpt>rxGetJobOutput<ept id="p2">](rxGetJobOutput.md)</ept> until the  <bpt id="p3">[</bpt>rxCleanupJobs<ept id="p3">](rxCleanup.md)</ept> is used to delete the results and other artifacts.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Leaving this flag set to <ph id="ph1">`FALSE`</ph> can result in accumulation of compute artifacts which you may eventually need to delete before they fill up your hard drive.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>character string specifying a working directory for the processes  on the master node.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>NOT YET IMPLEMENTED.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>character vector defining the search path(s) for the data source(s).</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>NOT YET IMPLEMENTED.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>or character vector defining the search path(s) for   new output data file(s).</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>If not <ph id="ph1">`NULL`</ph>, this overrides any specification for <ph id="ph2">`outDataPath`</ph> in <bpt id="p1">[</bpt>rxOptions<ept id="p1">](rxOptions.md)</ept></source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>or an <bpt id="p1">[</bpt>RxHdfsFileSystem<ept id="p1">](RxHdfsFileSystem.md)</ept> to use as the default file system for data sources when created when this compute context is active.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>optional character vector specifying additional packages to be  loaded on the nodes when jobs are run in this compute context.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>A numeric value indicating for how long attempts should be made  to retrieve results from the cluster.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Under normal conditions, results are available immediately.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>However, under certain high load conditions, the processes on the nodes have reported as completed, but the results have not been fully committed to disk by the operating system.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Increase this parameter if results retrievial is failing on high load clusters.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Microsoft R Services Compute Engine.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>This compute context is supported for Cloudera (CDH4 and CDH5), Hortonworks (HDP 1.3 and 2.x), and MapR (3.0.2, 3.0.3, 3.1.0, and 3.1.1) Hadoop distributions on Red Hat Enterprise Linux 5 and 6.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>object of class RxHadoopMR.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxGetJobStatus<ept id="p1">](rxGetJobResults.md)</ept>, <bpt id="p2">[</bpt>rxGetJobOutput<ept id="p2">](rxGetJobOutput.md)</ept>, <bpt id="p3">[</bpt>rxGetJobResults<ept id="p3">](rxGetJobResults.md)</ept>, <bpt id="p4">[</bpt>rxCleanupJobs<ept id="p4">](rxCleanup.md)</ept>, <bpt id="p5">[</bpt>RxSpark<ept id="p5">](RxSpark.md)</ept>, <bpt id="p6">[</bpt>RxInSqlServer<ept id="p6">](RxInSqlServer.md)</ept>,</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>, <bpt id="p2">[</bpt>rxSetComputeContext<ept id="p2">](rxSetComputeContext.md)</ept>, <bpt id="p3">[</bpt>RxHadoopMR-class<ept id="p3">](RxHadoopMR-class.md)</ept>.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>