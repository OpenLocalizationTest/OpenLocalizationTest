<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-administrator-getting-started.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3eee86e27f9ccef6152a1c0fb5d28e8c9f8d8d2529.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">ee86e27f9ccef6152a1c0fb5d28e8c9f8d8d2529</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-administrator-getting-started.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Getting Started for DeployR Administrators - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Getting started for DeployR Administrators: high level introduction to DeployR for the server administrator</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Getting Started - Administrators</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>This guide is for system administrators of DeployR, the <bpt id="p1">*</bpt>R Integration Server<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>If you are responsible for creating or maintaining an evaluation or a production deployment of the DeployR server, then this guide is for you.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>As an administrator, your key responsibilities are to ensure the DeployR server is properly provisioned and configured to meet the demands of your user community.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>In this context, the following policies are of central importance:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Server <bpt id="p1">[</bpt>security policies<ept id="p1">](#security-policies)</ept>, which include user authentication and authorization</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Server <bpt id="p1">[</bpt>R package management policies<ept id="p1">](#r-package-policies)</ept></source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Server <bpt id="p1">[</bpt>runtime policies<ept id="p1">](#runtime-policies)</ept>, which affect availability, scalability, and throughput</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Whenever your policies fail to deliver the expected runtime behavior or performance, you'll need to <bpt id="p1">[</bpt>troubleshoot<ept id="p1">](#troubleshooting)</ept> your deployment.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>For that we provide diagnostic tools and numerous recommendations.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>But first, you must install the server.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Comprehensive installation guides are available <bpt id="p1">[</bpt>here<ept id="p1">](deployr-installation.md)</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>For a general introduction to DeployR, read the <bpt id="p1">[</bpt>About DeployR<ept id="p1">](deployr-about.md)</ept> document.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Security Policies</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>User access to the DeployR server and the services offered on its <bpt id="p1">[</bpt>API<ept id="p1">](deployr-api-reference.md)</ept> are entirely under your control as the server administrator.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The principal method of granting access to DeployR is to use the <bpt id="p1">[</bpt>Administration Console<ept id="p1">](deployr-admin-console-about.md)</ept> to create <bpt id="p2">[</bpt>user accounts<ept id="p2">](deployr-admin-console-user-accounts.md)</ept> for each member of your community.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The creation of user accounts establishes a trust relationship between your user community and the DeployR server.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Your users can then supply simple <ph id="ph1">`username`</ph> and <ph id="ph2">`password`</ph> credentials in order to verify their identity to the server.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>You can grant additional <bpt id="p1">[</bpt>permissions<ept id="p1">](deployr-admin-console-permissions-with-roles.md)</ept> on a user-by-user basis to expose further functionality and data on the server.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>However, basic user authentication and authorization are only one small part of the full set of <bpt id="p1">[</bpt>DeployR security<ept id="p1">](../operationalize/configure-authentication.md)</ept> features, which includes full HTTPS/SSL encryption support, IP filters, and <ph id="ph1">`password`</ph> format and auto-locking policies.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>DeployR Enterprise also offers seamless integration with popular enterprise security solutions.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The full set of DeployR security features available to you as a system administrator are detailed in this <bpt id="p1">[</bpt>Security guide<ept id="p1">](deployr-security.md)</ept>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>R Package Policies</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The primary function of the DeployR server is to support the execution of R code on behalf of client applications.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>One of your key objectives as a DeployR administrator is to ensure a reliable, consistent execution environment for that code.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The R code developed and deployed by <bpt id="p1">[</bpt>data scientists<ept id="p1">](deployr-data-scientist-getting-started.md)</ept> within your community will frequently depend on one or more R packages.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Those R packages may be hosted on <bpt id="p1">[</bpt>CRAN<ept id="p1">](https://cran.r-project.org/)</ept>, <bpt id="p2">[</bpt>MRAN<ept id="p2">](https://mran.microsoft.com)</ept>, <bpt id="p3">[</bpt>GitHub<ept id="p3">](https://github.com/)</ept>, in your own local CRAN repository or elsewhere.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Making sure that these R package dependencies are available to the code executing on the DeployR server requires active participation from you, the administrator.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>There are two R package management policies you can adopt for your deployment, which are detailed in this <bpt id="p1">[</bpt>R Package Management guide<ept id="p1">](../operationalize/configure-manage-r-packages.md)</ept>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Runtime Policies</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The DeployR server supports a wide range of runtime policies that affect many aspects of the server runtime environment.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>As an administrator, you can select the preferred policies that best reflect the needs of your user community.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>General</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>Administration Console<ept id="p1">](deployr-admin-console-about.md)</ept> offers a <bpt id="p2">[</bpt>Server Policies<ept id="p2">](deployr-admin-managing-server-policies.md)</ept> tab within which can be found a wide range of policy configuration options, including:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Global settings such as server name, default server boundary, and so on</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Project persistence policies governing resource usage (sizes and autosave)</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Runtime policies governing authenticated, asynchronous, and anonymous operations</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Runtime policies governing concurrent operation limits, file upload limits, and event stream access</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The full set of general policy options available with the <bpt id="p1">**</bpt>Server Policies<ept id="p1">**</ept> tab is detailed in this <bpt id="p2">[</bpt>online help topic<ept id="p2">](deployr-admin-managing-server-policies.md)</ept>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Availability</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The DeployR product consists of a number of software components that combine to deliver the full capabilities of the R Integration Server: the server, the grid and the database.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Each component can be configured for High Availability (HA) in order to deliver a robust, reliable runtime environment.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>For a discussion of the available server, grid, and database HA policy options, see the <bpt id="p1">[</bpt>DeployR High Availability Guide<ept id="p1">](deployr-admin-configure-high-availability.md)</ept>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Scalability &amp; Throughput</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>In the context of a discussion on DeployR server runtime policies, the topics of scalability and throughput are closely related.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Some of the most common questions that arise when planning the configuration and provisioning of the DeployR server and grid are:</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>How many users can I support?</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>How many grid nodes do I need?</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>What throughput can I expect?</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>The answer to these questions will ultimately depend on the configuration and size of the server and grid resources allocated to your deployment.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>For detailed information and recommendations on tuning the server and grid for optimal throughput, read the <bpt id="p1">[</bpt>DeployR Scale &amp; Throughput Guide<ept id="p1">](deployr-admin-scale-and-throughput.md)</ept>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Big Data Policies</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>There may be times when your DeployR user community needs access to genuinely large data files, or big data.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>When such files are stored in the DeployR Repository or at any network-accessible URI, the R code executing on the DeployR server can load the desired file data on-demand.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>However, physically moving big data is expensive both in terms of bandwidth and throughput.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>To alleviate this overhead, the DeployR server supports a set of NFS-mounted directories dedicated to managing large data files.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>We refer to these directories as 'big data' external directories.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>As an administrator, you can enable this service by:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configuring<ept id="p1">](deployr-admin-manage-big-data.md#setting-up-nfs-setup)</ept> the big data directories within your deployment.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Informing your DeployR users that they must <bpt id="p1">[</bpt>use the R function, <ph id="ph1">`deployrExternal`</ph><ept id="p1">](deployr-admin-manage-big-data.md#adding-files-to-external-directories)</ept> in their R code to reference big data files within these directories.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>For the complete configuration and usage documentation, read the guide "<bpt id="p1">[</bpt>Managing External Directories for Big Data<ept id="p1">](deployr-admin-manage-big-data.md)</ept>".</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Troubleshooting</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>There is no doubt that, as an administrator, you've experienced failures with servers, networks, and systems.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Likewise, your chosen runtime policies may sometime fail to deliver the runtime behavior or performance needed by your community of users.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>When those failures occur in the DeployR environment, we recommend you first turn to the <bpt id="p1">[</bpt>DeployR diagnostic testing tool<ept id="p1">](deployr-admin-diagnostics-troubleshooting.md)</ept> to attempt to identify the underlying cause of the problem.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Beyond the diagnostics tool, the <bpt id="p1">[</bpt>Troubleshooting<ept id="p1">](deployr-admin-diagnostics-troubleshooting.md#troubleshooting)</ept> documentation offers suggestions and recommendations for common problems with known solutions.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>More Resources</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>This section provides a quick summary of useful links for administrators working with DeployR.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Use the table of contents to find all of the guides and documentation needed by the administrator.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Key Documents</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>About DeployR</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Installation &amp; Configuration</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Security</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>R Package Management</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Scale &amp; Throughput</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Diagnostic Testing &amp; Troubleshooting</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Other Getting Started Guides</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Application Developers</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Data Scientists</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Support Channel</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Microsoft R Server (and DeployR) Forum</source>
        </trans-unit></group></body></file></xliff>