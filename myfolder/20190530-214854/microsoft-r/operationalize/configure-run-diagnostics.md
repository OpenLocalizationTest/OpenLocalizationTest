<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="configure-run-diagnostics.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e0df7a834727c3fb5b679697538ddd33a521e492c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">0df7a834727c3fb5b679697538ddd33a521e492c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\configure-run-diagnostics.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Diagnostics &amp; troubleshooting the Machine Learning Server configuration</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Troubleshooting and test your Machine Learning Server and R Server configuration or trace code executions</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Troubleshooting &amp; diagnostics for Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies to:  Machine Learning Server, Microsoft R Server 9.1</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>You can assess the health of your web and compute node environment using the diagnostic tests in the Administration Utility.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This utility is installed by default with Machine Learning Server (and R Server).</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Armed with this information, you can identify unresponsive components, execution problems, and access <bpt id="p1">[</bpt>the log files<ept id="p1">](#logs)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The set of diagnostic tests includes:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A general health check of the configuration</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>A trace of an execution (R code, Python code, or a web service)</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Additional <bpt id="p1">[</bpt>troubleshooting topics<ept id="p1">](#trouble)</ept> are also covered.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Test your configuration</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Launch the diagnostic tests:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>On Machine Learning Server 9.3 (or any other machine that has access to Machine Learning Server), launch a command-line window or terminal  with administrator (Windows) or root/sudo (Linux) privileges and run this command.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>On earlier versions (9.0 - 9.2):</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](configure-admin-cli-launch.md)</ept> with administrator privileges (Windows) or root/sudo privileges (Linux).</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>From menus, choose <bpt id="p1">**</bpt>Run Diagnostic Tests<ept id="p1">**</ept>, then <bpt id="p2">**</bpt>Test configuration<ept id="p2">**</ept> for a 'health report' of the configuration including a code execution test.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If you have not authenticated yet, provide your username and password.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Review the test results.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If any issues arise, a raw report appears.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>You can also investigate the <bpt id="p1">[</bpt>log files<ept id="p1">](#logs)</ept> and attempt to resolve the issues.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>After making your corrections, <bpt id="p1">[</bpt>restart the component<ept id="p1">](configure-admin-cli-stop-start.md)</ept> in question.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>It may take a few minutes for a component to restart.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Rerun the diagnostic test to make sure all is running smoothly now.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>You can also get a health report directly using the <bpt id="p1">[</bpt>status<ept id="p1">](https://microsoft.github.io/deployr-api-docs/#get-status)</ept> API call.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Trace a code execution</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>To go through the execution of a specific line of code and retrieve request IDs for debugging purposes, run a trace.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Launch the code trace tests:</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>On Machine Learning Server 9.3, launch a command-line window or terminal  with administrator (Windows) or root/sudo (Linux) privileges and run one of these commands to trace the execution of a code block or script:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>On earlier versions (9.0 - 9.2):</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](configure-admin-cli-launch.md)</ept> with administrator privileges (Windows) or root/sudo privileges (Linux).</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>From menus, choose <bpt id="p1">**</bpt>Run Diagnostic Tests<ept id="p1">**</ept>, then either <bpt id="p2">**</bpt>Trace R code execution<ept id="p2">**</ept> or <bpt id="p3">**</bpt>Trace Python code execution<ept id="p3">**</ept> depending on the language you are using.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>When prompted, enter the code you want to trace.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>To start the trace, press the Enter key (carriage return).</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Review the trace output.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Trace a web service execution</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>To go through the execution of a specific web service and retrieve request IDs for debugging purposes, run a trace.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Launch the web service execution tests:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>On Machine Learning Server 9.3, launch a command-line window or terminal  with administrator (Windows) or root/sudo (Linux) privileges and run this command specifying the web service name and version:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>On earlier versions (9.0 - 9.2):</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Launch the administration utility<ept id="p1">](configure-admin-cli-launch.md)</ept> with administrator privileges (Windows) or root/sudo privileges (Linux).</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>From menus, choose <bpt id="p1">**</bpt>Run Diagnostic Tests<ept id="p1">**</ept>, then <bpt id="p2">**</bpt>Trace service execution<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>If you have not authenticated yet, you must provide your username and password.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Enter the service name and version after the syntax '<ph id="ph1">\&lt;</ph>service-name&gt;/<ph id="ph2">\&lt;</ph>version&gt;' such as <ph id="ph3">`my-service/1.1`</ph>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>To start the trace, press the Enter key (carriage return).</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Review the trace output to better understand how the execution is running or failing.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Log files and levels</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Review the log and configuration files for any component that was identified as experiencing issues.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>You can find the logs in the <bpt id="p1">**</bpt><ph id="ph1">\&lt;</ph>node-install-path&gt;\logs<ept id="p1">**</ept> folder under your web and compute node installation paths.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>(Locate the <bpt id="p1">[</bpt>install path<ept id="p1">](configure-find-admin-configuration-file.md)</ept> for your version.)</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If there are any issues, you must solve them before continuing.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>For extra help, consult or post questions to our <bpt id="p1">[</bpt>forum<ept id="p1">](https://social.msdn.microsoft.com/Forums/home?forum=microsoftr)</ept> or contact technical support.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>By default, the logging level is set to Warning so as not to slow performance.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>However, whenever you encounter an issue that you want to share with technical support or a forum, you can change the logging level to capture more information.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>The following logging levels are available:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Level</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Verbose</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>The most detailed comprehensive logging level of all activity, which is rarely (if ever) enabled in production environments</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Debug</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Logs robust details including internal system events, which are not necessarily observable</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Information</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Logs system events that correspond to its responsibilities and functions</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Warning</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Logs only when service is degraded, endangered, or may be behaving outside of its expected parameters.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>(Default level)</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Error</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Logs only errors (functionality is unavailable or expectations broken)</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Critical</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Logs only fatal events that crash the application</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>To update the logging level:</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>On each compute node AND each web node, open the configuration file, <ph id="ph1">\&lt;</ph>node-install-path&gt;/appsettings.json.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>(Find the <bpt id="p1">[</bpt>install path<ept id="p1">](configure-find-admin-configuration-file.md)</ept> for your version.)</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Search for the section starting with</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Set the logging level for <ph id="ph1">`"Default"`</ph>, which captures Machine Learning Server default events.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>For debugging support, use the 'Debug' level.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Set the logging level for <ph id="ph1">`"System"`</ph>, which captures Machine Learning Server .NET core events.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>For debugging support, use the 'Debug' level.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Use the same value as for <ph id="ph1">`"Default"`</ph>.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Save the file.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Restart<ept id="p1">](configure-admin-cli-stop-start.md)</ept> the node services.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Repeat these changes on every compute node and every web node.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Each node should have the same appsettings.json properties.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Repeat the same operation(s) that were running when the error(s) occurred.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Collect the <bpt id="p1">[</bpt>log files<ept id="p1">](#logs)</ept> from each node for debugging.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Trace user actions</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Using Information Level logging, any <bpt id="p1">[</bpt>Core API<ept id="p1">](concept-api.md#core-apis-for-operationalization)</ept> or <bpt id="p2">[</bpt>Service Consumption API<ept id="p2">](concept-api.md#service-consumption-apis)</ept> call can be logged.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Additionally, the <bpt id="p1">**</bpt>UserPrincipalName<ept id="p1">**</ept> of the responsible user is also recorded in the logs.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>The user session is given a unique ID called <bpt id="p1">**</bpt>LoginSessionId<ept id="p1">**</ept> on successful login, which is included in subsequent log entries detailing actions (<bpt id="p2">[</bpt>REST APIs<ept id="p2">](concept-api.md)</ept>) performed by the user during that session.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>LoginSessionId<ept id="p1">**</ept> allows a more fine-grained association of user actions to a particular user session.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>To enable information logging, update the <ph id="ph1">`"LogLevel"`</ph> for <ph id="ph2">`"Default"`</ph> to <ph id="ph3">`"Information"`</ph> on the web node, using the instructions provided <bpt id="p1">[</bpt>above<ept id="p1">](#loglevel)</ept>.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Now consider a user action flow in which a user logs in, creates a session, and deletes that session.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Corresponding log entries for these actions might look as follows:</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Correlating the above logs using <bpt id="p1">**</bpt>LoginSessionId<ept id="p1">**</ept> value, you can determine that the user "azureuser" logged in, created a session, and then deleted that session during the time period range from 2018-01-23 22:21 to 2018-01-23 22:28.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>We can also obtain other information like the machine IP address from which "azureuser" performed these actions (<bpt id="p1">**</bpt>RemoteIpAddress<ept id="p1">**</ept>) and whether the requests succeeded or failed (<bpt id="p2">**</bpt>StatusCode<ept id="p2">**</ept>).</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>In the second entry, notice that the Request and Response for each user action can be correlated using the <bpt id="p1">**</bpt>CorrelationId<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Troubleshooting</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>This section contains pointers to help you troubleshoot some problems that can occur.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>In addition to the info below, review the issues listed in the <bpt id="p1">**</bpt><bpt id="p2">[</bpt>Known Issues article<ept id="p2">](../resources-known-issues.md)</ept><ept id="p1">**</ept> as well.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>If this section does not help solve your issue, file a ticket with technical support or post in our <bpt id="p1">&lt;a href="https://social.msdn.microsoft.com/Forums/home?forum=microsoftr" target="_blank"&gt;</bpt>forum<ept id="p1">&lt;/a&gt;</ept>.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>"BackEndConfiguration is missing URI" Error</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>If you get an <ph id="ph1">`BackEndConfiguration is missing URIs`</ph> error when trying to install a web node, then ensure your compute nodes are installed and <bpt id="p1">[</bpt>declared<ept id="p1">](../install/operationalize-r-server-enterprise-config.md#webnode)</ept> prior to installing web nodes.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>“Cannot establish connection with the web node” Error</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>If you get the <ph id="ph1">`Cannot establish connection with the web node`</ph> error, then the client is unable to establish a connection with the web node in order to log in.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Perform the following steps:</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Verify that the web address and port number displayed on the main menu of the admin utility are correct.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Learn how to launch the utility, in this article: <bpt id="p1">[</bpt>Machine Learning Server Administration<ept id="p1">](configure-admin-cli-launch.md)</ept></source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Look for web node startup errors or notifications in the stdout/stderr/<bpt id="p1">[</bpt>logs files<ept id="p1">](#logs)</ept>.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Restart the web node if you have recently changed the port the server is bound to or the certificate used for HTTPS.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Learn how to restart, in this article: <bpt id="p1">[</bpt>Machine Learning Server Operationalization Administration<ept id="p1">](configure-admin-cli-stop-start.md)</ept></source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>If the issue persists, verify you can post to the login API using curl, fiddler, or something similar.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Then, share this information with technical support or post it in our <bpt id="p1">&lt;a href="https://social.msdn.microsoft.com/Forums/home?forum=microsoftr" target="_blank"&gt;</bpt>forum<ept id="p1">&lt;/a&gt;</ept>.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Long delays when consuming web service on Spark</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>If you encounter long delays when trying to consume a web service created with mrsdeploy functions in a Spark compute context, you may need to add some missing folders.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>The Spark application belongs to a user called 'rserve2' whenever it is invoked from a web service using mrsdeploy functions.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>To work around this issue, create these required folders for user 'rserve2' in local and hdfs:</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Next, create a new Spark compute context:</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>When 'reset = TRUE', all cached Spark Data Frames are freed and all existing Spark applications belonging to the current user are shut down.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Compute Node Failed / HTTP status 503 on APIs (9.0.1 - Linux Only)</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>If you get an <ph id="ph1">`HTTP status 503 (Service Unavailable)`</ph> response when using the Rest APIs or encounter a failure for the compute node during diagnostic testing, then one or more of the symlinks needed by <bpt id="p1">[</bpt>deployr-rserve<ept id="p1">](https://github.com/Microsoft/deployr-rserve)</ept> are missing.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>deployr-rserve is the R execution component for the compute node,</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Launch a command window with administrator privileges with root/sudo privileges.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Run a <bpt id="p1">[</bpt>diagnostic test<ept id="p1">](#test)</ept> of the system on the machine hosting the compute node.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>If the test reveals that the compute node test has failed, type <ph id="ph1">`pgrep -u rserve2`</ph> at a command prompt.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>If no process ID is returned, then the R execution component is not running and we need to check which symlinks are missing.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>At the command prompt, type <ph id="ph1">`tail -f /opt/deployr/9.0.1/rserve/R/log`</ph>.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>The symlinks are revealed.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Compare these symlinks to the symlinks listed in the <bpt id="p1">[</bpt>configuration<ept id="p1">](../install/operationalize-r-server-one-box-config.md)</ept> article.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Add a few symlinks using the commands in the <bpt id="p1">[</bpt>configuration<ept id="p1">](../install/operationalize-r-server-one-box-config.md)</ept> article.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Restart<ept id="p1">](configure-admin-cli-stop-start.md)</ept> the compute node services.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Run the <bpt id="p1">[</bpt>diagnostic test<ept id="p1">](#test)</ept> or try the APIs again.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Unauthorized / HTTP status 401</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>If you <bpt id="p1">[</bpt>configured Machine Learning Server to authenticate<ept id="p1">](configure-authentication.md)</ept> against LDAP/AD, and you experience connection issues or a <ph id="ph1">`401`</ph> error, verify the LDAP settings you declared in appsettings.json.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Use the ldp.exe tool to search the correct LDAP settings and compare them to what you have declared.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>You can also consult with any Active Directory experts in your organization to identify the correct parameters.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Configuration did not restore after upgrade</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>If you followed the upgrade instructions but your configuration did not persist, then put the backup of the appsettings.json file under the following directories and reinstall Machine Learning Server again:</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>On Windows: C:\Users\Default\AppData\Local\DeployR\current</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>On Linux: /etc/deployr/current</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Alphanumeric error message when consuming service</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>If you get an error similar to <ph id="ph1">`Message: b55088c4-e563-459a-8c41-dd2c625e891d`</ph> when consuming a web service, search <bpt id="p1">[</bpt>compute node's log file<ept id="p1">](#logs)</ept> for the alphanumeric error code to read the full error message.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Failed code execution with “ServiceBusyException” in the log</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>If a code execution fails and returns a <ph id="ph1">`ServiceBusyException`</ph> error in the Web node log file, then a proxy issue may be blocking the execution.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>The workaround is to:</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Open the R initialization file <ph id="ph1">\&lt;</ph>install folder&gt;\R_SERVER\etc\Rprofile.site.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Add the following code as a new line in Rprofile.site:</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Save the file and restart Machine Learning Server.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Repeat on every machine on which Machine Learning Server is installed.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Run the diagnostic test or code execution again.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Error: "Microsoft.AspNetCore.Server.Kestrel.Internal.Networking.UvException: Error -97 EAFNOSUPPORT address family not supported"</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Applies to: Machine Learning Server</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>If the following error occurs when attempting to start a web node <bpt id="p1">_</bpt>"Microsoft.AspNetCore.Server.Kestrel.Internal.Networking.UvException: Error -97 EAFNOSUPPORT address family not supported"<ept id="p1">_</ept>, then disable IPv6 on your operating system.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>az: error: argument command_package: invalid choice: ml</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Applies to: Machine Learning Server 9.3</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>If for some reason your <ph id="ph1">`azure-ml-admin-cli`</ph> extension is not available or has been removed you will be met with the following error:</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>If you encounter this error, you can re-add the extension as such:</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Windows:</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Linux:</source>
        </trans-unit></group></body></file></xliff>