<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="what-is-microsoft-r-client.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea9265d8f37fe5f2888e2fb55a6398ca0df43369a4712.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5d8f37fe5f2888e2fb55a6398ca0df43369a4712</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-client\what-is-microsoft-r-client.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>What is Microsoft R Client?</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>- Machine Learning Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Microsoft R Client is a free data science tool for high performance analytics.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>With it, you can use any open-source R package.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Client, Microsoft R Client, Introduction, Get Started with R Client</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>About Microsoft R Client</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Microsoft R Client is a free, <bpt id="p1">[</bpt>community-supported<ept id="p1">](https://social.msdn.microsoft.com/Forums/en-US/home?forum=MicrosoftR)</ept>, data science tool for high performance analytics.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>R Client is built on top of <bpt id="p1">[</bpt>Microsoft R Open<ept id="p1">](https://mran.microsoft.com/open/)</ept> so you can use any open-source R package to build your analytics.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Additionally, R Client includes the <bpt id="p1">[</bpt>powerful RevoScaleR technology<ept id="p1">](../r/tutorial-revoscaler-data-import-transform.md)</ept> and its proprietary functions to benefit from parallelization and remote computing.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>R Client allows you to work with production data locally using the full set of RevoScaleR functions, but there are some constraints.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Data must fit in local memory, and processing is limited to two threads for RevoScaleR functions.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>To work with larger data sets or offload heavy processing, you can access a remote production instance of <bpt id="p1">[</bpt>Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept> from the command line or push the <bpt id="p2">[</bpt>compute context<ept id="p2">](../r/concept-what-is-compute-context.md)</ept> to the remote server.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more about its compatibility<ept id="p1">](compatibility-with-server.md)</ept>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Machine Learning Server vs R Client</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Machine Learning Server and Microsoft R Client offer virtually identical <bpt id="p1">[</bpt>R packages<ept id="p1">](../r-reference/introducing-r-server-r-package-reference.md#r-function-libraries)</ept>, but each one targets different scenarios.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>R Client is intended for data scientists who create solutions that run locally.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Machine Learning Server is commercial software that runs on a range of platforms, at much greater scale, with infrastructure for handling major workloads, on client-server topologies that support remote access over authenticated connections.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>You can work with R Client standalone.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>You can also use it with Machine Learning Server, where you learn and develop on R Client, and then migrate your work to Machine Learning Server or execute it remotely on a Machine Learning Server whenever you need the scale, support, and infrastructure of a server configured for operationalization.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>From R Client, shift data-centric RevoScaleR operations to a remote Machine Learning Server by creating a <bpt id="p1">[</bpt>remote compute context<ept id="p1">](../r/concept-what-is-compute-context.md)</ept>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Remote compute context is supported for <bpt id="p1">[</bpt>SQL Server Machine Learning Services<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/r/sql-server-r-services)</ept> or a <bpt id="p2">[</bpt>Spark cluster<ept id="p2">](../install/machine-learning-server-hadoop-install.md)</ept>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Typically, you shift the compute context to bring computations to where the data resides, thus avoiding data transfer over the network.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>From R Client, run arbitrary R code on a remote production instance of Machine Learning Server.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>This is a general-purpose capability: from a command line, you can switch between local and remote sessions interactively, useful for testing, administration, or  to use the additional processing power of a production server.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>For remote code execution, use <bpt id="p1">[</bpt>mrsdeploy<ept id="p1">](../r-reference/mrsdeploy/mrsdeploy-package.md)</ept>and <bpt id="p2">[</bpt>remoteLogin()<ept id="p2">](../r-reference/mrsdeploy/remotelogin.md)</ept> or <bpt id="p3">[</bpt>remoteLoginAAD()<ept id="p3">](../r-reference/mrsdeploy/remoteloginaad.md)</ept>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Execute on a remote server <ept id="p1">](../r/how-to-execute-code-remotely.md)</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Get started with R Client</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Getting started with Microsoft R Client is as easy as 1-2-3.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Click a step to get started:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Step 1</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>1. Install R Client</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The first step is to download Microsoft R Client for your operating system and install it.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>To learn more about the supported platforms or installation steps, please see the following articles:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Microsoft R Client on Windows<ept id="p1">](install-on-windows.md)</ept></source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Microsoft R Client for Linux<ept id="p1">](install-on-linux.md)</ept></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Compatibility with Machine Learning Server &amp; R Server<ept id="p1">](compatibility-with-server.md)</ept></source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>2. Configure Your IDE</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>While R is a command-line driven program, you can also use your favorite R integrated development environment (IDE) to interact with Microsoft R Client.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>To do so, you must point that IDE to the R Client R executable.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>This way, whenever you execute your R code, you'll do so using R Client and benefit from the proprietary packages installed with R Client.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>R IDE options include R Tools for Visual Studio on Windows (Recommended), RStudio, or any other R development environment.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Set up RTVS for R Client on Windows<ept id="p1">**</ept>: <bpt id="p2">[</bpt>R Tools for Visual Studio<ept id="p2">](https://docs.microsoft.com/visualstudio/rtvs/installation)</ept> (RTVS) is an integrated development environment available as a free add-in for any edition of Visual Studio.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>To make R Client the default R engine for RTVS, choose Change R to Microsoft R Client from the R Tools menu.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Set up RStudio for R Client on Windows or Linux<ept id="p1">**</ept>: <bpt id="p2">[</bpt>RStudio<ept id="p2">](https://www.rstudio.com/products/rstudio/download2/)</ept> is another popular R IDE.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>To make R Client the default R engine for RStudio, <bpt id="p1">[</bpt>update the path to R<ept id="p1">](https://support.rstudio.com/hc/en-us/articles/200486138-Using-Different-Versions-of-R)</ept>. For example, point to <ph id="ph1">`C:\Program Files\Microsoft\R Client\R_SERVER\bin\x64`</ph> on Windows.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Similarly, on Linux add "R_LIBS_SITE=/opt/microsoft/rclient/3.4.3/libraries/RServer" on bottom of the file "/opt/microsoft/rclient/3.4.3/runtime/R/etc/Renviron".</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Source<ept id="p1">](https://github.com/rstudio/rstudio/issues/2455#issuecomment-375327109)</ept>.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>After you configure the IDE, a message appears in the console signaling that the Microsoft R Client packages were loaded.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>You can connect remotely from your local IDE to an Machine Learning Server instance using <bpt id="p1">[</bpt>functions from the mrsdeploy package<ept id="p1">](../r/how-to-execute-code-remotely.md)</ept>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Then, the R code you enter at the remote command line executes on the remote server.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>This is very convenient when you need to offload heavy processing on server or to test your analytics during their development.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Your <bpt id="p1">[</bpt>Machine Learning Server administrator must configure Machine Learning Server<ept id="p1">](../operationalize/configure-start-for-administrators.md#configure-server-for-operationalization)</ept> for this functionality.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>3. Try Out R Client</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Now that you've installed R Client, you can start building and running some R code.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Launch R on the command line or in your IDE and:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Run the sample R code as described in this <bpt id="p1">[</bpt>quickstart guide<ept id="p1">](../r/quickstart-run-r-code.md)</ept>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Or, develop your own solutions using <bpt id="p1">[</bpt>RevoScaleR functions<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept>, <bpt id="p2">[</bpt>MicrosoftML functions<ept id="p2">](../r-reference/microsoftml/microsoftml-package.md)</ept>, and APIs.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>When ready, you can run that R code using R Client or even send those R commands to a <bpt id="p1">[</bpt>remote Machine Learning Server<ept id="p1">](../r/how-to-execute-code-remotely.md)</ept> for execution if Machine Learning Server is also installed in your organization.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>What's new in Microsoft R Client</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Microsoft R Client 3.4.3</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>This release of R Client, built on open-source R 3.4.3, is at the same functional level as Machine Learning Server 9.3.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Download R Client from <ph id="ph1">https://aka.ms/rclient</ph> (Windows) or <ph id="ph2">https://aka.ms/rclientlinux</ph> (Linux).</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>R Client includes these enhancements:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>R Client (Linux) now supports a remote SQL Server compute context on Windows.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>sqlrutils<ept id="p1">](../r-reference/sqlrutils/sqlrutils.md)</ept> is now supported for R Client (Linux).</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Microsoft R Client 3.4.1</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>This release of R Client, built on open-source R 3.4.1, is at the same functional level as Machine Learning Server 9.2.1.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>For more information about features in that release, see <bpt id="p1">[</bpt>here<ept id="p1">](../whats-new-in-machine-learning-server.md#921)</ept>.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Microsoft R Client 3.3.3</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>This release of R Client, built on open-source R 3.3.3.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Key release features include:</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Installations on Linux are now possible for R Client</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Several of the packages installed have been updated.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Learn more about <bpt id="p1">[</bpt>here<ept id="p1">](../whats-new-in-r-server.md)</ept>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Microsoft R Client 3.3.2</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The following release notes apply to Microsoft R Client, which can be downloaded from <ph id="ph1">https://aka.ms/rclient/download</ph>.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>New enhanced Microsoft R Client <bpt id="p1">[</bpt>Getting Started<ept id="p1">](what-is-microsoft-r-client.md)</ept> guide</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>A new 'version check' and auto-update is now possible using CheckForUpdates() in your R Console</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Offline installations<ept id="p1">](what-is-microsoft-r-client.md#installrclient)</ept> are now possible for R Client</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>New packages now bundled with Microsoft R Client:</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`mrsdeploy`</ph> - adds remote execution and web service deployment from R Client 3.3.2 to a remote R Server 9.0.1 instance</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`MicrosoftML`</ph> - adds machine learning algorithms to R script that executes on either R Client or R Server</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`olapR`</ph>- adds MDX query support through connections to OLAP cubes on a SQL Server 2016 Analysis Services instance</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>and the packages bundled with <bpt id="p1">[</bpt>Microsoft R Open 3.3.2<ept id="p1">](https://mran.microsoft.com/rro/installed/#enhance)</ept></source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Learn more about <bpt id="p1">[</bpt>the new and updated packages in this release<ept id="p1">](../whats-new-in-r-server.md)</ept>.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Updated end-user license agreement</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Telemetry collection is now enabled.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more<ept id="p1">](../resources-opting-out.md)</ept> about this feature and how to turn it off.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Learn More</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>You can learn more with these guides:</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Quickstart: Running R code in Microsoft R<ept id="p1">](../r/quickstart-run-r-code.md)</ept> (example)</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Compatibility with Machine Learning Server<ept id="p1">](compatibility-with-server.md)</ept></source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How-to guides in Machine Learning Server<ept id="p1">](../r/how-to-introduction.md)</ept></source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR R package reference<ept id="p1">](../r/tutorial-introduction.md)</ept></source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>MicrosoftML R package reference<ept id="p1">](../r-reference/microsoftml/microsoftml-package.md)</ept></source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>mrsdeploy R package reference<ept id="p1">](../r-reference/mrsdeploy/mrsdeploy-package.md)</ept></source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Execute R code on remote Machine Learning Server<ept id="p1">](../r/how-to-execute-code-remotely.md)</ept></source>
        </trans-unit></group></body></file></xliff>