<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-teradata.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e0584c60e53c323b9f5298ab03d4743e8c61e373c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">0584c60e53c323b9f5298ab03d4743e8c61e373c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-teradata.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RevoScaleR Teradata Getting Started Guide</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Overview and tutorial to using RevoScaleR in Teradata.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>RevoScaleR Teradata Getting Started Guide</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>For customers using R Server 9.1 and earlier, this guide serves as an introduction to high-performance big data analytics for Teradata using <bpt id="p1">[</bpt>RevoScaleR functions<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept>.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The Teradata compute context was discontinued in Machine Learning Server 9.2.1.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>If you have R Server 9.1 and use the Teradata compute context, you are covered by Microsoft's <bpt id="p1">[</bpt>service support policy<ept id="p1">](../resources-servicing-support.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>For future compatibility, we recommend modifying existing code to run in other compute contexts, and create a Teradata data source object to work with your data.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>For more information about Teradata as a data source, see [RxTeradata]../r-reference/revoscaler/rxteradata.md).</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>There are three key components to running <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> high-performance analytics:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The name and arguments of the analysis function: What analysis do you want to perform?</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The specification of your data source(s): Where is your data and what are its characteristics?</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>And, if you are creating new data, for example with scoring, where does the new data go?</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The specification for your compute context: Where do you want to perform the computations?</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> provides a variety of data sources and compute contexts that can be used with the high-performance analytics functions.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>This guide focuses on analyzing Teradata data in-database.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>That is, the data is located in a Teradata database and the computations are performed at the location of the data.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>We also consider a second use case: data is extracted from the Teradata database, taking advantage of the Teradata Parallel Transporter (TPT), and computations are performed on a computer alongside the Teradata Platform.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>More information on <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> can be found here:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Tutorial: Data Import</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>RevoScaleR Function Reference</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Distributed Computing</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>RevoScaleR ODBC Data Import</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>For information on other distributed computing compute contexts, see:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>How to use RevoScaleR on Spark</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Setting Up the Sample Data</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The Sample <bpt id="p1">*</bpt>ccFraud<ept id="p1">*</ept> Data</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>To follow the examples in this guide, you need the following comma-delimited text data files to load into your Teradata database:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>These data files each have 10 million rows, and should be put in tables called <bpt id="p1">*</bpt>ccFraud10<ept id="p1">*</ept> and <bpt id="p2">*</bpt>ccFraudScore10<ept id="p2">*</ept>, respectively.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>These data files are available <bpt id="p1">[</bpt>online<ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698896&amp;clcid=0x409)</ept>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>We recommend that you create a RevoTestDB database to hold the data table.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Loading Your Data into the Teradata Database</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>You can use the ‘fastload’ Teradata command to load the data sets into your data base.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>You can find sample scripts for doing this in Appendix I, and <bpt id="p1">[</bpt>online<ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698896&amp;clcid=0x409)</ept> with the sample data files.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>You need to edit the sample scripts to provide appropriate logon information for your site.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Check with your system administrator to see of the data has already been loaded into your database.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>There is an example later in this guide of loading data into your Teradata data base from R using the <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept> function.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Using a Teradata Data Source and ComputeContext</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> package provides a framework for quickly writing start-to-finish, scalable R code for data analysis.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Even if you are relatively new to R, you can get started with just a few basic functions.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>In this guide, we are focusing on analyzing data that is located in a <bpt id="p1">**</bpt>Teradata Database<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The first step is to create a <bpt id="p1">*</bpt>data source<ept id="p1">*</ept> R object that contains information about the data that is analyzed.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Creating an RxTeradata Data Source</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>To create a Teradata data source for use in RevoScaleR, you need basic information about your database connection.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The connection string can contain information about your driver, your Teradata ID, your database name, your user ID, and your password.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Modify the code following to specify the connection string appropriate to your setup:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Then we need an SQL query statement to identify the data we want to use.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>We’ll start with all of the variables in the <bpt id="p1">*</bpt>ccFraud10<ept id="p1">*</ept> data, a simulated data set with 10 million observations.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Modify the following code to specify the correct database name:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>We use this information to create an RxTeradata data source object:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>We have also specified <bpt id="p1">*</bpt>rowsPerRead<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>This parameter is important for handling memory usage and efficient computations.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Most of the <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> analysis functions process data in chunks and accumulate intermediate results, returning the final computations after all of the data has been read.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rowsPerRead<ept id="p1">*</ept> parameter controls how many rows of data are read into each chunk for processing.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>If it is too large, you may encounter slow-downs because you don’t have enough memory to efficiently process such a large chunk of data.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>On some systems, setting <bpt id="p1">*</bpt>rowsPerRead<ept id="p1">*</ept> to too small a value can also provide slower performance.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>You may want to experiment with this setting on your system.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Extracting Basic Information about Your Data</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The Teradata data source can be used as the ‘data’ argument in RevoScaleR functions.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>For example, to get basic information about the data and variables, enter:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>You should see the following information:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Specifying Column Information in Your Data Source</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>All of the variables in our data set are stored as integers in the data base, but some of them actually represent categorical data – called factor variables in R. We can specify this information in the data source, and have them automatically converted to factors when analyzed or imported.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>The variable <bpt id="p1">*</bpt>state<ept id="p1">*</ept> represents the 50 states plus the District of Columbia.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>We can specify the state abbreviations as follows to be used as labels for that variable:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Now we create a column information object specifying the mapping of the existing integer values to categorical levels in order to create factor variables for <bpt id="p1">*</bpt>gender<ept id="p1">*</ept>, <bpt id="p2">*</bpt>cardholder<ept id="p2">*</ept>, and <bpt id="p3">*</bpt>state<ept id="p3">*</ept>:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Next we can recreate a Teradata data source, adding the column information:</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>If we get the variable information for the new data source, we can see that the three variables specified in <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> are now treated as factors:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Teradata has a limit of 30 bytes for table and column names, and sometimes creates additional tables with six-character suffixes, so you restrict your table and variable names to no more than 24 characters.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Creating an RxInTeradata Compute Context</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Since we want to perform <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> analytic computations in-database, the next step is to create an <bpt id="p2">*</bpt>RxInTeradata<ept id="p2">*</ept> compute context.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>You need basic information about your Teradata platform.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Since the computations are tied to the database, a connection string is required for the <bpt id="p1">*</bpt>RxInTeradata<ept id="p1">*</ept> compute context.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>As when specifying an <bpt id="p1">*</bpt>RxTeradata<ept id="p1">*</ept> data source, the connection string can contain information about your driver, your Teradata ID, your database name, your user ID, and your password.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>If you have not done so already, modify the following code to specify the connection string appropriate to your setup:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Although the data source and compute context have overlapping information (and similar names), be sure to distinguish between them.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The data source (<bpt id="p1">*</bpt>RxTeradata<ept id="p1">*</ept>) tells us where the data is; the compute context (<bpt id="p2">*</bpt>RxInTeradata<ept id="p2">*</ept>) tells us where the computations are to take place.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The compute context only determines where the <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> high- performance analytics computations take place; it does not affect other standard R computations that you are performing on the client machine.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The compute context also requires information about your shared directory, both locally and remotely, and the path where Microsoft R Server is installed on each of the nodes of the <bpt id="p1">**</bpt>Teradata<ept id="p1">**</ept> platform.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Specify the appropriate information here:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Be sure that the <bpt id="p1">*</bpt>tdShareDir<ept id="p1">*</ept> specified exists on your client machine.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>To create the directory from R, you can run:</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Last, we need to specify some information about how we want output handled.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>We’ll request that our R session wait for the results, and not return console output from the in-database computations:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>We use all this information to create our <bpt id="p1">*</bpt>RxInTeradata<ept id="p1">*</ept> compute context object:</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Getting Information about Your RxInTeradata Compute Context</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>You can retrieve basic information about your Teradata platform using the <bpt id="p1">*</bpt>rxGetNodeInfo<ept id="p1">*</ept> function.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Your platform has at least one PE (Parsing Engine).</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>When RevoScaleR analytics are submitted to the Teradata platform, it is the Parsing Engine that receives and distributes instructions.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Each AMP(Access Module Processor) is connected to a disk, and has read/write access.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>When it receives an instruction from the PE, it retrieves its piece of the data.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>All of the AMPs work in parallel.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxGetNodeInfo<ept id="p1">*</ept> function sends a small task to each of the AMPS, and give a summary for each node.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>If you have a large platform, this may take some time:</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Troubleshooting the RxInTeradata Compute Context</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>If you encounter difficulties while using the <bpt id="p1">*</bpt>RxInTeradata<ept id="p1">*</ept> context, you may find it convenient to turn on run-time tracing.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>You can do this by passing the arguments <bpt id="p1">*</bpt>traceEnabled<ept id="p1">*</ept> and <bpt id="p2">*</bpt>traceLevel<ept id="p2">*</ept> to the <bpt id="p3">*</bpt>RxInTeradata<ept id="p3">*</ept> constructor.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Set the <bpt id="p1">*</bpt>traceLevel<ept id="p1">*</ept> to 7 to show all tracing information:</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>High-Performance In-Database Analytics in Teradata</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Computing Summary Statistics in Teradata</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Let’s start by computing summary statistics on our <bpt id="p1">*</bpt>teradataDS<ept id="p1">*</ept> data source, performing the computations in-database.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>The next step is to change the active compute context.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>When you run <bpt id="p1">*</bpt>rxSetComputeContext<ept id="p1">*</ept> with <bpt id="p2">*</bpt>tdCompute<ept id="p2">*</ept> as its argument, all subsequent RevoScaleR HPA computations take place in the in-database in Teradata until the compute context is switched back to a local compute context.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>We can use the high-performance <bpt id="p1">*</bpt>rxSummary<ept id="p1">*</ept> function to compute summary statistics for several of the variables.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>The formula used is a standard R formula:</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>You can see that the <bpt id="p1">*</bpt>ccFraud10<ept id="p1">*</ept> data set has 10 million observations with no missing data.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>To set the compute context back to our client machine, enter:</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Refining the RxTeradata Data Source</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>The computed summary statistics provide useful information about our data that can be put in the data source for use in further computations.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>For example, RevoScaleR uses minimum and maximum values in computing histograms, and can efficiently convert integer data to categorical factor data “on-the-fly” using the F function.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>You can include the specification of high and low values in an <bpt id="p1">*</bpt>RxTeradata<ept id="p1">*</ept> data source.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>We can add this information for <bpt id="p1">*</bpt>balance<ept id="p1">*</ept>, <bpt id="p2">*</bpt>numTrans,<ept id="p2">*</ept> <bpt id="p3">*</bpt>numIntlTrans<ept id="p3">*</ept>, and <bpt id="p4">*</bpt>creditLine<ept id="p4">*</ept> to the <bpt id="p5">*</bpt>colInfo<ept id="p5">*</ept> used to create the data source:</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Again, recreate a Teradata data source, adding the additional column information:</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Visualizing Your Data Using <bpt id="p1">*</bpt>rxHistogram<ept id="p1">*</ept> and <bpt id="p2">*</bpt>rxCube<ept id="p2">*</ept></source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxHistogram<ept id="p1">*</ept> function shows us the distribution of any of the variables in our data set.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>For example, let’s look at <bpt id="p1">*</bpt>creditLine<ept id="p1">*</ept> by <bpt id="p2">*</bpt>gender<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>First we’ll set the compute context back to <bpt id="p1">*</bpt>tdCompute<ept id="p1">*</ept> so that all of our analytics computations will be performed in Teradata rather than alongside:</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Next we’ll call <bpt id="p1">*</bpt>rxHistogram<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Internally, <bpt id="p1">*</bpt>rxHistogram<ept id="p1">*</ept> calls the <bpt id="p2">**</bpt>RevoScaleR<ept id="p2">**</ept> <bpt id="p3">*</bpt>rxCube<ept id="p3">*</ept> analytics function, which performs the required computations in-database in Teradata and return the results to your local workstation for plotting:</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>We can also call the <bpt id="p1">*</bpt>rxCube<ept id="p1">*</ept> function directly and use the results with one of many of R’s plotting functions.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>For example, <bpt id="p1">*</bpt>rxCube<ept id="p1">*</ept> can compute group means, so we can compute the mean of <bpt id="p2">*</bpt>fraudRisk<ept id="p2">*</ept> for every combination of <bpt id="p3">*</bpt>numTrans<ept id="p3">*</ept> and <bpt id="p4">*</bpt>numIntlTrans<ept id="p4">*</ept>.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>We use the <bpt id="p1">*</bpt>F()<ept id="p1">*</ept> notation to have integer variables treated as categorical variables (with a level for each integer value).</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>The low and high levels specified in <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> will automatically be used.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxResultsDF<ept id="p1">*</ept> function converts the results of the <bpt id="p2">*</bpt>rxCube<ept id="p2">*</ept> function into a data frame that can easily be used in one of R’s standard plotting functions.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Here we create a heat map using the <bpt id="p1">*</bpt>levelplot<ept id="p1">*</ept> function from the <bpt id="p2">*</bpt>lattice<ept id="p2">*</ept> package:</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>We can see that the risk of fraud increases with both the number of transactions and the number of international transactions:</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Analyzing Your Data with <bpt id="p1">*</bpt>rxLinMod<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Linear models are a work horse of predictive analytics.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>RevoScaleR<ept id="p1">*</ept> provides a high performance, scalable algorithm.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>As a simple example, let’s estimate a linear model with <bpt id="p1">*</bpt>balance<ept id="p1">*</ept> as the dependent variable and <bpt id="p2">*</bpt>gender<ept id="p2">*</ept> and <bpt id="p3">*</bpt>creditLine<ept id="p3">*</ept> as independent variables:</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>As long as we have not changed the compute context, the computations are performed in-database in Teradata.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>The function returns an object containing the model results to your local workstation.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>We can look at a summary of the results using the standard R <bpt id="p1">*</bpt>summary<ept id="p1">*</ept> function:</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Analyzing Your Data with <bpt id="p1">*</bpt>rxLogit<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Now, let’s estimate a logistic regression on whether or not an individual is a fraud risk.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>We continue to use the same compute context and data source, and specify a large model – 60 independent variables, including the 3 dummy variables that are dropped.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>In R (and RevoScaleR) every level of a categorical factor variable is automatically treated as a separate dummy variable:</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>We get the following output:</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Scoring a Data Set with Your Model</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>We can use the estimated logistic regression model to create scores for another data set with the same independent variables.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>We need to specify two new data sources: the new input data set to be scored, and a new table in the Teradata Database for the results.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Now we set our compute context.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>We’ll also make sure that the output table doesn’t exist by making a call to <bpt id="p1">*</bpt>rxTeradataDropTable<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Now we can use the <bpt id="p1">*</bpt>rxPredict<ept id="p1">*</ept> function to score.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>We set <bpt id="p1">*</bpt>writeModelVars<ept id="p1">*</ept> to TRUE to have all of the variables used in the estimation included in the new table.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>The new variable containing the scores are named <bpt id="p1">*</bpt>ccFraudLogitScore<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>We have a choice of having our predictions calculated on the scale of the response variable or the underlying ‘link’ function.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Here we choose the ‘link’ function, so that the predictions are on a logistic scale.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>To add additional variables to our output predictions, use the <bpt id="p1">*</bpt>extraVarsToWrite<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>For example, we can include the variable <bpt id="p1">*</bpt>custID<ept id="p1">*</ept> from our scoring data table in our table of predictions as follows:</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>After the new table has been created, we can compute and display a histogram of the 10 million predicted scores.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>The computations are faster if we pre-specify the low and high values.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>We can get this information from the data base using a special data source with <bpt id="p1">*</bpt>rxImport<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>(Note that the <bpt id="p1">*</bpt>RxOdbcData<ept id="p1">*</ept> data source type can be used with a Teradata data base.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>It is typically faster for small queries.)</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Now we create our data source:</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>Then we compute and display the histogram:</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Using rxDataStep and rxImport</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Using rxDataStep to Transform Variables</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept> function processes data a chunk at a time, reading from one data source and writing to another.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>In this example, we use a function in another R package.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>boot<ept id="p1">*</ept> package is ‘recommended’ package that is included with every distribution of R, but is not loaded automatically on start-up.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>It contains a function <bpt id="p1">*</bpt>inv.logit<ept id="p1">*</ept> that computes the inverse of a logit; that is, converts a logit back to a probability on the [0,1] scale.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>(Note that we could have gotten predictions in this scale by setting <bpt id="p1">*</bpt>type=”response”<ept id="p1">*</ept> in our call to <bpt id="p2">*</bpt>rxPredict<ept id="p2">*</ept>.) We’d like all of the variables in our <bpt id="p3">*</bpt>ccScoreOutput<ept id="p3">*</ept> table to be put in the new table, in addition to the newly created variable.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>So we specify our input and output data sources as follows:</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>Now we call the <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept> function, specifying the transforms we want in a list.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>We are also specifying the additional R packages that are needed to perform the transformations.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>These packages must be pre-installed on the nodes of your Teradata platform.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>We can now look at basic variable information for the new data set.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>Notice that factor variables are written to the data base as character data.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>To use them as factors in subsequent analysis, use <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> to specify the levels.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>Using <bpt id="p1">*</bpt>rxImport<ept id="p1">*</ept> to Extract a Subsample into a Data Frame in Memory</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>If we want to examine high risk individuals in more detail, we can extract information about them into a data frame in memory, order them, and print information about those with the highest risk.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>Since we are computing on our local computer, we can reset the compute context to local.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>We use the <bpt id="p1">*</bpt>sqlQuery<ept id="p1">*</ept> argument for the Teradata data source to specify the observations to select so that only the data of interest is extracted from the data base.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Now we have the high risk observations in a data frame in memory.</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>We can use any R functions to manipulate the data frame:</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>Using rxDataStep to Create a Teradata Table</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>When we are working in a local compute context, we have access to both local data files and the Teradata database via TPT.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>So, we can use rxDataStep to take a data set on our local system, perform any desired transformations, and create a new Teradata table.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>For example, one of the sample .xdf files shipped with RevoScaleR is AirlineDemoSmall.xdf.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>Let’s put this data into a Teradata table, storing DayOfWeek as an integer with values from 1 to 7.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>Now we can set our compute context back to in-Teradata, and look at summary statistics of the new table:</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>Performing Your Own ‘Chunking’ Analysis</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept> function also allows us to write our own ‘chunking’ analysis.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>Reading the data in chunks on multiple AMPS in Teradata, we can process each chunk of data using the R language, and write out summary results for each chunk into a common Teradata data source.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>Let’s look at an example using the <bpt id="p1">*</bpt>table<ept id="p1">*</ept> function in R, which computes a contingency table.</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>(If you actually have data sets to tabulate, use the <bpt id="p1">*</bpt>rxCrossTabs<ept id="p1">*</ept> or <bpt id="p2">*</bpt>rxCube<ept id="p2">*</ept> functions built into <bpt id="p3">**</bpt>RevoScaleR<ept id="p3">**</ept>; this example is meant for instructional purposes only.)</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>The first step is to write a function to process each chunk of data.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>The data will automatically be fed into the function as a rectangular list of data columns.</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>The function must also return a rectangular list of data columns (which a data frame is).</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>In the example below, we are summarizing the input data and returning a data frame with a single row.</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>Next we set our active compute context to compute in-database, and set up our data source:</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>Now set up a data source to hold the intermediate results.</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>Again, we’ll “drop” the table if it exists.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>Next we’ll call <ph id="ph1">`rxDataStep`</ph> with our <ph id="ph2">`ProcessChunk`</ph> function as the transformation function to use.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>To see our intermediate results for all of the chunks, we can import the data base table into memory:</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>To compute our final results, in this example we can just sum the columns:</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>To remove the intermediate results table:</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>Using rxDataStep for By-Group Analyses</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>When running in Teradata, it is also possible to control the data that is provided in each ‘chunk’ processed by <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>This allows us to perform by-group analyses, estimating a separate model for each group of observations defined by one or more categorical variables.</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>Creating a Simulated Data Set for By-Group Analysis</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>For example, let’s create a simulated data set that has 100,000 observations and three variables: <bpt id="p1">*</bpt>SKU<ept id="p1">*</ept>, <bpt id="p2">*</bpt>INCOME<ept id="p2">*</ept>, and <bpt id="p3">*</bpt>SALES<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>Our objective is to estimate a model of <bpt id="p1">*</bpt>SALES<ept id="p1">*</ept> on <bpt id="p2">*</bpt>INCOME<ept id="p2">*</ept> for each <bpt id="p3">*</bpt>SKU<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>To make it easy to interpret our results, we’ll set the underlying coefficient for <bpt id="p1">*</bpt>INCOME<ept id="p1">*</ept> equal to the <bpt id="p2">*</bpt>SKU<ept id="p2">*</ept> number.</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>Next, we upload this data frame into a table in our Teradata database, removing any existing table by that name first:</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>A Transformation Function for By-Group Analysis</source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>Next, let’s consider the analysis we want to perform for each group.</source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>As in the previous section, we write a transformation function that operates on a chunk of data, then writes out the results for that chunk into an “intermediate results” table.</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source>In this case, we estimate a linear model on the chunk of data, and put the components of the model we need for scoring into a string.</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>We will also include the SKU number and the estimated slope in our results table.</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>We are assuming, at this point, that we have all of the data for a single SKU in the chunk of data being processed by the transformation function.</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>Setting Up an Input Data Source for By-Group Analysis</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>The next step is to set up a data source that controls how the data is passed into the transformation function.</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>To do so, we specify the <bpt id="p1">*</bpt>tableOpClause<ept id="p1">*</ept> when creating an <bpt id="p2">*</bpt>RxTeradata<ept id="p2">*</ept> data source.</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>HASH BY<ept id="p1">*</ept>, <bpt id="p2">*</bpt>PARTITION BY<ept id="p2">*</ept>, <bpt id="p3">*</bpt>PARTITION<ph id="ph1">\_</ph>WITH<ph id="ph2">\_</ph>VIEW BY<ept id="p3">*</ept>, and <bpt id="p4">*</bpt>LOCAL ORDER BY<ept id="p4">*</ept> clauses can be used to organize the data.</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source>This data source parameter only affects <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept> running in an <bpt id="p2">*</bpt>RxInTeradata<ept id="p2">*</ept> compute context.</source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>(Note: when using Teradata software with versions before 14.10.01.07-1 or 14.10.02d, replace <bpt id="p1">*</bpt>PARTITION<ept id="p1">*</ept> with <bpt id="p2">*</bpt>PARTITION-WITH-VIEW<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source>However, working with these versions is unsupported.)</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>By using the partition clause, we have one computing resource for each SKU so that the transformation function will be operating on a single SKU of data.</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source>(For more details on using the partition clause, see Teradata’s <bpt id="p1">*</bpt>SQL Data Manipulation Language<ept id="p1">*</ept> manual.) For modeling, we need all rows for a given model (a single SKU) to fit in one read, so <bpt id="p2">*</bpt>rowsPerRead<ept id="p2">*</ept> is set high.</source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source>Estimating By-Group Linear Models</source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source>Before running the analysis, we need to set up the output results data source:</source>
        </trans-unit><trans-unit id="324" translate="yes" xml:space="preserve">
          <source>Since the <bpt id="p1">*</bpt>lm<ept id="p1">*</ept> function is called inside of our transformation function, we need to make sure that it is available wherever the computations are taking place.</source>
        </trans-unit><trans-unit id="325" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>lm<ept id="p1">*</ept> function is contained within the <bpt id="p2">*</bpt>stats<ept id="p2">*</ept> package, so we specify that in the <bpt id="p3">*</bpt>transformPackages<ept id="p3">*</ept> RevoScaleR option:</source>
        </trans-unit><trans-unit id="326" translate="yes" xml:space="preserve">
          <source>We want to make sure that our compute context is set appropriately, since the <bpt id="p1">*</bpt>tableOpClause<ept id="p1">*</ept> only has an effect when running in Teradata:</source>
        </trans-unit><trans-unit id="327" translate="yes" xml:space="preserve">
          <source>Now we can run use rxDataStep to process the data by SKU:</source>
        </trans-unit><trans-unit id="328" translate="yes" xml:space="preserve">
          <source>We can take a quick look at our estimated slopes by bringing the data from our results table into a data frame in memory.</source>
        </trans-unit><trans-unit id="329" translate="yes" xml:space="preserve">
          <source>Scoring Using the Estimated By-Group Linear Models</source>
        </trans-unit><trans-unit id="330" translate="yes" xml:space="preserve">
          <source>We can use a similar process to score the data, using a transformation function that will only be processing data from a single SKU:</source>
        </trans-unit><trans-unit id="331" translate="yes" xml:space="preserve">
          <source>Next, we set up an SQL query that joins our original simulated table with our intermediate results table, matching the SKUs:</source>
        </trans-unit><trans-unit id="332" translate="yes" xml:space="preserve">
          <source>For scoring, we do not need all rows for a given model to fit in one read.</source>
        </trans-unit><trans-unit id="333" translate="yes" xml:space="preserve">
          <source>As long as we compute in-database, all of the data in each chunk belongs to the same SKU.</source>
        </trans-unit><trans-unit id="334" translate="yes" xml:space="preserve">
          <source>We also need to set up our new output data source:</source>
        </trans-unit><trans-unit id="335" translate="yes" xml:space="preserve">
          <source>Now we set the compute context and perform the scoring:</source>
        </trans-unit><trans-unit id="336" translate="yes" xml:space="preserve">
          <source>rxSetComputeContext(tdCompute) rxDataStep( inData = inDataSource, outFile = scoresDataSource, transformFunc = ScoreChunk, reportProgress = 0, overwrite = TRUE )</source>
        </trans-unit><trans-unit id="337" translate="yes" xml:space="preserve">
          <source>Last, we can use an SQL query in a Teradata data source to extract summary results by SKU:</source>
        </trans-unit><trans-unit id="338" translate="yes" xml:space="preserve">
          <source>We display the first 15 rows of the results.</source>
        </trans-unit><trans-unit id="339" translate="yes" xml:space="preserve">
          <source>We would expect that <bpt id="p1">*</bpt>PREDICTED<ph id="ph1">\_</ph>SALES<ept id="p1">*</ept> should be roughly <bpt id="p2">*</bpt>SKU<ph id="ph2">\*</ph>INCOME<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="340" translate="yes" xml:space="preserve">
          <source>When done with the analysis, we can remove the created tables from the database and then reset the compute context to the local context.</source>
        </trans-unit><trans-unit id="341" translate="yes" xml:space="preserve">
          <source>Performing Simulations In-Database</source>
        </trans-unit><trans-unit id="342" translate="yes" xml:space="preserve">
          <source>There may be occasions when it is useful to perform computations on in-memory data in parallel on a Teradata platform.</source>
        </trans-unit><trans-unit id="343" translate="yes" xml:space="preserve">
          <source>A simple example is shown here, simulating many games of craps.</source>
        </trans-unit><trans-unit id="344" translate="yes" xml:space="preserve">
          <source>The game of craps is a familiar casino game that consists of rolling a pair of dice.</source>
        </trans-unit><trans-unit id="345" translate="yes" xml:space="preserve">
          <source>If you roll a 7 or 11 on your initial roll, you win.</source>
        </trans-unit><trans-unit id="346" translate="yes" xml:space="preserve">
          <source>If you roll 2, 3, or 12, you lose.</source>
        </trans-unit><trans-unit id="347" translate="yes" xml:space="preserve">
          <source>If you roll a 4, 5, 6, 8, 9, or 10, that number becomes your <bpt id="p1">*</bpt>point<ept id="p1">*</ept> and you continue rolling until you either roll your point again (in which case you win) or roll a 7, in which case you lose.</source>
        </trans-unit><trans-unit id="348" translate="yes" xml:space="preserve">
          <source>The game is easily simulated in R using the following function:</source>
        </trans-unit><trans-unit id="349" translate="yes" xml:space="preserve">
          <source>We can run the function to simulate a single game:</source>
        </trans-unit><trans-unit id="350" translate="yes" xml:space="preserve">
          <source>Did you win or lose?</source>
        </trans-unit><trans-unit id="351" translate="yes" xml:space="preserve">
          <source>We will now simulate 1000 games of craps to help determine the probability of a win.</source>
        </trans-unit><trans-unit id="352" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxExec<ept id="p1">*</ept> function allows computations to be distributed to each of the AMPS of your Teradata platform.</source>
        </trans-unit><trans-unit id="353" translate="yes" xml:space="preserve">
          <source>If the <bpt id="p1">*</bpt>timesToRun<ept id="p1">*</ept> argument is specified, runs may be performed multiple times on each AMP.</source>
        </trans-unit><trans-unit id="354" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxExec<ept id="p1">*</ept> function returns a list with one element for every run.</source>
        </trans-unit><trans-unit id="355" translate="yes" xml:space="preserve">
          <source>Setting <bpt id="p1">*</bpt>RNGseed<ept id="p1">*</ept> to <bpt id="p2">*</bpt>"auto"<ept id="p2">*</ept> causes separate parallel random number substreams (using the "MT2203" generator) to be generated and used for each of the 1000 invocations of playCraps.</source>
        </trans-unit><trans-unit id="356" translate="yes" xml:space="preserve">
          <source>To see a summary of the results, we can convert the returned list to a vector, and summarize the results using the table function.</source>
        </trans-unit><trans-unit id="357" translate="yes" xml:space="preserve">
          <source>Your results should look something like this:</source>
        </trans-unit><trans-unit id="358" translate="yes" xml:space="preserve">
          <source>Analyzing Your Data Alongside Teradata</source>
        </trans-unit><trans-unit id="359" translate="yes" xml:space="preserve">
          <source>Although typically it is much faster to perform in-database analyses, it is sometimes convenient to extract your data from Teradata and analyze it alongside with an alternative, powerful compute engine.</source>
        </trans-unit><trans-unit id="360" translate="yes" xml:space="preserve">
          <source>To perform the computations on your local machine, we just need to change the compute context back to local.</source>
        </trans-unit><trans-unit id="361" translate="yes" xml:space="preserve">
          <source>Perform an rxSummary Using a Local Compute Context</source>
        </trans-unit><trans-unit id="362" translate="yes" xml:space="preserve">
          <source>When extracting data from Teradata, it is often more performant to increase the number of rows extracted for each read.</source>
        </trans-unit><trans-unit id="363" translate="yes" xml:space="preserve">
          <source>We can do this by increasing the <bpt id="p1">*</bpt>rowsPerRead<ept id="p1">*</ept> in the data source:</source>
        </trans-unit><trans-unit id="364" translate="yes" xml:space="preserve">
          <source>Now we can call rxSummary using the new data source.</source>
        </trans-unit><trans-unit id="365" translate="yes" xml:space="preserve">
          <source>This will be slow if you have a slow connection to your database; the data is being transferred to your local computer for analysis.</source>
        </trans-unit><trans-unit id="366" translate="yes" xml:space="preserve">
          <source>You should see the same results as you did when you performed the computations in-database.</source>
        </trans-unit><trans-unit id="367" translate="yes" xml:space="preserve">
          <source>Import of Data from a Teradata Database to a Local File</source>
        </trans-unit><trans-unit id="368" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxImport<ept id="p1">*</ept> function allows you to import data from a data source to a local “xdf” file.</source>
        </trans-unit><trans-unit id="369" translate="yes" xml:space="preserve">
          <source>This can be convenient if you want to repeatedly analyze a subset of your data initially stored in a Teradata Database.</source>
        </trans-unit><trans-unit id="370" translate="yes" xml:space="preserve">
          <source>Let’s store the variables <bpt id="p1">*</bpt>gender<ept id="p1">*</ept>, <bpt id="p2">*</bpt>cardholder<ept id="p2">*</ept>, <bpt id="p3">*</bpt>state<ept id="p3">*</ept>, and <bpt id="p4">*</bpt>balance<ept id="p4">*</ept> for the states of California, Oregon, and Washington on our local computer.</source>
        </trans-unit><trans-unit id="371" translate="yes" xml:space="preserve">
          <source>We create a new Teradata data source object to use as the <bpt id="p1">*</bpt>inData<ept id="p1">*</ept> argument for <bpt id="p2">*</bpt>rxImport<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="372" translate="yes" xml:space="preserve">
          <source>First, let’s specify the variables and selection we want to read in the SQL query.</source>
        </trans-unit><trans-unit id="373" translate="yes" xml:space="preserve">
          <source>(Make sure there are no hidden characters such as line feeds or tabs in the query.) We can use the <bpt id="p1">*</bpt>stateAbb<ept id="p1">*</ept> vector created earlier in this guide to identify the correct levels to include.</source>
        </trans-unit><trans-unit id="374" translate="yes" xml:space="preserve">
          <source>Next we create the <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> to be used.</source>
        </trans-unit><trans-unit id="375" translate="yes" xml:space="preserve">
          <source>In our new data set, we just want three factor levels for the three states being included.</source>
        </trans-unit><trans-unit id="376" translate="yes" xml:space="preserve">
          <source>We can use <bpt id="p1">*</bpt>statesToKeep<ept id="p1">*</ept> to identify the correct levels to include.</source>
        </trans-unit><trans-unit id="377" translate="yes" xml:space="preserve">
          <source>Since we are importing to our local computer, we are sure the compute context is set to local.</source>
        </trans-unit><trans-unit id="378" translate="yes" xml:space="preserve">
          <source>We store the data in a file named <bpt id="p1">*</bpt>ccFraudSub.xdf<ept id="p1">*</ept> in our current working directory</source>
        </trans-unit><trans-unit id="379" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>localDs<ept id="p1">*</ept> object returned from <bpt id="p2">*</bpt>rxImport<ept id="p2">*</ept> is a “light-weight” <bpt id="p3">*</bpt>RxXdfData<ept id="p3">*</ept> data source object representing the <bpt id="p4">*</bpt>ccFraud.xdf data<ept id="p4">*</ept> file stored locally on disk.</source>
        </trans-unit><trans-unit id="380" translate="yes" xml:space="preserve">
          <source>It can be used in analysis functions in the same way as the Teradata data source.</source>
        </trans-unit><trans-unit id="381" translate="yes" xml:space="preserve">
          <source>For example,</source>
        </trans-unit><trans-unit id="382" translate="yes" xml:space="preserve">
          <source>Managing Memory in In-Teradata Computations</source>
        </trans-unit><trans-unit id="383" translate="yes" xml:space="preserve">
          <source>Because a Teradata cluster node typically has many worker processes (AMPs) running constantly, it is important to limit how much memory a distributed analysis consumes.</source>
        </trans-unit><trans-unit id="384" translate="yes" xml:space="preserve">
          <source>Microsoft provides stored procedures in the revoAnalytics<ph id="ph1">\_</ph>Zqht2 scheduler database that allow a database administrator to set the memory limits for master and worker processes working on a RevoScaleR job.</source>
        </trans-unit><trans-unit id="385" translate="yes" xml:space="preserve">
          <source>By default, the master process memory limit is 2000 MB (approximately 2GB) and the worker process memory limit is 1000 MB (1GB).</source>
        </trans-unit><trans-unit id="386" translate="yes" xml:space="preserve">
          <source>These limits may be customized by a database administrator using the SetMasterMemoryLimitMB() and SetWorkerMemoryLimitMB() stored procedures, defined in the revoAnalytics<ph id="ph1">\_</ph>Zqht2 database created on installation.</source>
        </trans-unit><trans-unit id="387" translate="yes" xml:space="preserve">
          <source>For example, to set the master memory limit to 3000 MB:</source>
        </trans-unit><trans-unit id="388" translate="yes" xml:space="preserve">
          <source>call revoAnalytics_Zqht2.SetMasterMemoryLimitMB(3000);</source>
        </trans-unit><trans-unit id="389" translate="yes" xml:space="preserve">
          <source>To set the worker memory limit to 1500 MB:</source>
        </trans-unit><trans-unit id="390" translate="yes" xml:space="preserve">
          <source>The current memory limits can be viewed in the revoAnalytics<ph id="ph1">\_</ph>Zqht2.Properties table.</source>
        </trans-unit><trans-unit id="391" translate="yes" xml:space="preserve">
          <source>Memory limits that have been changed are in effect immediately, and no restart of the database is required.</source>
        </trans-unit><trans-unit id="392" translate="yes" xml:space="preserve">
          <source>Appendix I: Scripts for Loading Data into Teradata</source>
        </trans-unit><trans-unit id="393" translate="yes" xml:space="preserve">
          <source>Modify the following script to include your Log In information and data base name, then use the ‘fastload’ Teradata command to load the ccFraud.csv data.</source>
        </trans-unit><trans-unit id="394" translate="yes" xml:space="preserve">
          <source>(Copies of both scripts in this appendix can be found <bpt id="p1">[</bpt>online<ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698896&amp;clcid=0x409)</ept>.)</source>
        </trans-unit><trans-unit id="395" translate="yes" xml:space="preserve">
          <source>This similar script loads the ccFraudScore.csv data:</source>
        </trans-unit><trans-unit id="396" translate="yes" xml:space="preserve">
          <source>To run a fastload command, navigate to the directory containing the script from a command prompt and enter:</source>
        </trans-unit></group></body></file></xliff>