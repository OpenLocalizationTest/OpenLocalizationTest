<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-admin-diagnostics-troubleshooting.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a38ac972e7a7da34c2fe0304ffcd7cc0032f68d93.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">38ac972e7a7da34c2fe0304ffcd7cc0032f68d93</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-admin-diagnostics-troubleshooting.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Diagnostics &amp; Troubleshooting - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Diagnostic Testing and Troubleshooting FAQS for DeployR</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Diagnostics &amp; Troubleshooting</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Introduction</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This document describes how to run and interpret the DeployR diagnostic test.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Additionally, this document offers solutions to issues that you might be <bpt id="p1">[</bpt>troubleshooting<ept id="p1">](#troubleshooting)</ept> after installing or during your use of DeployR.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Diagnostic Testing</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>You can assess the state and health of your DeployR environment by running the diagnostic test described in this document.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The diagnostic script:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Outputs basic details about your environment</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Identifies unresponsive components, such as the server, grid nodes, or the database</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Gathers all relevant <bpt id="p1">[</bpt>log and configuration files<ept id="p1">](#inspecting-diagnostic-log-files)</ept></source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Armed with this information, you will be able to investigate and resolve most issues.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>And, in the event that you need additional support, you can send the diagnostics tar/zip file to the Microsoft Corporation technical support team.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Behind the scenes, the script evaluates the system and creates the <ph id="ph1">`logs`</ph> subdirectory to store:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The resulting log file (<ph id="ph1">`diagnostics.log`</ph>), which provides details, including the state of all components, plus pertinent configuration and environment information.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Copies of each <bpt id="p1">[</bpt>log and configuration file<ept id="p1">](#inspecting-diagnostic-log-files)</ept></source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The results are also printed to the screen.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Running the Diagnostic Check</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The easiest way to run diagnostics is to launch it from the <bpt id="p1">**</bpt>Diagnostics<ept id="p1">**</ept> tab on the DeployR landing page.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>After installing, you can log into the DeployR landing page at <ph id="ph1">`https://&lt;DEPLOYR_SERVER_IP&gt;:&lt;PORT&gt;/deployr/landing`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>is the IP address of the DeployR main server machine.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If you do not have a username or password, please contact your administrator.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>However, if you cannot reach the landing page, the <ph id="ph1">`admin`</ph> can log into the server and manually run it using the following commands:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>For DeployR for Microsoft R Server 8.0.5</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On Windows<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Launch the DeployR administrator utility script with administrator privileges:</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>From the main menu, run the DeployR diagnostic tests.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If there are any issues, you must solve them before continuing.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Consult the Troubleshooting section of this document for additional help or post questions to our <bpt id="p1">&lt;a href="https://social.msdn.microsoft.com/Forums/en-US/home?forum=microsoftr" target="_blank"&gt;</bpt>forum<ept id="p1">&lt;/a&gt;</ept>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>All output from the diagnostic test are stored in <ph id="ph1">`C:\Program Files\Microsoft\DeployR-&lt;VERSION&gt;\deployr\tmp\logs\diagnostics.zip`</ph>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On Linux<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Launch the DeployR administrator utility script as <ph id="ph1">`root`</ph> or a user with <ph id="ph2">`sudo`</ph> permissions:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>From the main menu, run the DeployR diagnostic tests.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>If there are any issues, you must solve them before continuing.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Consult the Troubleshooting section of this document for additional help or post questions to our <bpt id="p1">&lt;a href="https://social.msdn.microsoft.com/Forums/en-US/home?forum=microsoftr" target="_blank"&gt;</bpt>forum<ept id="p1">&lt;/a&gt;</ept>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>All output from the diagnostic test are stored into <ph id="ph1">`$DEPLOYR_HOME/deployr/tmp/logs/diagnostics.zip`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>For DeployR 8.0.0</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On Windows<ept id="p1">**</ept>: Run the following commands.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>All output from the diagnostic test is stored in <ph id="ph1">`C:\Program Files\Microsoft\DeployR-&lt;VERSION&gt;\deployr\logs\diagnostics.zip`</ph>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>If the server log, <ph id="ph1">`catalina.[YYYY-MM-DD].log`</ph>, contains information you do not wish to share with technical support, you can exclude that file.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>To do so, add <ph id="ph1">`--exclude-server-log`</ph>, such as:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On Linux / OS X<ept id="p1">**</ept>: Run the following commands.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>All output from the diagnostic test is stored in the <ph id="ph1">`$DEPLOYR_HOME/deployr/logs/diagnostics.tar.gz`</ph>.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If the server log, <ph id="ph1">`catalina.out`</ph>, contains information you do not wish to share with technical support, you can exclude that file.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>To do so, add <ph id="ph1">`--exclude-server-log`</ph>, such as:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Inspecting Diagnostic Log Files</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>A copy of the following log and configuration files is bundled together during the diagnostic check.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Review the log and configuration files for any component that was identified as experiencing issues.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>For Windows</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The following log files can be found in the resulting <ph id="ph1">`diagnostics.zip`</ph> file as well as under <ph id="ph2">`C:\Program Files\Microsoft\DeployR-&lt;VERSION&gt;\deployr\tmp\logs`</ph> directly on the DeployR host.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Component</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Log<ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;</ph><ph id="ph3">&amp;nbsp;</ph>Configuration<ph id="ph4">&amp;nbsp;</ph>Files</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Diagnostic Results</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>The DeployR diagnostic log provides details, including the state of all components, plus pertinent configuration and environment information.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>DeployR</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>is the DeployR external configuration file.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Tomcat's <ph id="ph1">`catalina.out`</ph> serves as the main <bpt id="p1">[</bpt>DeployR log<ept id="p1">](deployr-common-administration-tasks.md#inspecting-server-logs)</ept>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more<ept id="p1">](deployr-common-administration-tasks.md#inspecting-server-logs)</ept> about this file.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Tomcat</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The log and configuration files for Tomcat.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>MongoDB</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>(DeployR 8.0.0 only)</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The log and configuration files for the database used by DeployR.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The IP address is added to the filename for your convenience.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>DeployR RServe</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>The configuration file for the DeployR RServe component.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>The IP address is added to the filename for your convenience.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>DeployR Enterprise Only<ept id="p1">**</ept>: The RServe files for remote grid nodes are not bundled.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>If you suspect an issue on a node, please log onto that machine to retrieve its RServe log file.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>For Linux / OS X</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The following log files can be found under <ph id="ph1">`$DEPLOYR_HOME/deployr/tmp/logs`</ph> directly on the DeployR host.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Component</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Log<ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;</ph><ph id="ph3">&amp;nbsp;</ph>Configuration<ph id="ph4">&amp;nbsp;</ph>Files</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Diagnostic Results</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>The DeployR diagnostic log provides details, including the state of all components, plus pertinent configuration and environment information.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>DeployR</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>is the DeployR external configuration file.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Tomcat's <ph id="ph1">`catalina.out`</ph> serves as the main <bpt id="p1">[</bpt>DeployR log<ept id="p1">](deployr-common-administration-tasks.md#inspecting-server-logs)</ept>.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more<ept id="p1">](deployr-common-administration-tasks.md#inspecting-server-logs)</ept> about this file.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Tomcat</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>The log and configuration files for Tomcat.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>MongoDB</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>(DeployR 8.0.0 only)</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The log and configuration files for the database used by DeployR.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>The IP address of the host of the MongoDB database is added to the filename for your convenience.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>DeployR RServe</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>The log and configuration files for RServe.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>DeployR Enterprise Only<ept id="p1">**</ept>: The RServe files for remote grid nodes are not bundled.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>If you suspect an issue on a node, please log onto that machine to retrieve its RServe log file.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Resolving Issues</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Use the following instructions if you have <bpt id="p1">[</bpt>run the diagnostic test<ept id="p1">](#running-the-diagnostic-check)</ept> and a problem was indicated.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>To resolve component issues:</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Look through the <bpt id="p1">[</bpt>log and configuration files<ept id="p1">](#inspecting-diagnostic-log-files)</ept> for each component that was identified in the diagnostic report.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>If the log file indicates an error, then fix it.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>If Server Web Context points to the wrong IP, <bpt id="p1">[</bpt>update it now<ept id="p1">](#set-context)</ept>.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>After making your corrections, <bpt id="p1">[</bpt>restart the component<ept id="p1">](deployr-common-administration-tasks.md#startstop)</ept> in question.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>It may take a few minutes for a component to restart.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Re-run the diagnostic test<ept id="p1">](#running-the-diagnostic-check)</ept> again to make sure all is running smoothly now.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>If problem persists:</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>After trying the first time, repeat steps 1-4.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Review the other <bpt id="p1">[</bpt>Troubleshooting<ept id="p1">](#troubleshooting)</ept> topics.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Post your questions to our <bpt id="p1">[</bpt>DeployR Forum<ept id="p1">](https://social.msdn.microsoft.com/Forums/en-US/home?forum=microsoftr)</ept>.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>After the second time, send the diagnostics tar/zip file to the Microsoft Corporation technical support team.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Troubleshooting</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>This section contains pointers to help you troubleshoot some problems that can occur with DeployR.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Windows Installation Errors</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>DeployR RServe Package Download Failed</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>During the installation of DeployR on Windows, if you get the error <ph id="ph1">`DeployR RServe package download failed`</ph>, this may be due to several potential issues, including:</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Unavailable or poor network connectivity</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>The package zip could not be found in GitHub</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Download is disabled on machine for reasons such as corporate policy</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>If this should occur, do the following:</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Check your connectivity and firewall rules, and click <bpt id="p1">**</bpt>Try Again<ept id="p1">**</ept> in the DeployR setup installer.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>If this does not fix the issue, then manually install the supported DeployR Rserve package as follows: <bpt id="p1">&lt;a name="manual-package-install"&gt;</bpt><ept id="p1">&lt;/a&gt;</ept></source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Download zip from <ph id="ph1">https://github.com/deployr/deployr-rserve/releases/download/v8.0.5/deployrRserve_8.0.5.zip</ph></source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Open a Command Window with <bpt id="p1">**</bpt>“Run as Administrator”<ept id="p1">**</ept> and run the following:</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Confirm the package was installed by verifying that <ph id="ph1">`C:\Program Files\Microsoft SQL Server\130\R_SERVER\library\deployrRserve\Rserve.exe`</ph> is present.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Try Again<ept id="p1">**</ept> in installer or re-run the installer.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>DeployR RServe Package Installation Failed</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>During the installation of DeployR on Windows, if you get the error <ph id="ph1">`DeployR RServe package installation failed`</ph>, this may be due to several potential issues, including:</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>The package could not be installed in the correct location due to insufficient privileges.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>The package download was corrupted or interrupted.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Manually install DeployR RServe package as <bpt id="p1">[</bpt>described here<ept id="p1">](#manual-package-install)</ept>.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Could Not Stop the Service Apache-Tomcat-for-DeployR-<ph id="ph1">&amp;lt;</ph>version<ph id="ph2">&amp;gt;</ph></source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>During the installation of DeployR on Windows, you may get the error <ph id="ph1">`Could not stop the service Apache-Tomcat-for-DeployR-&lt;version&gt;`</ph> if Windows could not stop the service completely.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>If this should occur, do the following:</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Open a Command Window with <bpt id="p1">**</bpt>“Run as Administrator”<ept id="p1">**</ept> and run the following:</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>where <ph id="ph1">&amp;lt;</ph>version<ph id="ph2">&amp;gt;</ph> is the package version number such as, Apache-Tomcat-for-DeployR-8.0.5.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>If the installer is still open, click <bpt id="p1">**</bpt>Try Again<ept id="p1">**</ept> in installer.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>If the installer was canceled, try to install again.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>If the error persists, reboot the Windows machine on which you are installing and launch the installer again.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Could Not Stop the Service RServe<ph id="ph1">&amp;lt;</ph>version<ph id="ph2">&amp;gt;</ph></source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>During the installation of DeployR on Windows, the error <ph id="ph1">`Could not stop the service RServe&lt;version&gt;`</ph> can appear if Windows could not stop the service completely.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>If this should occur, do the following:</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Open a Command Window with <bpt id="p1">**</bpt>“Run as Administrator”<ept id="p1">**</ept> and run the following:</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>where <ph id="ph1">&amp;lt;</ph>version<ph id="ph2">&amp;gt;</ph> is the package version number such as, RServe8.0.5.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>If the installer is still open, click ‘Try Again’ in installer.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>If the installer was canceled, try to install again.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>If the error persists, reboot the Windows machine on which you are installing and launch the installer again.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Other Errors During Installation</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>If you should encounter any other errors while running the DeployR Windows installer, we recommend that you:</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Contact Microsoft support (DeployR Enterprise users only)</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Provide the installation logs <ph id="ph1">`DeployR-*.log`</ph> found in the <ph id="ph2">`%temp%`</ph> directory.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Landing Page Cannot Be Reached</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>If you cannot access the DeployR landing page or if the landing page looks disabled and you can't log in, we recommend that you first verify that the server is, in fact, running using <bpt id="p1">[</bpt>this diagnostic test<ept id="p1">](#running-the-diagnostic-check)</ept>.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>If the diagnostic logs reveal nothing and the DeployR landing page still isn't loading properly, then it is likely that the IP address in the Server Web Context is incorrectly defined.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>For more on the Server Web Context, refer to the <bpt id="p1">[</bpt>Administration Console Help<ept id="p1">](deployr-admin-managing-server-policies.md#basic-settings)</ept>.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Landing Page Inaccessible</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>This problem can arise for various reasons, including:</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>When an internal IP address was automatically assigned instead of an external address.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>This is most common with Azure or an Amazon Web Services (AWS) EC2 instances, but can occur with other configurations.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>When the underlying IP address of your DeployR server has changed.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>This is most common when you have installed the DeployR server on a portable laptop and have since changed networks (for example, between your office and your home).</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>It can be solved by updating the IP address in the DeployR Server Web Context.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>DeployR for Microsoft R Server 8.0.5: Update DeployR Web Context</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>To fix this issue, update the IP address in the DeployR Server Web Context as follows:</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Launch the DeployR administrator utility script with administrator privileges:</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>On Windows, run:</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>On Linux, run:</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>From the main menu, choose option <bpt id="p1">**</bpt>Run Diagnostics<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Make sure that the database is running.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>The database must be running before you can proceed to the next step.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>Return to the main menu, choose option <bpt id="p1">**</bpt>Web Context and Security<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>From the sub-menu, choose option <bpt id="p1">**</bpt>Specify New IP or Fully Qualified Domain Name (FQDN)<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>When prompted to specify a new IP or FQDN, enter the new IP or FQDN.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>When prompted to confirm the new value, enter <ph id="ph1">`Y`</ph>.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>This change will also disable Automatic IP detection to prevent the new value you just assigned from being overwritten.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>Return to the main menu and choose option <bpt id="p1">**</bpt>Start/Stop Server<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>You must restart DeployR so that the changes can take effect.</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>When prompted whether you want to stop (S) or restart (R) the DeployR server, enter <ph id="ph1">`R`</ph>.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>It may take some time for the Tomcat process to terminate and restart.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>Exit the utility.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>DeployR 8.0.0: Update DeployR Web Context</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>Run the <ph id="ph1">`setWebContext`</ph> script to update the IP address in the DeployR Server Web Context.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>Usage tips for the <ph id="ph1">`setWebContext`</ph> script arguments:</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>To see which IP is currently defined as the Server Web Context.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>To  specify a new IP address or DNS name for the DeployR Server Web Context.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>To turn off the automatic IP detection.</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>You can <bpt id="p1">[</bpt>turn this back on<ept id="p1">](deployr-admin-managing-server-policies.md#basic-settings)</ept> in the Administration Console.</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>To detect the external IP used for your AWS EC2 instance.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>From there you can choose to use that IP as the DeployR Server Web Context.</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>or</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>To enable or disable HTTPS in the server policies, including the Server Web Context.</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>This change requires other changes to complete SSL/HTTPS process as described in <bpt id="p1">[</bpt>these instructions<ept id="p1">](../operationalize/configure-https.md)</ept>.</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>On Windows:</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>Make sure that the MongoDB database is running.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>The database must be running before you can proceed to the next step before you update the Web Context.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>Open a Command Window with <bpt id="p1">**</bpt>“Run as Administrator”<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>Set the appropriate public IP where <ph id="ph1">`&lt;ip_address&gt;`</ph> is the public IP address of the machine.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>Confirm the IP address you entered.</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>Disable any automatic IP detection that might overwrite the IP you just assigned.</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>On Linux:</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>Set the IP using the <ph id="ph1">`setWebContext.sh`</ph> script where <ph id="ph2">`&lt;ip_address&gt;`</ph> is the public IP address of the machine.</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>Confirm the IP address you entered.</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>Disable any automatic IP detection that might overwrite the IP you just assigned.</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>For this change to take effect, <bpt id="p1">[</bpt>restart the DeployR 8.0.0 service<ept id="p1">](deployr-common-administration-tasks.md#startstop)</ept>.</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>Between stopping and starting, be sure to pause long enough for the Tomcat process to terminate.</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>If this doesn't resolve the issue and you have Internet Explorer 11 on Windows, <bpt id="p1">[</bpt>try this<ept id="p1">](#landing-page-blocked-in-i-e-11)</ept>.</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>Landing Page Blocked in Internet Explorer 11 (Windows Only)</source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>If you are attempting to access the DeployR landing page using <ph id="ph1">`https://localhost:&lt;PORT&gt;/deployr/landing`</ph> in Internet Explorer (I.E.) 11 and the <bpt id="p1">[</bpt>diagnostic tests<ept id="p1">](#diagnostic-testing)</ept> have turned up nothing, you may find that the landing page is blocked.</source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>This may be due to some default settings in I.E.</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source>11.</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>To solve this issue:</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>In Internet Explorer 11, go to the <bpt id="p1">**</bpt>Security<ept id="p1">**</ept> tab in the <bpt id="p2">**</bpt>Internet Options<ept id="p2">**</ept> dialog box.</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>Add <ph id="ph1">`http://localhost:&lt;PORT&gt;/deployr`</ph> to the <bpt id="p1">**</bpt>Trusted Sites<ept id="p1">**</ept> list.</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Connections<ept id="p1">**</ept> tab in the same <bpt id="p2">**</bpt>Internet Options<ept id="p2">**</ept> dialog box, click <bpt id="p3">**</bpt>LAN settings<ept id="p3">**</ept>.</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>Deselect the <bpt id="p1">**</bpt>Automatically detect settings<ept id="p1">**</ept> checkbox to enable custom entries in the HOSTS file.</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept> to apply the changes.</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source>Cannot Access DeployR (Windows Only)</source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>During the installation of DeployR on Windows, the 'Domain' profile is used to create inbound exceptions for the ports used by DeployR.</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source>These settings may need to be adjusted after installing to meet the needs of your deployment.</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>Multiple User Sign-ins</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source>You cannot log into DeployR from two different accounts within the same brand of browser program.</source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source>To use two or more different accounts, you'll need to log into each one in a separate brand of browser.</source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source>Issues After Reinstalling Microsoft R or R</source>
        </trans-unit><trans-unit id="324" translate="yes" xml:space="preserve">
          <source>If you want to upgrade or reinstall R, Microsoft R Server, or Revolution R Open or need help troubleshooting, then follow <bpt id="p1">[</bpt>these instructions precisely<ept id="p1">](deployr-admin-configure-reinstall-r.md)</ept>.</source>
        </trans-unit><trans-unit id="325" translate="yes" xml:space="preserve">
          <source>Upping R Session Memory Limits (Windows only)</source>
        </trans-unit><trans-unit id="326" translate="yes" xml:space="preserve">
          <source>By default, the maximum memory available to an R session under DeployR on Windows Rserve is 2 GB.</source>
        </trans-unit><trans-unit id="327" translate="yes" xml:space="preserve">
          <source>If this is insufficient for your purposes, then you can increase the memory allocated for your R sessions by executing the <ph id="ph1">`memory.limit()`</ph> R function on the R session.</source>
        </trans-unit><trans-unit id="328" translate="yes" xml:space="preserve">
          <source>This function allows you to specify a higher memory allocation for your R session.</source>
        </trans-unit><trans-unit id="329" translate="yes" xml:space="preserve">
          <source>The size parameter on that function call determines the final memory allocation for the R session.</source>
        </trans-unit><trans-unit id="330" translate="yes" xml:space="preserve">
          <source>In general:</source>
        </trans-unit><trans-unit id="331" translate="yes" xml:space="preserve">
          <source>It is often convenient to add this function call to the start of any R script that requires runtime memory resources in excess of the default 2 GB on Windows.</source>
        </trans-unit><trans-unit id="332" translate="yes" xml:space="preserve">
          <source>For example, the following line will raise the maximum memory limit to 10 GB for your R session:</source>
        </trans-unit><trans-unit id="333" translate="yes" xml:space="preserve">
          <source>The increase in the memory allocation takes place only once the line is executed.</source>
        </trans-unit><trans-unit id="334" translate="yes" xml:space="preserve">
          <source>The memory allocated during a session can only be increased, and not decreased.</source>
        </trans-unit><trans-unit id="335" translate="yes" xml:space="preserve">
          <source>The value for <ph id="ph1">`memory.limit`</ph> is not applied system wide.</source>
        </trans-unit><trans-unit id="336" translate="yes" xml:space="preserve">
          <source>Instead, it applies only to the R &gt;session where the <ph id="ph1">`memory.limit`</ph> function has been executed.</source>
        </trans-unit><trans-unit id="337" translate="yes" xml:space="preserve">
          <source>Grid nodes have finite memory resources.</source>
        </trans-unit><trans-unit id="338" translate="yes" xml:space="preserve">
          <source>Keep these resource limits in mind when adjusting memory allocations for individual R sessions.</source>
        </trans-unit><trans-unit id="339" translate="yes" xml:space="preserve">
          <source>Access Denied to Tomcat (Windows only)</source>
        </trans-unit><trans-unit id="340" translate="yes" xml:space="preserve">
          <source>If you reboot after installing and get an access error message for Tomcat, you can specify that Tomcat should be run “as an administrator” to stop the message from appearing.</source>
        </trans-unit><trans-unit id="341" translate="yes" xml:space="preserve">
          <source>The error is related to <ph id="ph1">`tomcat7w.exe`</ph>, which is an application for monitoring and configuring Tomcat services.</source>
        </trans-unit><trans-unit id="342" translate="yes" xml:space="preserve">
          <source>The error message is: <bpt id="p1">*</bpt>“Access is denied. Unable to open the service Tomcat”<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="343" translate="yes" xml:space="preserve">
          <source>To set Tomcat program to run as an administrator, do the following:</source>
        </trans-unit><trans-unit id="344" translate="yes" xml:space="preserve">
          <source>Right-click <ph id="ph1">`tomcat7w.exe`</ph> and choose <bpt id="p1">**</bpt>Properties<ept id="p1">**</ept> from the shortcut menu.</source>
        </trans-unit><trans-unit id="345" translate="yes" xml:space="preserve">
          <source>is a GUI application for monitoring and configuring Tomcat services.</source>
        </trans-unit><trans-unit id="346" translate="yes" xml:space="preserve">
          <source>In the Properties dialog, select the checkbox <bpt id="p1">*</bpt>Run this program as an administrator checkbox<ept id="p1">*</ept> in the <bpt id="p2">**</bpt>Privilege Level<ept id="p2">**</ept> area.</source>
        </trans-unit><trans-unit id="347" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="348" translate="yes" xml:space="preserve">
          <source>Launch DeployR again.</source>
        </trans-unit><trans-unit id="349" translate="yes" xml:space="preserve">
          <source>Inactive Grid Node (Windows only)</source>
        </trans-unit><trans-unit id="350" translate="yes" xml:space="preserve">
          <source>If the <bpt id="p1">**</bpt>DeployR Default Node<ept id="p1">**</ept> appears <bpt id="p2">**</bpt>Inactive<ept id="p2">**</ept> in the DeployR landing page directly after having installed DeployR on a Windows 7 machine, then the <ph id="ph1">`R_HOME`</ph> variable may not be set.</source>
        </trans-unit><trans-unit id="351" translate="yes" xml:space="preserve">
          <source>To correct this issue:</source>
        </trans-unit><trans-unit id="352" translate="yes" xml:space="preserve">
          <source>Check the status of the <bpt id="p1">**</bpt>DeployR Default Node<ept id="p1">**</ept> in the DeployR landing page at <ph id="ph1">`http://&lt;DEPLOYR_SERVER_IP&gt;:&lt;PORT&gt;/deployr/landing`</ph>.</source>
        </trans-unit><trans-unit id="353" translate="yes" xml:space="preserve">
          <source>If it appears <bpt id="p1">**</bpt>Inactive<ept id="p1">**</ept>, continue to the next step.</source>
        </trans-unit><trans-unit id="354" translate="yes" xml:space="preserve">
          <source>Verify the status of the DeployR Rserve service in the <bpt id="p1">**</bpt>Services<ept id="p1">**</ept> dialog box.</source>
        </trans-unit><trans-unit id="355" translate="yes" xml:space="preserve">
          <source>If it appears as <ph id="ph1">`Started`</ph>, continue to the next step.</source>
        </trans-unit><trans-unit id="356" translate="yes" xml:space="preserve">
          <source>If not, start it now and go back to step 1.</source>
        </trans-unit><trans-unit id="357" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Tip:<ept id="p1">**</ept> Go to <bpt id="p2">**</bpt>Start <ph id="ph1">&amp;gt;</ph> Control Panel<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="358" translate="yes" xml:space="preserve">
          <source>Search for <ph id="ph1">`admin`</ph> and select <bpt id="p1">**</bpt>Administrative Tools<ept id="p1">**</ept> from the results.</source>
        </trans-unit><trans-unit id="359" translate="yes" xml:space="preserve">
          <source>Choose <bpt id="p1">**</bpt>Services<ept id="p1">**</ept> to open the <bpt id="p2">**</bpt>Services<ept id="p2">**</ept> dialog box.</source>
        </trans-unit><trans-unit id="360" translate="yes" xml:space="preserve">
          <source>At a DOS command prompt, go to the directory for R and start RServe.</source>
        </trans-unit><trans-unit id="361" translate="yes" xml:space="preserve">
          <source>Pay particular attention to the messages printed to the window.</source>
        </trans-unit><trans-unit id="362" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="363" translate="yes" xml:space="preserve">
          <source>If you see the message "R<ph id="ph1">\_</ph>HOME must be set in the environment or Registry", then you must define that environment variable as follows:</source>
        </trans-unit><trans-unit id="364" translate="yes" xml:space="preserve">
          <source>Go to <bpt id="p1">**</bpt>Start <ph id="ph1">&amp;gt;</ph> Control Panel<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="365" translate="yes" xml:space="preserve">
          <source>Search for <ph id="ph1">`sys`</ph> and select <bpt id="p1">**</bpt>Edit the system environment variables<ept id="p1">**</ept> from the results.</source>
        </trans-unit><trans-unit id="366" translate="yes" xml:space="preserve">
          <source>Click the <bpt id="p1">**</bpt>Environment Variables...<ept id="p1">**</ept> button to open the <bpt id="p2">**</bpt>Environment Variables<ept id="p2">**</ept> dialog box.</source>
        </trans-unit><trans-unit id="367" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>New...<ept id="p1">**</ept> and enter <ph id="ph1">`R_HOME`</ph> as the <bpt id="p2">**</bpt>Variable name<ept id="p2">**</ept> and the path to R (such as <ph id="ph2">`C:\Program Files\Microsoft SQL Server\130\R_SERVER`</ph>) as the <bpt id="p3">**</bpt>Variable value<ept id="p3">**</ept>.</source>
        </trans-unit><trans-unit id="368" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept> to create the variable.</source>
        </trans-unit><trans-unit id="369" translate="yes" xml:space="preserve">
          <source>Reboot your machine.</source>
        </trans-unit><trans-unit id="370" translate="yes" xml:space="preserve">
          <source>Go back to landing page and verify that the grid node is now active.</source>
        </trans-unit><trans-unit id="371" translate="yes" xml:space="preserve">
          <source>Cannot See API Explorer Tool</source>
        </trans-unit><trans-unit id="372" translate="yes" xml:space="preserve">
          <source>Ensure Adobe Flash Player is installed and configured to work with your browser.</source>
        </trans-unit><trans-unit id="373" translate="yes" xml:space="preserve">
          <source>Clear your browser’s cache before launching the API Explorer tool.</source>
        </trans-unit><trans-unit id="374" translate="yes" xml:space="preserve">
          <source>This is particularly important if you are upgrading from a previous version of DeployR.</source>
        </trans-unit><trans-unit id="375" translate="yes" xml:space="preserve">
          <source>Port Conflicts with Other Applications</source>
        </trans-unit><trans-unit id="376" translate="yes" xml:space="preserve">
          <source>If you run into conflicts with other applications, consider changing the port numbers.</source>
        </trans-unit><trans-unit id="377" translate="yes" xml:space="preserve">
          <source>You only need to change the port numbers of those applications that are actively conflicting.</source>
        </trans-unit><trans-unit id="378" translate="yes" xml:space="preserve">
          <source>Consequently, not all of the following steps may apply to your situation.</source>
        </trans-unit><trans-unit id="379" translate="yes" xml:space="preserve">
          <source>Changing Ports for DeployR Enterprise for Microsoft R Server 8.0.5</source>
        </trans-unit><trans-unit id="380" translate="yes" xml:space="preserve">
          <source>Launch the DeployR administrator utility script with administrator privileges:</source>
        </trans-unit><trans-unit id="381" translate="yes" xml:space="preserve">
          <source>On Windows:</source>
        </trans-unit><trans-unit id="382" translate="yes" xml:space="preserve">
          <source>On Linux:</source>
        </trans-unit><trans-unit id="383" translate="yes" xml:space="preserve">
          <source>From the main menu, choose the option to <bpt id="p1">**</bpt>Change DeployR Ports<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="384" translate="yes" xml:space="preserve">
          <source>Choose the option corresponding to the port you want to change and change the port number.</source>
        </trans-unit><trans-unit id="385" translate="yes" xml:space="preserve">
          <source>Return to the main menu and choose the option to restart the server.</source>
        </trans-unit><trans-unit id="386" translate="yes" xml:space="preserve">
          <source>Changing Ports for DeployR 8.0.0</source>
        </trans-unit><trans-unit id="387" translate="yes" xml:space="preserve">
          <source>For Windows:</source>
        </trans-unit><trans-unit id="388" translate="yes" xml:space="preserve">
          <source>In the <ph id="ph1">`C:\Program Files\Microsoft\DeployR-&lt;DEPLOYR_VERSION&gt;\Apache_Tomcat`</ph> directory, open the file <ph id="ph2">`server.xml`</ph>.</source>
        </trans-unit><trans-unit id="389" translate="yes" xml:space="preserve">
          <source>Find</source>
        </trans-unit><trans-unit id="390" translate="yes" xml:space="preserve">
          <source>Replace the port value with a new, unique port number.</source>
        </trans-unit><trans-unit id="391" translate="yes" xml:space="preserve">
          <source>Save the file.</source>
        </trans-unit><trans-unit id="392" translate="yes" xml:space="preserve">
          <source>Restart Tomcat for the changes to take effect.</source>
        </trans-unit><trans-unit id="393" translate="yes" xml:space="preserve">
          <source>For Linux / OS X</source>
        </trans-unit><trans-unit id="394" translate="yes" xml:space="preserve">
          <source>Edit the file <ph id="ph1">`&lt;DeployR_Install_Dir&gt;/tomcat/tomcat7/conf/server.xml`</ph>.</source>
        </trans-unit><trans-unit id="395" translate="yes" xml:space="preserve">
          <source>Find the port number value by searching for</source>
        </trans-unit><trans-unit id="396" translate="yes" xml:space="preserve">
          <source>Replace the port value with a new, unique port number.</source>
        </trans-unit><trans-unit id="397" translate="yes" xml:space="preserve">
          <source>Save the file.</source>
        </trans-unit><trans-unit id="398" translate="yes" xml:space="preserve">
          <source>Restart Tomcat for the changes to take effect.</source>
        </trans-unit><trans-unit id="399" translate="yes" xml:space="preserve">
          <source>At the prompt, type:</source>
        </trans-unit><trans-unit id="400" translate="yes" xml:space="preserve">
          <source>Verify that the port changes are working as expected.</source>
        </trans-unit><trans-unit id="401" translate="yes" xml:space="preserve">
          <source>At the prompt, type:</source>
        </trans-unit></group></body></file></xliff>