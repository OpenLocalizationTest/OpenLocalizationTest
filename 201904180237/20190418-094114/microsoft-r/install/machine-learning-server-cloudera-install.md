<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="machine-learning-server-cloudera-install.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea9265e1c4b4670267e9553201216e643090a5dbb58d8.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5e1c4b4670267e9553201216e643090a5dbb58d8</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\machine-learning-server-cloudera-install.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install Machine Learning Server on Cloudera</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to install, connect to, and use Machine Learning Server on a Cloudera Hadoop disribution.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server using Cloudera Manager</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Machine Learning Server 9.2.1 | 9.3<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>This article explains how to generate, deploy, and activate an installation parcel for Machine Learning Server on a Cloudera distribution of Apache Hadoop (CDH).</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Cloudera offers a parcel installation methodology for adding services and features to a cluster.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>On a Hadoop cluster, Machine Learning Server runs on the edge node and all data nodes.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>You can use a parcel to distribute and activate the service on all nodes within your CDH cluster.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Platform requirements</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>You can create a parcel generation script on any <bpt id="p1">[</bpt>supported version of Linux<ept id="p1">](r-server-install-supported-platforms.md)</ept>, but execution requires CentOS or RHEL 7.0 as the native file system.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The parcel generator excludes any R Server features that it cannot install, such as <bpt id="p1">[</bpt>operationalization<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If parcel installation is too restrictive, follow the instructions for a generic <bpt id="p1">[</bpt>Hadoop installation<ept id="p1">](machine-learning-server-hadoop-install.md)</ept> instead.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Prepare for installation</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This section explains how to obtain the parcel generation script and simulate parcel creation.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Download a Machine Learning Server distribution</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>A package manager installation used for Linux or Hadoop won't provide the parcel generation scripts.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>To get the scripts, obtain a gzipped distribution of Machine Learning Server from <bpt id="p1">[</bpt>Visual Studio Dev Essentials<ept id="p1">](https://msdn.microsoft.com/subscriptions/downloads/hh442898.aspx)</ept> or <bpt id="p2">[</bpt>Volume licensing<ept id="p2">](https://go.microsoft.com/fwlink/?LinkId=717966&amp;clcid=0x409)</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Go to <bpt id="p1">[</bpt>Visual Studio Dev Essentials<ept id="p1">](https://www.visualstudio.com/dev-essentials/)</ept>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Join or Access Now<ept id="p1">**</ept> and enter your <bpt id="p2">[</bpt>Microsoft account<ept id="p2">](https://account.microsoft.com/account)</ept> (such as a Live ID, Hotmail, or Outlook account).</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Make sure you're in the right place: <bpt id="p1">*</bpt><ph id="ph1">https://my.visualstudio.com/Benefits</ph><ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Search for <bpt id="p1">*</bpt>Machine Learning Server<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Download <bpt id="p1">**</bpt>Machine Learning Server 9.3.0 for Hadoop<ept id="p1">**</ept> to a writable directory, such as <bpt id="p2">**</bpt>/tmp/<ept id="p2">**</ept>, on one of the nodes.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Download page on Visual Studio benefits page</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Unpack the distribution</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Log on as root or a user with super user privileges:<ph id="ph1">`sudo su`</ph></source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Switch to the <bpt id="p1">**</bpt>/tmp/<ept id="p1">**</ept> directory (assuming it's the download location): <ph id="ph1">`cd /tmp/`</ph></source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Unpack the file: <ph id="ph1">`tar zxvf en_microsoft_ml_server_930_for_hadoop_x64_&lt;some-number&gt;.tar.gz`</ph></source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The distribution is unpacked into a <bpt id="p1">**</bpt>Hadoop<ept id="p1">**</ept> folder at the download location.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The distribution includes the following files:</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>File or folder</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Script for installing Machine Learning Server.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Do not use this for a parcel install.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Script for generating a parcel used for installing Machine Learning Server on CDH.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>End-user license agreements for each separately licensed component.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>DEB folder</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Contains Machine Learning packages for deployment on Ubuntu.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>RPM folder</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Contains Machine Learning packages for deployment on CentOS/RHEL and SUSE</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Parcel folder</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Contains files used to generate a parcel for installation on CDH.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Test with a dry run</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The script includes a <bpt id="p1">**</bpt>-n<ept id="p1">**</ept> flag that simulates parcel generation.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Start with a dry run to review the prompts.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The script downloads Microsoft R Open and builds a parcel by extracting information from RPM packages.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>You can <bpt id="p1">[</bpt>append flags<ept id="p1">](#flags)</ept> to run unattended setup or customize feature selections.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Switch to the Hadoop directory: <ph id="ph1">`cd /Hadoop`</ph></source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Run the script with <bpt id="p1">**</bpt>-n<ept id="p1">**</ept> to simulate parcel generation: <ph id="ph1">`bash generate_mlserver_parcel.sh -n`</ph></source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>You are prompted to read and accept license agreements.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>You are also asked to specify the underlying operating system.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If the platform supports it, the parcel generator adds installation instructions for features having a dependency on .NET Core, such as Microsoft machine learning and <bpt id="p1">[</bpt>operationalization features<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>When the script is finished, the location of the parcel, checksum, and CSD is printed to the console.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Remember the files do not yet exist.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>This is just a dry run.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Running the script without <bpt id="p1">**</bpt>-n<ept id="p1">**</ept> generates the files.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Flags used for parcel generation</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>You can run parcel generator with the following flags to suppress prompts or choose components.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>flag</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Option</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>-m</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>--distro-name [DISTRO]</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Target Linux distribution for this parcel, one of: el6 el7 sles11</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>-l</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>--add-mml</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Add Python and microsoftml to the Parcel regardless of the target system.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>-a</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>--accept-eula</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Accept all end-user license agreements.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>-d</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>--download-mro</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Download Microsoft r open for distribution to an offline system.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>-s</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>--silent</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Perform a silent, unattended install.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>-u</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>--unattended</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Perform an unattended install.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>-n</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>--dry-run</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Don't do anything, just show what would be done.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>-h</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>--help</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Print this help text.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Run the script</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Repeat the command without <bpt id="p1">**</bpt>-n<ept id="p1">**</ept> parameter to create the files: <ph id="ph1">`bash generate_mlserver_parcel.sh`</ph></source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>The parcel generator file name is <bpt id="p1">**</bpt>MLServer-9.3.0-[DISTRO].parcel<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>The CSD file name is <bpt id="p1">**</bpt>MLServer<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The parcel generator file name includes a placeholder for the distribution.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Remember to replace it with a valid value before executing the copy commands.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Distribute parcels and CSDs</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>This section explains how to place parcel generator script and CSD files in CDH.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Copy to the parcel repository</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>By default, Cloudera Manager finds parcels in the Cloudera parcel repository.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>In this step, copy the parcel you generated to the repository.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Copy <bpt id="p1">**</bpt>MLServer-9.3.0<ept id="p1">**</ept> and <bpt id="p2">**</bpt>MLServer-9.3.0.sha<ept id="p2">**</ept> to the Cloudera parcel repository, typically /opt/cloudera/parcels.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Copy to the CSD repository</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>The Custom Service Descriptor (CSD) enables monitoring and administration from within Cloudera Manager.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>In this step, copy the CSD (a .jar file) to the Cloudera repository for CSD files.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Copy the CSD file <bpt id="p1">**</bpt>MLServer-9.3.0-CONFIG.jar<ept id="p1">**</ept> to the Cloudera CSD directory, typically /opt/cloudera/csd.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Modify the permissions of CSD file as follows:</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Restart the cloudera-scm-server service:</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Activate in Cloudera Manager</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>In Cloudera Manager, click the parcel icon on the top right menu bar.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>parcel icon in cloudera manager</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>On the left, find and select <bpt id="p1">**</bpt>MLServer-9.3.0<ept id="p1">**</ept> in the parcel list.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>If you don't see it, check the parcel-repo folder.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>On the right, in the parcel details page, <bpt id="p1">**</bpt>MLServer-9.3.0<ept id="p1">**</ept> should have a status of <bpt id="p2">*</bpt>Downloaded<ept id="p2">*</ept> with an option to <bpt id="p3">*</bpt>Distribute<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Distribute<ept id="p1">**</ept> to roll out Machine Learning Server on available nodes.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Status changes to <bpt id="p1">*</bpt>distributed<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Activate<ept id="p1">**</ept> on the button to make Machine Learning Server operational in the cluster.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Activate button in parcel detail</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>You are finished with this task when status is "distributed, activated" and the next available action is <bpt id="p1">*</bpt>Deactivate<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Add MLServer-9.3.0 as a service</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>In Cloudera Manager home page, click the down arrow by the cluster name and choose <bpt id="p1">**</bpt>Add Service<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>add service command in cloudera manager</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Find and select <bpt id="p1">**</bpt>MLServer-9.3.0<ept id="p1">**</ept> and click <bpt id="p2">**</bpt>Continue<ept id="p2">**</ept> to start a wizard for adding services.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>In the next page, add role assignments on all nodes used to run the service, both edge and data nodes.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Continue<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>On the last page, click <bpt id="p1">**</bpt>Finish<ept id="p1">**</ept> to start the service.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Machine Learning Server should now be deployed in the cluster.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Rollback a deployment</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>You have the option of rolling back the active deployment in Cloudera Manager, perhaps to use an older version.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>You can have multiple versions in Cloudera, but only can be active at any given time.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>In Cloudera Manager, click the Parcel icon to open the parcel list.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Find MLServer-9.3.0 and click <bpt id="p1">**</bpt>Deactivate<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>The parcel still exists, but Machine Learning Server is not operational in the cluster.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>The above steps apply to 9.3.0.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>If you have R Server (either 9.1 or 9.0.1), see <bpt id="p1">[</bpt>Install R Server 9.1 on CDH<ept id="p1">](r-server-install-cloudera.md)</ept> and <bpt id="p2">[</bpt>Install R Server 9.0.1 on CDH<ept id="p2">](r-server-install-cloudera-901.md)</ept> for release-specific documentation.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>We recommend starting with <bpt id="p1">[</bpt>How to use RevoScaleR with Spark<ept id="p1">](../r/how-to-revoscaler-spark.md)</ept> or <bpt id="p2">[</bpt>How to use RevoScaleR with Hadoop MapReduce<ept id="p2">](../r/how-to-revoscaler-hadoop.md)</ept>.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>For a list of functions that utilize Yarn and Hadoop infrastructure to process in parallel across the cluster, see <bpt id="p1">[</bpt>Running a distributed analysis using RevoScaleR functions<ept id="p1">](../r/how-to-revoscaler-distributed-computing-distributed-analysis.md)</ept>.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>R solutions that execute on the cluster can call functions from any R package.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>To add new R packages, you can use any of these approaches:</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Use a parcel and <bpt id="p1">[</bpt>create new parcel<ept id="p1">](machine-learning-server-cloudera-install.md#flags-used-for-parcel-generation)</ept> using generate_mlserver_parcel.sh script.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Use the RevoScaleR <bpt id="p1">[</bpt>rxExec function to add new packages<ept id="p1">](r-server-install-hadoop-manual-package.md#install-additional-packages-on-each-node-using-rxexec)</ept>.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Manually run <bpt id="p1">[</bpt>install.packages()<ept id="p1">](https://www.rdocumentation.org/packages/utils/versions/3.4.3/topics/install.packages)</ept> on all nodes in Hadoop cluster (using distributed shell or some other mechanism).</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install on Linux<ept id="p1">](machine-learning-server-linux-install.md)</ept></source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Machine Learning Server<ept id="p1">](r-server-install.md)</ept></source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>What's new in Machine Learning Server<ept id="p1">](../whats-new-in-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Supported platforms<ept id="p1">](r-server-install-supported-platforms.md)</ept></source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Known Issues<ept id="p1">](../resources-known-issues.md)</ept></source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure Machine Learning Server to operationalize your analytics<ept id="p1">](../what-is-operationalization.md)</ept></source>
        </trans-unit></group></body></file></xliff>