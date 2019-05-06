<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="concept-what-is-xdf.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750a9917cd0f652b2c17cc0b3993abb1dc8f4cfcbd2.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a9917cd0f652b2c17cc0b3993abb1dc8f4cfcbd2</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\concept-what-is-xdf.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Create an XDF file (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to import CSV and other files to create an XDF file on Machine Learning Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Create an XDF file in Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>XDF is the native file format for persisted data in Machine Learning Server and it offers the following benefits:</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Compression, applied when the file is written to disk.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Columnar storage, one column per variable, for efficient read-write operations of variable data.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>In data science and machine learning, variables rather than rowsets are the data structures typically used in analysis.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Modular data access and management so that you can work with chunks of data at a time.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>XDF files are not strictly required for statistical analysis and data mining, but when data sets are large or complex, XDF offers stability in the form of persisted data under your control, plus the ability to subset and transform data for repeated analysis.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>To create an XDF file, use the <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> function in RevoScaleR to pipe external data to Machine Learning Server.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>By default, <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> loads data into an in-memory data frame, but by specifying the <bpt id="p2">*</bpt>outFile<ept id="p2">*</ept> parameter, <bpt id="p3">**</bpt>rxImport<ept id="p3">**</ept> creates an XDF file.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Example: Create an XDF</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>You can create an XDF using any data that can be loaded by <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept>, and by specifying an <bpt id="p2">*</bpt>outFile<ept id="p2">*</ept> consisting of a file path to a writable directory.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This example uses an R console and <bpt id="p1">[</bpt>sample data<ept id="p1">](sample-built-in-data.md)</ept> to create an XDF using data from a single CSV file.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>On Windows, you can run <bpt id="p1">**</bpt>Rgui.exe<ept id="p1">**</ept>, located at \Program Files\Microsoft\ML Server\R_SERVER\bin\x64.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>On Linux, you can type <bpt id="p1">**</bpt>Revo64<ept id="p1">**</ept> at the command line.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Notice the direction of the path delimiter.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>By default, R script uses forward slashes as path delimiters.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>At this point, the object is created, but the XDF file won't exist until you run <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> creates the file, builds and populates columns for each variable in the dataset, and then computes metadata for each variable and the XDF as a whole.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Output returned from this operation is as follows:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">**</bpt>rxGetInfo<ept id="p1">**</ept> function to return information about an object.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>In this case, the object is the XDF file created in a previous step, and the information returned is the precomputed metadata for each variable, plus a summary of observations, variables, blocks, and compression information.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Output is below.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Variables are based on fields in the CSV file.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>In this case, there are 6 variables.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Precomputed metadata about each one appears in the output below.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Set compression levels</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>You can set data compression via the <bpt id="p1">*</bpt>xdfCompressionLevel<ept id="p1">*</ept> argument to <bpt id="p2">**</bpt>rxImport<ept id="p2">**</ept> (and most other RevoScaleR functions that write .xdf files).</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>You specify this as an integer in the range -1 to 9.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The value -1 tells <bpt id="p1">*</bpt>rxImport<ept id="p1">*</ept> to use the current default compression value.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The integers 1 through 9 specify increasing levels of compression, where higher numbers perform more compression, but take more time.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The value 0 specifies no compression.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The .xdf format allows different blocks to have different compression levels (but not within a single call to <bpt id="p1">*</bpt>rxImport<ept id="p1">*</ept>).</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>This can be useful, for example, when appending to an existing data set of unknown compression level.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>You can specify the compression for the new data without affecting the compression of the existing data.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>You can specify a standard compression level for all future .xdf file writes by setting <bpt id="p1">*</bpt>xdfCompressionLevel<ept id="p1">*</ept> using <bpt id="p2">*</bpt>rxOptions<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>For example, to specify a compression level of 3, use <bpt id="p1">*</bpt>rxOptions<ept id="p1">*</ept> as follows:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The default value of this option is 1.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>If you have one or more existing .xdf files and would like to compress them, you can use the function <bpt id="p1">*</bpt>rxCompressXdf<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>You can specify a single file or xdf data source, a character vector of files and data sources, or the path to a directory containing .xdf files.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>For example, to compress all the .xdf files in the C:<ph id="ph1">\\</ph>data directory, you would call <bpt id="p1">*</bpt>rxCompressXdf<ept id="p1">*</ept> as follows:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Append new observations</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>If you have observations on the same variables in multiple input files, you can use the <bpt id="p1">*</bpt>append<ept id="p1">*</ept> argument to <bpt id="p2">**</bpt>rxImport<ept id="p2">**</ept> to combine them into one file.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>For example, we could append another copy of the claims text data set in a second block to the claimCAOrdered2.xdf file:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Read XDF data into a data frame</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>It is often convenient to store a large amount of data in an .xdf file and then read a subset of columns and rows of the data into a data frame in memory for analysis.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> function makes this easy.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>For example, let’s consider taking subsamples from the sample data set CensusWorkers.xdf.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Using a <bpt id="p1">*</bpt>rowSelection<ept id="p1">*</ept> expression and list of <bpt id="p2">*</bpt>varsToKeep<ept id="p2">*</ept>, we can extract the <bpt id="p3">*</bpt>age<ept id="p3">*</ept>, <bpt id="p4">*</bpt>perwt<ept id="p4">*</ept>, and <bpt id="p5">*</bpt>sex<ept id="p5">*</ept> variables for individuals over the age of 40 living in Washington State:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>When subsampling rows, we need to be aware that the rowSelection is processed on each chunk of data after it is read in.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Consider an example where we want to extract every 10<bpt id="p1">&lt;sup&gt;</bpt>th<ept id="p1">&lt;/sup&gt;</ept> row of the data set.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>For each chunk we will create a sequence starting with the start row number in that chunk (provided by the internal variable, .rxStartRow) with a length equal to the number of rows in the data chunk.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>We will determine that number of rows by using the length of one of the variables that has been read from the data set, age.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>We will keep only the rows where the remainder after dividing the row number by 10 is 0:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>We can also create transformed variables while we are reading in the data.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>For example, create an 10-year <bpt id="p1">*</bpt>ageGroup<ept id="p1">*</ept> variable, starting with 20 (the minimum age in the data set):</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Split an XDF into multiple files</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>RevoScaleR makes it possible to analyze huge data sets easily and efficiently, and for most purposes the most efficient computations are done on a single .xdf file.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>However, there are many circumstances when you will want to work with only a portion of your data.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>For example, you may want to distribute your data over the nodes of a cluster; in such a case, RevoScaleR’s analysis functions will process each node’s data separately, combining all the results for the final return value.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>You might also want to split your data into training and test data so that you can fit a model using the training data and validate it using the test data.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Use the function <bpt id="p1">**</bpt>rxSplit<ept id="p1">**</ept> to split your data.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>For example, to split variables of interest in the large 2000 U.S. Census data into five files for distribution on a five node cluster, you could use <bpt id="p1">**</bpt>rxSplit<ept id="p1">**</ept> as follows (change the location of the bigDataDir to the location of your downloaded file):</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>By default, <bpt id="p1">**</bpt>rxSplit<ept id="p1">**</ept> simply appends a number in the sequence from 1 to <bpt id="p2">*</bpt>numOutFiles<ept id="p2">*</ept> to the base file name to create the new file names, and in this case the resulting file names, for example, “Census5PCT20001.xdf”, are a bit confusing.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>You can exercise greater control over the output file names by using the <bpt id="p1">*</bpt>outFilesBase<ept id="p1">*</ept> and <bpt id="p2">*</bpt>outFilesSuffixes<ept id="p2">*</ept> arguments.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>With <bpt id="p1">*</bpt>outFilesBase<ept id="p1">*</ept>, you can specify either a single character string to be used for all files or a character vector the same length as the desired number of files.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The latter option is useful, for example, if you would like to create four files with the same file name, but different paths:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>This creates the four directories C:/compute10, etc., and creates a file named “DistCensusData.xdf” in each directory.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>You should adopt an approach like this when using distributed data with the standard RevoScaleR analysis functions such as <bpt id="p1">**</bpt>rxLinMod<ept id="p1">**</ept> and <bpt id="p2">**</bpt>rxLogit<ept id="p2">**</ept> in an <bpt id="p3">**</bpt>RxSpark<ept id="p3">**</ept> or <bpt id="p4">**</bpt>RxHadoopMR<ept id="p4">**</ept> compute context.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>You can supply the <bpt id="p1">*</bpt>outFilesSuffixes<ept id="p1">*</ept> arguments to exercise greater control over what is appended to the end of each file.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Returning to our first example, we can add a hyphen between our base file name and the sequence 1 to 5 using <bpt id="p1">*</bpt>outFilesSuffixes<ept id="p1">*</ept> as follows:</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>splitBy<ept id="p1">*</ept> argument specifies whether to split your data file row-by-row or block-by-block.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>The default is <bpt id="p1">*</bpt>splitBy="rows",<ept id="p1">*</ept> which distributes data from each block into different files.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>The examples above use the faster split by blocks instead.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>splitBy<ept id="p1">*</ept> argument is ignored if you also specify the <bpt id="p2">*</bpt>splitByFactor<ept id="p2">*</ept> argument as a character string representing a valid factor variable.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>In this case, one file is created per level of the factor variable.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>You can use the <bpt id="p1">*</bpt>splitByFactor<ept id="p1">*</ept> argument and a transforms argument to easily create test and training data sets from an .xdf file.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Note that this will take longer than the previous examples because each block of data is being processed:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>This takes approximately 10% of the data as a test data set, with the remainder going into the training data.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>If your .xdf file is relatively small, you may want to set <bpt id="p1">*</bpt>outFilesBase = ""<ept id="p1">*</ept> so that a list of data frames is returned instead of having files created.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>You can also use <bpt id="p1">**</bpt>rxSplit<ept id="p1">**</ept> to split data frames (see the <bpt id="p2">**</bpt>rxSplit<ept id="p2">**</ept> help page for details).</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Re-Block an .xdf File</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>After a series of data import or row selection steps, you may find that you have an .xdf file with very uneven block sizes.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>This may make it difficult to efficiently perform computations by “chunk.”</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>To find the sizes of the blocks in your .xdf file, use <bpt id="p1">**</bpt>rxGetInf<ept id="p1">**</ept> with the <bpt id="p2">*</bpt>getBlockSizes<ept id="p2">*</ept> argument set to TRUE.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>For example, let’s look at the block sizes for the sample CensusWorkers.xdf file:</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>The following information is provided:</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>We see that, in fact, the number of rows per block varies from a low of 1799 to a high of 131,234.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>To create a new file with more even-sized blocks, use the <bpt id="p1">*</bpt>rowsPerRead<ept id="p1">*</ept> argument in <bpt id="p2">**</bpt>rxDataStep<ept id="p2">**</ept>:</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>The new file has blocks sizes of 60,000 for all but the last slightly smaller block:</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>XDF is optimized for distributed file storage and access in the Hadoop Distributed File System (HDFS).</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>To learn more about using XDF in HDFS, see <bpt id="p1">[</bpt>Import and consume HDFS data files<ept id="p1">](how-to-revoscaler-data-hdfs.md)</ept>.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>You can import multiple text files into a single XDF.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>For instructions, see <bpt id="p1">[</bpt>Import text data<ept id="p1">](how-to-revoscaler-data-import.md)</ept>.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept> <bpt id="p2">[</bpt>Install Machine Learning Server on Windows<ept id="p2">](../install/machine-learning-server-windows-install.md)</ept></source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server on Linux</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server on Hadoop</source>
        </trans-unit></group></body></file></xliff>