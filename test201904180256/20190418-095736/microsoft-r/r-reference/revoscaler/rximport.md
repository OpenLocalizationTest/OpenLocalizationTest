<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rximport.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c67478407a367125de1c3bb2cc92b2be75cce2707.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">67478407a367125de1c3bb2cc92b2be75cce2707</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rximport.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxImport function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Import data into an .xdf file or data.frame.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxImport is multi-threaded.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxImport, file, connection</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>rxImport: Import Data to .xdf or data frame</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Import data into an .xdf file or <ph id="ph1">`data.frame`</ph>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>rxImport is multi-threaded.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>a character string with the path for the data  to import (delimited, fixed format, SPSS, SAS, ODBC, or XDF).</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Alternatively, a  data source object representing the input data source can be  specified.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>(See <bpt id="p1">[</bpt>RxTextData<ept id="p1">](RxTextData.md)</ept>, <bpt id="p2">[</bpt>RxSasData<ept id="p2">](RxSasData.md)</ept>, <bpt id="p3">[</bpt>RxSpssData<ept id="p3">](RxSpssData.md)</ept>, and <bpt id="p4">[</bpt>RxOdbcData<ept id="p4">](RxOdbcData.md)</ept>.) If a character  string is supplied and <ph id="ph1">`type`</ph> is set to <ph id="ph2">`"auto"`</ph>, the type of file is  inferred from its extension, with the default being a text file.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A  <ph id="ph1">`data.frame`</ph> can also be used for <ph id="ph2">`inData`</ph>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>a character string representing the output .xdf file, a  <bpt id="p1">[</bpt>RxHiveData<ept id="p1">](RxSparkData.md)</ept> data source, a<bpt id="p2">[</bpt>RxParquetData<ept id="p2">](RxSparkData.md)</ept> data source or   a <bpt id="p3">[</bpt>RxXdfData<ept id="p3">](RxXdfData.md)</ept> object.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, a data frame will be returned in memory.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>character vector of variable names to include when reading from the input data file.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToDrop`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Not supported for ODBC or fixed format text files.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>character vector of variable names to exclude when reading from the input data file.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToKeep`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Not supported for ODBC or fixed format text files.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>name of a logical variable in the data set (in quotes) or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rowSelection = (age &gt; 20) &amp; (age &lt; 65) &amp; (log(income) &gt; 10)`</ph> will use only observations in which the value of the <ph id="ph2">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph3">`log`</ph> of the <ph id="ph4">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations  (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function  call using the expression function.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>an expression of the form <ph id="ph1">`list(name = expression, ...)`</ph> representing the first round of variable transformations.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>)  can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>a named list containing objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>variable transformation function.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>character vector defining additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and  preloaded for use in variable transformation functions, e.g., those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments or those  defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>user-defined environment to serve as a parent to  all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>either <ph id="ph1">`"none"`</ph> to create a new .xdf file or <ph id="ph2">`"rows"`</ph> to append rows to an existing .xdf file.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outFile`</ph> exists and <ph id="ph2">`append`</ph> is <ph id="ph3">`"none"`</ph>, the <ph id="ph4">`overwrite`</ph> argument must be set to <ph id="ph5">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Ignored if a data frame is returned.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the existing <ph id="ph2">`outData`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Ignored if a dataframe is returned.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>integer value specifying the maximum number of rows to import.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If set to -1, all rows will be imported.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>logical indicating whether or not to automatically convert strings to factors on import.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>This can be overridden by specifying <ph id="ph1">`"character"`</ph> in <ph id="ph2">`colClasses`</ph> and <ph id="ph3">`colInfo`</ph>.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the factor levels will be coded in the order encountered.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent, the preferred method for handling factor columns is to use <ph id="ph1">`colInfo`</ph> with specified <ph id="ph2">`"levels"`</ph>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>character vector specifying the column types to use when converting the data.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The element names for the vector are used to identify which column should be converted to which type.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Allowable column types are:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"logical"`</ph> (stored as <ph id="ph2">`uchar`</ph>),</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"integer"`</ph> (stored as <ph id="ph2">`int32`</ph>),</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"float32"`</ph> (the default for floating point data for .xdf files),</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"numeric"`</ph> (stored as <ph id="ph2">`float64`</ph> as in R),</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"character"`</ph> (stored as <ph id="ph2">`string`</ph>),</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"factor"`</ph> (stored as <ph id="ph2">`uint32`</ph>),</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"ordered"`</ph> (ordered factor stored as <ph id="ph2">`uint32`</ph>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Ordered factors are treated the same as factors in RevoScaleR analysis functions.),</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"int16"`</ph> (alternative to integer for smaller storage space),</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"uint16"`</ph> (alternative to unsigned integer for smaller storage space),</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Date"`</ph> (stored as Date, i.e. <ph id="ph2">`float64`</ph>. Not supported for import types <ph id="ph3">`"textFast"`</ph>, <ph id="ph4">`"fixedFast"`</ph>, or <ph id="ph5">`"odbcFast"`</ph>.)</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"POSIXct"`</ph> (stored as POSIXct, i.e. <ph id="ph2">`float64`</ph>. Not supported for import types <ph id="ph3">`"textFast"`</ph>, <ph id="ph4">`"fixedFast"`</ph>, or <ph id="ph5">`"odbcFast"`</ph>.)</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Note for <ph id="ph1">`"factor"`</ph> and <ph id="ph2">`"ordered"`</ph> types, the levels will be coded in the order encountered.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent, the preferred method for handling factor columns is to use <ph id="ph1">`colInfo`</ph> with specified <ph id="ph2">`"levels"`</ph>.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Note that equivalent types share the same bullet in the list above; for some types we allow both 'R-friendly' type names, as well as our own, more specific type names for .xdf data.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Note also that specifying the column as a "factor" type is currently equivalent to "string" - for the moment, if you wish to import a column as factor data you must use the <ph id="ph1">`colInfo`</ph> argument, documented below.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>list of named variable information lists.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Each variable information list contains one or more of the named elements given below.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>When importing fixed format data, either <ph id="ph1">`colInfo`</ph> or an .sts schema file should be supplied.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>For fixed format text files, only the variables specified will be imported.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>For all text types, the information supplied for <ph id="ph1">`colInfo`</ph>overrides that supplied for <ph id="ph2">`colClasses`</ph>.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Currently available properties for a column information list are:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`type`</ph> - character string specifying the data type for the column.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>See <ph id="ph1">`colClasses`</ph> argument description for the available types.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`type`</ph> is not specified for fixed format data, it will be read as character data.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`newName`</ph> - character string specifying a new name for the variable.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`description`</ph> - character string specifying a description  for the variable.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`levels`</ph> - character vector containing the levels when <ph id="ph2">`type = "factor"`</ph>.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>If the levels property is not provided, factor levels will be determined by the values in the source column.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>If levels are provided, any value that does not match a provided level will be converted to a missing value.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`newLevels`</ph> - new or replacement levels  specified for a column of type "factor".</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>It must be used in conjunction with the <ph id="ph1">`levels`</ph> argument.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>After reading in the original data, the labels for each level will be replaced with the <ph id="ph1">`newLevels`</ph>.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`low`</ph> - the minimum data value in the variable (used in computations using the <ph id="ph2">`F()`</ph> function.)</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`high`</ph> - the maximum data value in the variable (used in computations using the <ph id="ph2">`F()`</ph> function.)</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`start`</ph> - the left-most position, in bytes, for the column  of a fixed format file respectively.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>When all elements of <ph id="ph1">`colInfo`</ph> have  <ph id="ph2">`start`</ph>, the text file is designated as a fixed format file.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>When none of the elements have it, the text file is designated as a delimited file.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Specification of <ph id="ph1">`start`</ph> must always be accompanied by specification of <ph id="ph2">`width`</ph>.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`width`</ph> - the number of characters in a fixed-width character column or the column of a fixed format file.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`width`</ph>is specified for a character column, it will be imported as a fixed-width character variable.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Any characters beyond the fixed width will be ignored.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Specification of <ph id="ph1">`width`</ph> is required for all columns of a fixed format file.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`decimalPlaces`</ph> - the number of decimal places.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>number of rows to read at a time.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>character string set specifying file type of <ph id="ph1">`inData`</ph>.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>This is ignored if <ph id="ph1">`inData`</ph> is a data source.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Possible values are:</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"auto"`</ph>: file type is automatically detected by looking at file extensions and argument values.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"textFast"`</ph>: delimited text import using faster, more limited import mode.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>By default variables containing the values <ph id="ph1">`TRUE`</ph> and <ph id="ph2">`FALSE`</ph> or <ph id="ph3">`T`</ph> and <ph id="ph4">`F`</ph> will be created as logical variables.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"text"`</ph>: delimited text import using enhanced, slower import mode (not supported with HDFS).</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>This allows for importing Date and POSIXct data types, handling the delimiter character inside a quoted string, and specifying decimal character and thousands separator.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>(See <bpt id="p1">[</bpt>RxTextData<ept id="p1">](RxTextData.md)</ept>.)</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"fixedFast"`</ph>: fixed format text import using faster, more limited import mode.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>You must specify a .sts format file or colInfo specifications with <ph id="ph1">`start`</ph> and <ph id="ph2">`width`</ph>for each variable.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"fixed"`</ph>: fixed format text import using enhanced, slower import mode (not supported with HDFS).</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>This allows for importing Date and POSIXct data types and specifying decimal character and thousands separator.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>You must specify a .sts format file or colInfo specifications with <ph id="ph1">`start`</ph> and <ph id="ph2">`width`</ph>for each variable.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"sas"`</ph>: SAS data files.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>(See <bpt id="p1">[</bpt>RxSasData<ept id="p1">](RxSasData.md)</ept>.)</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"spss"`</ph>: SPSS data files.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>(See <bpt id="p1">[</bpt>RxSpssData<ept id="p1">](RxSpssData.md)</ept>.)</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"odbcFast"`</ph>: ODBC import using faster, more limited import mode.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"odbc"`</ph>: ODBC import using slower, enhanced import on Windows.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>(See <bpt id="p1">[</bpt>RxOdbcData<ept id="p1">](RxOdbcData.md)</ept>.)</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>the maximum size of a data frame that will be read in if <ph id="ph1">`outData`</ph> is set to <ph id="ph2">`NULL`</ph>, measured by the number of rows times the number of columns.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>If the number of rows times the number of columns being imported exceeds this,  a warning will be reported and a smaller number of rows will be read in than requested.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`maxRowsByCols`</ph> is set to be too large, you may experience problems  from loading a huge data frame into memory.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, information on the import type is printed if <ph id="ph2">`type`</ph> is set  to <ph id="ph3">`auto`</ph>.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>integer in the range of -1 to 9.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the  amount of compression - resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>If  <ph id="ph1">`xdfCompressionLevel`</ph> is set to 0, there will be no compression and files will be compatible  with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression  will be used.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>logical value or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, a composite set of files will be created instead of a single .xdf file.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>A directory will be created whose name is the same as the .xdf file that would otherwise be created, but with no extension.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Subdirectories data and metadata will be created.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>In the data subdirectory, the data will be split across a set of .xdfd files (see <ph id="ph1">`blocksPerCompositeFile`</ph> below for determining how many blocks of data will be in each file).</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>In the metadata subdirectory  there is a single .xdfm file, which contains the meta data for all of the  .xdfd files in the  data subdirectory.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>When the compute context is <ph id="ph1">`RxHadoopMR`</ph> a composite set of files is always created.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`createCompositeSet=TRUE`</ph>, and if the compute context is not <ph id="ph2">`RxHadoopMR`</ph>, this will be the number of blocks put into each .xdfd file in the composite set.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>When importing is being done on Hadoop using MapReduce, the number of rows per .xdfd file is determined by the rows assigned to each MapReduce task, and the number of blocks per .xdfd file is therefore determined by <ph id="ph1">`rowsPerRead`</ph>.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`outFile`</ph> is an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object, set the value for <ph id="ph2">`blocksPerCompositeFile`</ph> there instead.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the underlying data source objects to be imported.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>These argument values will override the existing values in an existing data source, if it is passed in as the <ph id="ph1">`inData`</ph>.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>RxTextData<ept id="p1">](RxTextData.md)</ept>, <bpt id="p2">[</bpt>RxSasData<ept id="p2">](RxSasData.md)</ept>, <bpt id="p3">[</bpt>RxSpssData<ept id="p3">](RxSpssData.md)</ept>, and <bpt id="p4">[</bpt>RxOdbcData<ept id="p4">](RxOdbcData.md)</ept>.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>If a data source is passed in as <ph id="ph1">`inData`</ph>, argument values specified in the call to <ph id="ph2">`rxImport`</ph> will override any existing specifications in the data source.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>Setting <ph id="ph1">`type`</ph> to <ph id="ph2">`"text"`</ph>, <ph id="ph3">`"fixed"`</ph>, or <ph id="ph4">`"odbc"`</ph> is equivalent to setting <ph id="ph5">`useFastRead`</ph> to <ph id="ph6">`FALSE`</ph> in an <bpt id="p1">[</bpt>RxTextData<ept id="p1">](RxTextData.md)</ept> or <bpt id="p2">[</bpt>RxOdbcData<ept id="p2">](RxOdbcData.md)</ept> input data source.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Similarly, setting <ph id="ph1">`type`</ph> to <ph id="ph2">`"textFast"`</ph>, <ph id="ph3">`"fixedFast"`</ph>, or <ph id="ph4">`"odbcFast"`</ph> is equivalent to setting <ph id="ph5">`useFastRead`</ph> to <ph id="ph6">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>The input and output data sources are automatically opened and closed within the <ph id="ph1">`rxImport`</ph> function.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>For reasons of performance, the <ph id="ph1">`textFast`</ph> 'type' does not properly handle text files that contain the delimiter character inside a quoted string (for example, the entry "Wade, John" inside a comma delimited file.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Use the <ph id="ph1">`text`</ph> 'type' if your data set contains character data with this characteristic.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>For information on using a .sts schema file for fixed format text import, see the <bpt id="p1">[</bpt>RxTextData<ept id="p1">](RxTextData.md)</ept> help file.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Encoding Details<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Some files or data sources contain character data encoded in a particular format (for example, Excel files will always use UTF-16).</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Others may contain encoding information inside the file itself.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>When not determined by the file type, or specified within the file, character data in the input file or data source must be encoded as ASCII or UTF-8 in order to be imported correctly.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>If the data contains UTF-8 multibyte (i.e., non-ASCII) characters, make sure the <ph id="ph1">`type`</ph> parameter is set to <ph id="ph2">`"text"`</ph> or <ph id="ph3">`"fixed"`</ph> for text import and <ph id="ph4">`"odbc"`</ph> for ODBC import as the 'fast' versions of these values may not handle extended UTF-8 characters correctly.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>If an <ph id="ph1">`outFile`</ph> is not specified, an output data frame is returned.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>If an <ph id="ph1">`outFile`</ph> is specified, an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> data source is returned that can be used in subsequent RevoScaleR analysis.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxDataSource-class<ept id="p1">](RxDataSource-class.md)</ept>, <bpt id="p2">[</bpt>rxDataStep<ept id="p2">](rxDataStep.md)</ept>, <bpt id="p3">[</bpt>RxTextData<ept id="p3">](RxTextData.md)</ept>, <bpt id="p4">[</bpt>RxSasData<ept id="p4">](RxSasData.md)</ept>, <bpt id="p5">[</bpt>RxSpssData<ept id="p5">](RxSpssData.md)</ept>, <bpt id="p6">[</bpt>RxOdbcData<ept id="p6">](RxOdbcData.md)</ept>, <bpt id="p7">[</bpt>RxXdfData<ept id="p7">](RxXdfData.md)</ept>, <bpt id="p8">[</bpt>rxSplit<ept id="p8">](rxSplitXdf.md)</ept>, <bpt id="p9">[</bpt>rxTransform<ept id="p9">](rxTransform.md)</ept>.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>