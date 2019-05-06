<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscalepy.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750e916adcaf2fcdce0a05745240eaab22ab42f35a3.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">e916adcaf2fcdce0a05745240eaab22ab42f35a3</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python\how-to-revoscalepy.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to use revoscalepy with Apache Spark - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn what you can do with revoscalepy in a Spark compute context in Machine learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to use revoscalepy in a Spark compute context</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>This article introduces Python functions in a <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../python-reference/revoscalepy/revoscalepy-package.md)</ept> package with Apache Spark (Spark) running on a Hadoop cluster.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Within a Spark cluster, Machine Learning Server leverages these components:</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Hadoop distributed file system for finding and accessing data.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Yarn for job scheduling and management.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Spark as the processing framework (versions 2.0-2.1).</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The revoscalepy library provides cluster-aware Python functions for data management, predictive analytics, and visualization.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>When you set the <bpt id="p1">[</bpt>compute context<ept id="p1">](../r/concept-what-is-compute-context.md)</ept> to <bpt id="p2">[</bpt>rx-spark-connect<ept id="p2">](../python-reference/revoscalepy/rx-spark-connect.md)</ept>, revoscalepy f automatically distributes the workload across all the data nodes.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>There is no overhead in managing jobs or the queue, or tracking the physical location of data in HDFS; Spark does both for you.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>For installation instructions, see <bpt id="p1">[</bpt>Install Machine Learning Server for Hadoop<ept id="p1">](../install/machine-learning-server-hadoop-install.md)</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Start Python</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>On your cluster's edge node, start a session by typing <bpt id="p1">**</bpt>mlserver-python<ept id="p1">**</ept> at the command line.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Local compute context on Spark</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>By default, the local compute context is the implicit computing environment.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>All mlserver-python code runs here until you specify a remote compute context.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Remote compute context on Spark</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>From the edge node, you can push computations to the data layer by creating a remote Spark compute context.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>In this context, execution is on all data nodes.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The following example shows how to set a remote compute context to clustered data nodes, execute functions in the Spark compute context, switch back to a local compute context, and disconnect from the server.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Specify a data source and location</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>As part of execution in Spark, your data source must be a file format that Spark understands, such as text, Hive, Orc, and Parquet.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>You can also create and consume <bpt id="p1">[</bpt>.xdf files<ept id="p1">](../r/concept-what-is-xdf.md)</ept>, a data file format native to Machine Learning Server that you can read or write to from both Python and R script.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Data source objects provided by revoscalepy in a Spark compute context include <bpt id="p1">[</bpt>RxTextData<ept id="p1">](../python-reference/revoscalepy/rxtextdata.md)</ept> <bpt id="p2">[</bpt>RxXdfData<ept id="p2">](../python-reference/revoscalepy/rxxdfdata.md)</ept>, and the <bpt id="p3">[</bpt>RxSparkData<ept id="p3">](../python-reference/revoscalepy/rxSparkdata.md)</ept> with derivatives for RxHiveData, RxOrcData, RxParquetData and RxSparkDataFrame.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Create a data source</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The following example illustrates an Xdf data source object that pulls data from a local sample directory created when you install Machine Learning Server.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The "sampleDataDir" argument is a reference to the sampleDataDir folder, known to revoscalepy.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Import data into a data frame</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Data is automatically loaded into a data frame even without rx_import, but you can load it explicitly using the rx_import, which is useful if you want to include parameters.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>In mlserver-python, you can use head and tail functions, similar to R, to return the first or last part of the data set.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Summarize data</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>To quickly understand fundamental characteristics of your data, use the <bpt id="p1">**</bpt>rx_summary<ept id="p1">**</ept> function to return basic statistical descriptors.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Mean, standard deviation, and min-max values.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>A count of total observations, missing observations, and valid observations is included.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>A minimum specification of the <bpt id="p1">[</bpt>rx_summmary<ept id="p1">](../python-reference/revoscalepy/rx-summary.md)</ept> function consists of a valid data source object and a formula giving the fields to summarize.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The formula is symbolic, providing variables used in the model.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>and typically does not contain a response variable.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>It should be of the form of ~ terms.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Get the term list from a data source to see what is available:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Create models</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The following example produces a linear regression, followed by predicted values for the linear regression model.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Python function reference</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>microsoftml function reference</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>revoscalepy function reference</source>
        </trans-unit></group></body></file></xliff>