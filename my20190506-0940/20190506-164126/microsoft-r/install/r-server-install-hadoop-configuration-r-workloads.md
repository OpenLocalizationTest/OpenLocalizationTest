<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-hadoop-configuration-r-workloads.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750f299ff6f123bea4ce0007f2d81846be5348709e9.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">f299ff6f123bea4ce0007f2d81846be5348709e9</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-hadoop-configuration-r-workloads.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Adjust your Hadoop cluster configuration for R server workloads</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Adjust your Hadoop cluster configuration for R server workloads.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Adjust Hadoop configuration for RevoScaleR workloads</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Increase memory limits for R server workloads</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>On YARN-based Hadoop systems (CDH5, HDP 2.x, MapR 4.x), we sometimes find that the default settings for Map and Reduce memory limits are inadequate for large RevoScaleR jobs.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>To allow large RevoScaleR jobs to run, you can modify four properties in mapred-site.xml and one in yarn-site.xml, typically found in /etc/hadoop/conf.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The memory available for R is the difference between the container’s memory limit and the memory given to the Java Virtual Machine.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>mapred-site.xml</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>yarn-site.xml</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If you are using a cluster manager such as Cloudera Manager or Ambari, these settings must usually be modified using the Web interface.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Use HDFS Caching</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>HDFS caching<ept id="p1">*</ept>, more formally <bpt id="p2">*</bpt>centralized cache management in HDFS<ept id="p2">*</ept>, can greatly improve the performance of your Hadoop jobs by keeping frequently used data in memory.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>You enable HDFS caching on a path by path basis, first by creating a <bpt id="p1">*</bpt>pool<ept id="p1">*</ept> of cached paths, and then adding paths to the pool.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The HDFS command <ph id="ph1">`cacheadmin`</ph> is used to perform these tasks.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>This command should be run by the hdfs user (the mapr user on MapR installations).</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The cacheadmin command has many subcommands; the Apache Software Foundation has <bpt id="p1">[</bpt>complete documentation<ept id="p1">](http://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/CentralizedCacheManagement.html)</ept>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>To get started, the addPool and addDirective commands will suffice.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>For example, to specify HDFS caching for our /share/AirlineDemoSmall directory, we can first create a pool as follows:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>You can then add the path to /share/AirlineDemoSmall to the pool with an addDirective command as follows:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Hadoop Security with Kerberos Authentication</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>By default, most Hadoop configurations are relatively insecure.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Security features such as SELinux and IPtables firewalls are often turned off to help get the Hadoop cluster up and running quickly.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>However, Cloudera and Hortonworks distributions of Hadoop support Kerberos authentication, which allows Hadoop to operate in a much more secure manner.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>To use Kerberos authentication with your particular version of Hadoop, see one of the following documents:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Cloudera CDH5</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Cloudera CDH5 with Cloudera Manager 5</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Hortonworks HDP 1.3</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Hortonworks HDP 2.x</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Hortonworks HDP (1.3 or 2.x) with Ambari</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If you have trouble restarting your Hadoop cluster after enabling Kerberos authentication, the problem is most likely with your keytab files.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Be sure you have created all the required Kerberos principals and generated appropriate keytab entries for all of your nodes, and that the keytab files have been located correctly with the appropriate permissions.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>(We have found that in Hortonworks clusters managed with Ambari, it is important that the spnego.service.keytab file be present on <bpt id="p1">*</bpt>all<ept id="p1">*</ept> the nodes of the cluster, not just the name node and secondary namenode.)</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The MapR distribution also supports Kerberos authentication, but most MapR installations use that distribution’s <bpt id="p1">*</bpt>wire-level security<ept id="p1">*</ept> feature.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>MapR Security Guide<ept id="p1">](http://doc.mapr.com/display/MapR/Security+Guide)</ept> for details.</source>
        </trans-unit></group></body></file></xliff>