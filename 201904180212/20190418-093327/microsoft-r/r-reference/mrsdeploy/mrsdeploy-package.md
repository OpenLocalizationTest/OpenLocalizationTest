<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="mrsdeploy-package.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b47150cbbf1bf9ccad849b75a4970dc94e922bde86.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">7150cbbf1bf9ccad849b75a4970dc94e922bde86</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\mrsdeploy\mrsdeploy-package.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>mrsdeploy package for R - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Function help reference for the mrsdeploy R package of Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>mrsdeploy package reference</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>mrsdeploy package for R</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>mrsdeploy<ept id="p1">**</ept> library provides functions for establishing a remote session in a console application and for publishing and managing a web service that is backed by the R code block or script you provided.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Each capability can be used independently but the greatest value is achieved when you can leverage both.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Package details</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Current version:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>1.1.3</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Built on:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>R 3.4.3</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Package distribution:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server 9.2.1<ept id="p1">](../../what-is-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Microsoft R Server 9.1 and earlier<ept id="p1">](../../what-is-microsoft-r-server.md)</ept></source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SQL Server 2016 and later (Windows only)<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/getting-started-with-machine-learning-services)</ept></source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Azure HDInsight<ept id="p1">](https://docs.microsoft.com/azure/hdinsight/hdinsight-hadoop-r-server-get-started)</ept></source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Azure Data Science Virtual Machines<ept id="p1">](https://docs.microsoft.com/azure/machine-learning/machine-learning-data-science-provision-vm)</ept></source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>How to use mrsdeploy</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>First, configure the server before using this library.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Configuring Machine Learning Server to operationalize analytics<ept id="p1">](../../operationalize/configure-start-for-administrators.md#configure-server-for-operationalization)</ept>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>After configuration, you can call <bpt id="p1">**</bpt>mrsdeploy<ept id="p1">**</ept> functions from the command line or from script.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>On R Client, the mrsdeploy package is installed <bpt id="p1">**</bpt>and loaded<ept id="p1">**</ept> automatically.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>You can start a remote session on an operationalized R Server instance once the remote login succeeds.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>On Machine Learning Server or R Server, the mrsdeploy package is installed, <bpt id="p1">**</bpt>but not loaded<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Therefore, you'll have to load it before using any  <bpt id="p1">**</bpt>mrsdeploy<ept id="p1">**</ept> functions.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>At the R prompt in the Machine Learning Server / R Server session, type <ph id="ph1">`library(mrsdeploy)`</ph> to load the package.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Supported configurations</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>For remote execution, participating nodes can be either of the following configurations:</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Two machines running the same version of Machine Learning Server or R Server (v9+), even if on different supported platforms, such as one Linux and one Windows.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>One machine running R Client 3.x and one machine running Machine Learning Server v9+, where the R Client user issues a remote login sequence to the Machine Learning  Server instance.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Execution is always on the Machine Learning Server side.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>It's not possible to set up a remote session that runs on R Client.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The requirements for remote execution include:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>An R Integrated Development Environment (IDE) <bpt id="p1">[</bpt>configured to work with Microsoft R Client<ept id="p1">](../../r-client-get-started.md)</ept>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Authenticated access<ept id="p1">](../../operationalize/configure-authentication.md)</ept> to an instance of Machine Learning Server <bpt id="p2">[</bpt>configured to operationalize analytics<ept id="p2">](../../operationalize/configure-start-for-administrators.md#configure-server-for-operationalization)</ept>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Functions by category</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>This section lists the functions by category to give you an idea of how each one is used.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>You can also use the table of contents to find functions in alphabetical order.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>1-Authentication &amp; remote session functions</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>To use the functions in the mrsdeploy package, you must log into Machine Learning Server as an authenticated user.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>And if using the remote execution functionality, you can also create a remote R session upon login.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Learn more about these functions and their arguments in the article <bpt id="p1">[</bpt>Connecting to Machine Learning Server to use mrsdeploy<ept id="p1">](../../operationalize/how-to-connect-log-in-with-mrsdeploy.md)</ept>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>remoteLogin<ept id="p1">](remotelogin.md)</ept></source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Authenticates the user via Active Directory and creates a remote R session and puts you at the remote command line unless you specify otherwise.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>remoteLoginAAD<ept id="p1">](remoteloginaad.md)</ept></source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Authenticates the user via Azure Active Directory and creates a remote R session and puts you at the remote command line unless you specify otherwise.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>remoteLogout<ept id="p1">](remotelogout.md)</ept></source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Logout of the remote session on the Machine Learning Server.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>2-Service pool functions</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>configureServicePool<ept id="p1">](configureServicePool.md)</ept></source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Create or update a dedicated pool of connections for a published web service running on Machine Learning Server.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The service pool provides an initial and maximum number sessions allowed for a given service.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>getPoolStatus<ept id="p1">](getPoolStatus.md)</ept></source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Get the status of the dedicated pool for a published web service running on Machine Learning Server.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>deleteServicePool<ept id="p1">](deleteServicePool.md)</ept></source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Deletes the service pool.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>3-Remote execution functions</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The following functions are used to initialize and interact with a session on a <bpt id="p1">[</bpt>remote Machine Learning Server<ept id="p1">](../../r/how-to-execute-code-remotely.md)</ept>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Remote sessions are created when you authenticate and closed when you log out.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Learn more about executing remotely from your local machine in this <bpt id="p1">[</bpt>Remote Execution<ept id="p1">](../../r/how-to-execute-code-remotely.md)</ept> article.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>4-Execution functions</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Use these functions to indicate whether the payload is a code block or script.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>remoteExecute<ept id="p1">](remoteexecute.md)</ept></source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Base function for executing a block of R code or an R script in the remote R session.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>remoteScript<ept id="p1">](remotescript.md)</ept></source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>A simple wrapper function for executing a remote R script.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>diffLocalRemote<ept id="p1">](difflocalremote.md)</ept></source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Generate a 'diff' report between local and remote.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>5-Remote command-line functions</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>remoteCommandLine<ept id="p1">](remoteCommandLine.md)</ept></source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Displays the <ph id="ph1">`REMOTE&gt;`</ph> command prompt and provides a remote execution context.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>All R commands entered at the R console will be executed in the remote R session.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>pause<ept id="p1">](remoteCommandLine.md)</ept></source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>When executed from the remote R session, returns the user to the <ph id="ph1">`&gt;`</ph> command prompt, and sets a local execution context.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>resume<ept id="p1">](remoteCommandLine.md)</ept></source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>When executed from the local R session, returns the user to the <ph id="ph1">`REMOTE&gt;`</ph> command prompt, and sets a remote execution context.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>6-File management functions</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>listRemoteFiles<ept id="p1">](listRemoteFiles.md)</ept></source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Gets a list of all the files that are in the working directory of the remote session.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>putLocalFile<ept id="p1">](putLocalFile.md)</ept></source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Uploads a file from the local machine and writes it to the working directory of the remote R session.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>This function is often used if a data file needs to be accessed by a script running on the remote R session.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>getRemoteFile<ept id="p1">](getRemoteFile.md)</ept></source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Downloads the file from the working directory of the remote R session into the working directory of the local R session.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>deleteRemoteFile<ept id="p1">](deleteRemoteFile.md)</ept></source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Deletes the file from the working directory of the remote R session.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>7-Object functions</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>putLocalObject<ept id="p1">](putLocalObject.md)</ept></source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Puts an object from the workspace of the local R session and loads it into the workspace of the remote R session.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>getRemoteObject<ept id="p1">](getRemoteObject.md)</ept></source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Gets an object from the workspace of the remote R session and loads it into the workspace of the local R session.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>putLocalWorkspace<ept id="p1">](putLocalWorkspace.md)</ept></source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Takes all objects from the local R session and loads them into the remote R session.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>getRemoteWorkspace<ept id="p1">](getRemoteWorkspace.md)</ept></source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Takes all objects from the remote R session and loads them into the local R session.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>8-Snapshot functions</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>listSnapshots<ept id="p1">](listSnapshots.md)</ept></source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Get a list of all the snapshots on the Machine Learning Server that are available to the current user.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>createSnapshot<ept id="p1">](createSnapshot.md)</ept></source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Creates a snapshot of the remote session and saves it on the server.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Both the workspace and the files in the working directory are saved.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>loadSnapshot<ept id="p1">](loadSnapshot.md)</ept></source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Loads the specified snapshot from the server into the remote session.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>The workspace is updated with the objects saved in the snapshot, and saved files are restored to the working directory.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>deleteSnapshot<ept id="p1">](deleteSnapshot.md)</ept></source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Deletes the specified snapshot from the repository on the Machine Learning Server.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>downloadSnapshot<ept id="p1">](downloadSnapshot.md)</ept></source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Downloads a snapshot from Machine Learning Server.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>9-Web service functions</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>The following functions are used to bundle R code or script as a web service.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>web service deployment<ept id="p1">](../../operationalize/how-to-deploy-web-service-publish-manage-in-r.md)</ept> can be published to the local server or remotely if you set up a remote session.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>publishService<ept id="p1">](publishService.md)</ept></source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Publishes an R code block as a new web service running on Machine Learning Server.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>updateService<ept id="p1">](updateService.md)</ept></source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Updates an existing web service on a Machine Learning Server instance.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>listServices<ept id="p1">](listServices.md)</ept></source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Lists the different published web services on the Machine Learning Server instance.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>getService<ept id="p1">](getService.md)</ept></source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Gets a web service for consumption.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>deleteService<ept id="p1">](deleteService.md)</ept></source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Deletes a web service on a Machine Learning Server instance.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Add R packages to your computer by running setup for Machine Learning Server or R Client:</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>R Client<ept id="p1">](../../r-client/what-is-microsoft-r-client.md)</ept></source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server<ept id="p1">](../../what-is-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>After you are logged in to a remote server, you can publish a web service or issue interactive commands against the remote Machine Learning Server.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>For more information, see these links:</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Remote Execution<ept id="p1">](../../r/how-to-execute-code-remotely.md)</ept></source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to publish and manage web services in R<ept id="p1">](../../operationalize/how-to-deploy-web-service-publish-manage-in-r.md)</ept></source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to interact with and consume web services in R<ept id="p1">](../../operationalize/how-to-consume-web-service-interact-in-r.md)</ept></source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Asynchronous batch execution of web services in R<ept id="p1">](../../operationalize/how-to-consume-web-service-asynchronously-batch.md)</ept></source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>R Package Reference<ept id="p1">](../introducing-r-server-r-package-reference.md)</ept></source>
        </trans-unit></group></body></file></xliff>