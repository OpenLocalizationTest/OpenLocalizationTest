<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxPartition.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4d4ca208bab6114b4b63b74564c28597c262f4583.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d4ca208bab6114b4b63b74564c28597c262f4583</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxPartition.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxPartition function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Partition input data sources by key values and save the results to a partitioned Xdf on disk.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxPartition, Partition</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxPartition: Partition Data by Key Values and Save the results to a Partitioned .Xdf</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Partition input data sources by key values and save the results to a partitioned Xdf on disk.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>either a data source object, a character string specifying a .xdf file, or a data frame object.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>a partitioned data source object created by <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> with <ph id="ph1">`createPartitionSet = TRUE`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>character vector of variable names to specify the values in those variables to be used for partitioning</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>either "none" to create a new files or "rows" to append rows to an existing file.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If outData exists and append is "none", the <ph id="ph1">`overwrite`</ph> argument must be set to <ph id="ph2">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outData`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`overwrite`</ph> is ignored if <ph id="ph2">`append = "rows"`</ph>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Revolution Compute Engine.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>a data frame of partitioning values and data sources, each row in the data frame represents one partition and the data source in the last variable holds the data of a specifict partition.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>In the current version, this function is single threaded.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxExecBy<ept id="p1">](rxExecBy.md)</ept>, <bpt id="p2">[</bpt>RxXdfData<ept id="p2">](RxXdfData.md)</ept></source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>