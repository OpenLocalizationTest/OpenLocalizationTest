<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-common-administration-tasks.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc77501c42ee264dce07e0eb768521fcd85c21c112953b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1c42ee264dce07e0eb768521fcd85c21c112953b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-common-administration-tasks.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Common DeployR Administration Tasks - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Common DeployR Administration Tasks: Starting and Stopping DeployR, Inspecting Server Logs, Database Management</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Common DeployR Administration Tasks</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Starting and Stopping DeployR for Microsoft R Server 8.0.5</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>To start or stop all DeployR-related services on the main server (not nodes) at once, use the administrator utility.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Launch the DeployR administrator utility script with administrator privileges:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>On Windows:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>On Linux:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>From the main menu, choose option <bpt id="p1">**</bpt>Start/Stop Server<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>When prompted whether you want to stop (S) or restart (R) the DeployR server, enter your choice<ph id="ph1">`R`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>It may take some time for the Tomcat process to terminate and restart.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Starting and Stopping DeployR 8.0.0</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>To start or stop all DeployR-related services on the main server (not nodes) use the following commands.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Table: Starting DeployR 8.0.0</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Operating System</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Commands</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Windows</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>To start the services, run:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Linux</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>To start the services individually on the main server (not nodes):</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>To start all services on the main server (not nodes) at once:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Mac OS X</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>To start the services individually on the main server (not nodes):</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>To start all services on the main server (not nodes) at once:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Table: Stopping DeployR 8.0.0</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Operating System</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Commands</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Windows</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>To stop the services, run:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Linux</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>To stop the services individually on the main server (not nodes):</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>To stop all services on the main server (not nodes) at once:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Mac OS X</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>To stop the services individually on the main server (not nodes):</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>To stop all services on the main server (not nodes) at once:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Inspecting Server Logs</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`catalina.out`</ph> server log file is found at the following location:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Operating System</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Location</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Windows</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Linux</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Mac OS X</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Look here<ept id="p1">](deployr-admin-diagnostics-troubleshooting.md#inspecting-diagnostic-log-files)</ept> for more information on other log files associated with DeployR.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>By default, the DeployR server logs at the <ph id="ph1">`INFO`</ph> level, which is appropriate for production environments.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The server emits <ph id="ph1">`[DEPLOYR-EVENT]`</ph> log statements that provide a permanent record of the following:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>API Call / Response Events</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Authentication Events</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>HTTP Session Events</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Grid R Session Events</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Each <ph id="ph1">`[DEPLOYR-EVENT]`</ph> is rendered to the log file in a fixed format, which simplifies parsing and searching both manually or within log inspection tools.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The following section describes the different <ph id="ph1">`[DEPLOYR-EVENT]`</ph> that can be found in the server log file.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>API Call / Response Events</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The log file captures the following events related to API calls:</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>- denoting the start of an API call including call parameters.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>- denoting the response generated for the call.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>- denoting the end of an API call.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Authentication Events</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The log file captures the following events related to user authentications:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>- denoting a successful user authentication.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>- denoting a failed user authentication.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>HTTP Session Events</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The log file captures the following events related to HTTP session creation and release:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>- denoting the creation of an HTTP session</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>- denoting the release of an HTTP session</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Grid R Session Events</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>The log file captures the following events related to R session creation and release:</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>- denoting the creation of an R session on the grid</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>- denoting the release of an R session on the grid</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Tracing Related Log Events</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Related log events can be traced in a number of ways including but not limited to the use of the <ph id="ph1">`HTTP session`</ph> identifier or a DeployR-managed <ph id="ph2">`project`</ph> identifier.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>For example, using the <ph id="ph1">`HTTP session`</ph> identifier makes the tracing of a series of log events representing an anonymous execution of a repository-managed R script simple as follows.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>This sample log output captures an <ph id="ph1">`/r/repository/script/execute`</ph> API call, originating from <ph id="ph2">`180.183.148.137`</ph>, executed on behalf of an <ph id="ph3">`anonymous`</ph> user, on HTTP session <ph id="ph4">`2DD2302B91770E89333848DBB9505D0A`</ph>.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The log output also indicates the time taken on the call as well as the response data returned on call completion.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Backing Up and Restoring Data</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>For DeployR for Microsoft R Server 8.0.5</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>To back up and restore your Deployr data:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Log into the DeployR landing page.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>From the landing page, open the <bpt id="p1">**</bpt>Administration Console<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Follow these instructions<ept id="p1">](deployr-admin-console-database.md)</ept>.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>For DeployR 8.0.0</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Follow these instructions to back up  and restore your DeployR data or to reset the database to its initial post-installation state.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Follow these steps to back up the data in the database used by DeployR.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Log into the machine as a user with administrator privileges.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Ensure all users are logged out of DeployR.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>As admin, you can always check the grid activity in the <bpt id="p1">**</bpt>Grid<ept id="p1">**</ept> tab of the Administration Console.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Run the database utility script as follows:</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>On Windows:</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>On Linux:</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>When prompted by the script:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>To reinitialize the database, choose option <ph id="ph1">`2`</ph>.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>To back up the database, choose option <ph id="ph1">`3`</ph> and enter the path in which the database backup should be saved.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Verify that the backup was successful by checking the contents of the directory where you dumped the database.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>To restore the database, choose option <ph id="ph1">`4`</ph> and enter the path to your backup folder.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>By default, the backup path includes a date stamped folder and ends with the folder <ph id="ph1">`deployr`</ph>.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Opening DeployR Ports</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>To learn more about the ports you need to open, refer to the <bpt id="p1">[</bpt>DeployR Installation Guide<ept id="p1">](deployr-installation.md)</ept> for your operating system and DeployR version.</source>
        </trans-unit></group></body></file></xliff>