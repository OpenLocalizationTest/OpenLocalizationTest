<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-import.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c376652a63ab5a301b95642aa003d7bb7d16d75fc27.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">6652a63ab5a301b95642aa003d7bb7d16d75fc27</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-import.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_import: Import Data to .xdf or data frame (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Import data and store as an .xdf file on disk or in-memory as a data.frame object.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>import, datasource</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rx_import</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Import data and store as an .xdf file on disk or in-memory as a data.frame object.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>input_data</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>A character string with the path for the data to import (delimited, fixed format, ODBC, or XDF).</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Alternatively, a data source object representing the input data source can be specified.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If a Spark compute context is being used, this argument may also be an RxHiveData, RxOrcData, RxParquetData or RxSparkDataFrame object or a Spark data frame object from pyspark.sql.DataFrame.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>output_file</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A character string representing the output ‘.xdf’ file or an RxXdfData object.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If None, a data frame will be returned in memory.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If a Spark compute context is being used, this argument may also be an RxHiveData, RxOrcData, RxParquetData or RxSparkDataFrame object.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>vars_to_keep</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>List of strings of variable names to include when reading from the input data file.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If None, argument is ignored.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Cannot be used with vars_to_drop.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Not supported for ODBC or fixed format text files.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>vars_to_drop</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>List of strings of variable names to exclude when reading from the input data file.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If None, argument is ignored.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Cannot be used with vars_to_keep.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Not supported for ODBC or fixed format text files.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>row_selection</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>transforms</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>transform_objects</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>A dictionary of variables besides the data that are used in the transform function.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>See rx_data_step for examples.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>transform_function</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Name of the function that will be used to modify the data.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The variables used in the transformation function must be specified in transform_objects.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>See rx_data_step for examples.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>transform_variables</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>List of strings of the column names needed for the transform function.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>transform_packages</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>append</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Either “none” to create a new ‘.xdf’ file or “rows” to append rows to an existing ‘.xdf’ file.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If output_file exists and append is “none”, the overwrite argument must be set to True.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Ignored if a data frame is returned.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>overwrite</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If True, the existing output_file will be overwritten.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Ignored if a dataframe is returned.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>number_rows</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Integer value specifying the maximum number of rows to import.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If set to -1, all rows will be imported.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>strings_as_factors</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Bool value indicating whether or not to automatically convert strings to factors on import.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>This can be overridden by specifying “character” in column_classes and column_info.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>If True, the factor levels will be coded in the order encountered.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent, the preferred method for handling factor columns is to use column_info with specified “levels”.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>column_classes</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Dictionary of column name to strings specifying the column types to use when converting the data.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>The element names for the vector are used to identify which column should be converted to which type.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>treated the same as factors in RevoScaleR analysis functions.), ”int16” (alternative to integer for smaller storage space), “uint16” (alternative to unsigned integer for smaller storage space), “Date” (stored as Date, i.e. float64.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Not supported for import</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>types “textFast”, “fixedFast”, or “odbcFast”.) ”POSIXct” (stored as POSIXct, i.e. float64.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Not supported for</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>import types “textFast”, “fixedFast”, or “odbcFast”.) Note for “factor” and “ordered” types, the levels will be coded in the</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>order encountered.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent, the preferred method for handling factor columns is to use column_info with specified “levels”.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>some types we allow both ‘R-friendly’ type names, as well as our own, more specific type names for ‘.xdf’ data.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>equivalent to “string” - for the moment, if you wish to import a column as factor data you must use the column_info argument, documented below.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>column_info</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>List of named variable information lists.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Each variable information list contains one or more of the named elements given below.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>When importing fixed format data, either column_info or an ‘.sts’ schema file should be supplied.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>For fixed format text files, only the variables specified will be imported.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>For all text types, the information supplied for column_info overrides that supplied for column_classes.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Currently available properties for a column information list are:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>rows_per_read</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Number of rows to read at a time.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>type</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Character string set specifying file type of input_data.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>This is ignored if input_data is a data source.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Possible values are: “auto”: File type is automatically detected by looking at file</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>”textFast”: Delimited text import using faster, more limited import mode.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>By default variables containing the values True and False or T and F will be created as bool variables.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>”text”: Delimited text import using enhanced, slower import mode.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>This allows for importing Date and POSIXct data types, handling the delimiter character inside a quoted string, and specifying decimal character and thousands separator.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>(See RxTextData.)</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>”fixedFast”: Fixed format text import using faster, more limited import mode.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>You must specify a ‘.sts’ format file or column_info specifications with start and width for each variable.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>”fixed”: Fixed format text import using enhanced, slower import mode.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>This allows for importing Date and POSIXct data types and specifying decimal character and thousands separator.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>You must specify a ‘.sts’ format file or column_info specifications with start and width for each variable.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>”odbcFast”: ODBC import using faster, more limited import mode.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>“odbc”: ODBC import using slower, enhanced import on Windows.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>(See</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>max_rows_by_columns</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>The maximum size of a data frame that will be read in if output_file is set to None, measured by the number of rows times the number of columns.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>If the number of rows times the number of columns being imported exceeds this, a warning will be reported and a smaller number of rows will be read in than requested.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>If max_rows_by_columns is set to be too large, you may experience problems from loading a huge data frame into memory.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Integer value with options: 0: no progress is reported.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>1: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>2: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>3: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Integer value.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>If 0, no additional output is printed.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>If 1, information on the import type is printed if type is set to auto.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>xdf_compression_level</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Integer in the range of -1 to 9.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the amount of compression - resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>If xdfCompressionLevel is set to 0, there will be no compression and files will be compatible with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression will be used.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>create_composite_set</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Bool value or None.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>If True, a composite set of files will be created instead of a single ‘.xdf’ file.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>A directory will be created whose name is the same as the ‘.xdf’ file that would otherwise be created, but with no extension.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Subdirectories ‘data’ and ‘metadata’ will be created.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>In the ‘data’ subdirectory, the data will be split across a set of ‘.xdfd’ files (see blocks_per_composite_file below for determining how many blocks of data will be in each file).</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>In the ‘metadata’ subdirectory there is a single ‘.xdfm’ file, which contains the meta data for all of the ‘.xdfd’ files in the ‘data’ subdirectory.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>blocks_per_composite_file</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Integer value.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>If create_composite_set=True, this will be the number of blocks put into each ‘.xdfd’ file in the composite set.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>If the output_file is an RxXdfData object, set the value for blocks_per_composite_file there instead.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>kwargs</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed directly to the underlying data source objects to be imported.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>If an output_file is not specified, an output data frame is returned.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>If an output_file is specified, an RxXdfData data source is returned that can be used in subsequent revoscalepy analysis.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>