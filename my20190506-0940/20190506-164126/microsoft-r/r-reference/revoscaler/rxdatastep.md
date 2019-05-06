<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxdatastep.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750211c7287bc8920a7eae6f8f5d1e1e18e3b759ef2.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">211c7287bc8920a7eae6f8f5d1e1e18e3b759ef2</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxdatastep.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxDataStep function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxDataStep, manip, file</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>rxDataStep: Data Step for RevoScaleR data sources</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Transform data from an input data set to an output data set.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>The rxDataStep function is multi-threaded.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A data source object of these types: <bpt id="p1">[</bpt>RxTextData<ept id="p1">](RxTextData.md)</ept>, <bpt id="p2">[</bpt>RxXdfData<ept id="p2">](RxXdfData.md)</ept>,  <bpt id="p3">[</bpt>RxSasData<ept id="p3">](RxSasData.md)</ept>, <bpt id="p4">[</bpt>RxSpssData<ept id="p4">](RxSpssData.md)</ept>, <bpt id="p5">[</bpt>RxOdbcData<ept id="p5">](RxOdbcData.md)</ept>,  <bpt id="p6">[</bpt>RxSqlServerData<ept id="p6">](RxSqlServerData.md)</ept>, <bpt id="p7">[</bpt>RxTeradata<ept id="p7">](RxTeradata.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If not using a distributed compute context such as RxHadoopMR, a data frame,  a character string specifying the input .xdf file, or <ph id="ph1">`NULL`</ph> can also be used.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, a data set will be created automatically with a single variable, <ph id="ph2">`.rxRowNums`</ph>, containing row numbers.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>It will have a total of <ph id="ph1">`numRows`</ph> rows with <ph id="ph2">`rowsPerRead`</ph> rows in each block.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>A character string specifying the output .xdf file or any of these data sources: <bpt id="p1">[</bpt>RxTextData<ept id="p1">](RxTextData.md)</ept>, <bpt id="p2">[</bpt>RxXdfData<ept id="p2">](RxXdfData.md)</ept>,  <bpt id="p3">[</bpt>RxSasData<ept id="p3">](RxSasData.md)</ept>, <bpt id="p4">[</bpt>RxSpssData<ept id="p4">](RxSpssData.md)</ept>, <bpt id="p5">[</bpt>RxOdbcData<ept id="p5">](RxOdbcData.md)</ept>,  <bpt id="p6">[</bpt>RxSqlServerData<ept id="p6">](RxSqlServerData.md)</ept>, <bpt id="p7">[</bpt>RxTeradata<ept id="p7">](RxTeradata.md)</ept>, <bpt id="p8">[</bpt>RxHiveData<ept id="p8">](RxSparkData.md)</ept>,  <bpt id="p9">[</bpt>RxParquetData<ept id="p9">](RxSparkData.md)</ept>, <bpt id="p10">[</bpt>RxOrcData<ept id="p10">](RxSparkData.md)</ept>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, a data frame will be returned from <ph id="ph2">`rxDataStep`</ph> unless <ph id="ph3">`returnTransformObjects`</ph> is set to <ph id="ph4">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Setting <ph id="ph1">`outFile`</ph> to <ph id="ph2">`NULL`</ph> and <ph id="ph3">`returnTransformObjects=TRUE`</ph> allows chunkwise computations on the data without modifying the existing data or creating a new data set.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>can also be a delimited <bpt id="p1">[</bpt>RxTextData<ept id="p1">](RxTextData.md)</ept> data source if using a native file system and not appending.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>A character vector of variable names to include when reading from the input data file.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToDrop`</ph> or when <ph id="ph2">`outFile`</ph> is the same as the input data file.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Variables used in transformations or row selection will be retained even if not specified in <ph id="ph1">`varsToKeep`</ph>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`newName`</ph> is used in <ph id="ph2">`colInfo`</ph> in a non-xdf  data source, the <ph id="ph3">`newName`</ph> should be used in <ph id="ph4">`varsToKeep`</ph>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Not supported for <bpt id="p1">[</bpt>RxTeradata<ept id="p1">](RxTeradata.md)</ept>, <bpt id="p2">[</bpt>RxOdbcData<ept id="p2">](RxOdbcData.md)</ept>, or <bpt id="p3">[</bpt>RxSqlServerData<ept id="p3">](RxSqlServerData.md)</ept> data sources.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>A character vector of variable names to exclude when reading from the input data file.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToKeep`</ph> or when <ph id="ph2">`outFile`</ph> is the same as the input data file.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Variables used in transformations or row selection will be retained even if specified in <ph id="ph1">`varsToDrop`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`newName`</ph> is used in <ph id="ph2">`colInfo`</ph> in a non-xdf  data source, the <ph id="ph3">`newName`</ph> should be used in <ph id="ph4">`varsToDrop`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Not supported for <bpt id="p1">[</bpt>RxTeradata<ept id="p1">](RxTeradata.md)</ept>, <bpt id="p2">[</bpt>RxOdbcData<ept id="p2">](RxOdbcData.md)</ept>, or  <bpt id="p3">[</bpt>RxSqlServerData<ept id="p3">](RxSqlServerData.md)</ept> data sources.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The name of a logical variable in the data set or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = old`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>will use only observations in which the value of the <ph id="ph1">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph2">`log`</ph> of the <ph id="ph3">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations  (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function  call using the expression function.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>An expression of the form <ph id="ph1">`list(name = expression, ...)`</ph> representing the first round of variable transformations.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>)  can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>When using function call in the expression, <ph id="ph1">`transformObject`</ph> should be used to pass  the function name to remote context.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>In addition, calling and enclosing environment of the function  are very important if the function uses undefined variable.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>A named list containing objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>A variable transformation function.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The recommended way to do variable transformation.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>A character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>A character vector defining additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and  preloaded for use in variable transformation functions, e.g., those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments or those  defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>A user-defined environment to serve as a parent to  all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Either <ph id="ph1">`"none"`</ph> to create a new files, <ph id="ph2">`"rows"`</ph> to append rows to an existing file, or <ph id="ph3">`"cols"`</ph> to append columns to an existing file.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outFile`</ph> exists and <ph id="ph2">`append`</ph> is <ph id="ph3">`"none"`</ph>,  the <ph id="ph4">`overwrite`</ph> argument must be set to <ph id="ph5">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>You cannot append to <bpt id="p1">[</bpt>RxTextData<ept id="p1">](RxTextData.md)</ept> or append columns to <bpt id="p2">[</bpt>RxTeradata<ept id="p2">](RxTeradata.md)</ept> data sources,  and appending is not supported for composite .xdf files or when using the RxHadoopMR compute context.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>A logical value.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outFile`</ph> will be overwritten, or if appending columns existing columns with the same name will be overwritten.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>is ignored if appending rows.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>A character string or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`inData`</ph> is a <ph id="ph2">`data.frame`</ph>: If <ph id="ph3">`NULL`</ph>, the data frame's row names will be dropped.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If a character string, an additional variable of that name will be added to the data set containing the data frame's row names.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>If a <ph id="ph1">`data.frame`</ph> is being returned, a variable with the name <ph id="ph2">`rowVarName`</ph> will be removed as a column from the data frame and will be used as the row names.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>A logical value.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, rows with missing values will be removed on read.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>A logical value.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, rows with missing values will not be included in the output data.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>A logical value.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, low and high values will not automatically be computed.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>This should only be set to <ph id="ph1">`FALSE`</ph> in special circumstances, such as when <ph id="ph2">`append`</ph> is being used repeatedly.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The maximum size of a data frame that will be returned if <ph id="ph1">`outFile`</ph> is set to <ph id="ph2">`NULL`</ph> and <ph id="ph3">`inData`</ph> is an .xdf file , measured by the number of rows times the number of columns.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>If the number of rows times the number of columns being created from the .xdf file exceeds this, a warning will be reported and the number of rows in the returned data frame will be truncated.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`maxRowsByCols`</ph> is set to be too large, you may experience problems  from loading a huge data frame into memory.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>The number of rows to read for each chunk of data read from the input data source.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Use this argument for finer control of the number of rows per block in the output data source.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>If greater than 0, <ph id="ph1">`blocksPerRead`</ph> is ignored.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Cannot be used if <ph id="ph1">`inFile`</ph> is the same as <ph id="ph2">`outFile`</ph>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>The default value of <ph id="ph1">`-1`</ph> specifies that data should be read by blocks according to the <ph id="ph2">`blocksPerRead`</ph> argument.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The starting row to read from the input data source.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Cannot be used if <ph id="ph1">`inFile`</ph> is the same as <ph id="ph2">`outFile`</ph>.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The number of rows to read from the input data source.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`rowSelection`</ph> or <ph id="ph2">`removeMissings`</ph> are used, the output data set may have fewer rows than specified by <ph id="ph3">`numRows`</ph>.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Cannot be used  if <ph id="ph1">`inFile`</ph> is the same as <ph id="ph2">`outFile`</ph>.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>A logical value.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>,  the list of <ph id="ph2">`transformObjects`</ph> will be returned instead of  a data frame or data source object.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>If the input <ph id="ph1">`transformObjects`</ph> have been modified, by using <ph id="ph2">`.rxSet`</ph> or <ph id="ph3">`.rxModify`</ph> in the <ph id="ph4">`transformFunc`</ph>, the updated values will be returned.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Any data returned from the <ph id="ph1">`transformFunc`</ph> is ignored.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>If no <ph id="ph1">`transformObjects`</ph> are used, <ph id="ph2">`NULL`</ph> is returned.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>This argument allows for user-defined  computations within a <ph id="ph1">`transformFunc`</ph> without creating new data.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>is not supported in distributed compute contexts  such as RxHadoopMR.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>The number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Ignored for data frames or if <ph id="ph1">`rowsPerRead`</ph> is positive.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>An integer value with options:</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>An integer in the range of -1 to 9.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the  amount of compression - resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>If  <ph id="ph1">`xdfCompressionLevel`</ph> is set to 0, there will be no compression and files will be compatible  with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression  will be used.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed to the input data source.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>If  <ph id="ph1">`stringsAsFactors`</ph>is specified and the input data source is <ph id="ph2">`RxXdfData`</ph>,  strings with be converted to factors when returning a data frame to R.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxDataStep`</ph>, if <ph id="ph2">`returnTransformObjects`</ph> is <ph id="ph3">`FALSE`</ph>)and an <ph id="ph4">`outFile`</ph> is specified, an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> data source is returned invisibly.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>If no <ph id="ph1">`outFile`</ph> is specified, a data frame is returned invisibly.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Either can be used in subsequent RevoScaleR analysis.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`returnTransformObjects`</ph> is <ph id="ph2">`TRUE`</ph>, the <ph id="ph3">`transformObjects`</ph> list as modified by the transformation function is returned invisibly.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>When working with an <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context, both the input and output data sources must be <bpt id="p2">[</bpt>RxSqlServerData<ept id="p2">](RxSqlServerData.md)</ept>.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxImport<ept id="p1">](rxImport.md)</ept>, <bpt id="p2">[</bpt>RxXdfData<ept id="p2">](RxXdfData.md)</ept>, <bpt id="p3">[</bpt>RxTextData<ept id="p3">](RxTextData.md)</ept>, <bpt id="p4">[</bpt>RxSqlServerData<ept id="p4">](RxSqlServerData.md)</ept>, <bpt id="p5">[</bpt>RxTeradata<ept id="p5">](RxTeradata.md)</ept>, <bpt id="p6">[</bpt>rxGetInfo<ept id="p6">](rxGetInfoXdf.md)</ept>, <bpt id="p7">[</bpt>rxGetVarInfo<ept id="p7">](rxGetVarInfo.md)</ept>, <bpt id="p8">[</bpt>rxTransform<ept id="p8">](rxTransform.md)</ept></source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>