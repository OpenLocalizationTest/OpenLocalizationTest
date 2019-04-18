<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="resources-known-issues.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18cd0314758f03863b16dcc7f63e9e6c6e1b9f29c4b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d0314758f03863b16dcc7f63e9e6c6e1b9f29c4b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\resources-known-issues.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Machine Learning Server and Microsoft R Server - Known Issues - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Known Issues with Machine Learning Server and Microsoft R Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Known issues in Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>The following issues are known in the 9.3 release.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Known issues in 9.3</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>1. Missing <ph id="ph1">`azure-ml-admin-cli`</ph> extension on DSVM environments</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>If for some reason your <ph id="ph1">`azure-ml-admin-cli`</ph> extension is not available or has been removed, you will be met with the following error:</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>If you encounter this error,  you can re-add the extension as such:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Windows:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Linux:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>2. Compute nodes fail on a Python-only install on Ubuntu 14.04</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>This issue applies to both 9.3 and 9.2.1 installations.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>On an Ubuntu 14.04 installation of a Python-only Machine Learning Server configured for operationalization, the compute node eventually fails.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>For example, if you run <bpt id="p1">[</bpt>diagnostics<ept id="p1">](operationalize/configure-run-diagnostics.md)</ept>, the script fails with "BackEndBusy Exception".</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>To work around this issue, comment out the stop service entry in the config file:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>On the compute node, edit the /etc/init/computenode.service file.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Comment out the command: "stop on stopping rserve" by inserting # at beginning of the line.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Restart the compute node: <ph id="ph1">`az ml admin node start --computenode`</ph></source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>For more information on service restarts, see <bpt id="p1">[</bpt>Monitor, stop, and start web &amp; compute nodes<ept id="p1">](operationalize/configure-admin-cli-stop-start.md)</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>3. ImportError for Matplotlib.pyplot</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>This is a <bpt id="p1">[</bpt>known Anaconda issue<ept id="p1">](https://github.com/ContinuumIO/anaconda-issues/issues/1068)</ept> not specific to Machine Learning Server, but Matplotlib.pyplot fails to load on some systems.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Since using Matplotlib.pyplot with revoscalepy is a common scenario, we recommend the following workaround if you are blocked by an import error.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The workaround is to assign a non-interactive backend to matplotlib prior to loading pyplot:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>For more information, search for "Agg backend" in the <bpt id="p1">[</bpt>Matplotlib FAQ<ept id="p1">](https://matplotlib.org/faq/howto_faq.html)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>4. Model deserialization on older remote servers</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Applies to: <bpt id="p1">[</bpt>rxSerializeModel (RevoScaleR)<ept id="p1">](r-reference/revoscaler/rxserializemodel.md)</ept>, referencing "Error in memDecompress(data, type = decompress)"</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If you customarily switch the compute context among multiple machines, you might have trouble deserializing a model if the RevoScaleR library is out of sync. Specifically, if you serialized the model on a newer client, and then attempt deserialization on a remote server having older copies of those libraries, you might encounter this error:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>To deserialize the model, switch to a newer server or consider upgrading the older remote server.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>As a best practice, it helps when all servers and client apps are at the same functional level.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>5. azureml-model-management-sdk only supports up to 3 arguments as the input of the web service</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>When consuming the web services using python, sending multiple variables (more than three) as inputs of consume() or the alias function is returning KeyError or TypeError.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Alternative: use DataFrames as the input type.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Previous releases</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>This document also describes the known issues for the last several releases:</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Known issues for 9.2.1<ept id="p1">](#921)</ept></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Known issues for 9.1.0<ept id="p1">](#910)</ept></source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Known issues for 9.0.1<ept id="p1">](#901)</ept></source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Known issues for 8.0.5<ept id="p1">](#805)</ept></source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Machine Learning Server 9.2.1</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The following issues are known in this release:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure Machine Learning Server web node warning: "Web Node was not able to start because it is not configured."<ept id="p1">](#o16n-node)</ept></source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Client certificate is ignored when the Subject or Issue is blank.<ept id="p1">](#o16n-clientcert)</ept></source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Web node connection to compute node times out during a batch execution.<ept id="p1">](#o16n-batchtimeout)</ept></source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Other release-specific pages include <bpt id="p1">[</bpt>What's New in 9.2.1<ept id="p1">](whats-new-in-machine-learning-server.md)</ept> and <bpt id="p2">[</bpt>Deprecated and Discontinued Features<ept id="p2">](resources-deprecated-features.md)</ept>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>For known issues in the previous releases, see <bpt id="p1">[</bpt>Previous Releases<ept id="p1">](#Prev)</ept>.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>1. Configure Machine Learning Server web node warning: "Web Node was not able to start because it is not configured."</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>When configuring your web node, you might see the following message:  "Web Node was not able to start because it is not configured."</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Typically, this is not really an issue since the web node is automatically restarted within 5 minutes by an auto-recovery mechanism.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>After five minutes, run the <bpt id="p1">[</bpt>diagnostics<ept id="p1">](operationalize/configure-run-diagnostics.md)</ept>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>2. Client certificate is ignored when the Subject or Issue is blank.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If you are using a client certificate, both the Subject AND Issuer need to be set to a value in order for the certificate to be used.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If any of those is not set, the certificate settings are ignored without warning.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>3. Web node connection to compute node times out during a batch execution.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>If you are consuming a long-running web service via batch mode, you may encounter a connection timeout between the web and compute node.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>In batch executions, if a web service is still running after 10 minutes, the connection from the web node to the compute node times out. The web node then starts another session on another compute node or shell.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The initial shell that was running when the connection timed out continues to run but never returns a result.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>The workaround to bypass the timeout is to modify the web node appsetting.json file.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Change the field "ConnectionTimeout" under the "ComputeNodesConfiguration" section.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>The default value is "01:00:00", which is one hour.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Add a new field "BatchExecutionCheckoutTimeSpan" at the base level of the json file.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The value of "BatchExecutionCheckoutTimeSpan" and "ConnectionTimeout" should be set to same value.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>If both web and compute nodes are on the same machine (a one-box configuration) or on the same virtual network, then the "ConnectionTimeout" can be shorter because there is minimal latency.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>To reduce the risk of timeouts, we recommend same-machine or same-network deployments.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>On Azure, you can set these up easily using a template.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Configure Machine Learning Server using Resource Manager templates<ept id="p1">](https://blogs.msdn.microsoft.com/mlserver/2017/11/21/configuring-microsoft-machine-learning-server-to-operationalize-analytics-using-arm-templates/)</ept>.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Microsoft R Server 9.1.0</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR: rxMerge() behaviors in RxSpark compute context<ept id="p1">](#revoscaler-rxmerge)</ept></source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR: rxExecBy() terminates unexpectedly when NA values do not have a factor level<ept id="p1">](#revoscaler-rxexecby)</ept></source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>MicrosoftML error: "Transform pipeline 0 contains transforms that do not implement IRowToRowMapper"<ept id="p1">](#ml-ensembling)</ept></source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Spark compute context: modelCount=1 does not work with rxTextData<ept id="p1">](#ml-ensembling-modelcount)</ept></source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Cloudera: "install_mrs_parcel.py" does not exist<ept id="p1">](#cdh-parcel-message)</ept></source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Cloudera: Connection error due to libjvm and libhdfs package dependencies<ept id="p1">](#cdh-rstudio-loc-cc)</ept></source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Long delays when consuming web service on Spark<ept id="p1">](#sparkdelays)</ept></source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Other release-specific pages include <bpt id="p1">[</bpt>What's New in 9.1<ept id="p1">](whats-new-in-r-server.md)</ept> and <bpt id="p2">[</bpt>Deprecated and Discontinued Features<ept id="p2">](resources-deprecated-features.md)</ept>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>For known issues in the 9.0.1 or 8.0.5 releases, see <bpt id="p1">[</bpt>Previous Releases<ept id="p1">](#Prev)</ept>.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>1. rxMerge() behaviors in RxSpark compute context</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Applies to: RevoScaleR package &gt; rxMerge function<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>In comparison with the local compute context, rxMerge() used in a RxSpark compute context has slightly different behaviors:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>NULL return value.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Column order may be different.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Factor columns may be written as character type.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>In a local compute context, duplicate column names are made unique by adding “.”, plus the extensions provided by the user via the duplicateVarExt parameter (for example “Visibility.Origin”).</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>In an RxSpark compute context, the “.”</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>is omitted.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>2. rxExecBy() terminates unexpectedly when NA values do not have a factor level</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Applies to: RevoScaleR package &gt; rxExecBy function<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>R script using rxExecBy suddenly aborts when the data set presents factor columns containing NA values, and NA is not a factor level.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>For example, consider a variable for Gender with three factor levels: Female, Male, Unknown.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>If an existing value is not represented by one of the factors, the function fails.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>There are two possible workarounds:</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Option 1: Add an 'NA' level using <bpt id="p1">**</bpt>addNA()<ept id="p1">**</ept> to catch the "not applicable" case.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Option 2: Clean the input dataset (remove the NA values).</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Pseudo code for the first option might be:</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Output would now include a fourth factor level called NA that would catch all values not covered by the other factors:</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>3. MicrosoftML error: "Transform pipeline 0 contains transforms that do not implement IRowToRowMapper"</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Applies to: MicrosoftML package &gt; Ensembling<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Certain machine learning transforms that don’t implement the <bpt id="p1">**</bpt>IRowToRowMapper<ept id="p1">**</ept> interface fail during Ensembling.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Examples include getSentiment() and featurizeImage().</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>To work around this error, you can pre-featurize data using rxFeaturize().</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>The only other alternative is to avoid mixing Ensembling with transforms that produce this error.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Finally, you could also wait until the issue is fixed in the next release.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>4. Spark compute context: modelCount=1 does not work with rxTextData</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Applies to: MicrosoftML package &gt; Ensembling<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`modelCount = 1`</ph> does not work when used with <ph id="ph2">`rxTextData()`</ph> on Hadoop/Spark.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>To work around this issue, set the property to greater than 1.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>5. Cloudera: "install_mrs_parcel.py" does not exist</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>If you are performing a <bpt id="p1">[</bpt>parcel installation of R Server in Cloudera<ept id="p1">](install/r-server-install-cloudera.md)</ept>, you might notice a message directing you to use a python installation script for automated deployment.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>The exact message is "If you wish to automate the Parcel installation please run:", followed by "install_mrs_parcel.py".</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Currently, that script is not available.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Ignore the message.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>6. Cloudera: Connection error related to libjvm or libhdfs package dependencies</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>R Server has a package dependency that is triggered only under a very specific configuration:</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>R Server was installed on CDH via parcel generator</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>RStudio is the IDE</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Operation runs in local compute context on an edge node in a Hadoop cluster</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Under this configuration, a failed operation could be the result of a package dependency, which is evident in the error message stack through warnings about a missing libjvm or libhdfs package.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>The workaround is to recreate the symbolic link, update the site file, and restart R Studio.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Create this symlink:</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Copy the site file to the parcel repo and rename it to RevoHadoopEnvVars.site:</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Restart RStudio after the changes:</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>7. Long delays when consuming web service on Spark</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>If you encounter long delays when trying to consume a web service created with mrsdeploy functions in a Spark compute context, you may need to add some missing folders.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>The Spark application belongs to a user called 'rserve2' whenever it is invoked from a web service using mrsdeploy functions.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>To work around this issue, create these required folders for user 'rserve2' in local and hdfs:</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Next, create a new Spark compute context:</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>When 'reset = TRUE', all cached Spark Data Frames are freed and all existing Spark applications belonging to the current user are shut down.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>If you encounter long delays when trying to consume a web service created with mrsdeploy functions in a Spark compute context, you may need to add some missing folders.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>The Spark application belongs to a user called “rserve2” whenever it is invoked from a web service using mrsdeploy functions.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>To work around this issue, create these required folders for user “rserve2” in local and hdfs:</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Now, to create a clean Spark compute context, then run:</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>The 'reset' parameter kills all pre-existing yarn applications, and create a new one.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>8. Web node connection to compute node times out during a batch execution.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>If you are consuming a long-running web service via batch mode, you may encounter a connection timeout between the web and compute node.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>In batch executions, if a web service is still running after 10 minutes, the connection from the web node to the compute node times out. The web node then starts another session on another compute node or shell.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>The initial shell that was running when the connection timed out continues to run but never returns a result.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Microsoft R Server 9.0.1</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Package: RevoScaleR &gt; Distributed Computing</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>On SLES 11 systems, there have been reports of threading interference between the Boost and MKL libraries.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>The value of consoleOutput that is set in the <ph id="ph1">`RxHadoopMR`</ph> compute context when <ph id="ph2">`wait=FALSE`</ph> determines whether or not <ph id="ph3">`consoleOutput`</ph> is displayed when <ph id="ph4">`rxGetJobResults`</ph> is called; the value of <ph id="ph5">`consoleOutput`</ph> in the latter function is ignored.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>When using <ph id="ph1">`RxInTeradata`</ph>, if you encounter an intermittent failure, try resubmitting your R command.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxDataStep`</ph> function does not support the <ph id="ph2">`varsToKeep`</ph> and <ph id="ph3">`varsToDrop`</ph> arguments in <ph id="ph4">`RxInTeradata`</ph>.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`dataPath`</ph> and <ph id="ph2">`outDataPath`</ph> arguments for the <ph id="ph3">`RxHadoopMR`</ph> compute context are not yet supported.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxSetVarInfo`</ph> function is not supported when accessing xdf files with the <ph id="ph2">`RxHadoopMR`</ph> compute context.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>When specifying a non-default <ph id="ph1">`RNGkind`</ph> as an argument to <ph id="ph2">`rxExec`</ph>, identical random number streams can be generated unless the <ph id="ph3">`RNGseed`</ph> is also specified.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>When using small test data sets on a Teradata appliance, some test failures may occur due to insufficient data on each AMP.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Adding multiple new columns using <ph id="ph1">`rxDataStep`</ph> with <ph id="ph2">`RxTeradata`</ph> data sources fails in local compute context.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>As a workaround, use <ph id="ph1">`RxOdbcData`</ph> data sources or the <ph id="ph2">`RxInTeradata`</ph> compute context.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Package: RevoScaleR &gt; Data Import and Manipulation</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Appending to an existing table is not supported when writing to a Teradata database.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>When reading <ph id="ph1">`VARCHAR`</ph> columns from a database, white space is trimmed.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>To prevent this, enclose strings in non-white-space characters.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>When using functions such as <ph id="ph1">`rxDataStep`</ph> to create database tables with <ph id="ph2">`VARCHAR`</ph> columns, the column width is estimated based on a sample of the data.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>If the width can vary, it may be necessary to pad all strings to a common length.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Using a transform to change a variable's data type is not supported when repeated calls to <ph id="ph1">`rxImport`</ph> or <ph id="ph2">`rxTextToXdf`</ph> are used to import and append rows, combining multiple input files into a single .xdf file.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>When importing data from the Hadoop Distributed File System, attempting to interrupt the computation may result in exiting the software.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Package: RevoScaleR &gt; Analysis Functions</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Composite xdf data set columns are removed when running <ph id="ph1">`rxPredict(.)`</ph> with <ph id="ph2">`rxDForest(.)`</ph> in Hadoop and writing to the input file.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxDTree`</ph> function does not currently support in-formula transformations; in particular, using the <ph id="ph2">`F()`</ph> syntax for creating factors on the fly is not supported.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>However, numeric data is automatically binned.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Ordered factors are treated the same as factors in all RevoScaleR analysis functions except <ph id="ph1">`rxDTree`</ph>.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Package: RevoIOQ</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`RevoIOQ`</ph> function is run concurrently in separate processes, some tests may fail.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Package: RevoMods</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`RevoMods`</ph> timestamp() function, which masks the standard version from the utils package, is unable to find the <ph id="ph2">`C_addhistory`</ph> object when running in  an Rgui, Rscript, etc. session.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>If you are calling <ph id="ph1">`timestamp()`</ph>, call the <ph id="ph2">`utils`</ph> version directly as <ph id="ph3">`utils::timestamp()`</ph>.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>R Base and Recommended Packages</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>In the <ph id="ph1">`nls`</ph> function, use of the <ph id="ph2">`port`</ph> algorithm occasionally causes the R front end to stop unexpectedly.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`nls`</ph> help file advises caution when using this algorithm.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>We recommend avoiding it altogether and using either the default Gauss-Newton or plinear algorithms.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>Operationalize (Deploy &amp; Consume Web Services) <bpt id="p1">_</bpt>features formerly referred to as DeployR<ept id="p1">_</ept></source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>When Azure active directory authentication is the only form of authentication enabled, it is not possible to run diagnostics.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>Microsoft R Server 8.0.5</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>Package: RevoScaleR &gt; Distributed Computing</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>On SLES 11 systems, there have been reports of threading interference between the Boost and MKL libraries.</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>The value of consoleOutput defined in the <ph id="ph1">`RxHadoopMR`</ph> compute context when <ph id="ph2">`wait=FALSE`</ph> determines whether <ph id="ph3">`consoleOutput`</ph> is displayed when <ph id="ph4">`rxGetJobResults`</ph> is called.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>The value of <ph id="ph1">`consoleOutput`</ph> in the latter function is ignored.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>When using <ph id="ph1">`RxInTeradata`</ph>, if you encounter an intermittent failure, try resubmitting your R command.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxDataStep`</ph> function does not support the <ph id="ph2">`varsToKeep`</ph> and <ph id="ph3">`varsToDrop`</ph> arguments in <ph id="ph4">`RxInTeradata`</ph>.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`dataPath`</ph> and <ph id="ph2">`outDataPath`</ph> arguments for the <ph id="ph3">`RxHadoopMR`</ph> compute context are not yet supported.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxSetVarInfo`</ph> function is not supported when accessing xdf files with the <ph id="ph2">`RxHadoopMR`</ph> compute context.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>Package: RevoScaleR &gt; Data Import and Manipulation</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>Appending to an existing table is not supported when writing to a Teradata database.</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>When reading <ph id="ph1">`VARCHAR`</ph> columns from a database, white space is trimmed.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>To prevent this, enclose strings in non-white-space characters.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>When using functions such as <ph id="ph1">`rxDataStep`</ph> to create database tables with <ph id="ph2">`VARCHAR`</ph> columns, the column width is estimated based on a sample of the data.</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>If the width can vary, it may be necessary to pad all strings to a common length.</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>Using a transform to change a variable's data type is not supported when repeated calls to <ph id="ph1">`rxImport`</ph> or <ph id="ph2">`rxTextToXdf`</ph> are used to import and append rows, combining multiple input files into a single .xdf file.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>When importing data from the Hadoop Distributed File System, attempting to interrupt the computation may result in exiting the software.</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>Package: RevoScaleR &gt; Analysis Functions</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>Composite xdf data set columns are removed when running <ph id="ph1">`rxPredict(.)`</ph> with <ph id="ph2">`rxDForest(.)`</ph> in Hadoop and writing to the input file.</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxDTree`</ph> function does not currently support in-formula transformations; in particular, using the <ph id="ph2">`F()`</ph> syntax for creating factors on the fly is not supported.</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>However, numeric data is automatically binned.</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>Ordered factors are treated the same as factors in all RevoScaleR analysis functions except <ph id="ph1">`rxDTree`</ph>.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>DeployR</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>On Linux, if you attempt to change the DeployR RServe port using the <ph id="ph1">`adminUtilities.sh`</ph>, the script incorrectly updates Tomcat's <ph id="ph2">`server.xml`</ph> file, which prevents Tomcat from starting, and does not update the necessary the <ph id="ph3">`Rserv.conf`</ph> file.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>You must revert back to an earlier version of <ph id="ph1">`server.xml`</ph> to restore service.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>Using <ph id="ph1">`deployrExternal()`</ph> on the DeployR Server to reference a file that in a specified folder produces a ‘Connection Error’ due to an improperly defined environment variable.</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>For this reason, you must log into the Administration Console and go to <bpt id="p1">**</bpt>The Grid<ept id="p1">**</ept> tab. In that tab, edit <bpt id="p2">**</bpt>Storage Context value for each and every node<ept id="p2">**</ept> and specify the <bpt id="p3">**</bpt>full path<ept id="p3">**</ept> to the external data directory on that node’s machine, such as <ph id="ph1">`&lt;DEPLOYR_INSTALLATION_DIRECTORY&gt;/deployr/external/data`</ph>.</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>RevoIOQ Package</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`RevoIOQ`</ph> function is run concurrently in separate processes, some tests may fail.</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>RevoMods Package</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`RevoMods`</ph> timestamp() function, which masks the standard version from the utils package, is unable to find the <ph id="ph2">`C_addhistory`</ph> object when running in  an Rgui, Rscript, etc. session.</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>If you are calling <ph id="ph1">`timestamp()`</ph>, call the <ph id="ph2">`utils`</ph> version directly as <ph id="ph3">`utils::timestamp()`</ph>.</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>R Base and Recommended Packages</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>In the nls function, use of the <ph id="ph1">`port`</ph> algorithm occasionally causes the R front end to stop unexpectedly.</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>The nls help file advises caution when using this algorithm.</source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>We recommend avoiding it altogether and using either the default Gauss-Newton or plinear algorithms.</source>
        </trans-unit></group></body></file></xliff>