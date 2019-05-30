<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-data-import.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e59a042bce87eb59f479faf6fe76d2c830af4795d.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">59a042bce87eb59f479faf6fe76d2c830af4795d</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-data-import.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Import text, SAS, and SPSS data into Machine Learning Server using rxImport</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Load data in Machine Learning Server using the RevoScaleR rxImport function.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Importing text data in Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RevoScaleR can use data from a wide range of external data sources, including text files, database files on disk (SPSS and SAS), and relational data sources.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>This article puts the focus on text files: delimited (.csv) and fixed-format, plus database files accessed through simple file reads.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>To store text data for analysis and visualization, you can load it into memory as a <bpt id="p1">*</bpt>data frame<ept id="p1">*</ept> for the duration of your session, or save it to disk as a .xdf file.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>For either approach, the RevoScaleR <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> function loads the data.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>To get the best use of persisted data in XDF, you need Machine Learning Server (as opposed to R Client).</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Reading and writing <bpt id="p1">*</bpt>chunked data<ept id="p1">*</ept> on disk is exclusive to Machine Learning Server.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>About rxImport</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Converting external data into a format understood by RevoScaleR is achieved using the <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> function.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Although the function takes several arguments, it's just loading data from a source file that you provide.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>In the simplest case, you can give it a file path.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If the data is delimited by commas or tabs, this is all that is required loading the data.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>To illustrate, the following example creates a data object loaded with data from a local text-delimited file:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Depending on arguments, <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> either loads data as a data frame, or outputs the data to a .xdf file saved to disk.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>This article covers a range of data access scenarios for text files and file-based data access of SPSS and SAS data.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>To learn more about other data sources, see related articles in the table of contents or in the link list at the end of this article.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>How to import a text file</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Set the location of the source file.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>One approach is to use R's <ph id="ph1">`file.path`</ph> command.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>To try this out using <bpt id="p1">[</bpt>built-in samples<ept id="p1">](sample-built-in-data.md)</ept>, run the first command to verify the files are available, and the second command to set the location and source file.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Run <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> to load the data into a data frame.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Follow up with the <bpt id="p1">**</bpt>rxGetInfo<ept id="p1">**</ept> function to get summary information.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If we include the argument <bpt id="p1">*</bpt>getVarInfo=TRUE<ept id="p1">*</ept>, the summary includes the names of the variables and their types:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>For just variables in the data file, use the <bpt id="p1">*</bpt>names<ept id="p1">*</ept> function:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>To save the data into a .xdf file rather than importing data into a data frame in memory, add the <bpt id="p1">*</bpt>outFile<ept id="p1">*</ept> parameter.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Specify a path to a writable directory:</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>A .xdf file is created, and instead of returning a data frame, the <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> function returns a data source object.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>This is a small R object that contains information about a data source, in this case the name and path of the .xdf file it represents.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>This data source object can be used as the input data in most RevoScaleR functions.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Optionally, you can simplify the path designation by using the working directory.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Use R's working directory commands to get and set the folder.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Run the first command to determine the default working directory, and the second command to switch to a writable folder.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Modifications during import</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>During import, you can fix problems in the underlying data by specifying arguments for replacement values, changing metadata on the variable, changing data types, and creating new variables based on calculations.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Set a replacement string</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If your text data file uses a string other than NA to identify missing values, you can use the <bpt id="p1">*</bpt>missingValueString<ept id="p1">*</ept> argument to define the replacement string.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Only one missing value string is allowed per file.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The following example is from the <bpt id="p1">[</bpt>Airline demo tutorial<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept>:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Change variable metadata</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>If you need to modify the name of a variable or the names of the factor levels, or add a description of a variable, you can do this using the <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>For example, the claims data includes a variable <bpt id="p1">*</bpt>type<ept id="p1">*</ept> specifying the type of car, but the levels A, B, C, and D give us no particular information.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>If we knew what the types signified, perhaps “Subcompact”, “Compact”, “Mid-size”, and “Full-size”, we could relabel the levels as follows:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>This produces the following output:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>To specify <bpt id="p1">*</bpt>newLevels<ept id="p1">*</ept>, you must also specify <bpt id="p2">*</bpt>levels<ept id="p2">*</ept>, and it is important to note that the <bpt id="p3">*</bpt>newLevels<ept id="p3">*</ept> argument can only be used to rename levels.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>It cannot be used to fully recode the factor.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>That is, the number of <bpt id="p1">*</bpt>levels<ept id="p1">*</ept> and number of <bpt id="p2">*</bpt>newLevels<ept id="p2">*</ept> must be the same.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Change data types</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> function supports three arguments for specifying variable data types: <bpt id="p2">*</bpt>stringsAsFactors<ept id="p2">*</ept>, <bpt id="p3">*</bpt>colClasses<ept id="p3">*</ept>, and <bpt id="p4">*</bpt>colInfo<ept id="p4">*</ept>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>For example, consider storing character data.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Often data stored in text files as string data actually represents categorical or <bpt id="p1">*</bpt>factor<ept id="p1">*</ept> data, which can be more compactly represented as a set of integers denoting the distinct <bpt id="p2">*</bpt>levels<ept id="p2">*</ept> of the factor.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>This is common enough that users frequently want to transform <bpt id="p1">*</bpt>all<ept id="p1">*</ept> string data to factors.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>This can be done using the <bpt id="p1">*</bpt>stringsAsFactors<ept id="p1">*</ept> argument:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>You can also specify data types for individual variables using the <bpt id="p1">*</bpt>colClasses<ept id="p1">*</ept> argument, and even more specific instructions for converting each variable using the <bpt id="p2">*</bpt>colInfo<ept id="p2">*</ept> argument.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Here we use the <bpt id="p1">*</bpt>colClasses<ept id="p1">*</ept> argument to specify that the variable <bpt id="p2">*</bpt>number<ept id="p2">*</ept> in the claims data be stored as an integer:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>We can use the <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> argument to specify the levels of the <bpt id="p2">*</bpt>car.age<ept id="p2">*</ept> column.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>This is useful when reading data in chunks, to assure that factors levels are in the desired order.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Gives the following output:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>These various methods of providing column information can be combined as follows:</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Produces the following output:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>In general, variable specifications provided by the <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> argument are used in preference to <bpt id="p2">*</bpt>colClasses<ept id="p2">*</ept>, and those in <bpt id="p3">*</bpt>colClasses<ept id="p3">*</ept> are used in preference to the <bpt id="p4">*</bpt>stringsAsFactors<ept id="p4">*</ept> argument.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Also note that the .xdf data format supports a wider variety of data types than R, allowing for efficient storage.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>For example, by default floating point variables are stored as 32-bit floats in .xdf files.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>When they are read into R for processing, they are converted to doubles (64-bit floats).</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Create or modify variables</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>You can use the <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept> argument to <bpt id="p2">**</bpt>rxImport<ept id="p2">**</ept> to create new variables or modify existing variables when you initially read the data into .xdf format.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>For example, we could create a new variable, <bpt id="p1">*</bpt>logcost<ept id="p1">*</ept>, by taking the log of the existing cost variable as follows:</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Gives the following output, showing the new variable:</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Change date formats</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>The .xdf format can store dates using the standard R <bpt id="p1">**</bpt>Date<ept id="p1">**</ept> class.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>When importing data from other data formats that support dates such as SAS or SPSS, the <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> function converts dates data automatically.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>However, some data sets even in those formats include dates as character string data.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>You can store such data more efficiently by converting it to <bpt id="p1">*</bpt>Date<ept id="p1">*</ept> data using the <bpt id="p2">*</bpt>transforms<ept id="p2">*</ept> argument.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>For example, suppose you have a character variable <bpt id="p1">*</bpt>TransactionDate<ept id="p1">*</ept> with a representative date of the form "14 Sep 2017".</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>You could convert this to a <bpt id="p1">*</bpt>Date<ept id="p1">*</ept> variable using the following <bpt id="p2">*</bpt>transforms<ept id="p2">*</ept> argument:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>format<ept id="p1">*</ept> argument is a character string that may contain conversion specifications, as in the example shown.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>These conversion specifications are described in the <bpt id="p1">*</bpt>strptime<ept id="p1">*</ept> help file.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Change a delimiter</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>You cannot create or modify delimiters through <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept>, but for text data, you can create an <bpt id="p2">**</bpt>RxTextData<ept id="p2">**</ept> data source and specify the delimiter using the <bpt id="p3">*</bpt>delimiter<ept id="p3">*</ept> argument.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>For more information about creating a data source object, see <bpt id="p1">[</bpt>Data Sources in Microsoft R<ept id="p1">](how-to-revoscaler-data-source.md)</ept>.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>As a simple example, RevoScaleR includes a sample text data file hyphens.txt that is not separated by commas or tabs, but by hyphens, with the following contents:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>By creating an <bpt id="p1">**</bpt>RxTextData<ept id="p1">**</ept> data source for this file, you can specify the delimiter using the <bpt id="p2">*</bpt>delimiter<ept id="p2">*</ept> argument:</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>In normal usage, the <bpt id="p1">*</bpt>delimiter<ept id="p1">*</ept> argument is a single character, such as <bpt id="p2">*</bpt>delimiter="<ph id="ph1">\\</ph>t"<ept id="p2">*</ept> for tab-delimited data or <bpt id="p3">*</bpt>delimiter=","<ept id="p3">*</ept> for comma-delimited data.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>However, each column may be delimited by a different character; all the delimiters must be concatenated together into a single character string.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>For example, if you have one column delimited by a comma, a second by a plus sign, and a third by a tab, you would use the argument *delimiter=",+<ph id="ph1">\\</ph>t".</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>This section provides example script demonstrating additional import tasks.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Import multiple files</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>This example demonstrates an approach for importing multiple text files at once.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>You can use <bpt id="p1">[</bpt>sample data<ept id="p1">](sample-built-in-data.md)</ept> for this exercise.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>It includes mortgage default data for consecutive years, with each year's data in a separate file.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>In this exercise, you will import all of them to a single XDF by appending one after another, using a combination of base R commands and RevoScaleR functions.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Create a source object for a list of files, obtained using the R <ph id="ph1">`list.files`</ph> function with a pattern for selecting specific file names:</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Create an object for the XDF file at a writable location:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>To iterate over multiple files, use the R <ph id="ph1">`lapply`</ph> function and create a function to call <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> with the <bpt id="p2">**</bpt>append<ept id="p2">**</ept> argument.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Importing multiple files requires the <bpt id="p1">**</bpt>append<ept id="p1">**</ept> argument on <bpt id="p2">**</bpt>rxImport<ept id="p2">**</ept> to avoid overwriting existing content from the first iteration.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Each new chunk of data is imported as a block.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Partial output from this operation reports out the processing details.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Use <bpt id="p1">**</bpt>rxGetInfo<ept id="p1">**</ept> to view precomputed metadata.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>As you would expect, the block count reflects the presence of multiple concatenated data sets.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Results from this command confirm that you have 10 blocks, one for each .csv file.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>On a distributed file system, you could place these blocks on separate nodes.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>You could also retrieve or overwrite individual blocks.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Import and consume data on HDFS<ept id="p1">](how-to-revoscaler-data-hdfs.md)</ept> and <bpt id="p2">[</bpt>XDF files<ept id="p2">](concept-what-is-xdf.md)</ept>.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Import fixed-format data</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Fixed-format<ept id="p1">*</ept> data is text data in which each variable occupies a fixed-width column in the input data file.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Column width, rather than a delimiter, gives the data its structure.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>You can import fixed-format data using the <bpt id="p1">*</bpt>rxImport<ept id="p1">*</ept> function.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Optionally, fixed-format data might be associated with a <bpt id="p1">*</bpt>schema file<ept id="p1">*</ept> having a .sts extension.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>The schema describes the width and type of each column.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>For complete details on creating a schema file, see page 93 of the Stat/Transfer PDF Manual (<ph id="ph1">&lt;http://www.stattransfer.com/stman10.pdf&gt;</ph>).</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>If you have a schema file, you can create the input data source simply by specifying the schema file name as the input data file.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>built-in samples<ept id="p1">](sample-built-in-data.md)</ept> include a fixed-format version of the claims data as the file claims.dat and a schema file named claims.sts.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>To import the data using this schema file, we use <bpt id="p1">*</bpt>RxImport<ept id="p1">*</ept> as follows:</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Return summary information using <bpt id="p1">*</bpt>rxGetInfo<ept id="p1">*</ept>:</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>To read all string data as factors, set the <bpt id="p1">*</bpt>stringsAsFactors<ept id="p1">*</ept> argument to <bpt id="p2">*</bpt>TRUE<ept id="p2">*</ept> in your call to <bpt id="p3">*</bpt>rxImport<ept id="p3">*</ept></source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>If you have fixed-format data without a schema file, you can specify the start, width, and type information for each variable using the <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> argument to the <bpt id="p2">*</bpt>RxTextData<ept id="p2">*</ept> data source constructor, and then read in the data using <bpt id="p3">*</bpt>rxImport<ept id="p3">*</ept>:</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>If you have a schema file, you can still use the <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> argument to specify type information or factor level information.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>However, in this case, all the variables are read according to the schema file, and then the <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> data specifications are applied.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>This means that you cannot use your <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> list to omit variables, as you can when there is no schema file.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Fixed-width character data is treated as a special type by RevoScaleR for efficiency purposes.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>You can use this same type for character data in delimited data by specifying a colInfo argument with a width argument for the character column.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>(Typically, you need to find the longest string in the column and specify a width sufficient to include it.)</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Import SAS data</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> function can also be used to read data from SAS files having a .sas7bdat or .sd7 extension.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>You do not need to have SAS installed on your computer; simple file access is used to read in the data.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>The sample directory contains a SAS version of the claims data as claims.sas7bdat.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>We can read it into .xdf format most simply as follows:</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Gives the following output:</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Sometimes, SAS data files on Windows come in two pieces, a <bpt id="p1">*</bpt>.sas7bdat<ept id="p1">*</ept> file containing the data and a <bpt id="p2">*</bpt>.sas7bcat<ept id="p2">*</ept> file containing value label information.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>You can read both the data and the value label information by specifying the <bpt id="p1">*</bpt>.sas7bdat<ept id="p1">*</ept> file with the <bpt id="p2">*</bpt>inData<ept id="p2">*</ept> argument and the <bpt id="p3">*</bpt>.sas7bcat<ept id="p3">*</ept> file with the <bpt id="p4">*</bpt>formatFile<ept id="p4">*</ept> argument.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>To do so, in the following code replace <bpt id="p1">*</bpt>myfile<ept id="p1">*</ept> with your SAS file name:</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Import SPSS data</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> function can also be used to read data from SPSS files.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>The sample directory contains an SPSS version of the claims data as claims.sav.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>We can read it into .xdf format as follows:</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Gives the following output:</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Variables in SPSS data sets often contain value labels with important information about the data.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>SPSS variables with value labels are typically most usefully imported into R as categorical “factor” data; that is, there is a one-to-one mapping between the values in the data set (such as 1, 2, 3) and the labels that apply to them (Gold, Silver, Bronze).</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Interestingly, SPSS allows for value labels on a subset of existing values.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>For example, a variable with values from 1 to 99 might have value labels of “NOT HOME” for 97, “DIDN’T KNOW” for 98, and “NOT APPLICABLE” for 99.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>If this variable is converted to a factor in R using the value labels as the factor labels, all of the values from 1 to 96 would be set to missing because there would be no corresponding factor level.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Essentially all of the actual data would be thrown away.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>To avoid data loss when converting to factors, use the flag <bpt id="p1">*</bpt>labelsAsLevels=FALSE<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>By default, the information from the value labels is retained even if the variables aren’t converted to factors.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>This information can be returned using <bpt id="p1">**</bpt>rxGetVarInfo<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>If you don’t wish to retain the information from the value labels, you can specify <bpt id="p1">*</bpt>labelsAsInfo=FALSE<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Importing wide data</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Big data mainly comes in two forms, long or wide, each presenting unique challenges.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>The common case is long data, having many observations relative to the number of variables in the data set.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>With wide data, or data sets with a large number of variables, there are specific considerations to take into account during import.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>First, we recommend importing wide data into the .xdf format using the <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> function whenever you plan to do repeated analyses on your dat aset.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Doing so allows you to read subsets of columns into a data frame in memory for specific analyses.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Transform and subset data<ept id="p1">](how-to-revoscaler-data-transform.md)</ept>.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Second, review the data set for categorical variables that can be marked as factors.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>If possible use the <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> argument to define the levels rather than <bpt id="p2">*</bpt>stringsAsFactors<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Explicitly setting the levels results in faster processing speeds because you avoid recomputations of variable metadata whenever a new level is encountered.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>For wide data sets having a very large number of variables, the extra processing due to recomputation can be significant so its worth considering the <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> argument as a way to speed up the import.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Third, if you are using <bpt id="p1">*</bpt>colinfo<ept id="p1">*</ept>, considering creating it as an object prior to using <bpt id="p2">**</bpt>rxImport<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>The following is an example of defining the colInfo with factor levels for the claims data from earlier examples:</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>The colInfo list can then be used as the <bpt id="p1">*</bpt>colInfo<ept id="p1">*</ept> argument in the <bpt id="p2">**</bpt>rxImport<ept id="p2">**</ept> function to get your data into .xdf format:</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>Continue on to the following data import articles to learn more about XDF, data source objects, and other data formats:</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>XDF files</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Data Sources</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Import relational data using ODBC</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>Import and consume data on HDFS</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>Tutorial: data import</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>Tutorial: data manipulation</source>
        </trans-unit></group></body></file></xliff>