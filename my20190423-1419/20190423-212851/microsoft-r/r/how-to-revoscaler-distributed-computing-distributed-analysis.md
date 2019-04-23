<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-distributed-computing-distributed-analysis.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a9f73182fe55556ac9e02c92de7c4769a3e0c1566.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9f73182fe55556ac9e02c92de7c4769a3e0c1566</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-distributed-computing-distributed-analysis.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Distributed analysis (RevoScaleR in Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Distribute an analysis over multiple nodes using RevoScaleR functions.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Running distributed analyses using RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Many RevoScaleR functions support parallelization.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>On a standalone multi-core server, functions that are multithreaded run on all available cores.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>In an rxSparkConnect or RxHadoop remote compute context, multithreaded analyses run on all data nodes having the RevoScaleR engine.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>RevoScaleR can structure an analysis for parallel execution with no additional configuration on your part, assuming you set the <bpt id="p1">[</bpt>compute context<ept id="p1">](how-to-revoscaler-distributed-computing-compute-context.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Setting the compute context to rxSparkConnect or RxHadoopMR tells RevoScaleR to look for data nodes.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>In contrast, using the default local compute context tells the engine to look for available processors on the local machine.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>RevoScaleR also runs on R Client.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>On R Client, RevoScaleR is limited to two threads for processing and in-memory datasets.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>To avoid paging data to disk, R Client is engineered to ignore the <ph id="ph1">`blocksPerRead`</ph> argument, which results in all data being read into memory.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If your datasets exceed memory, you should push the compute context to a server instance on a supported platform (Hadoop, Linux, Windows, SQL Server).</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Given a registered a distributed compute context, the following functions can perform distributed computations:</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>(and its convenience functions, <ph id="ph1">`rxCov`</ph>, <ph id="ph2">`rxCor`</ph>, and <ph id="ph3">`rxSSCP`</ph>)</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>and</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Except for <ph id="ph1">`rxExec`</ph>, we refer to these functions as the RevoScaleR <bpt id="p1">*</bpt>high-performance analytics<ept id="p1">*</ept>, or HPA functions.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The exception, <ph id="ph1">`rxExec`</ph>, is used to execute an arbitrary function on specified nodes (or cores) of your compute context.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>It can be used for traditional high-performance computing functions.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxExec`</ph> function offers great flexibility in how arguments are passed, so that you can specify that all nodes receive the same arguments, or provide different arguments to each node.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>on a cluster is only redistributed if the data file is split.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Obtain node information</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>You can use informational functions, such as <ph id="ph1">`rxGetInfo`</ph> and <ph id="ph2">`rxGetVarInfo`</ph>, to confirm data availability.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Before beginning data analysis, you can use <ph id="ph1">`rxGetInfo`</ph> to confirm the data set is available on the compute resources.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>You can request basic information about a data set from each node using the <ph id="ph1">`rxGetInfo`</ph> function.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Assuming a data source named "airData", you can call <ph id="ph1">`rxGetInfo`</ph> as follows:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>To load a dataset, use AirOntime2012.xdf from the <bpt id="p1">[</bpt>data set download site<ept id="p1">](http://packages.revolutionanalytics.com/datasets)</ept> and make sure it is in your dataPath.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>You can then run <ph id="ph1">`airData &lt;- RxXdfData("AirOnTime2012.xdf")`</ph> to load the data on a cluster.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>On a five-node cluster, the call to <bpt id="p1">*</bpt>rxGetInfo<ept id="p1">*</ept> returns the following:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>This confirms that our data set is in fact available on all nodes of our cluster.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Obtain a Data Summary</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxSummary`</ph> function returns summary statistics on a data set, including datasets that run in a distributed context.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>When you run one of <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept>’s HPA functions in a distributed compute context, it automatically distributes the computation among the available compute resources and coordinates the returned values to create the final return value.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Assuming a job is waiting (or blocking), control is not returned until a computation is complete.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>We assume that the airline data has been copied to the appropriate data directory on all the computing resources and its location specified by the airData data source object.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if script runs locally using R Client.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>For example, we start by taking a summary of three variables from the airline data:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>We get the following results (identical to what we would have gotten from the same command in a local compute context):</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Perform an rxCube computation</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>We can perform an <ph id="ph1">`rxCube`</ph> computation using the same data set to compute the average arrival delay for departures for each hour of the day for each day of the week.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Again, the code is identical to the code used when performing the computations on a single computer, as are the results.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if script runs locally using R Client.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Notice that in this case we have returned an <ph id="ph1">`rxCube`</ph> object.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>We can use this object locally to, for example, extract a data frame and plot the results:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Plotted Results</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Perform an rxCrossTabs computation</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxCrossTabs`</ph> function provides essentially the same computations as <ph id="ph2">`rxCube`</ph>, but presents the results in a more traditional cross-tabulation.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Here we look at late flights (those whose arrival delay is 15 or greater) by late departure and day of week:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>which yields:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Compute a Covariance or Correlation Matrix</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxCovCor`</ph> function is used to compute covariance and correlation matrices; the convenience functions <ph id="ph2">`rxCov`</ph>, <ph id="ph3">`rxCor`</ph>, and <ph id="ph4">`rxSSCP`</ph> all depend upon it and are usually used in practical situations.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>For examples, see <bpt id="p1">[</bpt>Correlation and variance/covariance matrices<ept id="p1">](how-to-revoscaler-covcor.md)</ept>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The following example shows how the main function can be used directly:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Compute a Linear Model</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>We can model the arrival delay as a function of day of the week, departure time, and flight distance as follows:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>We can then view a summary of the results as follows:</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Compute a Logistic Regression</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>We can compute a similar logistic regression using the logical variable ArrDel15 as the response.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>This variable specifies whether a flight’s arrival delay was 15 minutes or greater:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>View Console Output</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>You may notice when running distributed computations that you get virtually no feedback while running waiting jobs.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Since the computations are in general not running on the same computer as your R Console, the “usual” feedback is not returned by default.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>However, you can set the <bpt id="p1">*</bpt>consoleOutput<ept id="p1">*</ept> parameter in your compute context to TRUE to enable return of console output from all the nodes.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>For example, here we update our compute context <bpt id="p1">*</bpt>myCluster<ept id="p1">*</ept> to include <bpt id="p2">*</bpt>consoleOutput=TRUE<ept id="p2">*</ept>:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if script runs locally using R Client.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Then, rerunning our previous example results in much more verbose output:</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Distributed and parallel processing in Machine Learning Server</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Compute context in Machine Learning Server</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>What is RevoScaleR</source>
        </trans-unit></group></body></file></xliff>