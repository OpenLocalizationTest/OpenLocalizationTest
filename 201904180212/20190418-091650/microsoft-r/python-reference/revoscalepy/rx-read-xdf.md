<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-read-xdf.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b44d7187c04ad04418d1d6dfb58dee325f30f23adf.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">4d7187c04ad04418d1d6dfb58dee325f30f23adf</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-read-xdf.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_read_xdf: Read an XDF data source object (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Read data from an “.xdf” file into a data frame.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>xdf</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rx_read_xdf</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Read data from an “.xdf” file into a data frame.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>file</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Either an RxXdfData object or a character string specifying the “.xdf” file.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>vars_to_keep</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>List of strings of variable names to include when reading from the input data file.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If None, argument is ignored.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Cannot be used with vars_to_drop.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>vars_to_drop</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>List of strings of variable names to exclude when reading from the input data file.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If None, argument is ignored.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Cannot be used with vars_to_keep.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>row_var_name</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Optional character string specifying the variable in the data file to use as row names for the output data frame.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>start_row</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Starting row for retrieval.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>num_rows</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Number of rows of data to retrieve.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If -1, all are read.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>return_data_frame</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Bool indicating whether or not to create a data frame.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If False, a list is returned.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>strings_as_factors</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Bool indicating whether or not to convert strings into factors.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>max_rows_by_columns</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The maximum size of a data frame that will be read in, measured by the number of rows times the number of columns.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If the number of rows times the number of columns being extracted from the “.xdf” file exceeds this, a warning will be reported and a smaller number of rows will be read in than requested.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If max_rows_by_columns is set to be too large, you may experience problems from loading a huge data frame into memory.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>To extract a subset of rows and/or columns from an “.xdf” file, use rx_data_step.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Integer value with options: 0: No progress is reported.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>1: The number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>2: Rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>3: Rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>read_by_block</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Read data by blocks.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>This argument is deprecated.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>cpp_interp</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>List of information sent to C++ interpreter.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>a data frame.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`rx_import`</ph><ept id="p1">](rx-import.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`rx_data_step`</ph><ept id="p2">](rx-data-step.md)</ept>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit></group></body></file></xliff>