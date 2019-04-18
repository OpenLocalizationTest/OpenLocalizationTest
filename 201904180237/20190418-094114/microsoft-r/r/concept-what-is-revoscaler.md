<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="concept-what-is-revoscaler.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926b23fc13dfd44549ef78dd85f04e257236630d35d.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">b23fc13dfd44549ef78dd85f04e257236630d35d</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\concept-what-is-revoscaler.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Get started with RevoScaleR - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn about the benefits of RevoScaleR and how to use it in custom script and code.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>What is RevoScaleR?</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RevoScaleR is a collection of proprietary functions in Machine Learning Server used for practicing data science at scale.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>For data scientists, RevoScaleR gives you data-related functions for import, transformation and manipulation, summarization, visualization, and analysis.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>At scale<ept id="p1">*</ept> refers to the core engine's ability to perform these tasks against very large datasets, in parallel and on distributed file systems, chunking and reconstituting data when it cannot fit in memory.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>RevoScaleR functions are provided through the <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> package installed for free in <bpt id="p2">[</bpt>Microsoft R Client<ept id="p2">](../r-client/what-is-microsoft-r-client.md)</ept> or commercially in <bpt id="p3">[</bpt>Machine Learning Server<ept id="p3">](../what-is-machine-learning-server.md)</ept> on supported platforms.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>RevoScaleR is also embedded in Azure HDInsight, Azure Data Science virtual machines, and SQL Server.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The RevoScaleR functions run on a computational engine include in the aforementioned products.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>As such, the package cannot be downloaded or used independently of the products and services that provide it.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>RevoScaleR is engineered to adapt to the computational power of the platform it runs on.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>On Machine Learning Server for Hadoop, script using RevoScaleR functions that run in parallel will automatically use nodes in the cluster.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Whereas on the free R Client, scale is provided at much lower levels (2 processors, data resides in-memory).</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>RevoScaleR provides enhanced capabilities to many elements of the open-source R programming language.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>In fact, there are <bpt id="p1">[</bpt>RevoScaleR equivalents for many common base R functions<ept id="p1">](../r-reference/revoscaler/revoscaler-compared-to-base-r.md)</ept>, such as <bpt id="p2">*</bpt>rxSort<ept id="p2">*</ept> for <bpt id="p3">*</bpt>sort()<ept id="p3">*</ept>, <bpt id="p4">*</bpt>rxMerge<ept id="p4">*</ept> for <bpt id="p5">*</bpt>merge()<ept id="p5">*</ept>, and so forth.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Because RevoScaleR is compatible with the open-source R language, solutions often use a combination of base R and RevoScaleR functions.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>RevoScaleR functions are denoted with an <bpt id="p1">**</bpt>rx<ept id="p1">**</ept> or <bpt id="p2">**</bpt>Rx<ept id="p2">**</ept> prefix to make them readily identifiable in your R script that uses the RevoScaleR package.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>What can you do with RevoScaleR?</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Data scientists and developers can include RevoScaleR functions in custom script or solutions that run locally against R Client or remotely on Machine Learning Server.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Solutions leveraging RevoScaleR functions will run wherever the RevoScaleR engine is installed.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Analyzing data using RevoScaleR functions requires three distinct pieces of information:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Where the computations should take place (the compute context)</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Which data to use (the data source)</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>What analysis to perform (the analysis function)</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>A common workflow is to write the initial code or script against a subset of data on a local computer, change the compute context to specify a large set of data on a big data platform, and then operationalize the solution by deploying it to the target environment, thus making it accessible to users.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>At a high level, RevoScaleR functions are grouped as follows:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Platform-specific utilities.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Data-related functions are used for import, transformation, summarization, visualization, and analysis.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>These functions comprise the bulk of the RevoScaleR function library.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The data manipulation and analysis functions in RevoScaleR are appropriate for small and large datasets, but are particularly useful in three common situations:</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Analyze data sets that are too big to fit in memory.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Perform computations distributed over several cores, processors, or nodes in a cluster.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Create scalable data analysis routines that can be developed locally with smaller data sets, then deployed to larger data and/or a cluster of computers.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>RevoScaleR enables these scenarios because it operates on chunks of data and uses <bpt id="p1">*</bpt>updating algorithms<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Data is stored in an efficient XDF file format designed for rapid reading of arbitrary rows and columns of data.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Functions in RevoScaleR are used to import data into XDF before performing analysis, but you can also work directly with data stored in a text, SPSS, or SAS file or an ODBC connection, or extract a subset of a data file into a data frame in memory for further analysis.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>To perform an analysis, you must provide the following information: where the computations should take place (the compute context), the data to use (the data source), and what analysis to perform (the analysis function).</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Data management and analysis using RevoScaleR</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>RevoScaleR provides functions for scalable data management and analysis.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>These functions can be used with data sets in memory, and applied the same way to huge data sets stored on disk.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>It includes functionality for:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Accessing external data sets (SAS, SPSS, ODBC, Teradata, and delimited and fixed format text) for analysis in R</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Efficiently storing and retrieving data in a high performance data file</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Cleaning, exploring, and manipulating data</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Fast, basic statistical analyses</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>RevoScaleR also includes an extensible framework for writing your own analyses for big data sets.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>With RevoScaleR, you can analyze data sets far larger than can be kept in memory.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>This is possible because RevoScaleR uses external memory algorithms that allow it to work on one chunk of data at a time (that is, a subset of the rows and perhaps the variables in the data set), update the results, and proceed through all available data.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Accessing External Data Sets</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Data can be stored in a wide-variety of formats.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Typically, the first step in any RevoScaleR analysis is to make the data accessible.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>With RevoScaleR’s data import capability, you can access data from a SAS file, SPSS file, fixed format or delimited text file, an ODBC connection, SQL Server, or a Teradata database, bringing it into a data frame in memory, or storing it for fast access in chunks on disk.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Defining Compute Context</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>RevoScaleR has the concept of <bpt id="p1">*</bpt>compute context<ept id="p1">*</ept> that sets the location for calculations.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>The compute context is either local or remote, where remote offloads processing and analysis of chunked data to one or more remote Machine Learning Servers.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Local is the default, and it supports the full range of data source inputs.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>As its name suggests, a local compute context uses only the physical cores of the local computer.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Local compute context is provided by RevoScaleR on both R Client and Machine Learning Server instances.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Remote compute context requires the explicit creation of a compute context object, a single logical object defining location (a remote network resource that has Machine Learning Server and local data) and modes of processing (such as wait versus no-wait jobs).</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Remote compute context is supported for RevoScaleR analytical functions that can be performed in a distributed fashion, and is available on these platforms in Machine Learning Server only: HDInsight, Hadoop (Spark), Teradata, SQL Server, and Machine Learning Server (Windows and Linux).</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Compute Context<ept id="p1">](concept-what-is-compute-context.md)</ept>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Efficiently Storing and Retrieving Data</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>A key component of RevoScaleR is a data file format (.xdf) that is extremely efficient for both reading and writing data.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>You can create .xdf files by importing data files or from R data frames, and add rows or variables to an existing .xdf file (appending rows is currently only supported in a local compute context).</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Once your data is in this file format you can use it directly with analysis functions provided with RevoScaleR, or quickly extract a subsample and read it into a data frame in memory for use in other R functions.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Data Cleaning, Exploration, and Manipulation</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>When working with a new data set, the first step is to clean and explore.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>With RevoScaleR, you can quickly obtain information about your data set (e.g., how many rows and variables) and the variables in your data set (such as name, data type, value labels).</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>With RevoScaleR’s summary statistics and cube functionality, you can examine summary information about your data and quickly plot histograms or relationships between variables.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>RevoScaleR also provides all of the power of R to use in data transformations and manipulations.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>In RevoScaleR’s data step functionality, you can specify R expressions to transform specific variables and have them automatically applied to a single data frame or to each block of data as it is read in from an .xdf file.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>You can create new variables, recode variables, and set missing values with all the flexibility of the R language.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Statistical Analysis</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>In addition to descriptive statistics and crosstabs, RevoScaleR provides functions for fitting linear and binary logistic regression models, generalized linear models, k-means models, and decision trees and forests, among others.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>These functions access .xdf files or other data sources directly or operate on data frames in memory.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Because these functions are so efficient and do not require that all of the data be in memory at one time, you can analyze huge data sets without requiring huge computing power.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>In particular, you can relax assumptions previously required.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>For example, instead of assuming a linear or polynomial functional form in a model, you can break independent variables into many categories providing a completely flexible functional form.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>The many degrees of freedom provided by large data sets, combined with RevoScaleR’s efficiency, make this approach feasible.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Writing Your Own Analyses for Large Data Sets</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>All of the main analysis functions in RevoScaleR use updating or external memory algorithms, that is, they analyze a chunk of data, update the results, then move on to the next chunk of data and repeat the process.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>When all the data has been processed (sometimes multiple times), final results can be calculated and the analysis is complete.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>You can write your own functions to process a chunk of data and update results, and use RevoScaleR functionality to provide you with access to your data file chunk by chunk.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Write custom chunking algorithms in RevoScaleR<ept id="p1">](how-to-developer-write-chunking-algorithms.md)</ept>.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Introduction to Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept><ph id="ph1"> </ph></source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How-to guides for Machine Learning Server<ept id="p1">](how-to-introduction.md)</ept> <bpt id="p2">[</bpt>RevoScaleR Functions<ept id="p2">](~/r-reference/revoscaler/revoscaler.md)</ept></source>
        </trans-unit></group></body></file></xliff>