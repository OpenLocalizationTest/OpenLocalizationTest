<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-admin-scale-and-throughput.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c324dda202ad5e34690d8f0ec40062f9c21087c47.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">324dda202ad5e34690d8f0ec40062f9c21087c47</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-admin-scale-and-throughput.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Scale &amp; Throughput - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Understanding Scale and Throughput in DeployR</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>scalability, throughput, DeployR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Scale &amp; Throughput</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Introduction</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>DeployR is a server framework that exposes the R platform as a service allowing the integration of R statistics, analytics, and visualizations inside Web, desktop, and mobile applications.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Within the server, a grid framework provides sophisticated load-balancing capabilities for a single DeployR server instance.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The overall capacity of your server and grid, in conjunction with the nature and volume of your anticipated workload, determines the runtime characteristics for the tasks that are executing within the DeployR environment.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Some of the most common questions that arise when planning the configuration and provisioning of the DeployR server and grid are:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>How many users can I support?</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>How many grid nodes do I need?</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>What throughput can I expect?</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The answer to these questions will depend on the configuration and size of the server and grid resources allocated to your deployment.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The information in this document will help you familiarize yourself with the central issues related to deployment, and also offers specific recommendations you can use to tailor your DeployR environment.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>While this document is primarily intended for DeployR administrators, the section <bpt id="p1">[</bpt>About Throughput<ept id="p1">](#about-throughput)</ept> also helps application and R script developers optimize their throughput.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Get More DeployR Power:<ept id="p1">**</ept> Multiple grid node support is available for DeployR Enterprise only.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Tuning Server Capacity</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>DeployR offers the ability to expand and contract server capacity to effectively handle increasing workloads comprised of user sessions, live projects, and background jobs.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>When a single DeployR server instance is working with an arbitrarily large number of grid nodes, this server acts as the sole gatekeeper to the grid and all of its resources.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>It is for this reason that the server has the potential, under a certain load, to become a bottleneck at runtime.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Whenever you increase the resources allocated to the DeployR server, thereby increasing its capacity, this server can handle a higher workload.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The act of increasing or even decreasing the resources that are allocated to the server is referred to as <bpt id="p1">*</bpt>vertically scaling<ept id="p1">*</ept> the server.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>In theory, the more memory you allocate to a server, the more work it can perform.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>However, increasing the amount of allocated memory only works to a point, and part of the configuration process is to tune the system to your particular needs.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>By default, the DeployR server instance should be able to comfortably accommodate hundreds of concurrent users, each performing a moderate number of tasks.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>At runtime, each task consumes server resources regardless of whether that task is an authenticated operation running as a persistent project, an asynchronous operation running as a background job, or an anonymous operation running as a stateless project.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>All server resources are allocated on the Java Virtual Machine (JVM) heap, which is a finite block of dedicated memory.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>By default, DeployR attempts to allocate a JVM heap size of 1024MB, which is a required minimum system requirement in production environments.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Take Action!<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If you expect or encounter a server load that exceeds the resources provided by the default DeployR configuration, use the JVM command line options <ph id="ph1">`-Xms`</ph> and <ph id="ph2">`-Xmx`</ph> to increase JVM heap space, and <ph id="ph3">`-Xss`</ph> to reduce Java thread stack size used by the server.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>You can allocate a JVM heap size of up to one fourth of the physical memory size of your server computer.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For example, if your server computer has 8 GB of physical memory, allocate a heap size of no more than 2 GB.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Tuning Grid Capacity</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>DeployR Enterprise offers the ability to expand and contract grid capacity to effectively handle increasing workloads comprised of user sessions, live projects, and background jobs.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>With DeployR Enterprise, not only can you point this default grid node to a remote location and customize its slot limit, but you can also install and configure additional grid nodes to scale for increasing load.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Each node on the grid contributes its own processor, memory, and disk resources.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>These resources can be leveraged by the DeployR server to run R code as part of user authenticated, asynchronous, and anonymous operations.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Whenever you increase the number of nodes on your DeployR grid, you effectively increase the grid’s capacity.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Increasing or even decreasing the number of nodes on your grid is referred to as <bpt id="p1">*</bpt>horizontally scaling<ept id="p1">*</ept> the grid.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>An increased grid capacity enables the grid to perform more tasks on behalf of the server.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Additionally, increasing or decreasing the resources allocated to the nodes on the grid further contributes to the grid’s horizontal scaling since those resources determine the slot limits.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>And, slot limits directly impact the overall grid capacity.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>By tuning settings under the <bpt id="p1">**</bpt>Grid<ept id="p1">**</ept> tab in the DeployR Enterprise Administration Console, a server administrator can horizontally scale the capacity of the grid at runtime.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The server will automatically distribute the workload across all grid nodes.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>A well-configured grid maximizes throughput while minimizing resource contention.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The best way to start planning the provisioning of your grid is to gain an understanding of the anticipated workload for this grid.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>With that workload in mind, you can then scale the grid to handle this load.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The DeployR Enterprise server and grid deployment model can be described as follows, where N is defined as the optimal number of nodes on the grid: <ph id="ph1">`Server[1] -&gt; Node[1..N]`</ph> Based on this deployment model, the appropriate value for <ph id="ph2">`N`</ph>, when horizontally scaling the grid, will always be a function of the nature and the volume of the anticipated workload.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The following scenarios demonstrate different deployment configurations based on specific workload expectations.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>These configurations are not mutually exclusive.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Project Workloads</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>When tuning your DeployR Enterprise grid’s capacity for the anticipated project workload, use the following formula to determine the optimal number of nodes (N) to have on your grid that can handle authenticated operations:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Formula</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Where:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`N`</ph> is the optimal number of nodes required to handle the anticipated workload.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>For project workloads, these nodes must be configured to support authenticated operations.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The system administrator can specify a node’s operating mode when creating or editing that node in the <bpt id="p1">**</bpt>Grid<ept id="p1">**</ept> tab of the DeployR Administration Console.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`Max. Concurrent Users`</ph> is the maximum number of DeployR users you anticipate will work concurrently.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`Max. Concurrent Projects`</ph> is the maximum number of projects a single user can work on concurrently.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>The system administrator can control the concurrent project limit using the Per-user authenticated limit setting in the <bpt id="p1">**</bpt>Server Policies<ept id="p1">**</ept> tab of the DeployR Administration Console.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`Average Slot Limit`</ph> is the average value for the <bpt id="p1">**</bpt>Slot Limit<ept id="p1">**</ept> setting for each of the grid nodes.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The system administrator can set the value for each node’s <bpt id="p1">**</bpt>Slot Limit<ept id="p1">**</ept> in the <bpt id="p2">**</bpt>Grid<ept id="p2">**</ept> tab of the DeployR Administration Console.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>For more on managing your grid, see the <bpt id="p1">[</bpt>Administration Console Help<ept id="p1">](deployr-admin-managing-the-grid.md)</ept>.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Recommended Number of Cores<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>To prevent resource exhaustion when provisioning the grid, carefully consider the processor, memory, and disk resources available on the node as you define the slot limit.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>For optimal throughput, the slot limit on a given node should equal the number of CPU cores on the node.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Example<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Let’s say that we have a DeployR Enterprise deployment with <ph id="ph1">`50`</ph> authenticated users, each of which is actively working on their own projects.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>During the working day, each user may work on up to <ph id="ph1">`3`</ph> different projects simultaneously.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>With as many as 50 users working on as many as three projects, the grid’s capacity must support <ph id="ph1">`150`</ph> simultaneous, live projects in order to be capable of handling peak workloads.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>In this example, if each grid node is configured with sufficient resources for <ph id="ph1">`30`</ph> slots, the appropriate value of <ph id="ph2">`N`</ph> is at least <ph id="ph3">`5`</ph> nodes dedicated to authenticated operations.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Formula</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Asynchronous Job Workloads</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>When tuning your DeployR Enterprise grid’s capacity for your anticipated asynchronous job workload, use the following formula to determine the optimal number of nodes (N) capable of handling asynchronous operations to have on your grid:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Formula</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Where:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`N`</ph> is the optimal number of nodes required to handle the anticipated workload.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>For job workloads, these nodes must be configured to support asynchronous operations.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>The system administrator can define a node’s operating mode when creating or editing that node in the <bpt id="p1">**</bpt>Grid<ept id="p1">**</ept> tab of the DeployR Administration Console.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`Target Number of Jobs per Hour`</ph> is the average number of jobs to execute per hour.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`Average Time to Complete Job`</ph> is an estimate of the average amount of time it should take to complete each job in the anticipated workload.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3600`</ph> is the number of seconds in an hour.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`Average Slot Limit`</ph> is the average value for the <bpt id="p1">**</bpt>Slot Limit<ept id="p1">**</ept> setting for each of the grid nodes.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>The system administrator can set the value for each node’s <bpt id="p1">**</bpt>Slot Limit<ept id="p1">**</ept> in the <bpt id="p2">**</bpt>Grid<ept id="p2">**</ept> tab of the DeployR Administration Console.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>For more on managing your grid, see the <bpt id="p1">[</bpt>Administration Console Help<ept id="p1">](deployr-admin-managing-the-grid.md)</ept>.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>To prevent resource exhaustion when provisioning the grid, carefully consider the processor, memory, and disk resources available on the node as you define the slot limit.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>For optimal throughput, the slot limit on a given node should equal the number of CPU cores on the node.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Example<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Let’s say that we have a DeployR Enterprise deployment where <ph id="ph1">`1000`</ph> asynchronous jobs execute per hour (<ph id="ph2">`3600`</ph> seconds).</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Let’s assume that given the nature of these jobs, the total execution time per job is an average of ten minutes (<ph id="ph1">`600`</ph> seconds).</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>If each grid node is configured with sufficient resources for <ph id="ph1">`30`</ph> slots, then the optimal value of <ph id="ph2">`N`</ph> is at least <ph id="ph3">`6`</ph> nodes dedicated to asynchronous operations.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Formula</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Considering &amp; Configuring for Throughput</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>In this section, we present you with a description and some examples to help you understand throughput and the impact that DeployR artifacts have on this throughput.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Additionally, we highlight the settings needed to optimize DeployR for high-volume throughput.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Artifacts<ept id="p1">**</ept> are workspace objects and working directory files that are generated during R code execution.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>In practical terms, the <bpt id="p1">**</bpt>throughput<ept id="p1">**</ept> for your system is determined by your server and grid capacity in conjunction with the nature and volume of the tasks being processed.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>DeployR throughput measures the number of tasks processed on the DeployR grid in a fixed time period.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Understanding the Nature of Tasks</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>To illustrate the nature of a task, let’s begin with a summary of the basic workflow for an asynchronous job.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Workflow</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>A DeployR user submits an asynchronous job.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>The DeployR server queues the job for execution.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>The server’s internal job scheduler sees a job queued for execution and attempts to locate an available slot on the grid in which to execute that job.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Once located, the scheduler reserves the slot and dispatches the job onto that slot for execution.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>When the job execution completes, the server captures a complete snapshot of the R session associated with that slot.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Then, the server saves the snapshot as a persistent project in the server database and releases the slot so it is available for further tasks.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>By default, a snapshot of the R session is saved as a persistent DeployR project once a job has finished executing.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>As an alternative, use the <ph id="ph1">`storenoproject`</ph> parameter when scheduling a job to instruct the server not to save a persistent project.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>If you specify that no project should be saved using the <ph id="ph1">`storenoproject`</ph> parameter, you can still store specific artifacts to the repository.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>In certain scenarios, storing these artifacts to the repository rather than creating a persistent project can result in greatly improved throughput.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Example of How Tasks Affects Throughput</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>To demonstrate how throughput is highly dependent on the nature of the tasks, see the following table for a side-by-side comparison of two jobs with very different natures that are executing on the grid.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>These jobs are contrived to clearly show how the nature of the task itself has significant impact on the observed throughput.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Sample R Code for Job</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Sample R Code for Job</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>rnorm(1:300000)</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>1. Time needed to execute R code</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>1178 ms</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>1180 ms</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>2. Resulting size of R workspace</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>0.003 Mb</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>2.5 Mb</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>3. Time needed to save artifacts to the database</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>177 ms</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>1435 ms</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>4. Total job time<bpt id="p1">&lt;sup&gt;</bpt>1<ept id="p1">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>1580 ms</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>2850 ms</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;sup&gt;</bpt>1<ept id="p1">&lt;/sup&gt;</ept> The time needed to spin up the job on its slot, execute the job, persist the data, spin down, and release the slot.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>From the data in this table, we can learn a lot about the nature of jobs:</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Almost the same amount of time was needed to execute the R code in both jobs.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>The size of the R workspace generated by the second job is more than 500 times larger than the R workspace generated by the first job.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Due to the significant differences in the size of the artifacts generated by these jobs, it took eight times longer to save the artifacts (R workspace and directory data) from the second job to the DeployR database than it took to save the artifacts for the first job.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>As a consequence of the artifacts generated and persisted, the total time taken to handle the second job from start to finish was nearly twice as much as the total time taken to handle the first job.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Beyond the time it takes to execute the R code for a job, we can see that if you are going to save a persistent project after your job finishes executing, then the size of the resulting artifacts have a big impact on the total job time.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>This simple and somewhat contrived example demonstrates a key point when trying to understand the nature of your persistent tasks and DeployR throughput: <bpt id="p1">**</bpt>artifacts matter<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Whether those artifacts are objects in the R workspace or files in the working directory, if the code you execute on a job leaves unnecessary artifacts behind, there can be very real consequences on the overall throughput of your grid.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>An unnecessary artifact is any workspace object or working directory file that is not required later when evaluating the final result of the job.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Guideline for Responsible Usage</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>There are guidelines for responsible task usage to help you maximize throughput.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Whenever tasks are performance-sensitive, the most effective step a user can take towards optimizing throughput for his or her own tasks is to ensure that the R code leaves no unnecessary artifacts behind.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Minimal artifacts ensure minimal data is stored in the resulting persistent project.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>In some cases, it may be best to use the <ph id="ph1">`storenoproject`</ph> parameter to skip the saving of a persistent project altogether, and instead, selectively store only specific workspace and directory data in the repository.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Configuring DeployR for High-Volume Throughput</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>For most DeployR deployments, the default configuration delivers adequate server runtime performance and resource usage.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>However, in some deployments, where the workload is anticipated to be significantly high-volumed, a specialized DeployR configuration may be required.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>The default runtime behavior of the DeployR server is determined by the settings in:</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt><bpt id="p2">**</bpt>Server Policies<ept id="p2">**</ept> tab<ept id="p1">](deployr-admin-managing-server-policies.md)</ept> in the Administration Console</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>The DeployR external configuration file, <ph id="ph1">`$DEPLOYR_HOME/deployr/deployr.groovy`</ph></source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Typically, high-volume throughput deployments are characterized by a very large number of short-lived tasks that need to be executed as transactions without direct end-user participation or intervention.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>For such high-volume throughput deployments, you may need to enable the following properties in the <ph id="ph1">`deployr.groovy`</ph> file:</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>Enabling these configuration properties will result in the following direct consequences on the runtime behavior of the DeployR server:</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>The DeployR server becomes capable of executing hundreds of thousands of short-lived tasks without risking resource exhaustion.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Grid node validation at runtime is disabled, which means the grid's ability to self-heal when grid nodes fail and recover is no longer supported.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Without self-healing, node failures on the grid may interfere with the future scheduling and execution of tasks on the grid.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Therefore, we recommend that you enable these <ph id="ph1">`deployr.groovy`</ph> file properties only if you determine that the default DeployR configuration fails under the anticipated loads.</source>
        </trans-unit></group></body></file></xliff>