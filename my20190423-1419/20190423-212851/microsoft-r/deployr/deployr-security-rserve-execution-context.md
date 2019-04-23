<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-security-rserve-execution-context.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a68847c73a46782d791b2e94b3461543722c69c3c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">68847c73a46782d791b2e94b3461543722c69c3c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-security-rserve-execution-context.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Security - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Security in DeployR: Authentication, HTTPS, SSL, and access controls for server, Project file and Repository File, and more.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>RServe Execution Context</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>As per the standard usage of R, the current user starts the R executable and interacts with the application via the R Language and the R Interpreter.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The R language provides OS-level access via the <ph id="ph1">`system`</ph> function.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>With this function, a user can execute an OS command such as <ph id="ph1">`system(“rmdir –r C:\\tmp”)`</ph>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>While this is useful functionality for individual users, <bpt id="p1">**</bpt>it is also a potential entry point through which the computer's security could be compromised.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>DeployR provides various <bpt id="p1">[</bpt>API calls<ept id="p1">](deployr-api-reference.md)</ept> that permit the execution of R scripts and R code.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The R scripts stored on the DeployR server can have different <bpt id="p1">[</bpt>levels of permissions<ept id="p1">](deployr-repository-manager-files.md#about-file-properties)</ept> dictating what a client can do.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>While public scripts can be executed by either anonymous or authenticated clients, private scripts can only be executed by the authenticated user that created the script.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Raw R code execution, via the DeployR API, can only be executed by an authenticated user that has the <bpt id="p1">[</bpt><ph id="ph1">`POWER_USER`</ph> role<ept id="p1">](deployr-admin-console-permissions-with-roles.md)</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>All authentication takes place on the DeployR server, and the execution of the R code is managed through the DeployR RServe add-on component.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Rserve provides a TCP/IP interface to the R Interpreter running on the machine.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>By default, Rserve runs on the same machine as the DeployR Server.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>RServe is started by Windows Service (RServeWinService) that runs under a virtual service account.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>RServe inherits the permissions of that virtual service account.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>In the default configuration, Rserve will only accept socket connections from <ph id="ph1">`localhost`</ph>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>In other words, only those processes running on the same machine where RServe is running can directly connect to it and execute R code.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The DeployR Server should, ideally, be the only local process that connects to RServe.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>To help ensure this is the case, a username and password is required to validate any connection between RServe and a client process.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>However, there exist several vulnerabilities of which you should be aware.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>They are:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>RServe only accepts usernames and passwords in plain text from connecting clients.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>RServe uses a plain text configuration file to store the username and password.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>RServe has the permissions of the virtual service account, so it may have unwanted access to resources on the computer.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If a DeployR instance requires additional compute capacity, <bpt id="p1">[</bpt>a network of grid nodes<ept id="p1">](deployr-admin-managing-the-grid.md)</ept> can be added to provide sophisticated load-balancing capabilities.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>A grid node is simply a DeployR server with R installed and the RServe component installed and configured to accept connections from remote clients.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Whenever remote grid nodes exist, a firewall should also be configured to accept only connections from the DeployR Server IP address.</source>
        </trans-unit></group></body></file></xliff>