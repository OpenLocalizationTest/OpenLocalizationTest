<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="tutorial-sparklyr-revoscaler.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86f66db3e4c45b19ec91610eb69dbb0893549975b6.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">f66db3e4c45b19ec91610eb69dbb0893549975b6</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\tutorial-sparklyr-revoscaler.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RevoScaleR with Sparklyr example (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Sparklyr interoperability with RevoScaleR on Machine Learning Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>RevoScaleR with sparklyr step-by-step examples</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Machine Learning Server supports the <bpt id="p1">[</bpt>sparklyr package from RStudio<ept id="p1">](https://cran.r-project.org/package=sparklyr)</ept>.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Machine Learning Server packages such as RevoScaleR and sparklyr can be used together within a single Spark session.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This walkthrough shows you two approaches for using these technologies together:</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Example 1: sparklyr data and MRS analytics</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Example 2: MRS data and sparklyr analytics</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>To run the example code, your environment must provide the following criteria:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>A Hadoop cluster with Spark and valid installation of Machine Learning Server</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Machine Learning Server configured for Hadoop and Spark</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Machine Learning Server SampleData loaded into HDFS</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>gcc and g++ installed on the edge node that the example runs on</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Write permissions to the R Library Directory</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Read/Write permissions to HDFS directory /user/RevoShare</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>An internet connection or the ability to download and manually install sparklyr</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Install the sparklyr package</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>How you install the sparklyr R package depends on whether or not you are on HDI.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Windows, Linux, or Hadoop users</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Since the default MRAN package snapshot for your version of Machine Learning Server is used automatically, you can install sparklyr like you would any other package.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Azure HDInsight (HDI) users</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If on HDI, you need to specify the MRAN snapshot date that contains the required package version.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>For Machine Learning Server use 2017-05-01.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Load data into HDFS</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>To load SampleData into HDFS, run these commands from within an edge node with MRS installed:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Example 1: sparklyr data with MRS modeling</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>This example assumes dployr and sparklyr data structures, with model training and predictive analysis using Machine Learning Server.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Create a connection to Spark using <ph id="ph1">`rxSparkConnect()`</ph>, specifying a sparklyr interop; using sparklyr and its interfaces to connect to Spark.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Call <ph id="ph1">`rxGetSparklyrConnection()`</ph> on the compute context to get a sparklyr connection object.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Use dplyr to load mtcars into a Spark DataFrame via the sparklyr connection object.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Partition the data in-Spark into a training and scoring set using dplyr.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>After partitioning, register the training set DataFrame in Spark to a Hive table.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Train a model in ScaleR using <ph id="ph1">`rxLinMod()`</ph> on an <ph id="ph2">`RxHiveData()`</ph> object.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>With the trained model, run a toy prediction using <ph id="ph1">`rxPredict()`</ph> on the test partition.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>After prediction, take the root mean square to determine accuracy.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Data is the Standard R dataset mtcars for this example.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Motor Trend Car Road Tests<ept id="p1">](https://stat.ethz.ch/R-manual/R-devel/library/datasets/html/mtcars.html)</ept>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Sample Code</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Sample Output, Comments Removed</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Example 2: MRS data with sparklyr and dplyR modeling</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>This example uses the airline data set.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>It includes multiple Machine Learning Server approaches for loading data, such as <ph id="ph1">`RxTextData`</ph> for CSV files, and <ph id="ph2">`RxOrcData`</ph> or <ph id="ph3">`RxParquetData`</ph> for those formats.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>You can try different approaches by commenting out inactive paths.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Given this data, the examples show you how to partition and train a model with sparklyr.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Create a connection to Spark using <ph id="ph1">`rxSparkConnect()`</ph>, specifying a sparklyr interop; using sparklyr and its interfaces to connect to Spark.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Call <ph id="ph1">`rxGetSparklyrConnection()`</ph> on the compute context to get a sparklyr connection object.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Use Machine Learning Server to load data from many sources.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Partition the data in-Spark into a training and scoring set using dplyr.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>After partitioning, register the training set DataFrame in Spark to a Hive table.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Train a model using sparklyr to call Spark ML algorithms.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Take a summary of the trained model to see estimates and errors.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Sample Code</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Sample Output, Comments Removed</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Conclusion</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The ability to use both Machine Learning Server and sparklyr from within one Spark session allow Machine Learning Server users to quickly and seamlessly utilize features provided by sparklyr within their solutions.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Next step</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>For more background, see <bpt id="p1">[</bpt>Get started with Machine Learning Server and RevoScaleR on Spark<ept id="p1">](how-to-revoscaler-spark.md)</ept>.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>What's new in Machine Learning Server</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Tips on computing with big data</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>How-to guides in Machine Learning Server</source>
        </trans-unit></group></body></file></xliff>