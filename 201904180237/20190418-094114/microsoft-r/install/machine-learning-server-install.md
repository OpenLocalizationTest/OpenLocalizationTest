<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="machine-learning-server-install.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea9267b58a6f5521718b1ee0140bed711c8407d367f33.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">7b58a6f5521718b1ee0140bed711c8407d367f33</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\machine-learning-server-install.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to install Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to install Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Install and configure Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Machine Learning Server is available on a number of <bpt id="p1">[</bpt>platforms<ept id="p1">](r-server-install-supported-platforms.md)</ept>.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Looking for earlier versions?</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>Installation guides for earlier releases<ept id="p1">](r-server-install.md)</ept> for links.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Choose a configuration</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This section covers topology configurations from single to multi-machine topologies.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Standalone deployments</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Standalone servers describe a working experience where script development and execution occur on the same Windows or Linux machine.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If you install the free developer edition on either Windows or Linux, a standalone server is the likely configuration.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>You could also install the server on a virtual machine accessed by multiple users in turn.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>standalone server on Windows or Linux</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Client and server multi-user topology</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>A client-server configuration is more common in a team environment.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>You can install free Python client libraries or free R Client on any workstation, write script on the workstation, and then deploy script as a <bpt id="p1">[</bpt>web service<ept id="p1">](~/operationalize/concept-what-are-web-services.md)</ept> to a Machine Learning Server configured to <bpt id="p2">[</bpt>operationalize<ept id="p2">](~/what-is-operationalization.md)</ept> analytics, thus extending your options for interacting with and consuming script on a server.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>For R development only, you can also use <bpt id="p1">[</bpt>remote execution<ept id="p1">](~/r/how-to-execute-code-remotely.md)</ept> in this configuration: switch from local to remote server within a session to write and run script interactively.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>On the consumption side, you can write custom apps or consume an R or Python solution as a web service.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>client server topology</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Large scale multi-user topologies</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Scale-out topologies are available in two forms.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>One option is to use a distributed platform like Hadoop MapReduce or Spark (on Linux).</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>A second option is to install Machine Learning Server on multiple computers (Windows or Linux), each one configured as either a web node or compute node that work together.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>For Hadoop and Spark, you can write and run script locally and then <bpt id="p1">[</bpt>push the compute context<ept id="p1">](~/r/concept-what-is-compute-context.md)</ept> to the Hadoop or Spark cluster.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>For web and compute nodes, use the <bpt id="p1">[</bpt>operationalization capabilities<ept id="p1">](~/what-is-operationalization.md)</ept> in Machine Learning Server to distribute workloads on appropriate nodes.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>scaleout topology on clustered computers</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Choose a platform</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Machine Learning Server runs on Windows, Linux, and Hadoop.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Review the <bpt id="p1">[</bpt>supported platforms list<ept id="p1">](r-server-install-supported-platforms.md)</ept> for specific operating system versions.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Begin installation</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The following links provide installation and configuration instructions.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install on Windows<ept id="p1">](machine-learning-server-windows-install.md)</ept></source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install on Linux<ept id="p1">](machine-learning-server-linux-install.md)</ept></source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install on Hadoop<ept id="p1">](machine-learning-server-hadoop-install.md)</ept></source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure server to operationalize (deploy/consume) analytics<ept id="p1">](../operationalize/configure-start-for-administrators.md)</ept></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Add pre-trained models<ept id="p1">](microsoftml-install-pretrained-models.md)</ept></source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Provision on the cloud<ept id="p1">](machine-learning-server-in-the-cloud.md)</ept></source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Local Tools</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Microsoft R Client<ept id="p1">](../r-client/what-is-microsoft-r-client.md)</ept></source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Link Python tools and IDES to the MLServer Python interpreter <ept id="p1">](../python/quickstart-python-tools.md)</ept></source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Python interpreter &amp; libraries on Windows<ept id="p1">](python-libraries-interpreter.md)</ept></source>
        </trans-unit></group></body></file></xliff>