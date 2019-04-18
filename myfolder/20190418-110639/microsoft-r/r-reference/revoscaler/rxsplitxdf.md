<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxsplitxdf.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907faf16cd4824a7c2d3908157bddc0882d326a7ad23.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">af16cd4824a7c2d3908157bddc0882d326a7ad23</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxsplitxdf.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxSplitXdf function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxSplitXdf, rxSplit, manip, file</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>rxSplitXdf: Split a Single Data Set into Multiple Sets</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Split an input .xdf file or data frame into multiple .xdf files or a list of data frames.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>a data frame, a character string defining the path to the input .xdf file,  or an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>a character string defining the path to the input .xdf file,  or an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>a character string or vector defining the file names/paths to use in forming the the output .xdf files.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>These names/paths will be embellished with any specified <ph id="ph1">`outFileSuffixes`</ph>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxSplit`</ph>, <ph id="ph2">`outFilesBase = NULL`</ph> means that the default value for .xdf and <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept><ph id="ph3">`inData`</ph> objects will be <ph id="ph4">`basename(rxXdfFileName(inData))`</ph> while it will be a blank string for <ph id="ph5">`inData`</ph> a data frame.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>a vector containing the suffixes to append to the base name(s)/path(s) specified in <ph id="ph1">`outFilesBase`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Before appending, <ph id="ph1">`outFileSuffixes`</ph> is converted to class character via the as.character function.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, <ph id="ph2">`seq(numOutFiles)`</ph> is used in its place if  <ph id="ph3">`numOutFiles`</ph> is not <ph id="ph4">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>number of outputs to create, e.g., the number of output files or number of data frames returned in the output list.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>number of files to create.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>This argument is used only when <ph id="ph1">`outFilesBase`</ph> and <ph id="ph2">`outFileSuffixes`</ph> do not provide sufficient information to form unique paths to multiple output files.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>See the Examples section for its use.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>a character string denoting the method to use in partitioning the <ph id="ph1">`inFile`</ph> .xdf file.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>With  <ph id="ph1">`numFiles`</ph> defined as the number of output files (formed by the combination of  <ph id="ph2">`outFilesBase`</ph>, <ph id="ph3">`outFileSuffixes`</ph>, and <ph id="ph4">`numOutFiles`</ph> arguments), the supported values for <ph id="ph5">`splitBy`</ph> are:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"rows"`</ph> - To the extent possible, a uniform partition of the number of <bpt id="p1">*</bpt>rows<ept id="p1">*</ept> in the <ph id="ph2">`inFile`</ph> .xdf file is performed.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The minimum number of rows in each output  file is defined by <ph id="ph1">`floor(numRows/numFiles)`</ph>, where <ph id="ph2">`numRows`</ph> is the number of rows in <ph id="ph3">`inFile`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Additional rows will be distributed uniformly amongst the last set of files.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"blocks"`</ph> - To the extent possible, a uniform partition of the number of <bpt id="p1">*</bpt>blocks<ept id="p1">*</ept> in the <ph id="ph2">`inFile`</ph> .xdf file is performed.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`blocksPerRead = 1`</ph>,  the minimum number of blocks in each output  file is defined by <ph id="ph2">`floor(numBlocks/numFiles)`</ph>, where <ph id="ph3">`numBlocks`</ph> is the number of blocks in <ph id="ph4">`inFile`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Additional blocks will be distributed uniformly amongst the last set of files.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`blocksPerRead &gt; 1`</ph>, the number of blocks in each output file is reduced accordingly since multiple blocks  read at one time are collapsed to a single block upon write.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>This argument is ignored if <ph id="ph1">`splitByFactor`</ph> is a valid factor variable name.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>character string identifying the name of the factor to use in splitting the <ph id="ph1">`inFile`</ph> .xdf data such that each file contains the data corresponding to a single level of the factor.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`splitBy`</ph> argument is ignored if <ph id="ph2">`splitByFactor`</ph> is a valid factor variable name.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`splitByFactor = NULL`</ph>, the <ph id="ph2">`splitBy`</ph> argument is used to define the split method.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>character vector of variable names to include when reading from the input data file.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToDrop`</ph>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>character vector of variable names to exclude when reading from the input data file.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToKeep`</ph>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>name of a logical variable in the data set (in quotes) or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rowSelection = (age &gt; 20) &amp; (age &lt; 65) &amp; (log(income) &gt; 10)`</ph> will use only observations in which the value of the <ph id="ph2">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph3">`log`</ph> of the <ph id="ph4">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations  (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function  call using the expression function.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>an expression of the form <ph id="ph1">`list(name = expression, ...)`</ph> representing the first round of variable transformations.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>)  can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>a named list containing objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Ignored for  data frames.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>variable transformation function.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>character vector defining additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and  preloaded for use in variable transformation functions, e.g., those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments or those  defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>user-defined environment to serve as a parent to  all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outFile`</ph> will be overwritten, or if appending columns existing columns with the same name will be overwritten.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`overwrite`</ph> is ignored if appending rows.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, rows with missing values will not be included in the output data.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>number of rows to read for each chunk of data read from the input data source.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Use this argument for finer control of the number of rows per block in the output data source.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If greater than 0, <ph id="ph1">`blocksPerRead`</ph> is ignored.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Cannot be used if <ph id="ph1">`inFile`</ph> is the same as <ph id="ph2">`outFile`</ph>.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Ignored for data frames or if <ph id="ph1">`rowsPerRead`</ph> is positive.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, the low and high values for each variable in the <ph id="ph2">`inFile`</ph> .xdf file will be copied to the header of each output file so that  all output files reflect the global range of the data.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, each variable's low and high values are updated to reflect the range of values in the corresponding file, likely resulting in different low and  high values for the same variable between output files.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Note that when using <ph id="ph1">`rxSplit`</ph> and the output is a list of data frames, the <ph id="ph2">`updateLowHigh`</ph> argument has no effect.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>argument sent directly to the <bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxDataStep.md)</ept> function behind the scenes when converting the output .xdf files (back) into a list of data frames.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>This parameter is provided primarily for the case where <ph id="ph1">`rxSplit`</ph> is being used to split a .xdf file or <ph id="ph2">`RxXdfData`</ph> data source into portions that are then read back into R as  a list of data frames.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>In this case, <ph id="ph1">`maxRowsByCols`</ph> provides a mechanism for the user to control the maximum number of of elements read from the output .xdf file in an effort to limit the amount of memory needed for storing each partition  as a data frame object in R.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, additional summary information is printed.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>integer in the range of -1 to 9.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the  amount of compression - resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>If  <ph id="ph1">`xdfCompressionLevel`</ph> is set to 0, there will be no compression and files will be compatible  with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression  will be used.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the function used to partition the data.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>For example,</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`Uniform Partition`</ph> - a <ph id="ph2">`fill`</ph> argument with supported values are <ph id="ph3">`"left"`</ph>, <ph id="ph4">`"center"`</ph>, or <ph id="ph5">`"right"`</ph>, can be used to place the remaining rows/blocks in the set of output files.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>For example, if <ph id="ph1">`sortBy = "blocks"`</ph>, <ph id="ph2">`inFile`</ph> has <ph id="ph3">`15`</ph> blocks, and the number of output files is <ph id="ph4">`6`</ph>, the distribution of blocks for the set of <ph id="ph5">`6`</ph> output files will be:</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`fill = "left"`</ph> - 3 3 3 2 2 2</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`fill = "center"`</ph> - 2 3 3 3 2 2</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`fill = "right"`</ph> - 2 2 2 3 3 3</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>rxSplit:<ept id="p1">**</ept> Use <ph id="ph1">`rxSplit`</ph> as a general function to partition a data frame or .xdf file.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Behind the scenes, the <ph id="ph1">`rxSplitXdf`</ph> function is called by <ph id="ph2">`rxSplit`</ph> after converting the <ph id="ph3">`inData`</ph> data source into a (temporary) .xdf file.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>If both <ph id="ph1">`outFilesBase`</ph> and <ph id="ph2">`outFileSuffixes`</ph> are <ph id="ph3">`NULL`</ph> (the default), then the type of output is determined by the type of inData: if the <ph id="ph4">`inData`</ph> is an .xdf file name or an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object, and list of <ph id="ph5">`RxXdfData`</ph> data sources representing the new split .xdf files is returned.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`inData`</ph> is a data frame, then the output is returned as a list of data frames.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outFilesBase`</ph> is an empty character string and <ph id="ph2">`outFileSuffixes`</ph> is <ph id="ph3">`NULL`</ph>, a list of data frames is always returned.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>In the case that a list of data frames is returned, the names of the list are in <ph id="ph1">`shortFileName.splitType.NumberOrFactor`</ph> format, e.g., <ph id="ph2">`iris.Species.versicolor`</ph> or <ph id="ph3">`myXdfFile.rows.3`</ph>.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>rxSplitXdf:<ept id="p1">**</ept> Use <ph id="ph1">`rxSplitXdf`</ph> to partition an .xdf file.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`inFile`</ph> .xdf file is uniformly partitioned (to the extent possible) and each partition is written to a distinct user-specified file.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>As an example, if <ph id="ph1">`inFile`</ph> contains a million rows, <ph id="ph2">`splitBy = "rows"`</ph>, and the number of output files we specify to create is five, then each output file will contain two hundred thousand observations, assuming none were dropped via a <ph id="ph3">`rowSelection`</ph> argument specification.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>The number of output files is controlled either directly or indirectly through a combination of</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>arguments: <ph id="ph1">`inFile`</ph>, <ph id="ph2">`outFilesBase`</ph>, <ph id="ph3">`outFileSuffixes`</ph>, and <ph id="ph4">`numOutFiles`</ph>.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>In general, the values of these arguments are pasted together to form a character vector of output file paths, with scalar values auto-expanded to vectors (of an appropriate size) prior to pasting.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>This scheme allows the user to either specify directly the full paths to the output files they wish to form or do so implicitly (and perhaps more conveniently) using various combinations of these arguments.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>We illustrate the use of these combinations in the examples below, which are assumed to be run under Windows.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Col  1</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Col  2</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Col  3</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>INPUT ARGUMENTS<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>OUTPUT FILE VECTOR<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>a list of data frames or an invisible list of <ph id="ph1">`RxXdfData`</ph> data source objects corresponding to the created output files.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxDataStep.md)</ept>, <bpt id="p2">[</bpt>rxImport<ept id="p2">](rxImport.md)</ept>, <bpt id="p3">[</bpt>rxTransform<ept id="p3">](rxTransform.md)</ept></source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>