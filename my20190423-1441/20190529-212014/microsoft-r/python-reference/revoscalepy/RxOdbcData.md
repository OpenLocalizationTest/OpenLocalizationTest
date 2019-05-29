<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="RxOdbcData.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3a41e13dff96982811433b5734f1d175f1ef479e0.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a41e13dff96982811433b5734f1d175f1ef479e0</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\RxOdbcData.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxOdbcData: Class generator for ODBC data source objects (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Main generator for class RxOdbcData, which extends RxDataSource.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>odbc, datasource</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RxOdbcData</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Main generator for class RxOdbcData, which extends RxDataSource.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>connection_string</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>None or character string specifying the connection string.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>table</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>None or character string specifying the table name.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Cannot be used with sqlQuery.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>sql_query</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>None or character string specifying a valid SQL select query.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Cannot be used with table.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>dbms_name</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>None or character string specifying the Database Management System (DBMS) name.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>database_name</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>None or character string specifying the name of the database.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>use_fast_read</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Bool specifying whether or not to use a direct ODBC connection.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>trim_space</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Bool specifying whether or not to trim the white character of string data for reading.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>row_buffering</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Bool specifying whether or not to buffer rows on read from the database.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If you are having problems with your ODBC driver, try setting this to False.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>return_data_frame</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Bool indicating whether or not to convert the result from a list to a data frame (for use in rxReadNext only).</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If False, a list is returned.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>string_as_factors</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Bool indicating whether or not to automatically convert strings to factors on import.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>This can be overridden by specifying “character” in column_classes and column_info.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If True, the factor levels will be coded in the order encountered.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent, the preferred method for handling factor columns is to use column_info with specified “levels”.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>column_classes</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Dictionary of column name to strings specifying the column types to use when converting the data.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The element names for the vector are used to identify which column should be converted to which type.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Allowable column types are:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Note for “factor” type, the levels will be coded in the order encountered.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent, the preferred method for handling factor columns is to use column_info with specified “levels”.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Note that equivalent types share the same bullet in the list above; for some types we allow both ‘R-friendly’ type names, as well as our own, more specific type names for ‘.xdf’ data.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Note also that specifying the column as a “factor” type is currently equivalent to “string” - for the moment, if you wish to import a column as factor data you must use the column_info argument, documented below.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>column_info</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>List of named variable information lists.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Each variable information list contains one or more of the named elements given below.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The information supplied for column_info overrides that supplied for column_classes.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Currently available properties for a column information list are:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>rows_per_read</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Number of rows to read at a time.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If 0, no additional output is printed.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If 1, information on the odbc data source type (odbc or odbcFast) is printed.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>write_factors_as_indexes</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Bool value, If True, when writing to an RxOdbcData data source, underlying factor indexes will be written instead of the string representations.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>kwargs</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed directly to the underlying functions.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Object of class RxOdbcData.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>