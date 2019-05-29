<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxexecbypartition.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3fa75d74f870150bd5696a125171896cee4c2c08a.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">fa75d74f870150bd5696a125171896cee4c2c08a</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxexecbypartition.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxExecByPartition function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This feature allows users to run analytics computation in parallel on individual data partitions split from an input data source based on the specified variables.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>In <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> version 9.1.0, we provide the necessary rx functions to be executed for funtionalities of By-group parallelism.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This document will describe different scenarios of By-group parallelism, running in a number of supported compute contexts.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxExecByPartition, partition, exec, group, execby, groupby</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>rxExecByPartition: RevoScaleR By Group Parallelism</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This feature allows users to run analytics computation in parallel on individual data partitions split from an input data source based on the specified variables.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> version 9.1.0, we provide the necessary rx functions to be executed for funtionalities of By-group parallelism.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>This document will describe different scenarios of By-group parallelism, running in a number of supported compute contexts.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>By-group Parallelism provides functionalities that allow users perform the following typical operations:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Create new data partitions: given an input data set and a list of partitioning variables, split the data set into multiple small data sets based on the values of the specified partitioning variables.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Append new data to existing data partitions: given an input data set and a list of partitioning variables, split the data set and append data in partitioned data sets to the existing corresponding data partitions.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>..</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Perform analytics computation on data partitions in parallel multiple times as needed.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Do all the above three operations in one step initially and then repeat computation multiple times.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> version 9.1.0, we introduce three new rx functions for partitioning data set and performing computation in parallel:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxExecBy<ept id="p1">](rxExecBy.md)</ept>() - to partition an input data source and execute user function on each partition in parallel.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If the input data source is already partitioned, the function will skip the partitioning step and directly trigger computation for user function on partitions.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxPartition<ept id="p1">](rxPartition.md)</ept>() - to partition an input data source and store data partitions on disk.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>For this functionality, a new xdf file format, called Partitioned Xdf (PXdf) is introduced for storing data partitions as well as partition metadata information on disk.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Partitioned Xdf file can then be loaded into an in-memory Partitioned Xdf object using <ph id="ph1">`RxXdfData`</ph> to be used for performing computation on data partitions repeatedly by <bpt id="p1">[</bpt>rxExecBy<ept id="p1">](rxExecBy.md)</ept>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxGetPartitions<ept id="p1">](rxGetPartitions.md)</ept>() - to enumerate unique partitioning values in an existing partitioned Xdf and return it as a data frame</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Running analytics computation in parallel on partitioned data set with <bpt id="p1">[</bpt>rxExecBy<ept id="p1">](rxExecBy.md)</ept>()</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Input data set provided as a data source object can be data sources of different types, such as data frame, text data, Xdf files, ODBC data source, SQL Server data source, etc. In version 9.1.0, <bpt id="p1">[</bpt>rxExecBy<ept id="p1">](rxExecBy.md)</ept>() is supported in local compute context, SQL Server compute context and Spark compute context.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Depending on input data sources and compute context, <bpt id="p1">[</bpt>rxExecBy<ept id="p1">](rxExecBy.md)</ept>() will execute in different modes which are summarized in the following table:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Col  1</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Col  2</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Col  3</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Data Source \ Compute Context</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Local</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>SQL Server</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Data frame, text data, xdf, other data sources that are not ODBC</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Generate PXdf for partitions and execute computation on PXdf</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>SQL Server data source or ODBC data source with <bpt id="p1">*</bpt>query<ept id="p1">*</ept> specified</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Generate PXdf for partitions and execute computation on PXdf</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Generate temporary Composite Xdf and PXdf for partitions and execute computation on PXdf</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>SQL Server data source or ODBC data source with <bpt id="p1">*</bpt>table<ept id="p1">*</ept> specified</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Do streaming with SQL rewrite partition queries and execute computation on streaming partitions</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Do streaming with SQL rewrite partition queries and execute computation on streaming</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>As shown in the table, when running analytics on local compute context, PXdf is first temporarily generated and saved on disk; then computation are applied on the generated PXdf.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The example for running this scenario can be found in the <bpt id="p1">[</bpt>rxExecBy<ept id="p1">](rxExecBy.md)</ept>() documentation.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>It's worth to note that the temporary PXdf generated will be removed once the computation is completed.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>If user plans to run the analytics multiple times with the same data set and different user functions, it would be more efficient to go with the following recommended flow:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>1 Create a new partitioned Xdf object with <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept>() by specifying <ph id="ph1">`createPartitionSet = TRUE`</ph>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>1 Construct data partitions for the newly created PXdf object from an input data set and save it to disk with <bpt id="p1">[</bpt>rxPartition<ept id="p1">](rxPartition.md)</ept>().</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>1 Run analysis with user defined function on the data partitions of the PXdf object with <bpt id="p1">[</bpt>rxExecBy<ept id="p1">](rxExecBy.md)</ept>().</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>This step can be repeated multiple times with different user defined functions and different subsets of data partitions using a <ph id="ph1">`filterFunc`</ph> specified as an argument of <bpt id="p1">[</bpt>rxExecBy<ept id="p1">](rxExecBy.md)</ept>().</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept>, <bpt id="p2">[</bpt>rxExecBy<ept id="p2">](rxExecBy.md)</ept>, <bpt id="p3">[</bpt>rxPartition<ept id="p3">](rxPartition.md)</ept>, <bpt id="p4">[</bpt>rxGetPartitions<ept id="p4">](rxGetPartitions.md)</ept>, <bpt id="p5">[</bpt>rxSplit<ept id="p5">](rxSplitXdf.md)</ept>, <bpt id="p6">[</bpt>rxExec<ept id="p6">](rxExec.md)</ept>, <bpt id="p7">[</bpt>rxImport<ept id="p7">](rxImport.md)</ept></source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>