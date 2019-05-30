<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-admin-managing-server-policies.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e1c4c0a54c874e205f62d1be625219fecda4a21dc.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1c4c0a54c874e205f62d1be625219fecda4a21dc</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-admin-managing-server-policies.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>DeployR Administration Console Help - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Managing Server Policies in the DeployR Administration Console</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Managing Server Policies</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Server Policies<ept id="p1">**</ept> tab contains the policies governing the DeployR server, including:</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Global settings such as name, default server boundary, and console timeout</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Project persistence policies governing resource usage (sizes and autosave)</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Runtime policies governing authenticated, asynchronous, and anonymous operations</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Runtime policies governing concurrent operation limits, file upload limits, and event stream access</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Figure: Server Policies tab</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Server Policy Properties</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>There are a number of settings that can be defined for each server.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>They are grouped into the following categories:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Basic settings</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Authenticated Operation Policies</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Asynchronous Operation Policies</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Anonymous Operation Policies</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Project Persistence Policies</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Concurrent Operation Policies</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Event Stream Access Policies</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Server Runtime Policies</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Basic Settings</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Properties</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Descriptive name for the server that is used in the R script developer summary page to identify this server instance.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>This is the base URL representing the IP address and Servlet Web application context for the live DeployR server.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The base URL for the Servlet Web application context defaults to<ph id="ph1"> `/deployr`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>By default, the server tries to automatically detect the machine’s IP address each time the server machine is rebooted.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>This IP address is then used to construct the URL displayed in this field.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>You can disable this function using the setting below this one on this page.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If the administrator wants to change the Web application context for the server, then they must update the Web application context component of this URL accordingly.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Use a valid IP address and port number, and follow the format:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>, where the default port is <ph id="ph1">`8000`</ph> or <ph id="ph2">`8500`</ph> depending on your version</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>or (<bpt id="p1">[</bpt>if HTTPS is enabled<ept id="p1">](../operationalize/configure-https.md)</ept>)</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>, where the default port is <ph id="ph1">`8001`</ph> or <ph id="ph2">`8501`</ph> depending on your version</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>In some cases, the auto-detection process may return an IP address that is not the one that the administrator intended for DeployR.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>For example, if the server host machine is configured to support multiple IP addresses, then there is a chance that the wrong address is auto-detected.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>In another case, when DeployR is installed on an <bpt id="p1">[</bpt>Azure or AWS EC2<ept id="p1">](deployr-admin-install-in-cloud.md)</ept> instance, then the internal IP might be detected rather that the external IP.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>And, in another example, the IP address that once worked may no longer be the right number.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>  There may also be times when the lease on a dynamically-allocated IP address expires, thereby causing the host machine to acquire a new IP address while the server is live.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>To remedy these cases, the administrator can override the IP that was auto-detected by replacing the IP number in the URL listed in this field with the desired IP address.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>This fix will work until the next time the server machine is restarted.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>After booting, the IP auto-detection process is run again and the IP number in theServer Web context URL is refreshed.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Important:<ept id="p1">**</ept> There may be times where you cannot reach the Administration Console due to this issue.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>In that case, you must update this value and disable autodetection<ept id="p1">](deployr-admin-diagnostics-troubleshooting.md#set-context)</ept>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>To impose an IP address, enter the correct IP address in the<bpt id="p1"> **</bpt>Server Web context<ept id="p1">**</ept><ph id="ph1"> </ph>field and then set<bpt id="p2"> **</bpt>Disable IP auto-detection<ept id="p2">**</ept><ph id="ph2"> </ph>to<ph id="ph3"> `True`</ph>.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If you set this option to True by selecting the checkbox, you will turn off the auto-detection process and the IP number listed in the<bpt id="p1"> **</bpt>Server Web context<ept id="p1">**</ept><ph id="ph1"> </ph>URL will persist across server reboots.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If set to False (no check), then auto-detection is enabled and the server machine will try to automatically detect and refresh the machine’s IP address each time the server machine is rebooted.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>This IP address is then used to create the URL displayed in<bpt id="p1"> **</bpt>Server Web context<ept id="p1">**</ept><ph id="ph1"> </ph>field.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Name of an R boundary to be applied as the system-wide default.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Grid node boundaries take precedence over boundaries associated with users.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Likewise, grid node R boundaries and user R boundaries take precedence over this default R boundary.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If no other boundary is specified, then the default system-wide boundary is applied.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The length of idle time in seconds before a session in the Administration Console expires.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Authenticated Operation Policies</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>These policies govern how<bpt id="p1"> [</bpt>authenticated operations<ept id="p1">](deployr-admin-managing-the-grid.md#node-operation-types)</ept><ph id="ph1"> </ph>are handled.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Authenticated operations refer to operations on projects requested by authenticated users.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>These operations are executed on grid nodes designated for either authenticated or mixed operation modes.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Properties</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>(Applies to DeployR 8.0.0 or older only)</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>By default this option is unchecked, which sets it to False, where incoming calls on the API can be made over a plain HTTP connection.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>If set to True, the server only accepts incoming API calls over an encrypted channel (HTTPS).</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Learn more about <bpt id="p1">[</bpt>DeployR Server Support for SSL/TLS (HTTPS)<ept id="p1">](../operationalize/configure-https.md)</ept>.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Note:<ept id="p1">**</ept> If you enable HTTPS for one or more operations types, you must also provide a valid HTTPS URL in the Server web context property on this page.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The name of the filter to be applied to all authenticated operations.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>If defined, then only authenticated users who connect from a qualified IP address (as defined by the filter) can make calls on the API.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The<bpt id="p1"> [</bpt>IP filtering<ept id="p1">](deployr-admin-managing-access-with-ip-filters.md)</ept><ph id="ph1"> </ph>restrictions specified on a server context determine the full publicly accessible exposure of that server context.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The length of time in seconds that an authenticated user can remain idle while connected to the server before the HTTP session is automatically timed-out and disconnected.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Asynchronous Operation Policies</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>These policies govern how<bpt id="p1"> [</bpt>asynchronous operations<ept id="p1">](deployr-admin-managing-the-grid.md#node-operation-types)</ept><ph id="ph1"> </ph>are handled.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Asynchronous operations are scheduled jobs executing in the background on behalf of authenticated users.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>These jobs are executed on grid nodes designated for either asynchronous or mixedoperation modes.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Properties</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>(Applies to DeployR 8.0.0 or older only)</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>By default this option is unchecked, which sets it to False, where calls on the API can be made over a plain HTTP connection.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>If set to true, the server will only accept API calls over an encrypted channel (HTTPS).</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Learn more about <bpt id="p1">[</bpt>DeployR Server Support for SSL/TLS (HTTPS)<ept id="p1">](../operationalize/configure-https.md)</ept>.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Note:<ept id="p1">**</ept> If you enable HTTPS for one or more operations types, you must also provide a valid HTTPS URL in the Server web context property on this page.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The filter to be applied to all authenticated operations.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>If defined, then only jobs from authenticated users who connect from a qualified IP address can make calls on the API.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>The<bpt id="p1"> [</bpt>IP filtering<ept id="p1">](deployr-admin-managing-access-with-ip-filters.md)</ept><ph id="ph1"> </ph>restrictions specified on a server context determine the full publicly accessible exposure of that server context.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Anonymous Operation Policies</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>These policies govern how<bpt id="p1"> [</bpt>anonymous operations<ept id="p1">](deployr-admin-managing-the-grid.md#node-operation-types)</ept><ph id="ph1"> </ph>are handled.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Anonymous operations are executed on grid nodes designated for either anonymous or mixed operation modes.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Anonymous operations refer to operations from users executing scripts anonymously.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Properties</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>(Applies to DeployR 8.0.0 or older only)</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>By default this option is unchecked, which sets it to False, where scripts can be executed over a plain HTTP connection.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>If set to true, the server only accepts script execution requests over an encrypted channel (HTTPS).</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Learn more about <bpt id="p1">[</bpt>DeployR Server Support for SSL/TLS (HTTPS)<ept id="p1">](../operationalize/configure-https.md)</ept>.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Note:<ept id="p1">**</ept><ph id="ph1"> </ph>If you enable HTTPS for one or more operations types, you must also provide a valid HTTPS URL in the Server web context property on this page.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>The name of the filter to be applied to all anonymous operations.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>If selected, then only anonymous users who connect from a qualified IP address (as defined by the filter) can execute R scripts on the API.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>The<bpt id="p1"> [</bpt>IP filtering<ept id="p1">](deployr-admin-managing-access-with-ip-filters.md)</ept><ph id="ph1"> </ph>restrictions specified on a server context determine the full publicly accessible exposure of that server context.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>The length of time in seconds an anonymous operation remains live on the grid before it is automatically terminated.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>The automatic termination will release all resources associated with that operation.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Project Persistence Policies</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>These policies govern certain project behaviors and limits.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Properties</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>The maximum storage size in bytes for snapshots of PNG and SVG plots generated by the R graphics device associated with a project over its lifespan.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Note:<ept id="p1">**</ept> This setting does not impact the size of a project’s working directory.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>The maximum depth of the execution command history retained for each project.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>When the limit is reached, each new execution will flush the oldest one from the history.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>When an execution is flushed from the history, all associated plots and R console output are permanently deleted.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>By default, this is unchecked, which sets the value to<ph id="ph1"> `False`</ph>, where temporary projects are not auto-saved when a project is closed or when a user logs out or times out on their connection.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>When<ph id="ph1"> `True`</ph>, temporary projects become candidates for auto-saving.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Whether projects are auto-saved on close, logout, or timeout depends on the value of the<ph id="ph1"> `autosave` </ph>flag set when a user logs in on the API.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>For more information on autosaving, see the<bpt id="p1"> [</bpt>API Reference Guide<ept id="p1">](deployr-api-reference.md)</ept>.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Concurrent Operation Policies</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>These policies govern the runtime grid usage limits on the number of concurrent operations that can be run simultaneously in the system by a given user.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Since these policies are disabled by default, no limits are enforced.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>This default behavior means that each user can take as many slots as desired on the grid framework until there are no more available slots.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>We typically recommend that these settings remain disabled if the DeployR server is being used:</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>By a single individual</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>To service a specific client application, which is common, for example, when an RBroker pool is in use</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>While leaving them disabled is typically recommended, enabling the policies can be quite useful in controlling slot usage on a per-user (operation type) basis.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Properties</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>When enabled/checked, the policies are in effect and enforced.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>If disabled/unchecked, the limits are ignored.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>This value limits the number of live projects that a given authenticated user can run simultaneously on the grid.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Whenever the number of live projects reaches this limit, all further requests to work on new projects are rejected on the API until one or more existing live projects are closed.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>This value limits the number of scheduled jobs that a given authenticated user can run simultaneously on the grid.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Whenever the number of scheduled jobs awaiting execution exceeds this limit for a given user, every pending job for that user remains queued until one or more of the currently running jobs complete.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>The value specified here limits the number of concurrent R scripts that an anonymous user at a given HTTP address can run simultaneously on the grid.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Where the number of executing R scripts reaches this limit all further requests by the user to execute R scripts will be rejected on the API until one or more of the existing R script executions complete.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Event Stream Access Policies</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>These settings limit access to the event streams.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>There are three distinct event streams pushed by DeployR.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>The authenticated event stream allows authenticated users to see their own server-wide or HTTP-session specific execution and job lifecycle events.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>By default, this stream is accessible to all authenticated users.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Access to this stream can be restricted using a role-based access control defined here.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>The anonymous event stream allows anonymous users to see execution events within their current HTTP session.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Access to this event stream can be disabled in the<bpt id="p1"> **</bpt>Server Policies<ept id="p1">**</ept><ph id="ph1"> </ph>tab.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>The management event stream allows authenticated users to see server runtime events, including grid activity and security access events.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>By default this stream is accessible to<ph id="ph1"> `admin` </ph>only.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source> Access to this stream can be restricted using a role-based access control specified here.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Properties</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Only those authenticated users assigned to the role defined for this property have permission to view their event stream.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>By default, all authenticated users can access the authenticated event stream.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>For example, the administrator might restrict access only to those users assigned the<ph id="ph1"> `POWER_USER` </ph>role.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>When selected, the anonymous event stream is off.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>  When this checkbox is unselected, the anonymous stream pushes events to anonymous users.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Only those authenticated users assigned to the role defined here can access the management event stream.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>By default, only<ph id="ph1"> `admin` </ph>can access this stream.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Server Runtime Policies</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Properties</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>This setting specifies the largest file size that can be uploaded to the server.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>This includes file uploads to both projects and the repository.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Tip:<ept id="p1">**</ept> Use the DeployR external data directories to store larger files to avoid the limitations set here.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>When enabled/true, the URLs returned in the API response markup are relative URLs.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>By default or when disabled, the URLs returned in the response markup are absolute URLs.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Specifies the server logging level.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Options are:<bpt id="p1"> **</bpt>WARN<ept id="p1">**</ept>,<bpt id="p2"> **</bpt>INFO<ept id="p2">**</ept>, and<bpt id="p3"> **</bpt>DEBUG<ept id="p3">**</ept>.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>If you change this setting, the new level will take effect immediately.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Any changes you make here persist until the server is restarted.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>After the server is restarted, the log level reverts to the default log level specified in the external configuration file, <ph id="ph1">`deployr.groovy`</ph>.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Viewing and Editing Server Policies</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>To view and edit server-wide settings:</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>Server Policies<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>From the <bpt id="p1">**</bpt>Server Policies<ept id="p1">**</ept> page, review the settings currently in place.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>To edit one or more defaults:</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Edit<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Edit Server Policies<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Make any changes.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Update<ept id="p1">**</ept> to save the changes.</source>
        </trans-unit></group></body></file></xliff>