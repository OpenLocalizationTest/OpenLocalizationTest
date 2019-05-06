<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-data-step.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750db18eeed9f7acd082a4f2e7538d97c4f428016a2.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">db18eeed9f7acd082a4f2e7538d97c4f428016a2</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-data-step.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_data_step: Transform data from input to output dataset (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Inline data transformations of an existing data set to an output data set</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>datasource</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rx_data_step</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Inline data transformations of an existing data set to an output data set</source>
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
          <source>A character string representing the output ‘.xdf’ file, or a RxXdfData object.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If None, a data frame will be returned in memory.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If a Spark compute context is being used, this argument may also be an RxHiveData, RxOrcData, RxParquetData or RxSparkDataFrame object.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>vars_to_keep</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>list of strings of variable names to include when reading from the input data file.</source>
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
          <source>See the example.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>transform_function</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Name of the function that will be used to modify the data.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The variables used in the transformation function must be specified in transform_variables.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>See the example.</source>
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
          <source>If True, the existing outData will be overwritten.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Ignored if a dataframe is returned.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>row_variable_name</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Character string or None.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If inData is a data.frame: If None, the data frame’s row names will be dropped.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>If a character string, an additional variable of that name will be added to the data set containing the data frame’s row names.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>If a data.frame is being returned, a variable with the name row_variable_name will be removed as a column from the data frame and will be used as the row names.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>remove_missings_on_read</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>If True, rows with missing values will be removed on read.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>remove_missings</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>If True, rows with missing values will not be included in the output data.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>compute_low_high</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>If False, low and high values will not automatically be computed.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>This should only be set to False in special circumstances, such as when append is being used repeatedly.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>max_rows_by_cols</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The maximum size of a data frame that will be returned if output_file is set to None and inData is an ‘.xdf’ file, measured by the number of rows times the number of columns.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>If the number of rows times the number of columns being created from the ‘.xdf’ file exceeds this, a warning will be reported and the number of rows in the returned data frame will be truncated.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>If max_rows_by_cols is set to be too large, you may experience problems from loading a huge data frame into memory.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>rows_per_read</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Number of rows to read for each chunk of data read from the input data source.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Use this argument for finer control of the number of rows per block in the output data source.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>If greater than 0, blocks_per_read is ignored.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Cannot be used if input_data is the same as output_file.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The default value of -1 specifies that data should be read by blocks according to the blocks_per_read argument.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>start_row</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The starting row to read from the input data source.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Cannot be used if input_data is the same as output_file.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>number_rows_read</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Number of rows to read from the input data source.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>If remove_missings are used, the output data set may have fewer rows than specified by number_rows_read.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Cannot be used if input_data is the same as output_file.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>return_transform_objects</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>If True, the list of transformObjects will be returned instead of a data frame or data source object.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>If the input transformObjects have been modified, by using .rxSet or .rxModify in the transformFunc, the updated values will be returned.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Any data returned from the transformFunc is ignored.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>If no transformObjects are used, None is returned.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>This argument allows for user-defined computations within a transform_function without creating new data.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Ignored for data frames or if rows_per_read is positive.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Integer value with options: 0: no progress is reported.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>1: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>2: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>3: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>xdf_compression_level</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Integer in the range of -1 to 9.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the amount of compression - resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>If xdf_compression_level is set to 0, there will be no compression and files will be compatible with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression will be used.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>strings_as_factors</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Bool indicating whether or not to automatically convert strings to factors on import.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>This can be overridden by specifying “character” in column_classes and column_info.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>If True, the factor levels will be coded in the order encountered.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent, the preferred method for handling factor columns is to use column_info with specified “levels”.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>kwargs</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed to the input data source.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>If an output_file is not specified, an output data frame is returned.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>If an output_file is specified, an RxXdfData data source is returned that can be used in subsequent revoscalepy analysis.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>