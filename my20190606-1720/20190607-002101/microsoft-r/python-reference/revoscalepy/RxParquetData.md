<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="RxParquetData.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37273f2d1550655d56f434f10f75431f5de6371c4b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">273f2d1550655d56f434f10f75431f5de6371c4b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\RxParquetData.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxParquetData: Class generator for Parquet data source objects (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Main generator for class RxParquetData, which extends RxSparkData.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>datasource, parquet</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RxParquetData</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Main generator for class RxParquetData, which extends RxSparkData.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>file</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Character string specifying the location of the data.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>e.g. “/tmp/AirlineDemoSmall.parquet”.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>column_info</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>List of named variable information lists.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Each variable information list contains one or more of the named elements given below.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Currently available properties for a column information list are: type: Character string specifying the data type for the column.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>levels: List of strings containing the levels when type = “factor”.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If the levels property is not provided, factor levels will be determined by the values in the source column.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If levels are provided, any value that does not match a provided level will be converted to a missing value.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>file_system</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Character string or RxFileSystem object indicating type of file system; It supports native HDFS and other HDFS compatible systems, e.g., Azure Blob and Azure Data Lake.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Local file system is not supported.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>write_factors_as_indexes</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Bool, if True, when writing to an RxParquetData data source, underlying factor indexes will be written instead of the string representations.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Object of class <ph id="ph1">`RxParquetData`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>