<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="RxSqlServerData.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3feb235904a3a61b08d34828d1f1285c10d31ca5b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">feb235904a3a61b08d34828d1f1285c10d31ca5b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\RxSqlServerData.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxSqlServerData: Class generator for SQL Server data source objects (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Main generator for class RxSqlServerData, which extends RxDataSource.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>datasource, sql</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RxSqlServerData</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Main generator for class RxSqlServerData, which extends RxDataSource.</source>
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
          <source>Cannot be used with sql_query.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>sql_query</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>None or character string specifying a valid SQL select query.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Cannot contain hidden characters such as tabs or newlines.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Cannot be used with table.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If you want to use TABLESAMPLE clause in sqlQuery, set row_buffering argument to False.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>row_buffering</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Bool value specifying whether or not to buffer rows on read from the database.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If you are having problems with your ODBC driver, try setting this to False.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>return_data_frame</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Bool value indicating whether or not to convert the result from a list to a data frame (for use in rxReadNext only).</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If False, a list is returned.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>string_as_factors</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Bool value indicating whether or not to automatically convert strings to factors on import.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>This can be overridden by specifying “character” in column_classes and column_info.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If True, the factor levels will be coded in the order encountered.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent, the preferred method for handling factor columns is to use column_info with specified “levels”.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>column_classes</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Dictionary of column name to strings specifying the column types to use when converting the data.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The element names for the vector are used to  identify which column should be converted to which type.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Allowable column types are: “bool” (stored as uchar), “integer” (stored as int32), “float32” (the default for floating point data for ‘.xdf’ files), “numeric” (stored as float64 as in R), “character” (stored as string), “factor” (stored as uint32), “int16” (alternative to integer for smaller storage space), “uint16” (alternative to unsigned integer for smaller storage space), “Date” (stored as Date, i.e. float64)</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Note for “factor” type, the levels will be coded in the order encountered.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent, the preferred method for handling factor columns is to use column_info with specified “levels”.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Note that equivalent types share the same bullet in the list above; for some types we allow both ‘R-friendly’ type names, as well as our own, more specific type names for ‘.xdf’ data.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Note also that specifying the column as a “factor” type is currently equivalent to “string” - for the moment, if you wish to import a column as factor data you must use the column_info argument, documented below.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>column_info</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>List of named variable information lists.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Each variable information list contains one or more of the named elements given below.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The information supplied for column_info overrides that supplied for column_classes.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Currently available properties for a column information list are: type: Character string specifying the data type for the column.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>See</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>newName: Character string specifying a new name for the variable.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>description: character string specifying a description for the variable.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>levels: List of strings containing the levels when type = “factor”.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>newLevels: New or replacement levels specified for a column of type “factor”.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>It must be used in conjunction with the levels argument.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>After reading in the original data, the labels for each level will be replaced with the newLevels.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>low: The minimum data value in the variable (used in computations using the F() function.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>high: The maximum data value in the variable (used in computations using the F() function.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>rows_per_read</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Number of rows to read at a time.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Integer value.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>If 0, no additional output is printed.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>If 1, information on the odbc data source type (odbc or odbcFast) is printed.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>use_fast_read</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Bool value, specifying whether or not to use a direct ODBC connection.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>On Linux systems, this is the only ODBC connection available.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>server</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Target SQL Server instance.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Can also be specified in the connection string with the Server keyword.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>database_name</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Database on the target SQL Server instance.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Can also be specified in the connection string with the Database keyword.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>user</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>SQL login to connect to the SQL Server instance.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>SQL login can also be specified in the connection string with the uid keyword.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>password</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Password associated with the SQL login.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Can also be specified in the connection string with the pwd keyword.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>write_factors_as_indexes</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Bool value, if True, when writing to an RxOdbcData data source, underlying factor indexes will be written instead of the string representations.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>kwargs</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed directly to the underlying functions.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>object of class <ph id="ph1">`RxSqlServerData`</ph>.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>