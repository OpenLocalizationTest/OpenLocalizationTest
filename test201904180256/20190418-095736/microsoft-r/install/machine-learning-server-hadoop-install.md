<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="machine-learning-server-hadoop-install.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18cd3d6ce1ee519160957b18bb4ec1d7e1244a27a62.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d3d6ce1ee519160957b18bb4ec1d7e1244a27a62</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\machine-learning-server-hadoop-install.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install Machine Learning Server for Hadoop</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to install, connect to, and use Machine Learning Server on a Hadoop cluster with Spark or MapReduce</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server for Hadoop</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Machine Learning Server 9.2.1 | 9.3<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>On a Spark cluster, Machine Learning Server must be installed on the edge node and all data nodes on a commercial distribution of Hadoop: Cloudera, HortonWorks, MapR.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Optionally, you can install <bpt id="p1">[</bpt>operationalization features<ept id="p1">](../what-is-operationalization.md)</ept> on edge nodes only.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Machine Learning Server is engineered for the following architecture:</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Hadoop Distributed File System (HDFS)</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Apache YARN</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>MapReduce or Spark 2.0-2.1</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>We recommend Spark for the processing framework.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>These instructions use package managers to connect to Microsoft sites, download the distributions, and install the server.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If you know and prefer working with gzip files on a local machine, you can download <bpt id="p1">**</bpt>en_machine_learning_server_9.2.1_for_hadoop_x64_100353069.gz<ept id="p1">**</ept> from <bpt id="p2">[</bpt>Visual Studio Dev Essentials<ept id="p2">](https://www.visualstudio.com/dev-essentials/)</ept>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>System and setup requirements</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Native operating system must be a <bpt id="p1">[</bpt>supported version of Hadoop on 64-bit Linux<ept id="p1">](r-server-install-supported-platforms.md)</ept>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Minimum RAM is 8 GB (16 GB or more is recommended).</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Minimum disk space is 500 MB per node.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>An internet connection.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If you do not have an internet connection, use the <bpt id="p1">[</bpt>offline installation instructions<ept id="p1">](machine-learning-server-linux-offline.md)</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Root or super user permissions</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Package managers</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Installation is through package managers.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Unlike previous releases, there is no install.sh script.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Package manager</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Platform</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>yum<ept id="p1">](https://access.redhat.com/documentation/Red_Hat_Enterprise_Linux/6/html/Deployment_Guide/ch-yum.html)</ept></source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>RHEL, CentOS</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>apt<ept id="p1">](https://help.ubuntu.com/lts/serverguide/apt.html)</ept></source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Ubuntu online</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>dpkg<ept id="p1">](https://help.ubuntu.com/lts/serverguide/dpkg.html)</ept></source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Ubuntu offline</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>zypper<ept id="p1">](https://www.suse.com/documentation/opensuse111/opensuse111_reference/data/sec_zypper.html)</ept></source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>SUSE</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rpm<ept id="p1">](https://access.redhat.com/documentation/en-US/Red_Hat_Enterprise_Linux/3/html/System_Administration_Guide/s1-rpm-using.html)</ept></source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>RHEL, CentOS, SUSE</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Running setup on existing installations</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The installation path for Machine Learning Server is new: <ph id="ph1">`/opt/microsoft/mlserver/9.3.0`</ph>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>However, if R Server 9.x is present, Machine Learning Server 9.x finds R Server at the old path (<ph id="ph1">`/usr/lib64/microsoft-r/9.1.0`</ph>) and replaces it with the new version.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>There is no support for side-by-side installations of older and newer versions, nor is there support for hybrid versions (such as R Server 9.1 and Python 9.3).</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>An installation is either entirely 9.3 or an earlier version.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Installation paths</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>After installation completes, software can be found at the following paths:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Install root: <ph id="ph1">`/opt/microsoft/mlserver/9.3`</ph></source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Microsoft R Open root: <ph id="ph1">`/opt/microsoft/ropen/3.4.3`</ph></source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Executables such as Revo64 and mlserver-python are at <ph id="ph1">`/usr/bin`</ph></source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>1 - Edge node installation</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Start here.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Machine Learning Server is required on the edge node.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>You should run full setup, following the installation commands for the Linux operating system used by your cluster: <bpt id="p1">[</bpt>Linux install &gt; How to install<ept id="p1">](machine-learning-server-linux-install.md#how-to-install)</ept>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Full setup gives you core components for both R and Python, machine learning algorithms and pretrained models, and <bpt id="p1">[</bpt>operationalization<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Operationalization features run on edge nodes, enabling additional ways of deploying and consuming script.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>For example, you can build and deploy web services, which allows you to invoke and access your solution programmatically, through a REST API.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>You cannot use operationalization on data nodes.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Operationalization does not support Yarn queues and cannot run in a distributed manner.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>2 - Data node installation</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>You can continue installation by running Setup on any data node, either sequentially or on multiple data nodes concurrently.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>There are two approaches for installing Machine Learning Server on data nodes.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Approach 1: Package managers for full installation<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Again, we recommend running the <bpt id="p1">[</bpt>full setup<ept id="p1">](machine-learning-server-linux-install.md)</ept> on every node.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>This approach is fast because package managers do most of the work, including adding the Hadoop package (microsoft-mlserver-hadoop-9.3.0) and setting it up for activation.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>As before, follow the installation steps for the Linux operating system used by your cluster: <bpt id="p1">[</bpt>Linux install &gt; How to install<ept id="p1">](machine-learning-server-linux-install.md#how-to-install)</ept>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Approach 2: Manual steps for partial installation<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Alternatively, you can install a subset of packages.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>You might do this if you do not want operationalization on your data nodes, or if you want to exclude a specific language.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Be prepared for more testing if you choose this approach.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>The packages are not specifically designed to run as standalone modules.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Hence, unexpected problems are more likely if you leave some packages out.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Install as root: <ph id="ph1">`sudo su`</ph></source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Refer to the <bpt id="p1">[</bpt>annotated package list<ept id="p1">](#package-list)</ept> and download individual packages from the package repo corresponding to your platform:</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Make a directory to contain your packages: <ph id="ph1">`hadoop fs -mkdir /tmp/mlsdatanode`</ph></source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Copy the packages: <ph id="ph1">`hadoop fs -copyFromLocal /tmp/mlserver /tmp/mlsdatanode`</ph></source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Switch to the directory: <ph id="ph1">`cd /tmp/mlsdatanode`</ph></source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Install the packages using the tool and syntax for your platform:</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>On Ubuntu online: <ph id="ph1">`apt-get install *.rpm`</ph></source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>On Ubuntu offline: <ph id="ph1">`dpkg -i *.deb`</ph></source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>On CentOS and RHEL: <ph id="ph1">`yum install *.rpm`</ph></source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Activate the server: <ph id="ph1">`/opt/microsoft/mlserver/9.3.0/bin/R/activate.sh`</ph></source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Repeat this procedure on remaining nodes.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Packages list</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The following packages comprise a full Machine Learning Server installation:</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>The microsoft-mlserver-python-9.3.0 package provides Anaconda 4.2 with Python 3.5, executing as mlserver-python, found in <ph id="ph1">`/opt/microsoft/mlserver/9.3.0/bin/python/python`</ph></source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Microsoft R Open is required for R execution:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Microsoft .NET Core 2.0, used for operationalization, must be added to Ubuntu:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Additional open-source packages could be required.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>The potential list of packages varies for each computer.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Refer to <bpt id="p1">[</bpt>offline installation<ept id="p1">](machine-learning-server-linux-offline.md)</ept> for an example list.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>We recommend starting with <bpt id="p1">[</bpt>How to use RevoScaleR with Spark<ept id="p1">](../r/how-to-revoscaler-spark.md)</ept> or <bpt id="p2">[</bpt>How to use RevoScaleR with Hadoop MapReduce<ept id="p2">](../r/how-to-revoscaler-hadoop.md)</ept>.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>For a list of functions that utilize Yarn and Hadoop infrastructure to process in parallel across the cluster, see <bpt id="p1">[</bpt>Running a distributed analysis using RevoScaleR functions<ept id="p1">](../r/how-to-revoscaler-distributed-computing-distributed-analysis.md)</ept>.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>R solutions that execute on the cluster can call functions from any R package.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>To add new R packages, you can use any of these approaches:</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Use the RevoScaleR <bpt id="p1">[</bpt>rxExec function to add new packages<ept id="p1">](r-server-install-hadoop-manual-package.md#install-additional-packages-on-each-node-using-rxexec)</ept>.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Manually run <bpt id="p1">[</bpt>install.packages()<ept id="p1">](https://www.rdocumentation.org/packages/utils/versions/3.4.3/topics/install.packages)</ept> on all nodes in Hadoop cluster (using distributed shell or some other mechanism).</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install on Linux<ept id="p1">](machine-learning-server-linux-install.md)</ept></source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Machine Learning Server<ept id="p1">](r-server-install.md)</ept></source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>What's new in Machine Learning Server<ept id="p1">](../whats-new-in-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Supported platforms<ept id="p1">](r-server-install-supported-platforms.md)</ept></source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Known Issues<ept id="p1">](../resources-known-issues.md)</ept></source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure Machine Learning Server to operationalize your analytics<ept id="p1">](../what-is-operationalization.md)</ept></source>
        </trans-unit></group></body></file></xliff>