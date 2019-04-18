<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="RxXdfData.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18cc4452950d3c33595a0f02ffeb709065e127cd01e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">c4452950d3c33595a0f02ffeb709065e127cd01e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\RxXdfData.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxXdfData: Class generator for XDF data source objects (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Main generator for class RxXdfData, which extends RxDataSource.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>datasource, xdf</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RxXdfData</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Main generator for class RxXdfData, which extends RxDataSource.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>file</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Character string specifying the location of the data.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>For single Xdf, it is a ‘.xdf’ file.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>For composite Xdf, it is a directory like ‘/tmp/airline’.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>When using distributed compute contexts like RxSpark, a directory should be used since those compute contexts always use composite Xdf.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>vars_to_keep</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>List of strings of variable names to keep around during operations.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If None, argument is ignored.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Cannot be used with vars_to_drop.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>vars_to_drop</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>list of strings of variable names to drop from operations.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If None, argument is ignored.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Cannot be used with vars_to_keep.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>return_data_frame</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Bool value indicating whether or not to convert the result to a data frame.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>strings_as_factors</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Bool value indicating whether or not to convert strings into factors (for reader mode only).</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>file_system</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Character string or RxFileSystem object indicating type of file system; “native” or RxNativeFileSystem object can be used for the local operating system.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If None, the file system will be set to that in the current compute context, if available, otherwise the fileSystem option.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>create_composite_set</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Bool value or None.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Used only when writing.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If True, a composite set of files will be created instead of a single ‘.xdf’ file.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Subdirectories ‘data’ and ‘metadata’ will be created.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>In the ‘data’ subdirectory, the data will be split across a set of ‘.xdfd’ files (see blocks_per_composite_file below for determining how many blocks of data will be in each file).</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>In the ‘metadata’ subdirectory there is a single ‘.xdfm’ file, which contains the meta data for all of the ‘.xdfd’ files in the ‘data’ subdirectory.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>When the compute context is RxSpark, a composite set of files is always created.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>create_partition_set</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Bool value or None.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Used only when writing.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If True, a set of files for partitioned Xdf will be created when assigning this RxXdfData object for outData of rxPartition.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Subdirectories ‘data’ and ‘metadata’ will be created.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>In the ‘data’ subdirectory, the data will be split across a set of ‘.xdf’ files (each file stores data of a single data partition, see rxPartition for details).</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>In the ‘metadata’ subdirectory there is a single ‘.xdfp’ file, which contains the meta data for all of the ‘.xdf’ files in the ‘data’ subdirectory.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The partitioned Xdf object is currently supported only in rxPartition and rxGetPartitions</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>blocks_per_composite_file</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Integer value.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If create_composite_set=True, this will be the number of blocks put into each ‘.xdfd’ file in the composite set.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>RxSpark compute context will optimize the number of blocks based upon HDFS and Spark settings.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Object of class <ph id="ph1">`RxXdfData`</ph>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>