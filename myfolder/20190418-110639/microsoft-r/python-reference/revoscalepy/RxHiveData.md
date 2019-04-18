<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="RxHiveData.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f614e454a484c8de90d93e009d4e7ded82fa9900a.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">614e454a484c8de90d93e009d4e7ded82fa9900a</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\RxHiveData.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxHiveData: Class generator for Hive data source objects (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Main generator for class RxHiveData, which extends RxSparkData.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>datasource, hive</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RxHiveData</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Main generator for class RxHiveData, which extends RxSparkData.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>query</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Character string specifying a Hive query, e.g. “select * from &gt;&gt;sample_&lt;&lt; table”.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Cannot be used with ‘table’.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>table</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Character string specifying the name of a Hive table, e.g. “sample_table”.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Cannot be used with ‘query’.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>column_info</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>List of named variable information lists.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Each variable information list contains one or more of the named elements given below.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Currently available properties for a column information list are: type: Character string specifying the data type for the column.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>levels: List of strings containing the levels when type = “factor”.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If the levels property is not provided, factor levels will be determined by the values in the source column.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If levels are provided, any value that does not match a provided level will be converted to a missing value.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>save_as_temp_table</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Bool value, only applicable when using as output with “table” parameter.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If “TRUE” register a temporary Hive table in Spark memory system otherwise generate a persistent Hive table.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The temporary Hive table is always cached in Spark memory system.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>write_factors_as_indexes</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Bool value, If True, when writing to an RxHiveData data source, underlying factor indexes will be written instead of the string representations.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>object of class <ph id="ph1">`RxHiveData`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>