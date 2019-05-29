<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-admin-configure-high-availability.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3d5ec80ef95928391bd6426521a1bad0a213d12e1.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d5ec80ef95928391bd6426521a1bad0a213d12e1</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-admin-configure-high-availability.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>DeployR Server, Grid &amp; Database High Availability - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to Configure High Availability HA for DeployR Server, Grid &amp; Database</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>DeployR Server and Grid High Availability</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept> (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Server High Availability</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>When discussing high-availability in the context of server systems, clustered Java Web applications are a common architectural solution.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>However, due to the non-serializable socket connections maintained per R session by the DeployR server, full distributed session management across servers in a cluster is not possible.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>It depends on serializable session state.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>There are however alternative deployment options that can be adopted to improve server availability and overall uptime.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The relative merits of these deployment options are discussed in the following sections.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Primary-Standby Deployment</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This deployment model while simple can be highly effective.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Your application makes use of a <ph id="ph1">`primary`</ph> server and a <ph id="ph2">`standby`</ph> server that share a single instance of the DeployR database.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>By default, your application talks only to the <ph id="ph1">`primary`</ph> server.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`primary`</ph> server becomes unresponsive at runtime, your application detects this condition and transitions away from the unresponsive <ph id="ph2">`primary`</ph> by redirecting all traffic to the <ph id="ph3">`standby`</ph> server.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The following is supported with a SQL Server or PostgreSQL database (not the default H2 database) for DeployR 8.0.5, or a MongoDB database for DeployR 8.0.0.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The following steps detail how to configure this type of deployment:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>DeployR Database Setup</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Install a single, standalone instance of the DeployR database.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This single database instance is used by the <ph id="ph1">`primary`</ph> and <ph id="ph2">`standby`</ph> servers, as detailed next.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Primary Server Setup</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Install a dedicated DeployR server and designate it as your <ph id="ph1">`primary`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Configure the database endpoint for the primary using deployr.groovy.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Set the primary <ph id="ph1">`deployr.server.policy.override.web.context`</ph> property using deployr.groovy.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Standby Server Setup</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Install a dedicated DeployR server and designate it as your <ph id="ph1">`standby`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Configure the database endpoint for the standby using deployr.groovy.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Set the standby <ph id="ph1">`deployr.server.policy.override.web.context`</ph> property using deployr.groovy.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>DeployR Grid Setup</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Using either the <ph id="ph1">`primary`</ph> or <ph id="ph2">`standby`</ph> server administration console:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Add details for each grid node you have provisioned for your deployment.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>At this point, your <ph id="ph1">`Primary-Standby Deployment`</ph> is fully configured.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>As the <ph id="ph1">`primary`</ph> and <ph id="ph2">`standby`</ph> servers in your deployment are sharing a single instance of the DeployR database your servers are also sharing:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>A single DeployR repository where all R scripts, models, etc. are managed.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>A single DeployR grid.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>While this can be an effective deployment model, take careful note of the following:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Failover is not automatic.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Your application must detect when the <ph id="ph1">`primary`</ph> becomes unresponsive and then actively take steps to reroute all traffic to the <ph id="ph2">`standby`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>A single grid means zombie tasks (initiated by a <ph id="ph1">`primary`</ph> that then fails) can leak grid resources (memory and/or processor cycles) that cannot be reclaimed by the <ph id="ph2">`standby`</ph> when it takes over active management of the grid.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>This type of resource impairment can lead to performance degradation over time.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>A potentially better deployment model would isolate failures, in order to ensure that resource impairment by zombie tasks would not continue to impact overall availability or responsiveness of the system.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>This model forms the motivation for the next deployment model to be described, <ph id="ph1">`Load Balanced Deployment`</ph>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Load Balanced Deployment</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>While multiple DeployR servers cannot participate in a classic cluster configuration with automatic failover, it is possible to deploy multiple servers behind an HTTP load balancer to distribute load and even adapt to server failures at runtime.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The following steps detail how to configure this type of deployment:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Server Setup <ph id="ph1">\*</ph> N</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Install two or more DeployR servers.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Each server should be configured to use its own dedicated database.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Each server should be configured to use its own dedicated set of grid nodes.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Load Balancer Setup</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Install your preferred HTTP load balancer.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Configure the load balancer to enforce sticky HTTP sessions.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Register the IP endpoint of each DeployR server with your load balancer.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>At this point, your <ph id="ph1">`Load Balanced Deployment`</ph> is fully configured.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>In the event of a server failure all other servers in the cluster will continue functioning unaffected.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>However, given each server in your deployment operates independently of the other servers there is one important implication:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Your R scripts, models, etc. must be manually replicated across the DeployR repositories associated with each of your servers.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Grid High Availability</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The DeployR grid is designed to deliver high-availability at runtime, supporting both redundancy and failover.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The server monitors the health off all resources on the grid at runtime.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>If an individual slot on the grid or even an entire grid node becomes unresponsive, the server automatically contracts the grid, bypassing those failing resources.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If failing resources once again become responsive the server automatically expands the grid, to include the newly responsive grid resources.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>In this way, the DeployR grid can be said to be <ph id="ph1">`self-healing`</ph>, capable of automatically adjusting to system failures and recoveries at runtime, ensuring maximum uptime and responsiveness.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>RBroker High Availability!</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>RBroker Framework<ept id="p1">](deployr-rbroker-framework.md#pooledtaskbroker)</ept> includes a fault-tolerant implementation of the <ph id="ph1">`PooledTaskBroker`</ph>.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Tasks executing on the new PooledTaskBroker that fail due to grid failures at runtime are automatically detected and re-executed without requiring client application intervention.</source>
        </trans-unit></group></body></file></xliff>