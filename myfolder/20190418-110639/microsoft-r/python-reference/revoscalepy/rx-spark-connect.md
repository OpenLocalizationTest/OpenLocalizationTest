<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-spark-connect.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907fa0fcac189d17b5fc137b33396c1aaa09573c0c81.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a0fcac189d17b5fc137b33396c1aaa09573c0c81</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-spark-connect.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_spark_connect: Connect to remote Spark applications (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Creates the compute context object with RxSpark and then immediately starts the remote Spark application.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>rx_spark_connect</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Creates the compute context object with RxSpark and then immediately starts the remote Spark application.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>hdfs_share_dir</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Character string specifying the file sharing location within HDFS.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>You must have permissions to read and write to this location.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>When you are running in Spark local mode, this parameter will be ignored and it will be forced to be equal to the parameter share_dir.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>share_dir</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Character string specifying the directory on the master (perhaps edge) node that is shared among all the nodes of the cluster and any client host.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>You must have permissions to read and write in this directory.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>user</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Character string specifying the username for submitting job to the Spark cluster.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Defaults to the username of the user running the python (that is, the value of getpass.getuser()).</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>name_node</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Character string specifying the Spark name node hostname or IP address.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Typically you can leave this at its default value.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If set to a value other than “default” or the empty string (see below), this must be an address that can be resolved by the data nodes and used by them to contact the name node.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Depending on your cluster, it may need to be set to a private network address such as “master.local”.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If set to the empty string, “”, then the master process will set this to the name of the node on which it is running, as returned by platform.node().</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If you are running in Spark local mode, this parameter defaults to “[file:///](file:///.md)”; otherwise it defaults to RxOptions.get_option(“hdfsHost”).</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>master</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Character string specifying the master URL passed to Spark.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The value of this parameter could be “yarn”, “standalone” and “local”.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The formats of Spark’s master URL (except for mesos) specified in this website <bpt id="p1">[</bpt><ph id="ph1">https://spark.apache.org/docs/latest/submitting-applications.html</ph><ept id="p1">](https://spark.apache.org/docs/latest/submitting-applications.html)</ept> are also supported.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>port</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Integer value specifying the port used by the name node for HDFS.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Needs to be able to be cast to an integer.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Defaults to RxOptions.get_option(“hdfsPort”).</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>auto_cleanup</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Bool value, if True, the default behavior is to clean up the temporary computational artifacts and delete the result objects upon retrieval.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If False, then the computational results are not deleted.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Leaving this flag set to False can result in accumulation of compute artifacts which you may eventually need to delete before they fill up your hard drive.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>console_output</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Bool value, if True, causes the standard output of the python processes to be printed to the user console.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>packages_to_load</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Optional character vector specifying additional modules to be loaded on the nodes when jobs are run in this compute context.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>idle_timeout</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Integer value, specifying the number of seconds of being idle (i.e., not running any Spark job) before system kills the Spark process.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Setting a value greater than 600 is recommended.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Defaults to 3600.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Setting a negative value will not timeout.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>pyspark interoperation will have no timeout.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>num_executors</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Integer value, specifying the number of executors in Spark, which is equivalent to parameter –num-executors in spark-submit app.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>If not specified, the default behavior is to launch as many executors as possible, which may use up all resources and prevent other users from sharing the cluster.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Defaults to RxOptions.get_option(“spark.numExecutors”).</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>executor_cores</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Integer value, specifying the number of cores per executor, which is equivalent to parameter –executor-cores in spark-submit app.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Defaults to RxOptions.get_option(“spark.executorCores”).</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>executor_mem</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Character string specifying memory per executor (e.g., 1000M, 2G), which is equivalent to parameter –executor-memory in spark-submit app.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Defaults to RxOptions.get_option(“spark.executorMem”).</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>driver_mem</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Character string specifying memory for driver (e.g., 1000M, 2G), which is equivalent to parameter –driver-memory in spark-submit app.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Defaults to RxOptions.get_option(“spark.driverMem”).</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>executor_overhead_mem</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Character string specifying memory overhead per executor (e.g. 1000M, 2G), which is equivalent to setting spark.yarn.executor.memoryOverhead in YARN.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Increasing this value will allocate more memory for the python process and the ScaleR engine process in the YARN executors, so it may help resolve job failure or executor lost issues.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Defaults to RxOptions.get_option(“spark.executorOverheadMem”).</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>extra_spark_config</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Character string specifying extra arbitrary Spark properties (e.g., “–conf spark.speculation=true –conf spark.yarn.queue=aQueue”), which is equivalent to additional parameters passed into spark-submit app.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>spark_reduce_method</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Spark job collects all parallel tasks’ results to reduce as final result.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>This parameter decides reduce strategy: oneStage/twoStage/auto. oneStage: reduce parallel tasks to one result with one reduce function; twoStage: reduce parallel tasks to square root size with the first reduce function, then reduce to final result with the second reduce function; auto: spark will smartly select oneStage or twoStage.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>tmp_fs_work_dir</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Character string specifying the temporary working directory in worker nodes.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>It defaults to /dev/shm to utilize in-memory temporary file system for performance gain, when the size of /dev/shm is less than 1G, the default value would switch to /tmp for guarantee sufficiency.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>You can specify a different location if the size of /dev/shm is insufficient.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Please make sure that YARN run-as user has permission to read and write to this location</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>interop</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>None or string or list of strings.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Current supported interoperation values are, ‘pyspark’: active revoscalepy Spark compute context in existing pyspark application to support the usage of both</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>reset</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Bool value, if True, all cached Spark Data Frames will be freed and all existing Spark applications that belong to the current user will be shut down.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>