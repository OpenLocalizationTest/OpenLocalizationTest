<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="RxTextData.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e3314a6368fcd5a45fb8c6e822c94a3757f0877be.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">3314a6368fcd5a45fb8c6e822c94a3757f0877be</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\RxTextData.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxTextData: Class generator for text data source objects (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Main generator for class RxTextData, which extends RxDataSource.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>datasource, text file</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RxTextData</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Main generator for class RxTextData, which extends RxDataSource.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>file</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Character string specifying a text file.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If it has an ‘.sts’ extension, it is interpreted as a fixed format schema file.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If the column_info argument contains start and width information, it is interpreted as a fixed format data file.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Otherwise, it is treated as a delimited text data file.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>See the Details section for more information on using ‘.sts’ files.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>return_data_frame</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Bool value indicating whether or not to convert the result from a list to a data frame (for use in rxReadNext only).</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If False, a list is returned.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>strings_as_factors</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Bool value indicating whether or not to automatically convert strings to factors on import.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>This can be overridden by specifying “character” in column_classes and column_info.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If True, the factor levels will be coded in the order encountered.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Since this factor level ordering is row dependent, the preferred method for handling factor columns is to use column_info with specified “levels”.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>column_classes</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Dictionary of column names to strings specifying the column types to use when converting the data.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The element names for the vector are used to identify which column should be converted to which type.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>column_info</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>List of named variable information lists.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Each variable information list contains one or more of the named elements given below.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>When importing fixed format data, either column_info or an ‘.sts’ schema file should be supplied.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>For such fixed format data, only the variables specified will be imported.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>For all text types, the information supplied for column_info overrides that supplied for column_classes.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>vars_to_keep</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>List of strings of variable names to include when reading from the input data file.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If None, argument is ignored.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Cannot be used with vars_to_drop.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>vars_to_drop</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>List of strings of variable names to exclude when reading from the input data file.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If None, argument is ignored.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Cannot be used with vars_to_keep.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>missing_value_string</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Character string containing the missing value code.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>It can be an empty string: “”.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>rows_per_read</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Number of rows to read at a time.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>delimiter</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Character string containing the character to use as the separator between variables.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If None and the column_info argument does not contain “start” and “width” information (which implies a fixed-formatted file), the delimiter is auto-sensed from the list “,”, ”       “, “;”, and ” “.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>combine_delimiters</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Bool value indicating whether or not to treat consecutive non-space (” “) delimiters as a single delimiter.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Space ” ” delimiters are always combined.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>quote_mark</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Character string containing the quotation mark.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>It can be an empty string: “”.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>decimal_point</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Character string containing the decimal point.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Not supported when use_fast_read is set to True.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>thousands_separator</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Character string containing the thousands separator.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Not supported when use_fast_read is set to True.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>read_date_format</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Character string containing the time date format to use during read operations.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Not supported when use_fast_read is set to True.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Valid formats are:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>read_posixct_format</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Character string containing the time date format to use during read operations.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Not supported when use_fast_read is set to True.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Valid formats are:</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>components; if present, they are used, but they need not be there.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>century_cutoff</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Integer specifying the changeover year between the twentieth and twenty-first century if two-digit years are read.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Values less than century_cutoff are prefixed by 20 and those greater than or equal to century_cutoff are prefixed by 19.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>If you specify 0, all two digit dates are interpreted as years in the twentieth century.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Not supported when use_fast_read is set to True.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>first_row_is_column_names</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Bool indicating if the first row represents column names for reading text.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>If first_row_is_column_names is None, then column names are auto- detected.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The logic for auto-detection is: if the first row contains all values that are interpreted as character and the second row contains at least one value that is interpreted as numeric, then the first row is considered to be column names; otherwise the first row is considered to be the first data row.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Not relevant for fixed format data.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>As for writing, it specifies to write column names as the first row.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>If first_row_is_column_names is None, the default is to write the column names as the first row.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>rows_to_sniff</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Number of rows to use in determining column type.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>rows_to_skip</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Integer indicating number of leading rows to ignore.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Only supported for use_fast_read = True.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>default_read_buffer_size</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Number of rows to read into a temporary buffer.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>This value could affect the speed of import.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>default_decimal_column_type</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Used to specify a column’s data type when only decimal values (possibly mixed with missing (NA) values) are encountered upon first read of the data and the column’s type information is not specified via column_info or column_classes.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Supported types are “float32” and “numeric”, for 32-bit floating point and 64-bit floating point values, respectively.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>default_missing_column_type</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Used to specify a given column’s data type when only missings (NAs) or blanks are encountered upon first read of the data and the column’s type information is not specified via column_info or column_classes.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Supported types are “float32”, “numeric”, and “character” for 32-bit floating point, 64-bit floating point and string values, respectively.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Only supported for use_fast_read = True.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>write_precision</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Integer specifying the precision to use when writing numeric data to a file.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>strip_zeros</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Bool value if True, if there are only zeros after the decimal point for a numeric, it will be written as an integer to a file.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>quoted_delimiters</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Bool value, if True, delimiters within quoted strings will be ignored.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>This requires a slower parsing process.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Only applicable to use_fast_read is set to True; delimiters within quotes are always supported when use_fast_read is set to False.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>is_fixed_format</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Bool value, if true, the input data file is treated as a fixed format file.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Fixed format files must have a ‘.sts’ file or a column_info argument specifying the start and width of each variable.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>If False, the input data file is treated as a delimited text file.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>If None, the text file type (fixed or delimited text) is auto-determined.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>use_fast_read</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>None or bool value.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>If True, the data file is accessed directly by the Microsoft R Services Compute Engine.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>If False, StatTransfer is used to access the data file.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>If None, the type of text import is auto-determined.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>use_fast_read should be set to False if importing Date or POSIXct data types, if the data set contains the delimiter character inside a quoted string, if the decimalPoint is not “.”, if the thousandsSeparator is not “,”, if the quoteMark is not “”“, or if combineDelimiters is set to True.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>use_fast_read should be set to True if rowsToSkip or defaultMissingColType are set.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>If use_fast_read is True, by default variables containing the values True and False or T and F will be created as bool variables.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>use_fast_read cannot be set to False if an HDFS file system is being used.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>If an incompatible setting of use_fast_read is detected, a warning will be issued and the value will be changed.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>create_file_set</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Bool value or None.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Used only when writing.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>If True, a file folder of text files will be created instead of a single text file.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>A directory will be created whose name is the same as the text file that would otherwise be created, but with no extension.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>In the directory, the data will be split across a set of text files (see rows_per_out_file below for determining how many rows of data will be in each file).</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>If False, a single text file will be created.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>If None, a folder of files will be created if the input data set is a composite XDF file or a folder of text files.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>This argument is ignored if the text file is fixed format.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>rows_per_out_file</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Integer value or None.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>If a directory of text files is being created, this will be the number of rows of data put into each file in the directory.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Integer value.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>If 0, no additional output is printed.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>If 1, information on the text type (text or textFast) is printed.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>check_vars_to_keep</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>bool value.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>If True variable names specified in vars_to_keep will be checked against variables in the data set to make sure they exist.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>An error will be reported if not found.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>If there are more than 500 variables in the data set, this flag is ignored and no checking is performed.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>file_system</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Character string or RxFileSystem object indicating type of file system; “native” or RxNativeFileSystem object can be used for the local operating system.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>input_encoding</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Character string indicating the encoding used by input text.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>May be set to either “utf-8” (the default), or “gb18030”, a standard Chinese encoding.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Not supported when use_fast_read is set to True.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>write_factors_as_indexes</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>bool.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>If True, when writing to an RxTextData data source, underlying factor indexes will be written instead of the string representations.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Not supported when use_fast_read is set to False.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Object of class <ph id="ph1">`RxTextData`</ph>.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>