<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-get-info.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc775086da62177a96f52a9c86b8987fe068b4ede995a0.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">86da62177a96f52a9c86b8987fe068b4ede995a0</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-get-info.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_get_info: Get data source information (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Get basic information about a revoscalepy data source or data frame.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>xdf</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rx_get_info</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Get basic information about a revoscalepy data source or data frame.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>A data frame, a character string specifying an “.xdf”, or an RxDataSource object.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If a local compute context is being used, this argument may also be a list of data sources, in which case the output will be returned in a named list.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>See the details section for more information.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If a Spark compute context is being used, this argument may also be an RxHiveData, RxOrcData, RxParquetData or RxSparkDataFrame object or a Spark data frame object from pyspark.sql.DataFrame.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>get_var_info</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If True, variable information is returned.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>get_block_sizes</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If True, block sizes are returned in the output for an “.xdf” file, and when printed the first 10 block sizes are shown.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>get_value_labels</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If True and get_var_info is True or None, factor value labels are included in the output.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>vars_to_keep</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>List of strings of variable names for which information is returned.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If None or get_var_info is False, argument is ignored.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Cannot be used with vars_to_drop.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>vars_to_drop</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>List of strings of variable names for which information is not returned.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If None or get_var_info is False, argument is ignored.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Cannot be used with vars_to_keep.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>start_row</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Starting row for retrieval of data of a data frame or “.xdf” file.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>num_rows</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Number of rows of data to retrieve of a data frame or “.xdf” file.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>compute_info</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If True, and get_var_info is True, variable information (e.g., high/low values) for non-xdf data sources will be computed by reading through the data set.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>If True, and get_var_info is False, the number of variables will be gotten from non-xdf data sources (but not the number of rows).</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>all_nodes</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Ignored if the active RxComputeContext compute context is local or RxForeachDoPar.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Otherwise, if True, a list containing the information for the data set on each node in the active compute context will be returned.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>If False, only information on the data set on the master node will be returned.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Note that the determination of the master node is not controlled by the end user.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Integer value.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If 0, no additional output is printed.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If 1, additional summary information is printed for an “.xdf” file.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>List containing the following possible elements:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>fileName: Character string containing the file name and path (if an ”.xdf” file).</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>objName: Character string containing object name (if not an “.xdf” file).</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>class: Class of the object.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>length: Length of the object if it is not an “.xdf” file or data frame.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>numCompositeFiles: Number of composite data files(if a composite “.xdf”</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>numRows: Number of rows in the data set.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>numVars: Number of variables in the data set.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>numBlocks: Number of blocks in the data set.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>varInfo: List of variable information where each element is a list</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>rowsPerBlock: Integer vector containing number of rows in each block (if get_block_sizes is set to True).</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Set to None if data is a data frame.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>data: Data frame containing the data (if num_rows &gt; 0)</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`rx_data_step`</ph><ept id="p1">](rx-data-step.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`rx_get_var_info`</ph><ept id="p2">](rx-get-var-info.md)</ept>.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit></group></body></file></xliff>