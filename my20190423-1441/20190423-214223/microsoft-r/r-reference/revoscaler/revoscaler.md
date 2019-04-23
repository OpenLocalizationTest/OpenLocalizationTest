<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="revoscaler.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86502af974c2e4567706d030df7212d52e895be8e4.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">502af974c2e4567706d030df7212d52e895be8e4</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\revoscaler.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RevoScaleR package for R (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Function help reference for the RevoScaleR R package of Machine Learning Server and Microsoft R</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RevoScaleR, ScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RevoScaleR package</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> library is a collection of portable, scalable, and distributable R functions for importing, transforming, and analyzing data at scale.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>You can use it for descriptive statistics, generalized linear models, k-means clustering, logistic regression, classification and regression trees, and decision forests.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Functions run on the <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> interpreter, built on open-source R, engineered to leverage the multithreaded and multinode architecture of the host platform.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Package details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Current version:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>9.3</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Built on:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>R 3.4.3</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Package distribution:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Machine Learning Server</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>R Client (Windows and Linux)</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>R Server 9.1 and earlier</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>SQL Server 2016 and later (Windows only)</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Azure HDInsight</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Azure Data Science Virtual Machines</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>How to use RevoScaleR</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> library is found in Machine Learning Server and Microsoft R products.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>You can use any R IDE to write R script calling functions in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept>, but the script must run on a computer having the interpreter and libraries.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> is often preloaded into tools that integrate with Machine Learning Server and R Client, which means you can call functions without having to load the library.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If the library is not loaded, you can load <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> from the command line by typing <ph id="ph1">`library(RevoScaleR)`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Run it locally</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>This is the default.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> runs locally on all platforms, including R Client.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>On a standalone Linux or Windows system, data and operations are local to the machine.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>On Hadoop, a local compute context means that data and operations are local to current execution environment (typically, an edge node).</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Run in a remote compute context</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> runs remotely on computers that have a server installation.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>In a remote compute context, the script running on a local R Client or Machine Learning Server shifts execution to a remote Machine Learning Server.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>For example, script running on Windows might shift execution to a Spark cluster to process data there.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>On distributed platforms, such as Hadoop processing frameworks (Spark and MapReduce), set the compute context to <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> or <bpt id="p2">[</bpt>RxHadoopMR<ept id="p2">](RxHadoopMR.md)</ept> and give the cluster name.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>In this context, if you call a function that can run in parallel, the task is distributed across data nodes in the cluster, where the operation is co-located with the data.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>On SQL Server, set the compute context to <bpt id="p1">[</bpt>RxInSQLServer<ept id="p1">](RxInSqlServer.md)</ept>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>There are two primary use cases for remote compute context:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Call R functions in T-SQL script or stored procedures running on SQL Server.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Call <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions in R script executing in a SQL Server <bpt id="p2">[</bpt>compute context<ept id="p2">](../../r/concept-what-is-compute-context.md)</ept>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>In your script, you can set a compute context to shift execution of <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> operations to a remote SQL Server instance that has the <bpt id="p2">**</bpt>RevoScaleR<ept id="p2">**</ept> interpreter.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Some functions in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> are specific to particular compute contexts.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>A filtered list of functions includes the following:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Computing on a Hadoop Cluster</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Computing on SQL Server</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Typical workflow</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>import</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Whenever you want to perform an analysis using <ph id="ph1">`RevoScaleR`</ph> functions, you should specify three distinct pieces of information:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt><bpt id="p2">**</bpt>analytic function<ept id="p2">**</ept><ept id="p1">](#analytics)</ept>, which specifies the analysis to be performed</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt><bpt id="p2">**</bpt>compute context<ept id="p2">**</ept><ept id="p1">](#compute)</ept>, which specifies where the computations should take place</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt><bpt id="p2">**</bpt>data source<ept id="p2">**</ept><ept id="p1">](#data)</ept>, which is the data to be used</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Functions by category</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The library includes data transformation and manipulation, visualization, predictions, and statistical analysis functions.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>It also includes functions for controlling jobs, serializing data, and performing common utility tasks.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>This section lists the functions by category to give you an idea of how each one is used.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>The table of contents lists functions in alphabetical order.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Some function names begin with <ph id="ph1">`rx`</ph> and others with <ph id="ph2">`Rx`</ph>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`Rx`</ph> function name prefix is used for class constructors for data sources and compute contexts.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>1-Data source functions</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Function name</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>RxXdfData</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Creates an efficient XDF data source object.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>RxTextData</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Creates a comma-delimited text data source object.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>RxSasData</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Creates a SAS data source object.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>RxSpssData</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Creates an SPSS data source object.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>RxOdbcData</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Creates an ODBC data source object.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>RxTeradata</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Creates a Teradata data source object.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>RxSqlServerData</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Creates a SQL Server data source object.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>2-Import and save-as</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Function name</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxImport<ept id="p1">](rximport.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Creates an .xdf file or data frame from a data source (for example, text, SAS, SPSS data files, ODBC or Teradata connection, or data frame).</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxdatastep.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Transform and subset data.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Creates an .xdf file, a comma-delimited text file, or data frame in memory (assuming you have sufficient memory to hold the output data) from an .xdf file or a data frame.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxGetInfo<ept id="p1">](rxgetinfoxdf.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Retrieves summary information from a data source or data frame.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxSetInfo<ept id="p1">](rxsetinfo.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Sets a file description in an .xdf file or a description attribute in a data frame.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>rxGetVarInfo</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Retrieves variable information from a data source or data frame.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>rxSetVarInfo</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Modifies variable information in an .xdf file or data frame.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>rxGetVarNames</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Retrieves variable names from a data source or data frame.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>rxCreateColInfo</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Generates a colInfo list from a data source.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>rxCompressXdf</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Compresses an existing .xdf file, or a directory of .xdf files.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>rxIsOpen</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Indicates whether a data source can be accessed.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>rxOpen</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Opens a data source for reading.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>rxClose</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Closes a data source.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>rxReadNext</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Read data from a source.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>rxWriteNext</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Writes the next chunk when moving data between RevoScaleR data sources.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>rxSetFileSystem</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Specify a file system type for data for import.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>rxGetFileSystem</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Retrieve the current file system type.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>rxHdfsFileSystem</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Creates an HDFS file system object.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>rxNativeFileSystem</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Creates a native file system object.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>rxSqlServerDropTable</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Execute an SQL statement that drops a table.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>rxSqlServerTableExists</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Execute an SQL statement that checks for a table's existence.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p1">&lt;/sup&gt;</ept> Signifies the most popular functions in this category.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>3-Data transformation</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Function name</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxdatastep.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Transform and subset data.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Creates an .xdf file, a comma-delimited text file, or data frame in memory (assuming you have sufficient memory to hold the output) from an .xdf file or a data frame.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxFactors<ept id="p1">](rxfactors.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Recode a factor variable or convert non-factor variable into a factor in an .xdf file or data frame.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>rxGetFuzzyDist</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Get fuzzy distances for a character vector.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>rxGetFuzzyKeys</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Get fuzzy keys for a character vector.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>rxSplit</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Splits an .xdf file or data frame into multiple .xdf files or data frames.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>rxSort</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Multi-key sorting of the variables an .xdf file or data frame.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>rxMerge</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Merges two .xdf files or data frames using various merge types.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>rxExecuteSQLDDL</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>SQL Server R Services only.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Runs an arbitrary SQL DDL command.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p1">&lt;/sup&gt;</ept> Signifies the most popular functions in this category.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>4-Graphing functions</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Function name</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>rxHistogram</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Creates a histogram from data.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>rxLinePlot</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Creates a line plot from data.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>rxLorenz</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Computes a Lorenz curve that can be plotted.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>rxRocCurve</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Computes and plots ROC curves from actual and predicted data.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>5-Descriptive statistics</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Function name</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxQuantile<ept id="p1">](rxquantile.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Computes approximate quantiles for .xdf files and data frames without sorting.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxSummary<ept id="p1">](rxsummary.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Basic summary statistics of data, including computations by group.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Writing by group computations to .xdf file not supported.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxCrossTabs<ept id="p1">](rxcrosstabs.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Formula-based cross-tabulation of data.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxCube<ept id="p1">](rxcube.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Alternative formula-based cross-tabulation designed for efficient representation returning cube results.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>Writing output to .xdf file not supported.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>rxMarginals</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Marginal summaries of cross-tabulations.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>as.xtabs</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>Converts cross tabulation results to an xtabs object.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>rxChiSquaredTest</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>Performs Chi-squared Test on xtabs object.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>Used with small data sets and does not chunk data.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>rxFisherTest</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>Performs Fisher's Exact Test on xtabs object.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Used with small data sets and does not chunk data.</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>rxKendallCor</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>Computes Kendall's Tau Rank Correlation Coefficient using xtabs object.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>rxPairwiseCrossTab</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Apply a function to pairwise combinations of rows and columns of an xtabs object.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>rxRiskRatio</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>Calculate the relative risk on a two-by-two xtabs object.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>rxOddsRatio</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>Calculate the odds ratio on a two-by-two xtabs object.</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p1">&lt;/sup&gt;</ept> Signifies the most popular functions in this category.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>6-Prediction functions</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>Function name</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxLinMod<ept id="p1">](rxlinmod.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>Fits a linear model to data.</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxLogit<ept id="p1">](rxlogit.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>Fits a logistic regression model to data.</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxGlm<ept id="p1">](rxglm.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>Fits a generalized linear model to data.</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxCovCor<ept id="p1">](rxcovcor.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>Calculate the covariance, correlation, or sum of squares / cross-product matrix for a set of variables.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxDTree<ept id="p1">](rxdtree.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>Fits a classification or regression tree to data.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxBTrees<ept id="p1">](rxbtrees.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>Fits a classification or regression decision forest to data using a stochastic gradient boosting algorithm.</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxDForest<ept id="p1">](rxdforest.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>Fits a classification or regression decision forest to data.</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxPredict<ept id="p1">](rxPredict.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>Calculates predictions for fitted models.</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>Output must be an XDF data source.</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxKmeans<ept id="p1">](rxkmeans.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>Performs k-means clustering.</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxNaiveBayes<ept id="p1">](rxnaivebayes.md)</ept> <bpt id="p2">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p2">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>Performs Naive Bayes classification.</source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>rxCov</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source>Calculate the covariance matrix for a set of variables.</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>rxCor</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>Calculate the correlation matrix for a set of variables.</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>rxSSCP</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>Calculate the sum of squares / cross-product matrix for a set of variables.</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>rxRoc</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>Receiver Operating Characteristic (ROC) computations using actual and predicted values from binary classifier system.</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;sup&gt;</bpt><ph id="ph1">*</ph><ept id="p1">&lt;/sup&gt;</ept> Signifies the most popular functions in this category.</source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>7-Compute context functions</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source>Function name</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source>RxComputeContext</source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source>Creates a compute context.</source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source>rxSetComputeContext</source>
        </trans-unit><trans-unit id="324" translate="yes" xml:space="preserve">
          <source>Sets a compute context.</source>
        </trans-unit><trans-unit id="325" translate="yes" xml:space="preserve">
          <source>rxGetComputeContext</source>
        </trans-unit><trans-unit id="326" translate="yes" xml:space="preserve">
          <source>Gets the current compute context.</source>
        </trans-unit><trans-unit id="327" translate="yes" xml:space="preserve">
          <source>RxSpark</source>
        </trans-unit><trans-unit id="328" translate="yes" xml:space="preserve">
          <source>Creates an in-data, file-based Spark compute context.</source>
        </trans-unit><trans-unit id="329" translate="yes" xml:space="preserve">
          <source>Computations are parallelized and distributed across the nodes of a Hadoop cluster via Apache Spark.</source>
        </trans-unit><trans-unit id="330" translate="yes" xml:space="preserve">
          <source>RxHadoopMR</source>
        </trans-unit><trans-unit id="331" translate="yes" xml:space="preserve">
          <source>Creates an in-data, file-based Hadoop compute context.</source>
        </trans-unit><trans-unit id="332" translate="yes" xml:space="preserve">
          <source>RxInTeradata</source>
        </trans-unit><trans-unit id="333" translate="yes" xml:space="preserve">
          <source>Creates an in-database compute context for Teradata.</source>
        </trans-unit><trans-unit id="334" translate="yes" xml:space="preserve">
          <source>RxInSqlServer</source>
        </trans-unit><trans-unit id="335" translate="yes" xml:space="preserve">
          <source>Creates an in-database compute context for SQL Server.</source>
        </trans-unit><trans-unit id="336" translate="yes" xml:space="preserve">
          <source>RxLocalSeq</source>
        </trans-unit><trans-unit id="337" translate="yes" xml:space="preserve">
          <source>Creates a local compute context for rxExec using sequential computations.</source>
        </trans-unit><trans-unit id="338" translate="yes" xml:space="preserve">
          <source>RxLocalParallel</source>
        </trans-unit><trans-unit id="339" translate="yes" xml:space="preserve">
          <source>Creates a local compute context for rxExec using the <bpt id="p1">*</bpt><ph id="ph1">\*</ph><ph id="ph2">\*</ph>parallel<ept id="p1">*</ept><ph id="ph3">\*</ph> package as backend.</source>
        </trans-unit><trans-unit id="340" translate="yes" xml:space="preserve">
          <source>RxForeachDoPar</source>
        </trans-unit><trans-unit id="341" translate="yes" xml:space="preserve">
          <source>Creates a compute context for rxExec using the current <bpt id="p1">**</bpt>foreach<ept id="p1">**</ept> parallel backend.</source>
        </trans-unit><trans-unit id="342" translate="yes" xml:space="preserve">
          <source>8-Distributed computing</source>
        </trans-unit><trans-unit id="343" translate="yes" xml:space="preserve">
          <source>These functions and many more can be used for high performance computing and distributed computing.</source>
        </trans-unit><trans-unit id="344" translate="yes" xml:space="preserve">
          <source>Learn more about the entire set of functions in <bpt id="p1">[</bpt>Distributed Computing<ept id="p1">](../../r/how-to-revoscaler-distributed-computing.md)</ept>.</source>
        </trans-unit><trans-unit id="345" translate="yes" xml:space="preserve">
          <source>Function name</source>
        </trans-unit><trans-unit id="346" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="347" translate="yes" xml:space="preserve">
          <source>rxExec</source>
        </trans-unit><trans-unit id="348" translate="yes" xml:space="preserve">
          <source>Run an arbitrary R function on nodes or cores of a cluster.</source>
        </trans-unit><trans-unit id="349" translate="yes" xml:space="preserve">
          <source>rxRngNewStream</source>
        </trans-unit><trans-unit id="350" translate="yes" xml:space="preserve">
          <source>Support for Parallel Random Number Generation.</source>
        </trans-unit><trans-unit id="351" translate="yes" xml:space="preserve">
          <source>rxRngDelStream</source>
        </trans-unit><trans-unit id="352" translate="yes" xml:space="preserve">
          <source>Support for Parallel Random Number Generation.</source>
        </trans-unit><trans-unit id="353" translate="yes" xml:space="preserve">
          <source>rxRngGetStream</source>
        </trans-unit><trans-unit id="354" translate="yes" xml:space="preserve">
          <source>Support for Parallel Random Number Generation.</source>
        </trans-unit><trans-unit id="355" translate="yes" xml:space="preserve">
          <source>rxRngSetStream</source>
        </trans-unit><trans-unit id="356" translate="yes" xml:space="preserve">
          <source>Support for Parallel Random Number Generation.</source>
        </trans-unit><trans-unit id="357" translate="yes" xml:space="preserve">
          <source>rxGetAvailableNodes</source>
        </trans-unit><trans-unit id="358" translate="yes" xml:space="preserve">
          <source>Get all the available nodes on a distributed compute context.</source>
        </trans-unit><trans-unit id="359" translate="yes" xml:space="preserve">
          <source>rxGetNodeInfo</source>
        </trans-unit><trans-unit id="360" translate="yes" xml:space="preserve">
          <source>Get information on nodes specified for a distributed compute context.</source>
        </trans-unit><trans-unit id="361" translate="yes" xml:space="preserve">
          <source>rxPingNodes</source>
        </trans-unit><trans-unit id="362" translate="yes" xml:space="preserve">
          <source>Test round trip from user through computation node(s) in a cluster or cloud.</source>
        </trans-unit><trans-unit id="363" translate="yes" xml:space="preserve">
          <source>rxGetJobStatus</source>
        </trans-unit><trans-unit id="364" translate="yes" xml:space="preserve">
          <source>Get the status of a non-waiting distributed computing job.</source>
        </trans-unit><trans-unit id="365" translate="yes" xml:space="preserve">
          <source>rxGetJobResults</source>
        </trans-unit><trans-unit id="366" translate="yes" xml:space="preserve">
          <source>Get the return object(s) of a non-waiting distributed computing job.</source>
        </trans-unit><trans-unit id="367" translate="yes" xml:space="preserve">
          <source>rxGetJobOutput</source>
        </trans-unit><trans-unit id="368" translate="yes" xml:space="preserve">
          <source>Get the console output from a non-waiting distributed computing job.</source>
        </trans-unit><trans-unit id="369" translate="yes" xml:space="preserve">
          <source>rxGetJobs</source>
        </trans-unit><trans-unit id="370" translate="yes" xml:space="preserve">
          <source>Get the available distributed computing job information objects.</source>
        </trans-unit><trans-unit id="371" translate="yes" xml:space="preserve">
          <source>rxLocateFile</source>
        </trans-unit><trans-unit id="372" translate="yes" xml:space="preserve">
          <source>Get the first occurrence of a specified input file in a set of specified paths.</source>
        </trans-unit><trans-unit id="373" translate="yes" xml:space="preserve">
          <source>9-Utility functions</source>
        </trans-unit><trans-unit id="374" translate="yes" xml:space="preserve">
          <source>Some of the utility functions are operational in local compute context only.</source>
        </trans-unit><trans-unit id="375" translate="yes" xml:space="preserve">
          <source>Check the documentation of individual functions to confirm.</source>
        </trans-unit><trans-unit id="376" translate="yes" xml:space="preserve">
          <source>Function name</source>
        </trans-unit><trans-unit id="377" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="378" translate="yes" xml:space="preserve">
          <source>rxOptions</source>
        </trans-unit><trans-unit id="379" translate="yes" xml:space="preserve">
          <source>Gets or sets a specific option.</source>
        </trans-unit><trans-unit id="380" translate="yes" xml:space="preserve">
          <source>rxGetOption</source>
        </trans-unit><trans-unit id="381" translate="yes" xml:space="preserve">
          <source>Retrieves a specific RevoScaleR option.</source>
        </trans-unit><trans-unit id="382" translate="yes" xml:space="preserve">
          <source>rxGetEnableThreadPool</source>
        </trans-unit><trans-unit id="383" translate="yes" xml:space="preserve">
          <source>Gets the current state of the thread pool, which on Linux can be either persistent or on-demand.</source>
        </trans-unit><trans-unit id="384" translate="yes" xml:space="preserve">
          <source>rxSetEnableThreadPool</source>
        </trans-unit><trans-unit id="385" translate="yes" xml:space="preserve">
          <source>Sets the thread pool state.</source>
        </trans-unit><trans-unit id="386" translate="yes" xml:space="preserve">
          <source>rxStepControl</source>
        </trans-unit><trans-unit id="387" translate="yes" xml:space="preserve">
          <source>Construct a variable.selection argument for rxLinMod.</source>
        </trans-unit><trans-unit id="388" translate="yes" xml:space="preserve">
          <source>10-Package management</source>
        </trans-unit><trans-unit id="389" translate="yes" xml:space="preserve">
          <source>Function name</source>
        </trans-unit><trans-unit id="390" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="391" translate="yes" xml:space="preserve">
          <source>rxInstallPackages</source>
        </trans-unit><trans-unit id="392" translate="yes" xml:space="preserve">
          <source>Installs a package.</source>
        </trans-unit><trans-unit id="393" translate="yes" xml:space="preserve">
          <source>rxInstalledPackages</source>
        </trans-unit><trans-unit id="394" translate="yes" xml:space="preserve">
          <source>Returns the list of installed packages for a compute context.</source>
        </trans-unit><trans-unit id="395" translate="yes" xml:space="preserve">
          <source>rxFindPackage</source>
        </trans-unit><trans-unit id="396" translate="yes" xml:space="preserve">
          <source>Returns the path to one or more packages for a compute context.</source>
        </trans-unit><trans-unit id="397" translate="yes" xml:space="preserve">
          <source>rxRemovePackages</source>
        </trans-unit><trans-unit id="398" translate="yes" xml:space="preserve">
          <source>Removes installed packages from a compute context.</source>
        </trans-unit><trans-unit id="399" translate="yes" xml:space="preserve">
          <source>rxSqlLibPaths</source>
        </trans-unit><trans-unit id="400" translate="yes" xml:space="preserve">
          <source>Gets the search path for the library trees for packages while executing inside the SQL server.</source>
        </trans-unit><trans-unit id="401" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="402" translate="yes" xml:space="preserve">
          <source>Add R packages to your computer by running setup:</source>
        </trans-unit><trans-unit id="403" translate="yes" xml:space="preserve">
          <source>Machine Learning Server</source>
        </trans-unit><trans-unit id="404" translate="yes" xml:space="preserve">
          <source>R Client</source>
        </trans-unit><trans-unit id="405" translate="yes" xml:space="preserve">
          <source>Next, follow these tutorials for hands-on experience:</source>
        </trans-unit><trans-unit id="406" translate="yes" xml:space="preserve">
          <source>Explore R and RevoScaleR in 25 functions</source>
        </trans-unit><trans-unit id="407" translate="yes" xml:space="preserve">
          <source>Quickstart: Run R Code</source>
        </trans-unit><trans-unit id="408" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="409" translate="yes" xml:space="preserve">
          <source>R Package Reference</source>
        </trans-unit></group></body></file></xliff>