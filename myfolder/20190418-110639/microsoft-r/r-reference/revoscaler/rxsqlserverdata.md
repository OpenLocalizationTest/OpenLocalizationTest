<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxsqlserverdata.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f71fef203f94b57119dbb1911b997263284f2ac07.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">71fef203f94b57119dbb1911b997263284f2ac07</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxsqlserverdata.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxSqlServerData function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This is the main generator for S4 class RxSqlServerData, which extends RxDataSource.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), RxSqlServerData, head.RxSqlServerData, tail.RxSqlServerData, database, connection</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RxSqlServerData: Generate SqlServer Data Source Object</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This is the main generator for S4 class RxSqlServerData, which extends RxDataSource.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or character string specifying the table name.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`sqlQuery`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or character string specifying a valid SQL select query.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Cannot contain hidden characters such as tabs or newlines.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`table`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If you want to use <ph id="ph1">`TABLESAMPLE`</ph> clause in <ph id="ph2">`sqlQuery`</ph>, set <ph id="ph3">`rowBuffering`</ph> argument to <ph id="ph4">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or character string specifying the connection string.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>logical specifying whether or not to buffer rows on read from the database.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If you are having problems with your ODBC driver,  try setting this to <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>logical indicating whether or not to convert the result from a list to a data frame (for use in <ph id="ph1">`rxReadNext`</ph> only).</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>,  a list is returned.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>logical indicating whether or not to automatically convert strings to factors on import.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>This can be overridden by specifying <ph id="ph1">`"character"`</ph> in <ph id="ph2">`colClasses`</ph> and <ph id="ph3">`colInfo`</ph>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the factor levels will be coded in the order encountered.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent, the preferred method for handling factor columns is to use <ph id="ph1">`colInfo`</ph> with specified <ph id="ph2">`"levels"`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>character vector specifying the column types to use when converting the data.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The element names for the vector are used to identify which column should be converted to which type.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Allowable column types are:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"logical"`</ph> (stored as <ph id="ph2">`uchar`</ph>),</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"integer"`</ph> (stored as <ph id="ph2">`int32`</ph>),</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"float32"`</ph> (the default for floating point data for .xdf files),</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"numeric"`</ph> (stored as <ph id="ph2">`float64`</ph> as in R),</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"character"`</ph> (stored as <ph id="ph2">`string`</ph>),</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"factor"`</ph> (stored as <ph id="ph2">`uint32`</ph>),</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"int16"`</ph> (alternative to integer for smaller storage space),</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"uint16"`</ph> (alternative to unsigned integer for smaller storage space),</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Date"`</ph> (stored as Date, i.e. <ph id="ph2">`float64`</ph>)</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Note for <ph id="ph1">`"factor"`</ph> type, the levels will be coded in the order encountered.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent, the preferred method for handling factor columns is to use <ph id="ph1">`colInfo`</ph> with specified <ph id="ph2">`"levels"`</ph>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Note that equivalent types share the same bullet in the list above; for some types we allow both 'R-friendly' type names, as well as our own, more specific type names for .xdf data.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Note also that specifying the column as a "factor" type is currently equivalent to "string" - for the moment, if you wish to import a column as factor data you must use the <ph id="ph1">`colInfo`</ph> argument, documented below.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>list of named variable information lists.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Each variable information list contains one or more of the named elements given below.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The information supplied for <ph id="ph1">`colInfo`</ph> overrides that supplied for <ph id="ph2">`colClasses`</ph>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Currently available properties for a column information list are:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`type`</ph> - character string specifying the data type for the column.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>See <ph id="ph1">`colClasses`</ph> argument description for the available types.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Specify <ph id="ph1">`"factorIndex"`</ph> as the <ph id="ph2">`type`</ph> for 0-based factor indexes.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`levels`</ph> must also be specified.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`newName`</ph> - character string specifying a new name for the variable.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`description`</ph> - character string specifying a description  for the variable.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`levels`</ph> - character vector containing the levels when <ph id="ph2">`type = "factor"`</ph>.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If the levels property is not provided, factor levels will be determined by the values in the source column.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If levels are provided, any value that does not match a provided level will be converted to a missing value.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`newLevels`</ph> - new or replacement levels  specified for a column of type "factor".</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>It must be used in conjunction with the <ph id="ph1">`levels`</ph> argument.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>After reading in the original data, the labels for each level will be replaced with the <ph id="ph1">`newLevels`</ph>.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`low`</ph> - the minimum data value in the variable (used in computations using the <ph id="ph2">`F()`</ph> function.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`high`</ph> - the maximum data value in the variable (used in computations using the <ph id="ph2">`F()`</ph> function.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>number of rows to read at a time.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, information on the odbc data source type (<ph id="ph2">`odbc`</ph> or <ph id="ph3">`odbcFast`</ph>) is printed.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the underlying functions.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>an <ph id="ph1">`RxSqlServerData`</ph> object</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>positive integer.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Number of rows of the data set to extract.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, row numbers will be created to match the original data set.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>logical specifying whether or not to use a direct ODBC connection.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>On Linux systems, this is the only ODBC connection available.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Note: <ph id="ph1">`useFastRead = FALSE`</ph> is currently not supported in writing to SQL Server data source.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Target SQL Server instance.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Can also be specified in the connection string with the <ph id="ph1">`Server`</ph> keyword.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Database on the target SQL Server instance.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Can also be specified in the connection string with the <ph id="ph1">`Database`</ph> keyword.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>SQL login to connect to the SQL Server instance.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>SQL login can also be specified in the connection string with the <ph id="ph1">`uid`</ph> keyword.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Password associated with the SQL login.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Can also be specified in the connection  string with the <ph id="ph1">`pwd`</ph> keyword.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, when writing to an <ph id="ph2">`RxOdbcData`</ph> data source, underlying factor indexes will be written instead of the string representations.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`tail`</ph> method is not functional for this data source type and will report an error.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`user`</ph> and <ph id="ph2">`password`</ph> arguments take precedence over equivalent information provided within the <ph id="ph3">`connectionString`</ph> argument.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>If, for example, you provide the user name in both the <ph id="ph1">`connectionString`</ph> and <ph id="ph2">`user`</ph> arguments, the one in <ph id="ph3">`connectionString`</ph> is ignored.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>object of class RxSqlServerData.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>TODO: Update references.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxSqlServerData-class<ept id="p1">](RxSqlServerData-class.md)</ept>, <bpt id="p2">[</bpt>rxNewDataSource<ept id="p2">](rxNew.md)</ept>, <bpt id="p3">[</bpt>rxImport<ept id="p3">](rxImport.md)</ept>.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>