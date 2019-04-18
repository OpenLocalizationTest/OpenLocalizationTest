<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxtextdata.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef0690673357230545b758ef6deeed07f156db086c6060cd0d1.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">7230545b758ef6deeed07f156db086c6060cd0d1</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxtextdata.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxTextData function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This is the main generator for S4 class RxTextData, which extends RxDataSource.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), RxTextData, file, connection</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RxTextData: Generate Text Data Source Object</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This is the main generator for S4 class RxTextData, which extends RxDataSource.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>character string specifying a text file.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If it has an .stsextension, it is interpreted as a fixed format schema file.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`colInfo`</ph> argument contains <ph id="ph2">`start`</ph> and <ph id="ph3">`width`</ph> information, it is interpreted as a fixed format data file.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Otherwise, it is treated as a delimited text data file.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>See the Details section for more information on using .sts files.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>logical indicating whether or not to convert the result from a list to a data frame (for use in <ph id="ph1">`rxReadNext`</ph> only).</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>,  a list is returned.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>logical indicating whether or not to automatically convert strings to factors on import.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>This can be overridden by specifying <ph id="ph1">`"character"`</ph> in <ph id="ph2">`colClasses`</ph> and <ph id="ph3">`colInfo`</ph>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the factor levels will be coded in the order encountered.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent, the preferred method for handling factor columns is to use <ph id="ph1">`colInfo`</ph> with specified <ph id="ph2">`"levels"`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>character vector specifying the column types to use when converting the data.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The element names for the vector are used to identify which column should be converted to which type.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Allowable column types are:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"logical"`</ph> (stored as <ph id="ph2">`uchar`</ph>),</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"integer"`</ph> (stored as <ph id="ph2">`int32`</ph>),</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"float32"`</ph> (the default for floating point data for .xdf files),</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"numeric"`</ph> (stored as <ph id="ph2">`float64`</ph> as in R),</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"character"`</ph> (stored as <ph id="ph2">`string`</ph>),</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"factor"`</ph> (stored as <ph id="ph2">`uint32`</ph>),</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"ordered"`</ph> (ordered factor stored as <ph id="ph2">`uint32`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Ordered factors are treated the same as factors in RevoScaleR analysis functions.),</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"int16"`</ph> (alternative to integer for smaller storage space),</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"uint16"`</ph> (alternative to unsigned integer for smaller storage space),</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Date"`</ph> (stored as Date, i.e. <ph id="ph2">`float64`</ph>. Not supported if <ph id="ph3">`useFastRead`</ph><ph id="ph4"> = </ph><ph id="ph5">`TRUE`</ph>.)</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"POSIXct"`</ph> (stored as POSIXct, i.e. <ph id="ph2">`float64`</ph>. Not supported if <ph id="ph3">`useFastRead`</ph><ph id="ph4"> = </ph><ph id="ph5">`TRUE`</ph>.)</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Note for <ph id="ph1">`"factor"`</ph> and <ph id="ph2">`"ordered"`</ph> types, the levels will  be coded in the order encountered.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent,  the preferred method for handling factor columns is to use <ph id="ph1">`colInfo`</ph> with specified <ph id="ph2">`"levels"`</ph>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>list of named variable information lists.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Each variable information list contains one or more of the named elements given below.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>When importing fixed format data, either <ph id="ph1">`colInfo`</ph> or an .sts schema file should be supplied.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>For such fixed format data, only the variables specified will be imported.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>For all text types, the information supplied for <ph id="ph1">`colInfo`</ph>overrides that supplied for <ph id="ph2">`colClasses`</ph>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Currently available properties for a column information list are:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`type`</ph> - character string specifying the data type for the column.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>See <ph id="ph1">`colClasses`</ph> argument description for the available types.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`type`</ph> is not specified for fixed format data, it will be read as character data.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`newName`</ph> - character string specifying a new name for the variable.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`description`</ph> - character string specifying a description  for the variable.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`levels`</ph> - character vector containing the levels when <ph id="ph2">`type = "factor"`</ph>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>If the levels property is not provided, factor levels will be determined by the values in the source column.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>If levels are provided, any value that does not match a provided level will be converted to a missing value.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`newLevels`</ph> - new or replacement levels  specified for a column of type "factor".</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>It must be used in conjunction with the <ph id="ph1">`levels`</ph> argument.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>After reading in the original data, the labels for each level will be replaced with the <ph id="ph1">`newLevels`</ph>.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`low`</ph> - the minimum data value in the variable (used in computations using the <ph id="ph2">`F()`</ph> function.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`high`</ph> - the maximum data value in the variable (used in computations using the <ph id="ph2">`F()`</ph> function.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`start`</ph> - the left-most position, in bytes, for the column  of a fixed format file respectively.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>When all elements of <ph id="ph1">`colInfo`</ph> have  <ph id="ph2">`"start"`</ph>, the text file is designated as a fixed format file.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>When none of the elements have it, the text file is designated as a delimited file.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Specification of <ph id="ph1">`start`</ph> must always be accompanied by specification of <ph id="ph2">`width`</ph>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`width`</ph> - the number of characters in a fixed-width character column or the column of a fixed format file.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`width`</ph>is specified for a character column, it will be imported as a fixed-width character variable.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Any characters beyond the fixed width will be ignored.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Specification of <ph id="ph1">`width`</ph> is required for all columns of a fixed format file (if not provided in an .sts file).</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`decimalPlaces`</ph> - the number of decimal places.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`index`</ph> - column index in the original delimited text data file.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>It is used as an alternative to naming the variable information list if the  original delimited text file does not contain column names.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Ignored if a name for the list is specified.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Should not be used with fixed format files.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>character vector of variable names to include when reading from the input data file.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToDrop`</ph>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>character vector of variable names to exclude when reading from the input data file.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToKeep`</ph>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>character string containing the missing value code.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>It can be an empty string: <ph id="ph1">`""`</ph>.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>number of rows to read at a time.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>character string containing the character to use as the separator between variables.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> and the <ph id="ph2">`colInfo`</ph> argument does not contain <ph id="ph3">`"start"`</ph> and <ph id="ph4">`"width"`</ph> information (which implies a fixed-formatted file), the delimiter is auto-sensed from the list <ph id="ph5">`","`</ph>, <ph id="ph6">`"\t"`</ph>, <ph id="ph7">`";"`</ph>, and <ph id="ph8">`" "`</ph>.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>logical indicating whether or not to treat consecutive non-space (<ph id="ph1">`" "`</ph>) delimiters as a single delimiter.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Space <ph id="ph1">`" "`</ph> delimiters are always combined.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>character string containing the quotation mark.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>It can be an empty string: <ph id="ph1">`""`</ph>.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>character string containing the decimal point.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Not supported when <ph id="ph1">`useFastRead`</ph> is set to <ph id="ph2">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>character string containing the thousands separator.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Not supported when <ph id="ph1">`useFastRead`</ph> is set to <ph id="ph2">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>character string containing the time date format to use during read operations.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Not supported when <ph id="ph1">`useFastRead`</ph> is set to <ph id="ph2">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Valid formats are:</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%c`</ph> Skip a single character (see also <ph id="ph2">`%w`</ph>).</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%Nc`</ph> Skip <ph id="ph2">`N`</ph> characters.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%$c`</ph> Skip the rest of the input string.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%d`</ph> Day of the month as integer (01-31).</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%m`</ph> Month as integer (01-12) or as character string.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%w`</ph> Skip a whitespace delimited word (see also <ph id="ph2">`%c`</ph>).</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%y`</ph> Year.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>If less than 100, <ph id="ph1">`centuryCutoff`</ph> is used to determine the actual year.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%Y`</ph> Year as found in the input string.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%%`</ph>, <ph id="ph2">`%[`</ph>, <ph id="ph3">`%]`</ph> input the <ph id="ph4">`%`</ph>, <ph id="ph5">`[`</ph>, and <ph id="ph6">`]`</ph> characters from the input string.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`[...]`</ph> square brackets within format specifications indicate optional components; if present, they are used, but they need not be there.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>character string containing the time date format to use during read operations.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Not supported when <ph id="ph1">`useFastRead`</ph> is set to <ph id="ph2">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Valid formats are:</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%c`</ph> Skip a single character (see also <ph id="ph2">`%w`</ph>).</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%Nc`</ph> Skip <ph id="ph2">`N`</ph> characters.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%$c`</ph> Skip the rest of the input string.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%d`</ph> Day of the month as integer (01-31).</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%H`</ph> Hour as integer (00-23).</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%m`</ph> Month as integer (01-12) or as character string.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%M`</ph> Minute as integer (00-59).</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%n`</ph> Milliseconds as integer (00-999).</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%N`</ph> Milliseconds or tenths or hundredths of second.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%p`</ph> Character string defining 'am'/'pm'.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%S`</ph> Second as integer (00-59).</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%w`</ph> Skip a whitespace delimited word (see also <ph id="ph2">`%c`</ph>).</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%y`</ph> Year.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>If less than 100, <ph id="ph1">`centuryCutoff`</ph> is used to determine the actual year.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%Y`</ph> Year as found in the input string.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`%%`</ph>, <ph id="ph2">`%[`</ph>, <ph id="ph3">`%]`</ph> input the <ph id="ph4">`%`</ph>, <ph id="ph5">`[`</ph>, and <ph id="ph6">`]`</ph> characters from the input string.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`[...]`</ph> square brackets within format specifications indicate optional components; if present, they are used, but they need not be there.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>integer specifying the changeover year between the twentieth  and twenty-first century if two-digit years are read.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Values less than <ph id="ph1">`centuryCutoff`</ph>are prefixed by 20 and those greater than or equal to <ph id="ph2">`centuryCutoff`</ph> are prefixed by 19.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>If you specify 0, all two digit dates are interpreted as years in the twentieth century.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Not supported when <ph id="ph1">`useFastRead`</ph> is set to <ph id="ph2">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>logical indicating if the first row represents column names for reading text.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`firstRowIsColNames`</ph> is <ph id="ph2">`NULL`</ph>, then column names are auto- detected.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>The logic for auto-detection is: if the first row contains all values that are interpreted as character and the second row contains at least one value that is interpreted as numeric, then the first row is considered to be column names; otherwise the first row is considered to be the first data row.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Not relevant for fixed format data.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>As for writing, it specifies to write column names as the first row.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`firstRowIsColNames`</ph> is <ph id="ph2">`NULL`</ph>, the default is to  write the column names as the first row.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>number of rows to use in determining column type.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>integer indicating number of leading rows to ignore.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Only supported for <ph id="ph1">`useFastRead = TRUE`</ph>.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>number of rows to read into a temporary buffer.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>This value could affect the speed of import.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Used to specify a column's data type when  only decimal values (possibly mixed with missing (<ph id="ph1">`NA`</ph>) values) are encountered upon first read of the data and the column's type information is not specified via <ph id="ph2">`colInfo`</ph> or <ph id="ph3">`colClasses`</ph>.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Supported types are "float32" and "numeric", for 32-bit floating point and 64-bit  floating point values, respectively.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Used to specify a given column's data type when  only missings (<ph id="ph1">`NA`</ph>s) or blanks are encountered upon first read of the data  and the column's type information is not specified via <ph id="ph2">`colInfo`</ph> or <ph id="ph3">`colClasses`</ph>.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Supported types are "float32", "numeric", and "character" for 32-bit floating point, 64-bit floating point and string values, respectively.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Only supported for <ph id="ph1">`useFastRead = TRUE`</ph>.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>integer specifying the precision to use when  writing numeric data to a file.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, if there are only  zeros after the decimal point for a numeric, it will be written as  an integer to a file.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, delimiters  within quoted strings will be ignored.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>This requires a slower parsing  process.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Only applicable to <ph id="ph1">`useFastRead`</ph> is set to <ph id="ph2">`TRUE`</ph>;  delimiters within quotes are always supported when <ph id="ph3">`useFastRead`</ph>  is set to <ph id="ph4">`FALSE`</ph> .</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the input data file is treated as a fixed format file.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Fixed format files must have a .sts file or a <ph id="ph1">`colInfo`</ph> argument specifying the <ph id="ph2">`start`</ph> and <ph id="ph3">`width`</ph> of each variable.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, the input data file is treated as a delimited text file.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the text file type (fixed or delimited text) is auto-determined.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or logical scalar.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the data file is accessed directly by the Microsoft R Services Compute Engine.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>,  StatTransfer is used to access the data file.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the type of text import is auto-determined.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`useFastRead`</ph> should be set to <ph id="ph2">`FALSE`</ph> if importing <ph id="ph3">`Date`</ph> or <ph id="ph4">`POSIXct`</ph> data types, if the data set contains the delimiter character inside a quoted string, if the <ph id="ph5">`decimalPoint`</ph> is not <ph id="ph6">`"."`</ph>, if the <ph id="ph7">`thousandsSeparator`</ph> is not <ph id="ph8">`","`</ph>, if the <ph id="ph9">`quoteMark`</ph> is not <ph id="ph10">`"\""`</ph>, or if <ph id="ph11">`combineDelimiters`</ph> is set to <ph id="ph12">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`useFastRead`</ph> should be set to <ph id="ph2">`TRUE`</ph> if <ph id="ph3">`rowsToSkip`</ph> or <ph id="ph4">`defaultMissingColType`</ph> are set.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`useFastRead`</ph> is <ph id="ph2">`TRUE`</ph>, by default variables containing the values <ph id="ph3">`TRUE`</ph> and <ph id="ph4">`FALSE`</ph> or <ph id="ph5">`T`</ph> and <ph id="ph6">`F`</ph> will be created as logical variables.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`useFastRead`</ph> cannot be set to <ph id="ph2">`FALSE`</ph> if an HDFS file system is being used.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>If an incompatible setting of <ph id="ph1">`useFastRead`</ph> is detected, a warning will be issued and the value will be changed.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>logical value or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Used only when writing.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, a file folder of text files will be created instead of a single text file.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>A directory will be created whose name is the same as the text file that would otherwise be created, but with no extension.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>In the directory, the data will be split across a set of text files (see <ph id="ph1">`rowsPerOutFile`</ph> below for determining how many rows of data will be in each file).</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, a single text file will be created.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, a folder of files will be created if the input data set is a composite XDF file or a folder of text files.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>This argument is ignored if the text file is fixed format.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>numeric value or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>If a directory of text files is being created, and if the compute context is not <ph id="ph1">`RxHadoopMR`</ph>, this will be the number of rows of data put into each file in the directory.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>When importing is being done on Hadoop using MapReduce, the number of rows per file is determined by the rows assigned to each MapReduce task.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the rows of data will match the input data.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, information on the text type (<ph id="ph2">`text`</ph> or <ph id="ph3">`textFast`</ph>) is printed.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> variable names specified in <ph id="ph2">`varsToKeep`</ph> will be checked against variables in the data set to make sure they exist.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>An error will be reported if not found.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>If there are more than 500 variables in the data set, this flag is ignored and no checking is performed.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>character string or <bpt id="p1">[</bpt>RxFileSystem<ept id="p1">](RxFileSystem.md)</ept> object indicating type of file system;  <ph id="ph1">`"native"`</ph>or <ph id="ph2">`RxNativeFileSystem`</ph> object can be used for the local operating system, or an <ph id="ph3">`RxHdfsFileSystem`</ph> object for the Hadoop file system.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>character string indicating the encoding used by input text.</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>May be set to either <ph id="ph1">`"utf-8"`</ph> (the default), or <ph id="ph2">`"gb18030"`</ph>, a standard Chinese encoding.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>Not supported when <ph id="ph1">`useFastRead`</ph> is set to  <ph id="ph2">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, when writing to an <ph id="ph2">`RxTextData`</ph> data source, underlying factor indexes will be written instead of the string representations.</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>Not supported when  <ph id="ph1">`useFastRead`</ph> is set to <ph id="ph2">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Delimited Data Type Details<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>Imported <ph id="ph1">`POSIXct`</ph> will have the <ph id="ph2">`tzone`</ph> attribute set to <ph id="ph3">`"GMT"`</ph>.</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>Decimal data in text files can be imported into .xdf files and stored as either 32-bit floats or 64-bit doubles.</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>The default for this is 32-bit floats, which can be changed using <bpt id="p1">[</bpt>rxOptions<ept id="p1">](rxOptions.md)</ept>.</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>If the data type cannot be determined (i.e., only missing values are encountered), the column is imported as 64-bit doubles unless otherwise specified.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>If stored in 32-bit floats, they are converted into 64-bit doubles whenever they are brought into R. Because there may be no exact binary representation of a particular decimal number, the resulting double may be (slightly) different from a double created by directly converting a decimal value to a double.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>Thus exact comparisons of values may result in unexpected behavior.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>For example, if <ph id="ph1">`x`</ph> is imported from a text file with a decimal value of <ph id="ph2">`"1.2"`</ph> and stored as a float in an .xdf file, the closest decimal representation of the stored value displayed as a double is <ph id="ph3">`1.2000000476837158`</ph>.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>So, bringing it into R as a double and comparing with a decimal constant of <ph id="ph1">`1.2`</ph>, e.g. <ph id="ph2">`x == 1.2`</ph>, will result in <ph id="ph3">`FALSE`</ph> because the decimal constant <ph id="ph4">`1.2`</ph> in the code is being converted directly to a double.</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>To store imported text decimal data as 64-bit doubles in an .xdf file, set the <ph id="ph1">`defaultDecimalColType`</ph> to <ph id="ph2">`"numeric"`</ph>.</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>Doing so will increase the size of the .xdf file, since the size of a double is twice that of a float.</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Fixed Format Schema Details<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>The .sts schema for a fixed format data file consists of two required components (<ph id="ph1">`FILE`</ph> and <ph id="ph2">`VARIABLES`</ph>) and one optional component (<ph id="ph3">`FIRST LINE`</ph>), representing the first line of the data file to read.</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>where (A) is used to tag character columns, else use no tag for numeric columns.</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>If the data file names and .sts file name are different, the full path must be specified in the <ph id="ph1">`FILE`</ph> component.</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>See <ph id="ph1">`file.show(file.path(rxGetOption("sampleDataDir"), "claims.sts"))`</ph> for an example fixed format schema file.</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>If a .sts schema file is used in addition to a <ph id="ph1">`colInfo`</ph> argument, schema file is read first, then the <ph id="ph2">`colInfo`</ph> is used to modify that information (for example, to specify that a variable should be read as a factor).</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Encoding Details<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>Character data in the input file must be encoded as ASCII or UTF-8 in order to be imported correctly.</source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>If the data contains UTF-8 multibyte (i.e., non-ASCII) characters, make sure the <ph id="ph1">`useFastRead`</ph> parameter is set to <ph id="ph2">`FALSE`</ph> as the 'fast' version of this object may not handle extended UTF-8 characters correctly.</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>object of class RxTextData.</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxTextData-class<ept id="p1">](RxTextData-class.md)</ept>, <bpt id="p2">[</bpt>rxImport<ept id="p2">](rxImport.md)</ept>, <bpt id="p3">[</bpt>rxNewDataSource<ept id="p3">](rxNew.md)</ept>.</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>