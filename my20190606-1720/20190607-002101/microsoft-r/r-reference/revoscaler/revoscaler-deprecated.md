<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="revoscaler-deprecated.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37360542226950a8400f5f23365993bab9b27667fc.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">360542226950a8400f5f23365993bab9b27667fc</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\revoscaler-deprecated.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RevoScaleR-deprecated function (RevoScaleR)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>These functions are provided for compatibility with  older versions of RevoScaleR only, and may be defunct as soon as the next release.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(RevoScaleR), RevoScaleR-deprecated, rxGetNodes, RxHpcServer, rxImportToXdf, rxDataStepXdf, rxDataFrameToXdf, rxXdfToDataFrame, rxSortXdf</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RevoScaleR-deprecated: Deprecated functions in RevoScaleR</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>These functions are provided for compatibility with older versions of RevoScaleR only, and may be defunct as soon as the next release.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>a non-RxXdfData RxDataSource object representing the input data source or a non-empty character string representing a file path.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If a character string is supplied, the type of file is inferred from its extension, with the default being a text file.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>either an RxXdfData object or a character string specifying the .xdf file.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>an RxXdfData object or non-empty character string representing the output .xdf file.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>a character string specifying the output .xdf file, an  <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object, a <bpt id="p2">[</bpt>RxOdbcData<ept id="p2">](RxOdbcData.md)</ept> data source, or a <bpt id="p3">[</bpt>RxTeradata<ept id="p3">](RxTeradata.md)</ept> data source.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, a data frame will be returned from <ph id="ph2">`rxDataStep`</ph> unless <ph id="ph3">`returnTransformObjects`</ph> is set to <ph id="ph4">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Setting <ph id="ph1">`outFile`</ph> to <ph id="ph2">`NULL`</ph> and <ph id="ph3">`returnTransformObjects=TRUE`</ph> allows chunkwise computations on the data without modifying the existing data or creating a new data set.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>can also be a delimited <bpt id="p1">[</bpt>RxTextData<ept id="p1">](RxTextData.md)</ept> data source if using a native file system and not appending.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>name of a logical variable in the data set (in quotes) or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>will use only observations in which the value of the <ph id="ph1">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph2">`log`</ph> of the <ph id="ph3">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations  (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function  call using the expression function.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>an expression of the form <ph id="ph1">`list(name = expression, ...)`</ph> representing the first round of variable transformations.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>)  can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>a named list containing objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>variable transformation function.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>character vector defining additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and  preloaded for use in variable transformation functions, e.g., those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments or those  defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>user-defined environment to serve as a parent to  all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>either <ph id="ph1">`"none"`</ph> to create a new .xdf file or <ph id="ph2">`"rows"`</ph> to append rows to an existing .xdf file.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outSource`</ph> exists and <ph id="ph2">`append`</ph> is <ph id="ph3">`"none"`</ph>, the <ph id="ph4">`overwrite`</ph> argument must be set to <ph id="ph5">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the existing <ph id="ph2">`outSource`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>integer value specifying the maximum number of rows to import.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>If set to -1, all rows will be imported.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>the maximum size of a data frame that will be read in if <ph id="ph1">`outData`</ph> is set to <ph id="ph2">`NULL`</ph>, measured by the number of rows times the number of columns.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>If the number of rows times the number of columns being imported exceeds this,  a warning will be reported and a smaller number of rows will be read in than requested.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`maxRowsByCols`</ph> is set to be too large, you may experience problems  from loading a huge data frame into memory.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, information on the import type is printed.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>integer in the range of -1 to 9.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the  amount of compression - resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If  <ph id="ph1">`xdfCompressionLevel`</ph> is set to 0, there will be no compression and files will be compatible  with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression  will be used.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>logical value or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, a composite set of files will be created instead of a single .xdf file.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>A directory will be created whose name is the same as the .xdf file that would otherwise be created, but with no extension.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Subdirectories data and metadata will be created.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>In the data subdirectory, the data will be split across a set of .xdfd files (see <ph id="ph1">`blocksPerCompositeFile`</ph> below for determining how many blocks of data will be in each file).</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>In the metadata subdirectory  there is a single .xdfm file, which contains the meta data for all of the  .xdfd files in the  data subdirectory.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>When the compute context is <ph id="ph1">`RxHadoopMR`</ph> a composite set of files is always created.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`createCompositeSet=TRUE`</ph>, and if the compute context is not <ph id="ph2">`RxHadoopMR`</ph>, this will be the number of blocks put into each .xdfd file in the composite set.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>When importing is being done on Hadoop using MapReduce, the number of rows per .xdfd file is determined by the rows assigned to each MapReduce task, and the number of blocks per .xdfd file is therefore determined by <ph id="ph1">`rowsPerRead`</ph>.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`outSource`</ph> is an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object, set the value for <ph id="ph2">`blocksPerCompositeFile`</ph> there instead.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>either an RxXdfData object or a character string specifying the input .xdf file.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>character vector of variable names to include when reading from the input data file.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToDrop`</ph> or when <ph id="ph2">`outFile`</ph> is the same as the input data file.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Variables used in transformations or row selection will be retained even if not specified in <ph id="ph1">`varsToKeep`</ph>.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`newName`</ph> is used in <ph id="ph2">`colInfo`</ph> in a non-xdf  data source, the <ph id="ph3">`newName`</ph> should be used in <ph id="ph4">`varsToKeep`</ph>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Not supported for <bpt id="p1">[</bpt>RxTeradata<ept id="p1">](RxTeradata.md)</ept>, <bpt id="p2">[</bpt>RxOdbcData<ept id="p2">](RxOdbcData.md)</ept>, or <bpt id="p3">[</bpt>RxSqlServerData<ept id="p3">](RxSqlServerData.md)</ept> data sources.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>character vector of variable names to exclude when reading from the input data file.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToKeep`</ph> or when <ph id="ph2">`outFile`</ph> is the same as the input data file.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Variables used in transformations or row selection will be retained even if specified in <ph id="ph1">`varsToDrop`</ph>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`newName`</ph> is used in <ph id="ph2">`colInfo`</ph> in a non-xdf  data source, the <ph id="ph3">`newName`</ph> should be used in <ph id="ph4">`varsToDrop`</ph>.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Not supported for <bpt id="p1">[</bpt>RxTeradata<ept id="p1">](RxTeradata.md)</ept>, <bpt id="p2">[</bpt>RxOdbcData<ept id="p2">](RxOdbcData.md)</ept>, or  <bpt id="p3">[</bpt>RxSqlServerData<ept id="p3">](RxSqlServerData.md)</ept> data sources.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, rows with missing values will be removed on read.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, rows with missing values will not be included in the output data.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, low and high values will not automatically be computed.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>This should only be set to <ph id="ph1">`FALSE`</ph> in special circumstances, such as when <ph id="ph2">`append`</ph> is being used repeatedly.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>number of rows to read for each chunk of data read from the input data source.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Use this argument for finer control of the number of rows per block in the output data source.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>If greater than 0, <ph id="ph1">`blocksPerRead`</ph> is ignored.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Cannot be used if <ph id="ph1">`inFile`</ph> is the same as <ph id="ph2">`outFile`</ph>.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The default value of <ph id="ph1">`-1`</ph> specifies that data should be read by blocks according to the <ph id="ph2">`blocksPerRead`</ph> argument.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>the starting row to read from the input data source.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Cannot be used if <ph id="ph1">`inFile`</ph> is the same as <ph id="ph2">`outFile`</ph>.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>,  the list of <ph id="ph2">`transformObjects`</ph> will be returned instead of  a data frame or data source object.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>If the input <ph id="ph1">`transformObjects`</ph> have been modified, by using <ph id="ph2">`.rxSet`</ph> or <ph id="ph3">`.rxModify`</ph> in the <ph id="ph4">`transformFunc`</ph>, the updated values will be returned.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Any data returned from the <ph id="ph1">`transformFunc`</ph> is ignored.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>If no <ph id="ph1">`transformObjects`</ph> are used, <ph id="ph2">`NULL`</ph> is returned.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>This argument allows for user-defined  computations within a <ph id="ph1">`transformFunc`</ph> without creating new data.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>is not supported in distributed compute contexts  such as <bpt id="p1">[</bpt>RxHadoopMR<ept id="p1">](RevoScaleR-deprecated.md)</ept>.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>starting block to read.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Ignored if <ph id="ph1">`startRow`</ph> is set to greater than 1.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>number of blocks to read; all are read if set to -1.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Ignored if <ph id="ph1">`numRows`</ph> is not set to -1.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Ignored for data frames or if <ph id="ph1">`rowsPerRead`</ph> is positive.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>an optional list of arguments to be applied to the input data source.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> variable names specified in <ph id="ph2">`varsToKeep`</ph> will be checked against variables in the data set to make sure they exist.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>An error will be reported if not found.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Ignored if more than 500 variables in the data set.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>A compute context (preferred), a <ph id="ph1">`jobInfo`</ph> object, or (deprecated) a character scalar containing the name of the head node of a Microsoft HPC cluster.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Indicates whether to include the name of the head node in the list of returned nodes.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Determines if the names of the nodes should be normalized for use as R variables.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>See also <bpt id="p1">[</bpt>rxMakeRNodeNames<ept id="p1">](rxMakeRNodeNames.md)</ept> for details on name mangeling.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, returns only those nodes within the cluster that are configured to actually execute jobs (where applicable).</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>object of class RxHpcServer.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>This argument is optional.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>If supplied, the values of  the other specified arguments are used to replace those of <ph id="ph1">`object`</ph> and the modified object is returned.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>character string specifying the path to the directory on the cluster  nodes containing the files R.exe and Rterm.exe.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>The invocation of R on each  node must be identical (this is an HPC constraint).</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>See the Details section for more  information regarding the path format.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>character string specifying the directory on the head node that is  shared among all the nodes of the cluster and any client host.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>You must have permissions to read and write  in this directory.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>See the Details section for more information regarding the path format.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>character string specifying a working directory for the processes  on the cluster.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, will default to the standard Windows user directory (that is, the value of the environment variable <ph id="ph2">`USERPROFILE`</ph>).</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>character vector defining the search path(s) for the data source(s).</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>See the Details section for more information regarding the path format.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>or character vector defining the search path(s) for   new output data file(s).</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>If not <ph id="ph1">`NULL`</ph>, this overrides any specification for <ph id="ph2">`dataPath`</ph> in <bpt id="p1">[</bpt>rxOptions<ept id="p1">](rxOptions.md)</ept></source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the job will be blocking and will not return until   it has completed or has failed.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, the job will be non-blocking return immediately,  allowing you to continue running other R code.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>The object <ph id="ph1">`rxgLastPendingJob`</ph> is created with the job information.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>You can pass this object to the   <bpt id="p1">[</bpt>rxGetJobStatus<ept id="p1">](rxGetJobResults.md)</ept> function to check on the processing status of the job.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxWaitForJob<ept id="p1">](rxWaitForJob.md)</ept> will change a non-waiting job  to a waiting job.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Conversely, pressing ESC changes a waiting job to a non-waiting job, provided that the HPC scheduler has accepted the job.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>If you press ESC before the job has been accepted, the job is canceled.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, causes the standard output  of the R processes to be printed to the user console.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>character string specifying the path to the XML template (on your  local computer) that will be consumed by the job scheduler.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> (the default),  the standard template is used.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>See the Details section for more information regarding  the path format.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>We recommend that the user rely upon the default setting for <ph id="ph1">`configFile`</ph>.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>character string containing a comma-separated list of requested  nodes, e.g., <ph id="ph1">`"compute1,compute2,compute3"`</ph>, or a character vector like <ph id="ph2">`c("compute1", "compute2", "compute3")`</ph>.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>If you specify the nodes to be used,  <ph id="ph1">`minElems`</ph> and <ph id="ph2">`maxElems`</ph> are ignored if greater than the number of specified nodes.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>See the Details section for more information.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>The nodes parameter forces use of the specified nodes, rather than simply requesting them.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>This feature is provided so that jobs requiring only 10 out of 100 nodes, for example,  do not force you to deploy your data to all 100 nodes.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Should you need finer control, you will need to generate a new XML template through the MS  HPC job scheduler.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>See the Microsoft HPC Server 2008 documentation for details.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph> and nodes are automatically being selected, the head  node of the cluster will not be among the nodes to be used.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Furthermore, if <ph id="ph1">`FALSE`</ph> and the  head node is explicitly specified in the node list, a warning is issued, but the job proceeds with  a warning and the head node excluded from the node list.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>,  then the head node is treated exactly as any other node for the purpose of job resource allocations.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Note that setting this flag to <ph id="ph1">`TRUE`</ph> does not guarantee inclusion of the head node in a job; it simply allows the head node to be listed in an explicit list, or to be included by automatic node usage generation.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>minimum number of nodes required for a run.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`-1`</ph>, the value for <ph id="ph2">`maxElems`</ph> is used.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>If both <ph id="ph1">`minElems`</ph> and <ph id="ph2">`maxElems`</ph> are <ph id="ph3">`-1`</ph>, the number of nodes specified in the <ph id="ph4">`nodes`</ph> argument is used.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>See the Details section for more information.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>maximum number of nodes required for a run.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`-1`</ph>, the value for <ph id="ph2">`minElems`</ph> is used.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>If both <ph id="ph1">`minElems`</ph> and <ph id="ph2">`maxElems`</ph> are <ph id="ph3">`-1`</ph>, the number of nodes specified in the <ph id="ph4">`nodes`</ph> argument is used.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>See the Details section for more information.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>The priority of the job.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Allowable values are 0 (lowest), 1 (below normal), 2 (normal, the default), 3 (above normal), and 4 (highest).</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>See the Microsoft HPC Server 2008 documentation  for using job scheduling policy options and job templates to manage job priorities.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>These policy options may also affect the behavior of the <ph id="ph1">`exclusive`</ph> argument.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, no other jobs can run on a compute node at the same time as this job.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>This may fail if you do not have administrative privileges  on the cluster, and may also fail depending on the settings of your job scheduling policy options.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the default behavior is to clean up the  temporary computational artifacts and delete the result objects upon retrival.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>,  then the computational results are not deleted, and the results may be acquired using  <bpt id="p1">[</bpt>rxGetJobResults<ept id="p1">](rxGetJobResults.md)</ept>, and the output via <bpt id="p2">[</bpt>rxGetJobOutput<ept id="p2">](rxGetJobOutput.md)</ept> until the  <bpt id="p3">[</bpt>rxCleanupJobs<ept id="p3">](rxCleanup.md)</ept> is used to delete the results and other artifacts.</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>Leaving this flag set to <ph id="ph1">`FALSE`</ph> can result in accumulation of compute artifacts which you may eventually need to delete before they fill up your hard drive.If you set <ph id="ph2">`autoCleanup=TRUE`</ph>and experience performance degradation on a Windows XP client, consider  setting <ph id="ph3">`autoCleanup=FALSE`</ph>.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>a character string denoting how the data has been distributed.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`"all"`</ph> means that the entire data set has been copied to each compute node.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`"split"`</ph> means that the data set has been partitioned and that each compute node contains a different set of rows.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>optional character vector specifying additional packages to be  loaded on the nodes when jobs are run in this compute context.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>optional character string specifying an email address to which a job complete email should be sent.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>Note that the cluster administrator will have to enable email notifications for such job completion mails to be received.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>A numeric value indicating for how long attempts should be made  to retrieve results from the cluster.</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>Under normal conditions, results are available immediately upon completion of the job.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>However, under certain high load conditions, the processes on the nodes have reported as completed, but the results have not been fully committed to disk by the operating system.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>Increase this parameter if results retrievial is failing on high load clusters.</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>Optional character vector specifying the groups from which nodes should be selected.</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`groups`</ph>is specified and <ph id="ph2">`nodes`</ph> is <ph id="ph3">`NULL`</ph>, all the nodes in the groups specified will be candidates for computations.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>If both <ph id="ph1">`nodes`</ph> and <ph id="ph2">`groups`</ph> are specified, the candidate nodes will be the intersection of the set of nodes  explicitly specified in <ph id="ph3">`nodes`</ph> and the set of all the nodes in the <ph id="ph4">`groups`</ph> specified.</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>Note that the default value of <ph id="ph1">`"ComputeNodes"`</ph> is the name of the Microsoft defined group that includes all physically present nodes.</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>Another Microsoft default group name used is <ph id="ph1">`"HeadNodes"`</ph> which includes all nodes set up to act as head nodes.</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>While these  default names can be changed, this is not recommended.</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>Note also that <bpt id="p1">[</bpt>rxGetNodeInfo<ept id="p1">](rxGetNodeInfo.md)</ept> will honor group filtering.</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>See the help for <ph id="ph1">`rxGetNodeInfo`</ph> for more information.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>data frame to put into .xdf file.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>See details section for a listing of the supported column types in the data frame.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>character string or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the data frame's row names will be dropped.</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>If a character string, an additional variable of that name will be added to the data set containing the data frame's row names.</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>logical indicating whether or not to convert strings into factors in R.</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>character vector containing the names of the variables to use for sorting.</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>If multiple variables are used, the first <ph id="ph1">`sortByVars`</ph> variable is sorted and common values are grouped.</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>The second variable is then sorted within the first variable groups.</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>The third variable is then sorted within groupings formed by the first two variables, and so on.</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>a logical scalar or vector defining the whether or not the <ph id="ph1">`sortByVars`</ph> variables are  to be sorted in decreasing or increasing order.</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>If a vector, the length <ph id="ph1">`decreasing`</ph> must be that of <ph id="ph2">`sortByVars`</ph>.</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>If a logical scalar, the value of <ph id="ph1">`decreasing`</ph> is replicated to the length <ph id="ph2">`sortByVars`</ph>.</source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>a character string defining the sorting method to use.</source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`"auto"`</ph> automatically determines the sort method based on the amount of memory required for sorting.</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source>If possible, all of the data will be sorted in memory.</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`"mergeSort"`</ph> uses a merge sort method, where chunks of data are pre-sorted, then merged together.</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`"varByVar"`</ph> uses a variable-by-variable sort method,  which assumes that the <ph id="ph2">`sortByVars`</ph> variables and the calculated sorted index variable can be held in memory simultaneously.</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`type="varByVar"`</ph>, the variables in the sorted data are re-ordered so that the variables named in <ph id="ph2">`sortByVars`</ph> come first, followed by any remaining variables.</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>a logical scalar for controlling the treatment of missing values.</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, missing values  in the data are treated as the lowest value; if <ph id="ph2">`FALSE`</ph>, they are treated as the highest value.</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>a logical scalar.</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, case sensitive sorting is performed for character data.</source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, only the first observation will be   kept when duplicate values of the key (<ph id="ph2">`sortByVars`</ph>) are encountered.</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>The sort  <ph id="ph1">`type`</ph> must be set to <ph id="ph2">`"auto"`</ph> or <ph id="ph3">`"mergeSort"`</ph>.</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED information to be sent to the C++ interpreter.</source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed to the input data source.</source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source>object of class RxHadoopMR.</source>
        </trans-unit><trans-unit id="324" translate="yes" xml:space="preserve">
          <source>This argument is optional.</source>
        </trans-unit><trans-unit id="325" translate="yes" xml:space="preserve">
          <source>If supplied, the values of  e other specified arguments are used to replace those of <ph id="ph1">`object`</ph> and the modified object is turned.</source>
        </trans-unit><trans-unit id="326" translate="yes" xml:space="preserve">
          <source>character string specifying the file sharing location within HDFS.</source>
        </trans-unit><trans-unit id="327" translate="yes" xml:space="preserve">
          <source>You must ave permissions to read and write to this location.</source>
        </trans-unit><trans-unit id="328" translate="yes" xml:space="preserve">
          <source>character string specifying the directory on the master (perhaps edge) node that is  ared among all the nodes of the cluster and any client host.</source>
        </trans-unit><trans-unit id="329" translate="yes" xml:space="preserve">
          <source>You must have permissions to read and write   this directory.</source>
        </trans-unit><trans-unit id="330" translate="yes" xml:space="preserve">
          <source>character string specifying the absolute path of the temporary directory on the client.</source>
        </trans-unit><trans-unit id="331" translate="yes" xml:space="preserve">
          <source>faults to /tmp for POSIX-compliant non-Windows clients.</source>
        </trans-unit><trans-unit id="332" translate="yes" xml:space="preserve">
          <source>For Windows and non-compliant POSIX clients,  faults to the value of the TEMP environment variable if defined, else to the TMP environment variable   defined, else to <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="333" translate="yes" xml:space="preserve">
          <source>If the default directory does not exist, defaults to NULL.</source>
        </trans-unit><trans-unit id="334" translate="yes" xml:space="preserve">
          <source>C paths ("<ph id="ph1">`\\host\dir`</ph>") are not supported.</source>
        </trans-unit><trans-unit id="335" translate="yes" xml:space="preserve">
          <source>character string specifying the path to the directory on the cluster  mpute nodes containing the files R.exe and Rterm.exe.</source>
        </trans-unit><trans-unit id="336" translate="yes" xml:space="preserve">
          <source>The invocation of R on each  de must be identical.</source>
        </trans-unit><trans-unit id="337" translate="yes" xml:space="preserve">
          <source>character string specifying the path to the directory on the master (perhaps edge) node  ntaining the files R.exe and Rterm.exe.</source>
        </trans-unit><trans-unit id="338" translate="yes" xml:space="preserve">
          <source>character string specifying optional generic Hadoop command line switches, r example <ph id="ph1">`-conf myconf.xml`</ph>.</source>
        </trans-unit><trans-unit id="339" translate="yes" xml:space="preserve">
          <source>e <bpt id="p1">[</bpt><ph id="ph1">`http://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-common/CommandsManual.html`</ph><ept id="p1">](http://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-common/CommandsManual.html)</ept>  r details on the Hadoop command line generic options.</source>
        </trans-unit><trans-unit id="340" translate="yes" xml:space="preserve">
          <source>character string specifying the username for making an ssh connection to the doop cluster.</source>
        </trans-unit><trans-unit id="341" translate="yes" xml:space="preserve">
          <source>This is not needed if you are running your R client directly on the cluster.</source>
        </trans-unit><trans-unit id="342" translate="yes" xml:space="preserve">
          <source>faults to the username of the user running the R client (that is, the value of <ph id="ph1">`Sys.info()[["user"]]`</ph>).</source>
        </trans-unit><trans-unit id="343" translate="yes" xml:space="preserve">
          <source>character string specifying the hostname or IP address of the Hadoop cluster  de or edge node that the client will log into for launching Hadoop jobs and for copying files  tween the client machine and the Hadoop cluster.</source>
        </trans-unit><trans-unit id="344" translate="yes" xml:space="preserve">
          <source>Defaults to the hostname of the machine running  e R client (that is, the value of <ph id="ph1">`Sys.info()[["nodename"]]`</ph>)  This field is only used if  odeonClusterNode is <ph id="ph2">`NULL`</ph> or <ph id="ph3">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="345" translate="yes" xml:space="preserve">
          <source>If you are using PuTTY on a Windows system, this can be the name of a saved PuTTY session that n include the user name and authentication file to use.</source>
        </trans-unit><trans-unit id="346" translate="yes" xml:space="preserve">
          <source>character string specifying any switches needed for making an ssh connection to the doop cluster.</source>
        </trans-unit><trans-unit id="347" translate="yes" xml:space="preserve">
          <source>This is not needed if one is running one's R client directly on the cluster.</source>
        </trans-unit><trans-unit id="348" translate="yes" xml:space="preserve">
          <source>Optional character string specifying the absolute path to a profile script that will exists on the hHostname host.</source>
        </trans-unit><trans-unit id="349" translate="yes" xml:space="preserve">
          <source>This is used when the target ssh host does not automatically read in a .bash_profile, .profile or other shell vironment configuration file for the definition of requisite variables such as HADOOP_STREAMING.</source>
        </trans-unit><trans-unit id="350" translate="yes" xml:space="preserve">
          <source>character string specifying the Windows directory where Cygwin's ssh.exe  d scp.exe or PuTTY's plink.exe and pscp.exe executables can be found.</source>
        </trans-unit><trans-unit id="351" translate="yes" xml:space="preserve">
          <source>Needed only for Windows.</source>
        </trans-unit><trans-unit id="352" translate="yes" xml:space="preserve">
          <source>t needed if these executables are on the Windows Path or if Cygwin's location can be found in  e Windows Registry.</source>
        </trans-unit><trans-unit id="353" translate="yes" xml:space="preserve">
          <source>Defaults to the empty string.</source>
        </trans-unit><trans-unit id="354" translate="yes" xml:space="preserve">
          <source>logical scalar specifying whether run-as-user mode is being used on the Hadoop cluster.</source>
        </trans-unit><trans-unit id="355" translate="yes" xml:space="preserve">
          <source>en using run-as-user mode, local R processes started by the map-reduce framework will run as the same user that started the b, and will have any allocated local permissions.</source>
        </trans-unit><trans-unit id="356" translate="yes" xml:space="preserve">
          <source>When not using run-as-user mode (the default for many Hadoop systems), cal R processes will run as user mapred.</source>
        </trans-unit><trans-unit id="357" translate="yes" xml:space="preserve">
          <source>Note that when running as user mapred, permissions for files and directories will ve to be more open in order to allow hand-offs between the user and mapred.</source>
        </trans-unit><trans-unit id="358" translate="yes" xml:space="preserve">
          <source>n-as-user mode is controlled for the Hadoop map-reduce framework by the xml setting,  odemapred.task.tracker.task-controller, in the <ph id="ph1">`mapred-site.xml`</ph> nfiguration file.</source>
        </trans-unit><trans-unit id="359" translate="yes" xml:space="preserve">
          <source>If it is set to the value <ph id="ph1">`org.apache.hadoop.mapred.LinuxTaskController`</ph>, then  n-as-user mode is in use.</source>
        </trans-unit><trans-unit id="360" translate="yes" xml:space="preserve">
          <source>If it is set to the value <ph id="ph1">`org.apache.hadoop.mapred.DefaultTaskController`</ph>, then  n-as-user mode is not in use.</source>
        </trans-unit><trans-unit id="361" translate="yes" xml:space="preserve">
          <source>character string specifying the Hadoop name node hostname or IP address.</source>
        </trans-unit><trans-unit id="362" translate="yes" xml:space="preserve">
          <source>pically you can leave this at its default value.</source>
        </trans-unit><trans-unit id="363" translate="yes" xml:space="preserve">
          <source>set to a value other than "default" or the empty string (see below), is must be an address that can be resolved by the data nodes and used by them to contact the  me node.</source>
        </trans-unit><trans-unit id="364" translate="yes" xml:space="preserve">
          <source>Depending on your cluster, it may need to be set to a private network address  ch as <ph id="ph1">`"master.local"`</ph>.</source>
        </trans-unit><trans-unit id="365" translate="yes" xml:space="preserve">
          <source>If set to the empty string, "", then the master process will set  is to the name of the node on which it is running, as returned by <ph id="ph1">`Sys.info()[["nodename"]]`</ph>.</source>
        </trans-unit><trans-unit id="366" translate="yes" xml:space="preserve">
          <source>is is likely to work when the sshHostname points to the name node or the sshHostname is not  ecified and the R client is running on the name node.</source>
        </trans-unit><trans-unit id="367" translate="yes" xml:space="preserve">
          <source>Defaults to rxGetOption("hdfsHost").</source>
        </trans-unit><trans-unit id="368" translate="yes" xml:space="preserve">
          <source>character scalar specifying the full URL for the jobtracker web interface.</source>
        </trans-unit><trans-unit id="369" translate="yes" xml:space="preserve">
          <source>is is used only for the purpose of loading the job tracker web page from the <ph id="ph1">`rxLaunchClusterJobManager`</ph> nvenience function.</source>
        </trans-unit><trans-unit id="370" translate="yes" xml:space="preserve">
          <source>It is never used for job control, and its specification in the compute context is completely tional.</source>
        </trans-unit><trans-unit id="371" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>rxLaunchClusterJobManager<ept id="p1">](rxLaunchClusterTaskManager.md)</ept> page for more information.</source>
        </trans-unit><trans-unit id="372" translate="yes" xml:space="preserve">
          <source>numeric scalar specifying the port used by the name node for hadoop jobs.</source>
        </trans-unit><trans-unit id="373" translate="yes" xml:space="preserve">
          <source>Needs  be able to be cast to an integer.</source>
        </trans-unit><trans-unit id="374" translate="yes" xml:space="preserve">
          <source>Defaults to rxGetOption("hdfsPort").</source>
        </trans-unit><trans-unit id="375" translate="yes" xml:space="preserve">
          <source>logical scalar or NULL specifying whether the user is initiating the job from a client that will connect to ther an edge node or an actual cluster node, directly from either an edge node or node within the cluster.</source>
        </trans-unit><trans-unit id="376" translate="yes" xml:space="preserve">
          <source>If set to  odeFALSE or <ph id="ph1">`NULL`</ph>, then <ph id="ph2">`sshHostname`</ph> must be a valid host.</source>
        </trans-unit><trans-unit id="377" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="378" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the job will be blocking  nd will not return until it has completed or has failed.</source>
        </trans-unit><trans-unit id="379" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>,  he job will be non-blocking return immediately,  lowing you to continue running other R code.</source>
        </trans-unit><trans-unit id="380" translate="yes" xml:space="preserve">
          <source>The object <ph id="ph1">`rxgLastPendingJob`</ph> is created th the job information.</source>
        </trans-unit><trans-unit id="381" translate="yes" xml:space="preserve">
          <source>You can pass this object to the   ode<bpt id="p1">[</bpt>rxGetJobStatus<ept id="p1">](rxGetJobResults.md)</ept> function to check on the processing status of the job.</source>
        </trans-unit><trans-unit id="382" translate="yes" xml:space="preserve">
          <source>ode<bpt id="p1">[</bpt>rxWaitForJob<ept id="p1">](rxWaitForJob.md)</ept> will change a non-waiting job   a waiting job.</source>
        </trans-unit><trans-unit id="383" translate="yes" xml:space="preserve">
          <source>Conversely, pressing ESC changes a waiting job to a non-waiting job, ovided that the HPC scheduler has accepted the job.</source>
        </trans-unit><trans-unit id="384" translate="yes" xml:space="preserve">
          <source>If you press ESC before the job has en accepted, the job is canceled.</source>
        </trans-unit><trans-unit id="385" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="386" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, causes the standard output   the R processes to be printed to the user console.</source>
        </trans-unit><trans-unit id="387" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="388" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, causes the standard output   the remote primary R and hadoop job process to be printed to the user console while waiting for (blocking on)  job.</source>
        </trans-unit><trans-unit id="389" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="390" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the default behavior is to clean up the  mporary computational artifacts and delete the result objects upon retrival.</source>
        </trans-unit><trans-unit id="391" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>,  en the computational results are not deleted, and the results may be acquired using  ode<bpt id="p1">[</bpt>rxGetJobResults<ept id="p1">](rxGetJobResults.md)</ept>, and the output via <bpt id="p2">[</bpt>rxGetJobOutput<ept id="p2">](rxGetJobOutput.md)</ept> until the  ode<bpt id="p3">[</bpt>rxCleanupJobs<ept id="p3">](rxCleanup.md)</ept> is used to delete the results and other artifacts.</source>
        </trans-unit><trans-unit id="392" translate="yes" xml:space="preserve">
          <source>Leaving this ag set to <ph id="ph1">`FALSE`</ph> can result in accumulation of compute artifacts which you may entually need to delete before they fill up your hard drive.</source>
        </trans-unit><trans-unit id="393" translate="yes" xml:space="preserve">
          <source>character string specifying a working directory for the processes   the master node.</source>
        </trans-unit><trans-unit id="394" translate="yes" xml:space="preserve">
          <source>NOT YET IMPLEMENTED.</source>
        </trans-unit><trans-unit id="395" translate="yes" xml:space="preserve">
          <source>character vector defining the search path(s) for the data source(s).</source>
        </trans-unit><trans-unit id="396" translate="yes" xml:space="preserve">
          <source>NOT YET IMPLEMENTED.</source>
        </trans-unit><trans-unit id="397" translate="yes" xml:space="preserve">
          <source>or character vector defining the search path(s) for  ew output data file(s).</source>
        </trans-unit><trans-unit id="398" translate="yes" xml:space="preserve">
          <source>If not <ph id="ph1">`NULL`</ph>, this overrides any specification for <ph id="ph2">`outDataPath`</ph>n <bpt id="p1">[</bpt>rxOptions<ept id="p1">](rxOptions.md)</ept></source>
        </trans-unit><trans-unit id="399" translate="yes" xml:space="preserve">
          <source>or an <bpt id="p1">[</bpt>RxHdfsFileSystem<ept id="p1">](RxHdfsFileSystem.md)</ept> to use as the default file system for data sources when created when this compute context is active.</source>
        </trans-unit><trans-unit id="400" translate="yes" xml:space="preserve">
          <source>optional character vector specifying additional packages to be  aded on the nodes when jobs are run in this compute context.</source>
        </trans-unit><trans-unit id="401" translate="yes" xml:space="preserve">
          <source>A numeric value indicating for how long attempts should be made   retrieve results from the cluster.</source>
        </trans-unit><trans-unit id="402" translate="yes" xml:space="preserve">
          <source>Under normal conditions, results are available immediately.</source>
        </trans-unit><trans-unit id="403" translate="yes" xml:space="preserve">
          <source>wever, under certain high load conditions, the processes on the nodes have reported as completed, but e results have not been fully committed to disk by the operating system.</source>
        </trans-unit><trans-unit id="404" translate="yes" xml:space="preserve">
          <source>Increase this parameter  results retrievial is failing on high load clusters.</source>
        </trans-unit><trans-unit id="405" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Microsoft R Services Compute Engine.</source>
        </trans-unit><trans-unit id="406" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="407" translate="yes" xml:space="preserve">
          <source>Use <bpt id="p1">[</bpt>rxImport<ept id="p1">](rxImport.md)</ept> instead of <ph id="ph1">`rxImportToXdf`</ph>.</source>
        </trans-unit><trans-unit id="408" translate="yes" xml:space="preserve">
          <source>Use <bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxDataStep.md)</ept> instead of  <ph id="ph1">`rxDataStepXdf`</ph>.</source>
        </trans-unit><trans-unit id="409" translate="yes" xml:space="preserve">
          <source>Use <bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxDataStep.md)</ept> instead of  <ph id="ph1">`rxDataFrameToXdf`</ph>.</source>
        </trans-unit><trans-unit id="410" translate="yes" xml:space="preserve">
          <source>Use <bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxDataStep.md)</ept> instead of  <ph id="ph1">`rxXdfToDataFrame`</ph>.</source>
        </trans-unit><trans-unit id="411" translate="yes" xml:space="preserve">
          <source>Use <bpt id="p1">[</bpt>rxSort<ept id="p1">](rxSortXdf.md)</ept> instead of  <ph id="ph1">`rxSortXdf`</ph>.</source>
        </trans-unit><trans-unit id="412" translate="yes" xml:space="preserve">
          <source>Use <bpt id="p1">[</bpt>rxGetAvailableNodes<ept id="p1">](rxGetAvailableNodes.md)</ept> instead of  <ph id="ph1">`rxGetNodes`</ph>.</source>
        </trans-unit><trans-unit id="413" translate="yes" xml:space="preserve">
          <source>Use <bpt id="p1">[</bpt>rxSparkConnect<ept id="p1">](RxSpark.md)</ept> instead of  <ph id="ph1">`RxHadoopMR`</ph>.</source>
        </trans-unit><trans-unit id="414" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="415" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxSortXdf`</ph>: If sorting is successful, <ph id="ph2">`TRUE`</ph> is returned; otherwise <ph id="ph3">`FALSE`</ph>is returned.</source>
        </trans-unit><trans-unit id="416" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="417" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxImport<ept id="p1">](rxImport.md)</ept>, <bpt id="p2">[</bpt>rxDataStep<ept id="p2">](rxDataStep.md)</ept>, <bpt id="p3">[</bpt>rxSparkConnect<ept id="p3">](RxSpark.md)</ept>, <bpt id="p4">[</bpt>"RevoScaleR-defunct"<ept id="p4">](RevoScaleR-defunct.md)</ept>.</source>
        </trans-unit></group></body></file></xliff>