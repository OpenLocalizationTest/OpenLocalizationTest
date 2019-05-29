<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-partition.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3d550b0df8f6f9baef03ef44892ac76d96398022e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d550b0df8f6f9baef03ef44892ac76d96398022e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-partition.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_partition: Partition by key value and save to a partitioned .xdf (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Partition input data sources by key values and save the results to a partitioned .xdf file on disk.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>partition</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rx_partition</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Partition input data sources by key values and save the results to a partitioned .xdf file on disk.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>input_data</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Either a data source object, a character string specifying a ‘.xdf’ file, or a Pandas data frame object.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>output_data</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>A partitioned data source object created by RxXdfData with create_partition_set = True.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>vars_to_partition</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>List of strings of variable names to be used for partitioning the input data set.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>append</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Either “none” to create a new file or “rows” to append rows to an existing file.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If output_data exists and append is “none”, the overwrite argument must be set to True.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>overwrite</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If True, an existing output_data will be overwritten.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>overwrite is ignored if appending rows.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>kwargs</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Additional arguments.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>A Pandas data frame of partitioning values and data sources, each row in the Pandas data frame represents one partition and the data source in the last variable holds the data of a specific partition.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`rx_exec_by`</ph><ept id="p1">](rx-exec-by.md)</ept>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`RxXdfData`</ph><ept id="p1">](RxXdfData.md)</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>