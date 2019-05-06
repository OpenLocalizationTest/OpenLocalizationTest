<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-admin-managing-the-grid.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750f8ba48a6381f3c8760d8beab7f2292ebae721bf4.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">f8ba48a6381f3c8760d8beab7f2292ebae721bf4</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-admin-managing-the-grid.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>DeployR Administration Console Help - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Managing Grid Nodes in the DeployR Administration Console</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Managing the Grid</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>DeployR Enterprise supports an extensible grid framework, providing load balancing capabilities across a network of node resources.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Each node on the grid contributes its own processor, memory, and disk resources.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>These resources can be leveraged by the DeployR server to run R code as part of user authenticated, asynchronous, and anonymous operations.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>With the DeployR Enterprise, you can dynamically scale the overall workload capacity by enabling and disabling the number of available grid nodes, and by designating these nodes to specific modes of operation.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The grid can then automatically <bpt id="p1">[</bpt>distribute the workload<ept id="p1">](#grid-workload-distribution)</ept> across the set of enabled nodes.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Or, you can <bpt id="p1">[</bpt>create custom node clusters<ept id="p1">](#named-clusters-workload-distribution)</ept> tuned for specific operation types and resource requirements.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Note that DeployR Open supports only a static grid framework of a single, local grid node with a fixed slot limit.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>When configuring the grid, you should begin by gaining an understanding of the anticipated workload for the grid.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>With that workload in mind, you can then scale the grid to handle the load by adding or changing the resources of each grid node.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>A well-configured grid maximizes throughput while minimizing resource contention.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The server and grid deployment model is described as <ph id="ph1">`Server[1] -&gt; Node[1..N]`</ph> where <ph id="ph2">`N`</ph> is defined as the total number of nodes on the grid.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>For more on planning and provisioning, see the <bpt id="p1">[</bpt>Scale &amp; Throughput Guide<ept id="p1">](deployr-admin-scale-and-throughput.md)</ept>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Figure: Node List page</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Node Operation Types</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>You must designate an operation type for each node on the grid.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The following table describes the distinct types of operations recognized by the grid.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Operation Type</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Supported Operations</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Operations on projects requested by authenticated users</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Operations from asynchronous jobs executing in the background on behalf of authenticated users</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Operations from users executing scripts anonymously</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Tip: By limiting anonymous operations to one or more specific nodes, you can maintain complete control of the resources allocated to unauthenticated users, which in turn helps protect the system from malicious attacks.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Any operation.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>This mode is only used when the workload on the grid overflows or exhausts all of the nodes dedicated to the operation type requested.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>While a <ph id="ph1">`mixed`</ph> mode exists, dedicating a node to a specific operation type provides a simple yet powerful mechanism that guarantees processing isolation between the distinct modes of operation being handled concurrently on the grid.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>DeployR Open<ept id="p1">**</ept> includes only the local node, <bpt id="p2">**</bpt>DeployR Default Node<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Therefore, this node should generally remain designated to the <ph id="ph1">`mixed mode`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Once a node is dedicated to a specific operating type, the administrator can further tailor its configuration by provisioning processor, memory, and disk resources appropriate to the nature of the targeted operations.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Each operation type has a distinct set of <bpt id="p1">[</bpt>server policies<ept id="p1">](deployr-admin-managing-server-policies.md)</ept> that impact the time-out policy, IP filters, encryption, and so on.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Grid Workload Distribution</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>DeployR Enterprise supports an extensible grid framework, providing load balancing capabilities across a network of node resources.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>There are two workload distribution models supported by the DeployR grid:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Operation-cluster model</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Named-cluster model</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Each node on the grid is assigned an <bpt id="p1">[</bpt>operation type<ept id="p1">](#node-operation-types)</ept>: authenticated, asynchronous, anonymous, or mixed mode.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The operation type for a node indicates the types of operations that the node will accept at runtime.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>For example, a grid node configured for authenticated operations will only accept authenticated (project) operations at runtime and never accept asynchronous or anonymous operations.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>A grid node configured for 'mixed mode' accepts all types of operations.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The operation type assigned to a node and the cluster named for the request (if one was named) are the biggest determinants in how the workload is distributed.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>In the absence of a specified custom cluster name, the workload is automatically spread across nodes of the same operation type using the <bpt id="p1">[</bpt>operation-cluster model<ept id="p1">](#operation-clusters-workload-distribution)</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>However, you can further optimize that distribution by allowing a custom cluster to be named for an operation, which then follows the <bpt id="p1">[</bpt>named-cluster<ept id="p1">](#named-clusters-workload-distribution)</ept> workload distribution model.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Operation-Clusters Workload Distribution</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The set of nodes dedicated to the same operation type is automatically members of the same operation-cluster.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>In this way, the operation-cluster workload distribution model provides a simple and automatic way to partition the workload on the grid.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>There are four operation-clusters, one for each type of operation (authenticated, asynchronous, or anonymous) and one for mixed mode nodes.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The specific manner in which an operation is allocated onto a node using the operation-cluster workload distribution model is a function of:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The type of operation being requested (authenticated, asynchronous, or anonymous)</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The number of nodes on the grid that match the operation-cluster identity</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The current workload for those nodes</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If a request does not name a custom cluster, the grid begins by determining the operation type for that request, then identifying all nodes configured for that type of operation, and finally sending the request to the node with the least burden to minimize resource contention and to maximize throughput.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>When all of the nodes of a custom cluster are busy, any additional requests for that cluster will be rejected.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Whenever an operation-cluster on the grid or the entire grid is operating a maximum capacity, any additional requests for authenticated or anonymous operations will be rejected and any additional requests for asynchronous operations will be queued.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>For example, if the grid determines that a request is made for an asynchronous job, the grid will look for all nodes with the asynchronous type, and then send the request to the least busy node in that operation-cluster.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>However, if all nodes within the asynchronous operation-cluster are busy, then the request is funneled to the least burdened node of mixed mode type.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Named-Clusters Workload Distribution</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>While the default <bpt id="p1">[</bpt>operation-cluster model<ept id="p1">](#operation-clusters-workload-distribution)</ept> works well in many cases, there are some limitations to that model when operations within a single operation-cluster do not share the exact same runtime characteristics.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>To address this situation, the named-cluster workload distribution model was introduced in DeployR 7.4 to allow administrators to assign <bpt id="p1">[</bpt>custom cluster names<ept id="p1">](#node-properties)</ept> to nodes.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>As an example, it is not uncommon that authenticated operations that would otherwise execute on the same authenticated operation-cluster differ in need from one another.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Some authenticated operations may require nodes that deliver fast processing power, while other authenticated operations may require nodes that deliver large amounts of memory.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Named-cluster workload distribution solves this problem by allowing the administrator to designate a custom cluster name for an individual or groups of nodes on the grid that are intended for special purpose operations, such as "high-cpu" or "high-mem".</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Once a custom cluster has been designate to at least one node in the grid, individual operations can be targeted for execution within that named custom cluster, which ensures suitable runtime resources are available on the node where an operation eventually executes.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The specific manner in which an operation is allocated onto a node using this model is a function of:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>The custom cluster's identity specified as an API parameter for the operation being requested</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The number of nodes on the grid that match the name of the custom cluster</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The current workload for those nodes</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Whenever a custom cluster has been named for the requested operation, the grid begins by identifying the nodes that fall within that cluster, then sends the request to the node within that cluster that has the least burden to minimize resource contention and to maximize throughput.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>When all of the nodes of a custom cluster are busy, any additional requests for that cluster are funneled to a node configured for the mixed mode operation type, if one is available.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Whenever a custom cluster on the grid or the entire grid is operating a maximum capacity, any additional requests for authenticated or anonymous operations will be rejected and any additional requests for asynchronous operations will be queued.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>For example, if the grid determines that a request is made for an operation to use the "high-mem" cluster, the grid will look for all nodes within the "high-mem" cluster and then send the request to the least busy node within that cluster.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>However, if all nodes within the "high-mem" cluster are busy, then the request is funneled to the least burdened node of mixed mode type.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Any node can belong to a custom cluster if the administrator has assigned the node to that cluster by entering its custom name in the <bpt id="p1">**</bpt>Cluster name<ept id="p1">**</ept><ph id="ph1">&amp;nbsp;</ph><bpt id="p2">[</bpt>field<ept id="p2">](#node-properties)</ept>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Custom cluster names are not case-sensitive.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Node Validation and Errors</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The Administration Console performs a verification of node configurations whenever you:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Display the <bpt id="p1">**</bpt>Grid<ept id="p1">**</ept> tab</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Create or update a grid node configuration</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Import a grid node configuration</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>When you visit the <bpt id="p1">**</bpt>Grid<ept id="p1">**</ept> tab, any enabled nodes found to be unresponsive are highlighted to help you visually identify that these nodes are not operating properly.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>When you attempt to create, update or import a node, the verification process is run.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>If an issue is detected, the following message appears: <bpt id="p1">*</bpt>“Grid node details provided failed to validate, please check your node configuration and try again.”<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Common validation issues include:</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>The configuration points to a grid node that is improperly installed or not yet installed.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>The configuration points to a grid node that is currently unresponsive for any number of reasons including the RServe process not running on that node.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>The node is behind a firewall or temporarily unreachable.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>The node’s configuration details are incomplete such as an empty name field when the name is required.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Node Properties</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Basic Settings</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Properties</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>If checked, the node is available for processing operations on the grid.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>This name is displayed in the node list in the Administration Console.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>This optional node description is visible only in the node list.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>This is the hostname or IP on which the node is configured.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>This is the type of node<bpt id="p1"> [</bpt>operation mode<ept id="p1">](#node-operation-types)</ept>: authenticated, anonymous, asynchronous, or mixed.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>This field is optional.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Specifies the name of the custom node cluster to which this node will be (or is already) assigned.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Custom cluster names are not case-sensitive.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Learn more about the<bpt id="p1"> [</bpt>named-cluster workload distribution model<ept id="p1">](#named-clusters-workload-distribution)</ept>.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Runtime Constraints</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>These constraints govern limits for processor and memory usage at runtime.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Properties</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>This property determines the maximum number of concurrent operations permitted on a given node.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>To illustrate a case for adjusting the slot limit, consider a node dedicated to memory intensive operations.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>  You may want to lower the slot limit to minimize the risk that concurrently executing operations on the node might exhaust the memory.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Note<ept id="p1">*</ept>: For DeployR Open, a fixed slot limit of 12 is imposed.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>This property specifies an R boundary that was created in this console.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>This R boundary is used to impose CPU usage limits for a given node.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>  The R boundary applies to each slot individually.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>RServe Runtime and Security Configuration</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>After a default installation of DeployR, it is highly unlikely that these settings require any editing under most operating conditions.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>However, if DeployR is in conflict with another application on the server machine or if you have made edits to the file<ph id="ph1"> `Rserv.conf`</ph>, you must mirror your changes here as well.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Properties</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>This property lists the port defined during installation on which RServe is listening.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>This is the upper limit, expressed in bytes, imposed on the communication between DeployR server and the Rserve session.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>If a username was defined in<ph id="ph1"> `Rserv.cfg`</ph>, enter it for each node.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Note: <ph id="ph1">`Rserv.cfg`</ph> is under <ph id="ph2">`&lt;PATH TO R&gt;\bin\x64`</ph>.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>If a password was defined in<ph id="ph1"> `Rserv.cfg`</ph>, enter it for each node.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>External Directory Configuration</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>If the external data directories are properly configured across all grid nodes and an R script updates the data in the external directory, then those updates are automatically mirrored across all nodes without any manual or external intervention by the admin.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Properties</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>This setting must reflect the full path on that node’s machine to the directory defined for external data usage such as <ph id="ph1">`$DEPLOYR_HOME/deployr/external/data`</ph> where <ph id="ph2">`$DEPLOYR_HOME`</ph> is the installation directory.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;a id="slots-in-use"&gt;</bpt><ept id="p1">&lt;/a&gt;</ept><ph id="ph1">
</ph><bpt id="p2">**</bpt>Slots in Use<ept id="p2">**</ept></source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>You can see which slots are currently in use and how they are being used by a particular node in the<bpt id="p1"> **</bpt>Slots In Use<ept id="p1">**</ept><ph id="ph1"> </ph>section.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>For each slot, you can review the following details:</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Slot Details</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Lists the slot’s operating mode, which is interesting for mixed-mode nodes</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Provides the name of project, job, or script being executed</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Specifies the time that has elapsed since execution commenced</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>and</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Lists the username of person or IP address who initiated the request</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Lists the unique ID for this HTTP session</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Provides a link to open the event console</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>You can force the termination of a current operation on slot, by clicking the<bpt id="p1"> **</bpt>Shutdown<ept id="p1">**</ept><ph id="ph1"> </ph>link.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Creating New Nodes</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>While many default node settings are preconfigured during the installation process, the DeployR Enterprise administrator must still declare and configure each node individually in the Administration Console.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>For more information about installing, see the installation instructions for your server operating system.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>To create a new node:</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>The Grid<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>From the Grid Node List page, click the <bpt id="p1">**</bpt>New Grid Node<ept id="p1">**</ept> link in the menu bar.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Figure: New Node page</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>New Grid Node<ept id="p1">**</ept> page, define the applicable <bpt id="p2">[</bpt>properties for the node<ept id="p2">](#node-properties)</ept>, such as the <bpt id="p3">**</bpt>Name<ept id="p3">**</ept>, <bpt id="p4">**</bpt>Host<ept id="p4">**</ept>, <bpt id="p5">**</bpt>Operating Type<ept id="p5">**</ept>, and <bpt id="p6">**</bpt>Storage Context<ept id="p6">**</ept>.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Enter a name in the <bpt id="p1">**</bpt>Name<ept id="p1">**</ept> field.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Enter an IP address in the <bpt id="p1">**</bpt>Host<ept id="p1">**</ept> field.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Hostname or IP on which the node is configured.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>The DeployR Default Node is configured on localhost.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>Specify the <bpt id="p1">**</bpt>Operating Type<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>operating mode<ept id="p1">](#node-operation-types)</ept> you define for a grid node has an impact on the operations you can perform on that node.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Under <bpt id="p1">**</bpt>External directory<ept id="p1">**</ept> configuration, set the <bpt id="p2">[</bpt><bpt id="p3">**</bpt>Storage Context<ept id="p3">**</ept><ept id="p2">](deployr-admin-managing-server-policies.md#server-policy-properties)</ept> to reflect <bpt id="p4">**</bpt>the full path<ept id="p4">**</ept> to the external data directory on that node’s machine, such as <ph id="ph1">`$DEPLOYR_HOME/deployr/external/data`</ph> where <ph id="ph2">`$DEPLOYR_HOME`</ph> is the installation directory.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create<ept id="p1">**</ept> to save the new node.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>The node configuration is <bpt id="p1">[</bpt>validated<ept id="p1">](#node-validation-and-errors)</ept>.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>If the configuration works, then it is saved.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>If not, an <bpt id="p1">[</bpt>error message<ept id="p1">](#node-validation-and-errors)</ept> will appear.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Viewing and Editing Nodes</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>To view and edit a node:</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>The Grid<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Grid Node List<ept id="p1">**</ept>, click the node you want to view or edit.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Grid Node Details<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Edit<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>Make your changes.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Update<ept id="p1">**</ept> to save the changes.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>The node configuration is <bpt id="p1">[</bpt>validated<ept id="p1">](#node-validation-and-errors)</ept>.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>If the configuration works, then it is saved.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>If not, an <bpt id="p1">[</bpt>error message<ept id="p1">](#node-validation-and-errors)</ept> will appear.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>Enabling or Disabling Nodes</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>You can choose whether or not a configured node will be active in the grid or inactive using the <bpt id="p1">**</bpt>Enable<ept id="p1">**</ept> checkbox in the <bpt id="p2">**</bpt>Grid Node Details<ept id="p2">**</ept> page.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>When disabled, the node is no longer available to process any requests from DeployR and it will appear highlighted in the main grid node list.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Default Grid Node<ept id="p1">**</ept> cannot be disabled.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>To enable or disable a node (DeployR Enterprise Only):</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>The Grid<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Grid Node List<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>Click the node you want to edit.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Grid Node Details<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Edit<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>Select the <bpt id="p1">**</bpt>Enable<ept id="p1">**</ept> checkbox to activate the node, or unselect it to disable the node.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Update<ept id="p1">**</ept> to save the changes.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>Viewing or Stopping Slot Activity</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Grid Node Details<ept id="p1">**</ept> page, you can review the slot activity.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>Additionally, you can shut down slots in order to terminate activity.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>This is a last resort for unwanted activity on the server.</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>This list is not updated in real time.</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>Refresh your page to see the latest activity.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>To review the slot activity for a node and shutdown slots:</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>The Grid<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Grid Node List<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Grid Node List<ept id="p1">**</ept>, click the node whose slot activity you want to monitor.</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Grid Node Details<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>Look at the <bpt id="p1">**</bpt>Slots in Use<ept id="p1">**</ept> section at the bottom.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>Click a slot link to <bpt id="p1">[</bpt>see details<ept id="p1">](#slots-in-use)</ept> about a particular slot.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>To terminate all of the activity on the selected node, click <bpt id="p1">**</bpt>Shutdown<ept id="p1">**</ept> in the toolbar to terminate all R sessions.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>To terminate the activity on a specific slot, do the following:</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Grid Node Details<ept id="p1">**</ept> page, click the slot whose activity you want to see and terminate.</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Slot Details<ept id="p1">**</ept> page, click <bpt id="p2">**</bpt>Shutdown<ept id="p2">**</ept> to terminate the activity and release the slot.</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>Deleting Nodes</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Default Grid Node<ept id="p1">**</ept> cannot be deleted.</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>To delete a node:</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>The Grid<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Grid Node List<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>Click the name of the node you want to delete.</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Grid Node Details<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Delete<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>The node is removed.</source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>Exporting Node Configurations</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source>You can export one or more node configurations into one CSV file.</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>Exporting can be used to copy the basic node configurations to another machine or to preserve them as a backup.</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>Figure: Export Grid Configuration page</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>To export node configurations:</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>The Grid<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Grid Node List<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Export Grid Configuration<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source>Select individual node configurations or all nodes to be exported.</source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Export to File<ept id="p1">**</ept> and save the file.</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source>Importing Node Configurations</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>You can import node configurations into the server from a CSV file you previously exported.</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source>You can import the contents of this file to same server from which it was exported or across multiple server deployments.</source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source>Grid node configurations are <bpt id="p1">[</bpt>validated<ept id="p1">](#node-validation-and-errors)</ept> upon import.</source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source>If the configuration works, then the node configuration is imported.</source>
        </trans-unit><trans-unit id="324" translate="yes" xml:space="preserve">
          <source>If not, an <bpt id="p1">[</bpt>error message<ept id="p1">](#node-validation-and-errors)</ept> will appear.</source>
        </trans-unit><trans-unit id="325" translate="yes" xml:space="preserve">
          <source>You can only import these configurations into a server instance matching the same DeployR version from which they were exported.</source>
        </trans-unit><trans-unit id="326" translate="yes" xml:space="preserve">
          <source>To import:</source>
        </trans-unit><trans-unit id="327" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>The Grid<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="328" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Grid Node List<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="329" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Import Grid Configurations<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="330" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Browse<ept id="p1">**</ept> and select the CSV file to be imported.</source>
        </trans-unit><trans-unit id="331" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Load<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="332" translate="yes" xml:space="preserve">
          <source>Figure: Choose Grid Nodes to Import page</source>
        </trans-unit><trans-unit id="333" translate="yes" xml:space="preserve">
          <source>To disable grid nodes upon import so that you can individually enable them at a later time, select the <bpt id="p1">**</bpt>Disable grid nodes<ept id="p1">**</ept> option.</source>
        </trans-unit><trans-unit id="334" translate="yes" xml:space="preserve">
          <source>You can always enable/disable grid nodes one at a time later.</source>
        </trans-unit><trans-unit id="335" translate="yes" xml:space="preserve">
          <source>Enabled nodes are activated immediately in the grid and available for load balancing.</source>
        </trans-unit><trans-unit id="336" translate="yes" xml:space="preserve">
          <source>Choose the nodes to import.</source>
        </trans-unit><trans-unit id="337" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Import<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="338" translate="yes" xml:space="preserve">
          <source>If a node by the same name already exists, the incoming node configuration is skipped.</source>
        </trans-unit><trans-unit id="339" translate="yes" xml:space="preserve">
          <source>The node configuration settings are <bpt id="p1">[</bpt>validated<ept id="p1">](#node-validation-and-errors)</ept>.</source>
        </trans-unit><trans-unit id="340" translate="yes" xml:space="preserve">
          <source>If the configuration works, then it is saved.</source>
        </trans-unit><trans-unit id="341" translate="yes" xml:space="preserve">
          <source>If not, an error message will appear.</source>
        </trans-unit></group></body></file></xliff>