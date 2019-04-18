<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="tutorial-revoscaler-data-import-transform.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4cea32d2711f4fe7535a334c316eb09f2e831c04b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">cea32d2711f4fe7535a334c316eb09f2e831c04b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\tutorial-revoscaler-data-import-transform.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Tutorial: Data import and exploration (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn how to import and explore data using the RevoScaleR functions in Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Tutorial: Data import and exploration using RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: Microsoft R Client, Machine Learning Server<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>In data-driven projects, one action item guaranteed to be on the list is data acquisition and exploration.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>In this tutorial, you will learn how to import a text-delimited .csv file into an R session and use functions from <bpt id="p1">[</bpt>RevoScaleR<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept> to ascertain the shape of the data.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>To load data, use <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> from the RevoScaleR function library.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> function converts source data into a columnar format for consumption in R and returns a data source object that wraps a dataset with useful metadata.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Optionally, by specifying an <bpt id="p1">*</bpt>outFile<ept id="p1">*</ept> parameter, you can create an XDF file if you want to persist the data for future calculations.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>R Client and Machine Learning Server are interchangeable in terms of RevoScaleR as long as <bpt id="p1">[</bpt>data fits into memory and processing is single-threaded<ept id="p1">](#chunking)</ept>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If datasets exceed memory, we recommend pushing the <bpt id="p1">[</bpt>compute context<ept id="p1">](concept-what-is-compute-context.md)</ept> to Machine Learning Server.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>What you will learn</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>How to load CSV data using <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> and optionally save it as an XDF</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>How to obtain information about the data structure</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Use parameters for selective import and conversion</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Summarize data</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Subset and transform data</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>To complete this tutorial as written, use an R console application and built-in data.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>On Windows, go to \Program Files\Microsoft\R Client\R_SERVER\bin\x64 and double-click <bpt id="p1">**</bpt>Rgui.exe<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>On Linux, at the command prompt, type <bpt id="p1">**</bpt>Revo64<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The command prompt for R is <ph id="ph1">`&gt;`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>You can hand-type case-sensitive R commands, or copy-paste multi-line commands at the console command prompt.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The R interpreter can queue up multiple commands and run them sequentially.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>How to locate built-in data</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept> provides both functions and built-in datasets, including the <bpt id="p2">*</bpt>AirlineDemoSmall.csv<ept id="p2">*</ept> file used in this tutorial.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The sample data directory is registered with RevoScaleR.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Its location can be returned through a "sampleDataDir" parameter on the <bpt id="p1">**</bpt>rxGetOption<ept id="p1">**</ept> function.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Open the R console or start a Revo64 session.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The RevoScaleR library is loaded automatically.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Retrieve the list of <bpt id="p1">[</bpt>sample data files<ept id="p1">](sample-built-in-data.md)</ept> provided in RevoScaleR by entering the following command at the <ph id="ph1">`&gt;`</ph> command prompt:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The open-source R <ph id="ph1">`list.files`</ph> command returns a file list provided by the RevoScaleR <bpt id="p1">**</bpt>rxGetOption<ept id="p1">**</ept> function and the <bpt id="p2">*</bpt>sampleDataDir<ept id="p2">*</ept> argument.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If you are a Windows user and new to R, be aware that R script is case-sensitive.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If you mistype rxGetOption or sampleDataDir, you will get an error instead of the file list.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>How to locate the working directory</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Both R and RevoScaleR use the <bpt id="p1">*</bpt>working directory<ept id="p1">*</ept> to store any files that you create.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The following open-source R command provides the working directory location: <ph id="ph1">`getwd()`</ph>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Depending on your environment, you might not have permission to save files to this directory.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>On Windows, if the output is something like <ph id="ph1">`C:/Program Files/Microsoft/ML Server/R_SERVER/bin/x64`</ph>, you won't have write permissions on that older.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>To change the working directory, run <ph id="ph1">`setwd("C:/Users/TEMP")`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Alternatively, specify a fully-qualified path to a writable directory whenever a file name is required (for example, <ph id="ph1">`outFile="C:/users/temp/airExample.xdf"`</ph> on an <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> call).</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Windows users, please note the direction of the path delimiter.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>By default, R script uses forward slashes as path delimiters.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>About the airline dataset</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>AirlineDemoSmall.csv<ept id="p1">*</ept> dataset is used in this tutorial.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>It's a subset of a larger dataset containing information on flight arrival and departure details for all commercial flights within the USA, from October 1987 to April 2008.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The file contains three columns of data: <bpt id="p1">*</bpt>ArrDelay<ept id="p1">*</ept>, <bpt id="p2">*</bpt>CRSDepTime<ept id="p2">*</ept>, and <bpt id="p3">*</bpt>DayOfWeek<ept id="p3">*</ept>, with a total of 600,000 rows.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Load data</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>As a first step, perform a preliminary import using the airline data.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Initially, the data is loaded as a data frame that exists only in memory.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>On the first line,<ph id="ph1">`mysource`</ph> is an object specifying source data created using R's <ph id="ph2">`file.path`</ph> command.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The folder path is provided through RevoScaleR's rxGetOption("sampleDataDir"), with "AirlineDemoSmall.csv" for the file.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>On line two, <ph id="ph1">`airXdfData`</ph> is a data source object returned by <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept>, which we can query to learn about data characteristics.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Save as XDF</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Although we could work with the data frame for the duration of the session, it often helps to save the data as an .xdf file for reuse at a later date.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>To create an .xdf file, run <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> with an <bpt id="p2">*</bpt>outFile<ept id="p2">*</ept> parameter specifying the name and a folder for which you have write permissions:</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Common errors occurring on your first file save exercise might include:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>"Error: '\u' used without hex digits in character string..." indicates an invalid path delimiter.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>R uses forward slash delimiters (/), even if the path is on the Windows file system.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>"Error in file &lt;&lt;file-name&gt;&gt;; Permission denied" is obviously a permission error.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Choosing a different folder or granting write-access to the current folder will resolve the error.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>About data storage in Machine Learning Server</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server, you can work with in-memory data as a <bpt id="p1">*</bpt>data frame<ept id="p1">*</ept>, or save it to disk as an <bpt id="p2">*</bpt>XDF file<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>As noted, <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> can create a data source object with or without the .xdf file.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>If you omit the <bpt id="p1">*</bpt>outFile<ept id="p1">*</ept> argument or set it NULL, the return object is a data frame containing the data.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>A data frame is the fundamental data structure in R and is fully supported in Machine Learning Server.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>It is tabular, composed of rows and columns, where columns contain variables and the first row, called the <bpt id="p1">*</bpt>header<ept id="p1">*</ept>, stores column names.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Subsequent rows provide data values for each variable associated with a single observation.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>A data frame is a temporary data structure, created when you load some data.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>It exists only for the duration of the session.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>An .xdf file is a binary file format native to Machine Learning Server, used for persisting data on disk.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>The organization of an .xdf file is column-based, one column per variable, which is optimum for the variable orientation of data used in statistics and predictive analytics.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>With .xdf, you can load subsets of the data for targeted analysis.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Also, .xdf files include precomputed metadata that is immediately available with no additional processing.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Creating an .xdf is not required, but when datasets are large or complex, .xdf files can help by compressing data and by allocating data into chunks that can be read and refreshed independently.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Additionally, on distributed file systems like Hadoop's HDFS, XDF files can store data in multiple physical files to accommodate very large datasets.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>You can use <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> to load all or part of an .xdf into a data frame by specifying an .xdf file as the input.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Doing so instantiates a data source object for the .xdf file, but without loading its data.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Having an object represent the data source can come in handy.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>It doesn’t take up much memory, and it can be used in many other RevoScaleR objects interchangeably with a data frame.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Examine object metadata</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>You should now have a <ph id="ph1">`mysource`</ph> object and an <ph id="ph2">`airXdfData`</ph> object representing the data source.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Once a data source object exists, you can use the <bpt id="p1">**</bpt>rxGetInfo<ept id="p1">**</ept> function to return metadata and learn more about the structure.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Adding the <bpt id="p1">*</bpt>getVarInfo<ept id="p1">*</ept> argument returns metadata about variables:</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Notice how the output includes the precomputed metadata for each variable, plus a summary of observations, variables, blocks, and compression information.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Variables are based on fields in the CSV file.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>In this case, there are 3 variables.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>From the output, we can determine whether the number of observations is large enough to warrant subdivision into smaller blocks.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Additionally, we can see which variables exist, the data type, and for numeric data, the range of values.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The presence of string variables is a consideration.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>To use this data in subsequent analysis, we might need to convert strings to numeric data for ArrDelay.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Likewise, we might want to convert DayOfWeek to a factor variable so that we can group observations by day.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>We can do all of these things in a subsequent import.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>To get just the variable information, use the standalone <bpt id="p1">**</bpt>rxGetVarInfo()<ept id="p1">**</ept> function to return precomputed metadata about variables in the .xdf file (for example, <ph id="ph1">`rxGetVarInfo(airXdfData)`</ph>).</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Convert on re-import</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> function takes multiple parameters that can be used to modify data during import.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>In this exercise, repeat the import and change the dataset at the same time.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>By adding parameters to <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept>, you can:</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Convert the string column, <bpt id="p1">*</bpt>DayOfWeek<ept id="p1">*</ept>, to a factor variable using the <bpt id="p2">*</bpt>stringsAsFactors<ept id="p2">*</ept> argument.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Convert missing values to a specific value, such as the letter M rather than the default NA.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Allocate rows into blocks that you can subsequently read and write in <bpt id="p1">*</bpt>chunks<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>By specifying the argument <bpt id="p1">*</bpt>rowsPerRead<ept id="p1">*</ept>, you can read and write the data in 3 blocks of 200,000 rows each.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Running this command refreshes the airXdfData data source object.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Metadata for the new object reflects the allocation of rows among 3 blocks and conversion of string-to-numeric data for both ArrDelay and DayOfWeek.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Control string conversion and factor level ordering</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Setting <bpt id="p1">*</bpt>stringsAsFactors<ept id="p1">*</ept> to TRUE has built-in behaviors that can have unintended consequences.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>For example, we might not want every character variable to become a factor.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>In the case of ArrDelay, the data is actually numeric.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>You can use the <bpt id="p1">*</bpt>colClasses<ept id="p1">*</ept> argument to explicitly set the data type of a particular variable.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Additionally, factor levels are listed arbitrarily in the order in which they are encountered during import, which might not make sense.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>To override the default, you can explicitly specify the levels in a predefined order using the <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Rerun the import operation to use a fixed data type for ArrDelay and a fixed order for days of the week:</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Notice that once you supply the <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> argument, you no longer need to specify <bpt id="p2">*</bpt>stringsAsFactors<ept id="p2">*</ept> because <bpt id="p3">*</bpt>DayOfWeek<ept id="p3">*</ept> is the only factor variable.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Visualize data</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>To get a sense of data shape, use the <bpt id="p1">**</bpt>rxHistogram<ept id="p1">**</ept> function to show the distribution in arrival delay by day of week.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Internally, this function uses the <bpt id="p1">**</bpt>rxCube<ept id="p1">**</ept> function to calculate information for a histogram:</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>You can also compute descriptive statistics for the variable:</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Create a new variable</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>This first look at the data tells us two important things: arrival delay has a long “tail” for every day of the week, with a few flights delayed for well over two hours, and there are quite a few missing values (17,372).</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Presumably the missing values for arrival delay represent flights that never arrived and thus canceled.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>You can use RevoScaleR’s data step functionality to create a new variable, <bpt id="p1">*</bpt>VeryLate<ept id="p1">*</ept>, that represents flights that were either over two hours late or canceled.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Because the original data is safely preserved in the original text file, we can simply add this variable to our existing XDF file using the <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept> argument to <bpt id="p2">**</bpt>rxDataStep<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept> argument takes a list of one or more R expressions, typically in the form of assignment statements.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>In this case, we use the following expression: <bpt id="p1">*</bpt>list(VeryLate = (ArrDelay <ph id="ph1">\&gt;</ph> 120 | is.na(ArrDelay))<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>The full RevoScaleR data step consists of the following steps:</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Read in the <bpt id="p1">*</bpt>data<ept id="p1">*</ept> a block (200,000 rows) at a time.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>For each block, pass the <bpt id="p1">*</bpt>ArrDelay<ept id="p1">*</ept> data to the R interpreter for processing the transformation to create <bpt id="p2">*</bpt>VeryLate<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Write the data out to the dataset a block at a time.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>The argument <bpt id="p1">*</bpt>overwrite=TRUE<ept id="p1">*</ept> allows us to overwrite the data file.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Output from this command reflects the creation of the new variable:</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Summarize data</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>We already used <bpt id="p1">**</bpt>rxSummary<ept id="p1">**</ept> to get an initial impression of data shape, but let's take a closer look at its arguments.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rxSummary<ept id="p1">**</ept> function takes a formula as its first argument, and the name of the dataset as the second.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>To get summary statistics for all of the data in your data file, you can alternatively use the R <bpt id="p1">*</bpt>summary<ept id="p1">*</ept> method for the <bpt id="p2">*</bpt>airXdfData<ept id="p2">*</ept> object.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>or</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Summary statistics will be computed on the variables in the formula.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>By default, <bpt id="p1">**</bpt>rxSummary<ept id="p1">**</ept> computes data summaries term-by-term, and missing values are omitted on a term-by-term basis.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Notice that the summary information shows cell counts for categorical variables, and appropriately does not provide summary statistics such as <bpt id="p1">*</bpt>Mean<ept id="p1">*</ept> and <bpt id="p2">*</bpt>StdDev<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Also notice that the <bpt id="p1">*</bpt>Call:<ept id="p1">*</ept> line will show the actual call you entered or the call provided by <bpt id="p2">*</bpt>summary<ept id="p2">*</ept>, so will appear differently in different circumstances.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>You can also compute summary information by one or more categories by using interactions of a numeric variable with a factor variable.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>For example, to compute summary statistics on Arrival Delay by Day of Week:</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>The output shows the summary statistics for <bpt id="p1">*</bpt>ArrDelay<ept id="p1">*</ept> for each day of the week:</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>To get a better feel for the data, you can draw histograms for each variable.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Run each <bpt id="p1">**</bpt>rxHistogram<ept id="p1">**</ept> function one at a time.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>The histogram is rendered in the R Plot pane.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>ArrDelay Histogram</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>CRSDepTime Histogram</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>DayOfWeek Histogram</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>We can also easily extract a subsample of the data file into a data frame in memory.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>For example, we can look at just the flights that were between 4 and 5 hours late:</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>ArrDelay Histogram</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Load a data subset</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>This exercise shows you how to use <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> to read an arbitrary chunk of the dataset into a data frame for further examination.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>As a first step, lets get the number of rows, columns, and return the initial rows to better understand the available data.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Standard R methods provide this information.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>From <bpt id="p1">*</bpt>nrow<ept id="p1">*</ept> we see that the number of rows is 600,000.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>To read 10 rows into a data frame starting with the 100,000th row:</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>This code should generate the following output:</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>You can now compute summary statistics on the reduced dataset</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Create a new dataset with variable transformations</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>In this task, use the <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> function to create a new dataset containing the variables in airXdfData plus additional variables created through transformations.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Typically additional variables are created using the <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>You can refer to <bpt id="p1">[</bpt>Transform functions<ept id="p1">](concept-what-is-data-transformations.md)</ept> for information.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Remember that all expressions used in <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept> must be able to be processed on a chunk of data at a time.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>In the example below, three new variables are created.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Late<ept id="p1">*</ept> is a logical variable set to <bpt id="p2">*</bpt>TRUE<ept id="p2">*</ept> (or <bpt id="p3">*</bpt>1<ept id="p3">*</ept>) if the flight was more than 15 minutes late in arriving.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>DepHour<ept id="p1">*</ept> is an integer variable indicating the hour of the departure.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Night<ept id="p1">*</ept> is also a logical variable, set to <bpt id="p2">*</bpt>TRUE<ept id="p2">*</ept> (or <bpt id="p3">*</bpt>1<ept id="p3">*</ept>) if the flight departed between 10 P.M.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>and 5 A.M.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> function will read the existing dataset and perform the transformations chunk by chunk, and create a new dataset.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>You should see the following information in your output:</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>This tutorial demonstrated data import and exploration, but there are several more tutorials covering more scenarios, including instructions for working with bigger datasets.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Tutorial: Visualize and analyze data<ept id="p1">](tutorial-revoscaler-data-model-analysis.md)</ept></source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Analyze large data with RevoScaleR and airline flight delay data<ept id="p1">](tutorial-revoscaler-large-data-airline.md)</ept></source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Example: Analyzing loan data with RevoScaleR<ept id="p1">](tutorial-revoscaler-large-data-loan.md)</ept></source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Example: Analyzing census data with RevoScaleR<ept id="p1">](tutorial-revoscaler-large-data-census.md)</ept></source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>Try demo scripts</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Another way to learn about RevoScaleR is through demo scripts.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>Scripts provided in your Machine Learning Server installation contain code that's very similar to what you see in the tutorials.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>You can highlight portions of the script, right-click <bpt id="p1">**</bpt>Execute in Interactive<ept id="p1">**</ept> to run the script in <bpt id="p2">[</bpt>R Tools for Visual Studio<ept id="p2">](https://www.visualstudio.com/vs/rtvs/)</ept>.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>Demo scripts are located in the <bpt id="p1">*</bpt>demoScripts<ept id="p1">*</ept> subdirectory of your Machine Learning Server installation.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>On Windows, this is typically:</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>Watch this video</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>This 30-minute video is the second in a 4-part video series.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>It demonstrates RevoScaleR functions for data ingestion.</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>This video shows you how to create a source object for a list of files by using the R <ph id="ph1">`list.files`</ph> function and patterns for selecting specific file names.</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>It uses the multiple mortDefaultSmall<ph id="ph1">&lt;em&gt;</ph>.csv files to show the approach.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>To create an XDF comprised of all the files, use the following syntax: <ph id="ph1">`mySourceFiles &lt;- list.files(rxGetOption("sampleDataDir"), pattern = "mortDefaultSmall\\d&lt;/em&gt;.csv", full.names=TRUE)`</ph>.</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;lt;</ph>div align=center<ph id="ph2">&amp;gt;</ph></source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>Overcome R Client data chunking limitations by pushing compute context or migrating to Machine Learning Server</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Data chunking<ept id="p1">*</ept> is a RevoScaleR capability that partitions data into multiple parts for processing in parallel, reassembling it later for analysis.</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>It's one of the key mechanisms by which RevoScaleR processes and analyzes very large datasets.</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server, chunking functionality is available only when RevoScaleR functions are executed on Machine Learning Server for Windows, Teradata, SQL Server, Linux, or Hadoop.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>You cannot use chunking on systems that have just Microsoft R Client.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>R Client requires that data fits into available memory.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>Moreover, it can only use a maximum of two threads for analysis.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>Internally, when RevoScaleR is running in R Client, the <ph id="ph1">`blocksPerRead`</ph> argument is deliberately, which results in all data being read into memory.</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>You can work around this limitation by writing script on R Client, but then <bpt id="p1">[</bpt>pushing the compute context<ept id="p1">](concept-what-is-compute-context.md)</ept> from R Client to a remote Machine Learning Server  instance.</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>Optionally, you could use Machine Learning Server.</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>Developers can install the developer edition of Machine Learning Server which is a full-featured Machine Learning Server, but licensed for development workstations instead of production servers.</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept>.</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept><ph id="ph1"> </ph></source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Getting Started with Hadoop and RevoScaleR<ept id="p1">](how-to-revoscaler-hadoop.md)</ept><ph id="ph1">  </ph></source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Parallel and distributed computing in Machine Learning Server<ept id="p1">](how-to-revoscaler-distributed-computing.md)</ept><ph id="ph1"> </ph></source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Importing data<ept id="p1">](how-to-revoscaler-data-import.md)</ept><ph id="ph1">   </ph></source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>ODBC data import<ept id="p1">](how-to-revoscaler-data-odbc.md)</ept><ph id="ph1">   </ph></source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR Functions<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept></source>
        </trans-unit></group></body></file></xliff>