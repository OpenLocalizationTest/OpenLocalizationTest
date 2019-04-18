<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-create-col-info.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c21a84bf9c68d775da6511a39cf200ad85bac9184.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">21a84bf9c68d775da6511a39cf200ad85bac9184</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-create-col-info.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_create_col_info: Generate a column_info ordered dictionary from a data source (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>From the data source, generates an ordered dictionary of dictionaries with variable names as keys and column information dictionaries as values.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>It can be used in rx_import or an RxDataSource constructor.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This function can be used to ensure consistent categorical (factor) levels when importing a series of text files to xdf.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>It is also useful for repeated analysis on non-xdf data sources.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>column, information, col, info</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>From the data source, generates an ordered dictionary of dictionaries with variable names as keys and column information dictionaries as values.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>It can be used in rx_import or an RxDataSource constructor.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>This function can be used to ensure consistent categorical (factor) levels when importing a series of text files to xdf.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>It is also useful for repeated analysis on non-xdf data sources.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>:param data : An RxDataSource object, a character string containing an ‘.xdf’ file name, or a data frame.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>An object returned from rx_get_var_info is also supported.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>:param include_low_high : Bool value.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If True, the low/high values will be included in the column_info object.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Note that this will override any actual low/high values in the data set if the column_info object is applied to a different data source.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>:param factors_only : Bool value.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If True, only column information for categorical (factor) variables will be included in the output.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>:param vars_to_keep : None to include all variables, or list of strings of variable names to include :param sort_levels : Bool value.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If True, categorical (factor) levels will be sorted.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>:param compute_info : Bool value.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If True, a pass through the data will be taken for non-xdf data sources to compute categorical (factor) levels and low/high values.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>:param use_factor_index : Bool value.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If True, the factor_index variable type will be used instead of factor</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>:return : Ordered dict column_info of named variable information dicts.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>It can be used as input for rx_import and in data sources such as RxTextData and RxSqlServerData Each variable information dict contains one or more of the named elements given below..</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`RxDataSource`</ph>, <ph id="ph2">`RxTextData`</ph>, <ph id="ph3">`RxSqlServerData`</ph>, <ph id="ph4">`RxOdbcData`</ph>, <ph id="ph5">`RxXdfData`</ph>, <ph id="ph6">`rx_import`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>