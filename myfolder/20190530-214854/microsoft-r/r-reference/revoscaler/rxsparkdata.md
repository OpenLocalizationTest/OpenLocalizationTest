<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxsparkdata.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3eb85071056f16401253091b6f62921f1ca476460a.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">b85071056f16401253091b6f62921f1ca476460a</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxsparkdata.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxHiveData, RxParquetData, RxOrcData {RevoScaleR} function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>These are constructors for Hive, Parquet and ORC data sources which extend RxDataSource.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>These three data sources can be used only in RxSpark compute context.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), RxHiveData, RxParquetData, RxOrcData {RevoScaleR}, RxHiveData, RxParquetData, RxOrcData</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>RxHiveData, RxParquetData, RxOrcData {RevoScaleR}: Generate Hive, Parquet or ORC Data Source Object</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>These are constructors for Hive, Parquet and ORC data sources which extend <ph id="ph1">`RxDataSource`</ph>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>These three data sources can be used only in <ph id="ph1">`RxSpark`</ph> compute context.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>character string specifying a Hive query, e.g. <ph id="ph1">`"select * from sample_table"`</ph>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Cannot be used with 'table'.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>character string specifying the name of a Hive table, e.g. <ph id="ph1">`"sample_table"`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Cannot be used with 'query'.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>list of named variable information lists.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Each variable information list contains one or more of the named elements given below (see <bpt id="p1">[</bpt>rxCreateColInfo<ept id="p1">](rxCreateColInfo.md)</ept> for more details):</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Currently available properties for a column information list are:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>character string specifying the data type for the column.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Supported types are:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>(stored as <ph id="ph1">`uchar`</ph>)</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>(stored as <ph id="ph1">`int32`</ph>)</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>(alternative to integer for smaller storage space)</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>(stored as <ph id="ph1">`FloatType`</ph>)</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>(stored as <ph id="ph1">`float64`</ph>)</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>(stored as <ph id="ph1">`string`</ph>)</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>(stored as <ph id="ph1">`uint32`</ph>)</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>(stored as <ph id="ph1">`Date`</ph>, i.e. <ph id="ph2">`float64`</ph>)</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>(stored as <ph id="ph1">`POSIXct`</ph>, i.e. <ph id="ph2">`float64`</ph>)</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>character vector containing the levels when <ph id="ph1">`type = "factor"`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`"levels"`</ph> property is not provided, factor levels will be determined by the values in the source column.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>If levels are provided, any value that does not match a provided level will be converted to a missing value.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Only applicable when using as output with <ph id="ph1">`table`</ph> parameter.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> register a temporary Hive table in   Spark memory system otherwise generate a persistent Hive table.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The temporary Hive table is always cached in Spark memory system.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>character string specifying a file path, e.g. <ph id="ph1">`"/tmp/AirlineDemoSmall.parquet"`</ph> or <ph id="ph2">`"/tmp/AirlineDemoSmall.orc"`</ph>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>character string <ph id="ph1">`"hdfs"`</ph> or <ph id="ph2">`RxFileSystem`</ph> object indicating type of file system.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>It supports native HDFS and other HDFS compatible systems, e.g., Azure Blob and Azure Data Lake.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Local file system is not supported.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>[Deprecated] logical.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> data will be cached in the Spark application's memory system after the first use.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, when writing to an output data source, underlying factor indexes will be written instead of the string representations.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>object of RxHiveData, RxParquetData or RxOrcData.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>