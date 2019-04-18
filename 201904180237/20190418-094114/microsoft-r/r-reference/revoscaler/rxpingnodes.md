<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxpingnodes.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea9263a5977f8b06086c51452dce0a453723e746fe248.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">3a5977f8b06086c51452dce0a453723e746fe248</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxpingnodes.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxPingNodes function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This function provides a simple test of the compute context's ability to perform a round trip through one or more  computation nodes.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxPingNodes, IO</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxPingNodes:  Simple Test of Compute Cluster Nodes</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This function provides a simple test of the compute context's ability to perform a round trip through one or more computation nodes.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A distributed compute context.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> context is supported.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>See the details section for more information.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>A non-negative integer value.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Real valued numbers will be cast to integers.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This parameter sets a total (real clock) time to attempt to perform a ping.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The timer is not started until  the system has first determined which nodes are unavailable (meaning down, unreachable or not usable for jobs,  such as scheduler only nodes on LSF).</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>At least one attempt to complete a ping is performed regardless of the setting of <ph id="ph1">`timeout`</ph>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If the default value of <ph id="ph1">`0`</ph> is used, there is no timeout.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph>, or a character vector containing one or more of the ping states.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, no filtering is  performed.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If a character vector of one or more of the ping states is provided, then only those nodes determined to be in the  states enumerated will be returned.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This function provides an application level "ping" to one or more nodes in a cluster or cloud.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>To this end, a trivial job is launched for each node to be pinged.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>A successful ping means that communication between the end user and the scheduler and communication between the end user and the shared data directory was successful; that R was launched and ran a trivial function successfully on the host being pinged; and that the results were returned successfully.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>While this function does not test certain aspects of the messaging required for HPA functions (e.g., <ph id="ph1">`rxSummary`</ph>), it does allow the user to easily test the majority of the end-to-end job functionality within a supported cloud or cluster.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The compute context provided is used to determine the cluster or queue that is to be pinged.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Furthermore, the nodes to be pinged will be determined in the usual fashion; that is, <ph id="ph1">`NULL`</ph> in the <ph id="ph2">`nodes`</ph> indicates use of all nodes; values in the <ph id="ph3">`groups`</ph> or <ph id="ph4">`queue`</ph> fields will cause the set of nodes to be checked to be the intersection between all the nodes in the <ph id="ph5">`groups`</ph> or <ph id="ph6">`queue`</ph> specified, and the set of nodes specifically specified in the <ph id="ph7">`nodes`</ph> parameter, and so forth.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Note that for clusters and clouds that do have a head node, <ph id="ph1">`computeOnHeadNode`</ph> is respected.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>For more information, see the compute context constructors or the <bpt id="p1">[</bpt>rxGetNodeInfo<ept id="p1">](rxGetNodeInfo.md)</ept> for more information.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Most other values in the compute context are respected when determing how a ping will be sent.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The following fields in particular are of note when using this tool:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>May be used to allow the ping jobs to run sooner than other longer running jobs.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Should usually be avoided</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Should almost always be set to <ph id="ph1">`TRUE`</ph>; however, may be of use to a system administrator diagnosing a problem.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>An object of type <ph id="ph1">`rxPingResults`</ph>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>This is essentially a list in which component is named using an <bpt id="p1">[</bpt>rxMakeRNodeNames<ept id="p1">](rxMakeRNodeNames.md)</ept> translated node name in the same manner and for the same reasons described for <bpt id="p2">[</bpt>rxGetNodeInfo<ept id="p2">](rxGetNodeInfo.md)</ept>, with the <ph id="ph1">`getWorkersOnly`</ph> parameter set to FALSE.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Each element of this list contains two elements: <ph id="ph1">`nodeName`</ph> which holds the true, unmangled name of the node, and <ph id="ph2">`status`</ph>, which contains a character scalar with one of the following values:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The node failed its scheduler level check prior to an attempt to actually ping the node.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>This does not necessarily mean that the node is not not functional;  rather, it only means that it cannot support having a job run on it.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The round trip job was a success.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The scheduler failed the job.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>This could be due to permissions, corrupt libraries, or a problem relating to the GUID directory.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The R process on the worker host was started, but failed.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The ping was sent, but a response was never received.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>This could be due to a problem with the installation, or other long running jobs being queued ahead of the ping job, or a system failure.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>An <ph id="ph1">`as.vector`</ph> method is provided for the <ph id="ph2">`rxPingResults`</ph> object which returns a character vector of the non-mangled (<bpt id="p1">[</bpt>rxMakeRNodeNames<ept id="p1">](rxMakeRNodeNames.md)</ept> translated) node names for use in another compute context, filtered by the <ph id="ph3">`filter`</ph> parameter originally provided.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Finally, the <ph id="ph1">`rxPingResults`</ph> object has a <ph id="ph2">`logical`</ph> attribute associated with it: <ph id="ph3">`allOk`</ph>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>This attribute is set to <ph id="ph1">`TRUE`</ph> if all of the pinged nodes' states (after filtering) were set to <ph id="ph2">`"success"`</ph>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Otherwise, this attribute is set to <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxGetAvailableNodes<ept id="p1">](rxGetAvailableNodes.md)</ept>, <bpt id="p2">[</bpt>rxMakeRNodeNames<ept id="p2">](rxMakeRNodeNames.md)</ept>, <bpt id="p3">[</bpt>rxGetNodeInfo<ept id="p3">](rxGetNodeInfo.md)</ept>, <bpt id="p4">[</bpt>rxGetAvailableNodes<ept id="p4">](rxGetAvailableNodes.md)</ept>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>