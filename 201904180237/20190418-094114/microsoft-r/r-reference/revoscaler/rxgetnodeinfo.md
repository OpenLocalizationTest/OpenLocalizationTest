<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxgetnodeinfo.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926e2e39b5a4f8b3ffa7fd550374b7b90c701944343.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">e2e39b5a4f8b3ffa7fd550374b7b90c701944343</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxgetnodeinfo.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxGetNodeInfo function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Provides information about the capabilities of the nodes on a cluster.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxGetNodeInfo, IO</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxGetNodeInfo:  Provides information about all nodes on a cluster.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Provides information about the capabilities of the nodes on a cluster.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A distributed compute context (preferred), a jobInfo object, or (deprecated) a character scalar containing the name of the Microsoft HPC cluster head node being queried.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If you are interested in information about a particular node, be sure that node is included in the group specified in the compute context, or that the compute context has <ph id="ph1">`groups=NULL`</ph> (HPC compute contexts).</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Setting <ph id="ph1">`nodes=NULL`</ph> and <ph id="ph2">`groups=NULL`</ph> or <ph id="ph3">`queue="all"`</ph> in the compute context is the best way to ensure getting information on all nodes.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>additional arguments for modifying the compute context before requesting the node information.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>These arguments must be in the compute context constructor.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, only a vector containing the names of the nodes will be returned.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, names of the nodes will be normalized for use  as R variables.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxMakeRNodeNames<ept id="p1">](rxMakeRNodeNames.md)</ept> for details on name mangling.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, returns only those nodes within the cluster that are configured to actually execute jobs (where applicable; currently LSF only.).</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This function will return information on all the nodes on a given cluster if the <ph id="ph1">`nodes`</ph> slot of the compute context is <ph id="ph2">`NULL`</ph> and <ph id="ph3">`groups`</ph> and <ph id="ph4">`queue`</ph> are not specified in the compute context.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If either <ph id="ph1">`groups`</ph> or <ph id="ph2">`queue`</ph> is specified, information is provided only for nodes within the specified groups or queue, using the normal rules described in the compute context for taking the unions of node sets and nodes in queues.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The best way to get information on all nodes is to ensure that both the nodes and groups slots are set to <ph id="ph1">`NULL`</ph> for HPC, and that nodes and queues are set to <ph id="ph2">`NULL`</ph> and <ph id="ph3">`"all"`</ph>, respectively, for LSF.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Note that unlike <ph id="ph1">`rxGetAvailableNodes`</ph>, the return value of this function will contain all nodes in the compute context regardless of their state.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>(rxGetAvailableNodes returns only online nodes).</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If the return value of this function is used to populate node names elsewhere and <ph id="ph1">`namesOnly`</ph> is <ph id="ph2">`TRUE`</ph>, <ph id="ph3">`makeRNodeNames`</ph> should be set to the default <ph id="ph4">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`namesOnly`</ph> is <ph id="ph2">`FALSE`</ph>, the <ph id="ph3">`nodeName`</ph> element of each list element should be used, not the names of the list element, given that the list element names will be mangled to be proper R names.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>This operation is performed because names with a dash (-) are not permitted as variable names (the R interpreter interprets this as a minus operation).</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Thus, the mangling process replaces the dashes with an underscore _ to form the variable names.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxMakeRNodeNames<ept id="p1">](rxMakeRNodeNames.md)</ept> for details on name mangeling.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Also, note that</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>node names are always forced to all capital letters (node names should be case agnostic, but in some cluster related software, it is necessary to force them to be upper case.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>In general, however, machine names are always treated as being case insensitive.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>No other changes are made to node names during the mangling process.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>)</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`namesOnly`</ph> is <ph id="ph2">`TRUE`</ph>, a character vector containing the names of the nodes.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`makeRNodeNames`</ph> is <ph id="ph2">`TRUE`</ph>, these names will be normalized for use as R variables.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`namesOnly`</ph> is <ph id="ph2">`FALSE`</ph>, a named list of lists, where each top level name is a node name on the cluster, normalized for use as an R variable.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxMakeRNodeNames<ept id="p1">](rxMakeRNodeNames.md)</ept> for more details.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Each named element in the list will contain some or all of the following:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>character scalar.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The true name of the node (as opposd to the list item name).</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>float.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The processor speed in MHz for Microsoft HPC, or the CPU factor for LSF.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>integer.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The amount of RAM in MB.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>integer.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The number of cores.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>integer.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The number of CPU sockets.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>character scalar.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>May be either "online", "offline", "draining" (shutting down, but still with jobs in queue), or "unknown".</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Determines if there is an operational network path between the head node and the given compute node.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>list of character scalars.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The node groups (on MS HPC) or queues (under LSF) to which the node belongs.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxGetAvailableNodes<ept id="p1">](rxGetAvailableNodes.md)</ept>, <bpt id="p2">[</bpt>rxMakeRNodeNames<ept id="p2">](rxMakeRNodeNames.md)</ept>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>