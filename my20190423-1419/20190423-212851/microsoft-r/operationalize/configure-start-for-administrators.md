<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="configure-start-for-administrators.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a0d3d56851c121939bea1f76b3e0084f394626d5e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">0d3d56851c121939bea1f76b3e0084f394626d5e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\configure-start-for-administrators.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Get started for Administrators configuring Machine Learning Server to operationalize</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>If you are responsible for configuring or maintaining Machine Learning Server or R Server, then this guide is for you.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Manage and configure Machine Learning Server for operationalization</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies to:  Machine Learning Server, Microsoft R Server 9.x</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>You can configure Machine Learning Server after installation to act as a deployment server and host analytic web services as well as to execute code remotely.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>For a general introduction to  operationalization, read the <bpt id="p1">[</bpt>About<ept id="p1">](../what-is-operationalization.md)</ept> topic.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>This guide is for system administrators.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>If you are responsible for configuring or maintaining Machine Learning Server, then this guide is for you.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>As an administrator, your key responsibilities are to ensure Machine Learning Server is properly provisioned and configured to meet the demands of your user community.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>In this context, the following policies are of central importance:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Server <bpt id="p1">[</bpt>security policies<ept id="p1">](#security-policies)</ept>, which include user authentication and authorization</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Server <bpt id="p1">[</bpt>R package management policies<ept id="p1">](#r-package-policies)</ept></source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Server <bpt id="p1">[</bpt>runtime policies<ept id="p1">](#runtime-policies)</ept>, which affect availability, scalability, and throughput</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Whenever your policies fail to deliver the expected runtime behavior or performance, you need to troubleshoot your deployment.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>For that we provide <bpt id="p1">[</bpt>diagnostic tools<ept id="p1">](configure-run-diagnostics.md)</ept> and numerous recommendations.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Configure web &amp; compute nodes for analytic deployment and remote execution</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>To benefit from Machine Learning Server’s web service deployment and remote execution features, you must first configure the server after installation to act as a deployment server and host analytic web services.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Configuration components</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>All configurations have at least a single web node, single compute node, and a database.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Web nodes<ept id="p1">**</ept> act as HTTP REST endpoints with which users can interact directly to make API calls.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>These nodes also access the data in the database and send requests to the compute node for processing.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Web nodes are stateless, and therefore, session persistence ("stickiness") is not required.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>A single web node can route multiple requests simultaneously.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>However, you must have more than one web node to ensure high availability and avoid a single point of failure.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Compute nodes<ept id="p1">**</ept> are used to execute R and Python code as a session or service.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Each compute node has its own <bpt id="p1">[</bpt>pool of R and python shells<ept id="p1">](../operationalize/configure-evaluate-capacity.md#pool)</ept> and can therefore execute multiple requests at the same time.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Scaling out compute nodes enables you to have more R and Python execution shells and benefit from load balancing across these compute nodes.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>database<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>An SQLite 3.7+ database is installed by default, but you can, and in some cases must, <bpt id="p1">[</bpt>use a SQL Server or PostgreSQL<ept id="p1">](../operationalize/configure-remote-database-to-operationalize.md)</ept> database instead.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>One-box vs. Enterprise configurations</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>These nodes can be installed in one of two configurations:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>One-box</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>As the name suggests, a <bpt id="p1">[</bpt>one-box configuration<ept id="p1">](../operationalize/configure-machine-learning-server-one-box.md)</ept> involves one web node and one compute node run on a single machine.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Set-up is a breeze.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>This configuration is useful when you want to explore what it is to operationalize R and Python analytics using Machine Learning Server.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>It is perfect for testing, proof-of-concepts, and small-scale prototyping, but might not be appropriate for production usage.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>This configuration is covered in this article.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Learn more in this <bpt id="p1">[</bpt>One-box configuration<ept id="p1">](../operationalize/configure-machine-learning-server-one-box.md)</ept> article.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Configure Machine Learning Server on one-box architecture</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Enterprise</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt>enterprise configuration<ept id="p1">](../operationalize/configure-machine-learning-server-enterprise.md)</ept> where multiple nodes are configured on multiple machines along with other enterprise features.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>This configuration can be scaled out or in by adding or removing nodes.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Learn more about this setup in the <bpt id="p1">[</bpt>enterprise configuration<ept id="p1">](../operationalize/configure-machine-learning-server-enterprise.md)</ept> article.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>For added security, you can <bpt id="p1">[</bpt>configure SSL<ept id="p1">](../operationalize/configure-https.md)</ept> and authenticate against <bpt id="p2">[</bpt>Active Directory (LDAP) or Azure Active Directory<ept id="p2">](../operationalize/configure-authentication.md)</ept> in this configuration.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Configure Machine Learning Server for the enterprise architecture</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Supported platforms</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The web nodes and compute nodes are supported on these operating systems</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Windows</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Linux</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Windows<ph id="ph1">&amp;nbsp;</ph>Server<ph id="ph2">&amp;nbsp;</ph>2012<ph id="ph3">&amp;nbsp;</ph>R2<ph id="ph4">&amp;nbsp;</ph><ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph><ph id="ph7">&amp;nbsp;</ph><ph id="ph8">&amp;nbsp;</ph><ph id="ph9">&amp;nbsp;</ph><ph id="ph10">&amp;nbsp;</ph></source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Ubuntu 14.04, Ubuntu 16.04</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Windows Server 2016</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>CentOS/RHEL 7.x</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Security policies</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Machine Learning Server has many features that support the creation of secure applications.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Common security considerations, such as data theft or vandalism, apply regardless of the version of Machine Learning Server you are using.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Data integrity should also be considered as a security issue.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If data is not protected, it is possible that it could become worthless if improvised data manipulation is permitted and the data is inadvertently or maliciously modified.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>In addition, there are often legal requirements that must be adhered to, such as the correct storage of confidential information.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>User access to the Machine Learning Server and the operationalization services offered on its <bpt id="p1">[</bpt>API<ept id="p1">](concept-api.md)</ept> are entirely under your control as the server administrator.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Machine Learning Server offers seamless integration with popular enterprise security solutions like Active Directory LDAP or Azure Active Directory.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>You can configure Machine Learning Server to <bpt id="p1">[</bpt>authenticate<ept id="p1">](configure-authentication.md)</ept> using these methods to establish a trust relationship between your user community and the operationalization engine for Machine Learning Server.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Your users can then supply simple <ph id="ph1">`username`</ph> and <ph id="ph2">`password`</ph> credentials in order to verify their identity.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>A token is issued to an authenticated user.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>In addition to authentication, you can add other enterprise security around Machine Learning Server such as:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Secured connections using <bpt id="p1">[</bpt>SSL/TLS 1.2<ept id="p1">](configure-https.md)</ept>.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>For security reasons, we strongly recommend that you enable SSL/TLS 1.2 in <bpt id="p1">**</bpt>all production environments.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Cross-Origin Resource Sharing<ept id="p1">](configure-cors.md)</ept> to allow restricted resources on a web page to be requested from another domain outside the originating domain.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Role-based access control<ept id="p1">](configure-roles.md)</ept> over web services in Machine Learning Server.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Additionally, we recommend that you review the following Security Considerations:</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Enterprise Security, HTTPS, LDAPs for Machine Learning Server</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>R package policies</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>The primary function of the operationalization feature is to support the execution of R code on behalf of client applications.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>One of your key objectives as an administrator is to ensure a reliable, consistent execution environment for that code.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>The R code developed and deployed by data scientists within your community  frequently depends on one or more R packages.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Those R packages may be hosted on <bpt id="p1">[</bpt>CRAN<ept id="p1">](https://cran.r-project.org/)</ept>, <bpt id="p2">[</bpt>MRAN<ept id="p2">](https://mran.microsoft.com)</ept>, <bpt id="p3">[</bpt>GitHub<ept id="p3">](https://github.com/)</ept>, in your own local CRAN repository or elsewhere.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Making sure that these R package dependencies are available to the code executing on Machine Learning Server's operationalization feature requires active participation from you, the administrator.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>There are several R package management policies you can adopt for your deployment, which are detailed in this <bpt id="p1">[</bpt>R Package Management guide<ept id="p1">](configure-manage-r-packages.md)</ept>.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Runtime policies</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The operationalization feature supports a wide range of runtime policies that affect many aspects of the server runtime environment.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>As an administrator, you can select the preferred policies that best reflect the needs of your user community.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>General</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>The external configuration file, <ph id="ph1">\&lt;</ph>node-install-path&gt;\appsettings.json defines a number of policies used when deploying and operationalizing web services with Machine Learning Server.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>There is one appsettings.json file on each web node and on each compute node.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>This file contains a wide range of policy configuration options for each node.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>The location of this file depends on the server version, operating system, and the node.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Learn more in this article: <bpt id="p1">[</bpt>"Default installation paths for compute and web nodes"<ept id="p1">](configure-find-admin-configuration-file.md)</ept>.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>On the web node, this configuration file governs authentication, SSL, CORS support, service logging, database connections, token signing, and more.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>On the compute node, this configuration file governs SSL, logging, <bpt id="p1">[</bpt>shell pool size<ept id="p1">](configure-evaluate-capacity.md#pool)</ept>, execution ports, and more.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Asynchronous batch sizes</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Your users can perform speedy real-time and batch scoring.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>To reduce the risk of resource exhaustion by a single user, you can set the maximum number of operations that a single caller can execute in parallel during a specific asynchronous batch job.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>This value is defined in <ph id="ph1">`"MaxNumberOfThreadsPerBatchExecution"`</ph>  property in the appsettings.json on the web node.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>If you have multiple web nodes, we recommend you set the same values on every machine.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Availability</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Machine Learning Server consists of web and compute nodes that combine to deliver the full capabilities of this R and Python operationalization server.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Each component can be configured for Active-Active High Availability to deliver a robust, reliable runtime environment.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>You can configure Machine Learning Server to use multiple Web Nodes for Active-Active backup / recovery using a load balancer.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>For data storage high availability, you can leverage the high availability capabilities found in enterprise grade databases (SQL Server or PostgreSQL).</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Learn how to use one of those databases, <bpt id="p1">[</bpt>here<ept id="p1">](configure-remote-database-to-operationalize.md)</ept>.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Plan for High Availability with Machine Learning Server</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Scalability &amp; throughput</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>In the context of a discussion on runtime policies, the topics of scalability and throughput are closely related.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Some of the most common questions that arise when planning the configuration and provisioning of Machine Learning Server for operationalization are:</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>How many users can I support?</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>How web nodes and compute nodes do I need?</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>What throughput can I expect?</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>The answer to these questions ultimately depends on the configuration and node resources allocated to your deployment.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>To evaluate and simulate the capacity of a configuration, use the <bpt id="p1">[</bpt>Evaluate Capacity tool<ept id="p1">](configure-evaluate-capacity.md)</ept>.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>You can also <bpt id="p1">[</bpt>adjust the pool size<ept id="p1">](configure-evaluate-capacity.md#pool)</ept> of available R shells for concurrent operations.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Troubleshooting</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>There is no doubt that, as an administrator, you have experienced failures with servers, networks, and systems.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Likewise, your chosen runtime policies may sometime fail to deliver the runtime behavior or performance needed by your community of users.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>When those failures occur in the operationalization environment, we recommend you first turn to the <bpt id="p1">[</bpt>diagnostic testing tool<ept id="p1">](configure-run-diagnostics.md)</ept> to attempt to identify the underlying cause of the problem.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Beyond the diagnostics tool, the <bpt id="p1">[</bpt>Troubleshooting<ept id="p1">](configure-run-diagnostics.md#troubleshooting)</ept> documentation offers suggestions and recommendations for common problems with known solutions.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>More resources</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>This section provides a quick summary of useful links for administrators working with Machine Learning Server's operationalization feature.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Use the table of contents to find all of the guides and documentation needed by the administrator.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Key Documents</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>About Operationalization</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Configuration</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>R Package Management</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>What are web services?</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Diagnostic Testing &amp; Troubleshooting</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Capacity Evaluation</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Comparison between 8.x and 9.x</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Other Getting Started Guides</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>How to integrate web services and authentication into your application</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Support Channel</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Forum</source>
        </trans-unit></group></body></file></xliff>