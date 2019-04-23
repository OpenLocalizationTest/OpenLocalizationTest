<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxreadxdf.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86fb9dfb2f66e1a6df8eab379df2a8a5be549e419f.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">fb9dfb2f66e1a6df8eab379df2a8a5be549e419f</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxreadxdf.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxReadXdf function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Read data from an .xdf file into a data frame.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxReadXdf, file, connection</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxReadXdf: Read .xdf File</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Read data from an .xdf file into a data frame.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>either an RxXdfData object or a character string specifying the .xdf file.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>character vector of variable names to include when reading from the input data file.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToDrop`</ph>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>character vector of variable names to exclude when reading from the input data file.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToKeep`</ph>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>optional character string specifying the variable in the data file to use as row names for the output data frame.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>starting row for retrieval.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>number of rows of data to retrieve.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If -1, all are read.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>logical indicating whether or not to create a data frame.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, a list is returned.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>logical indicating whether or not to convert strings into factors in R.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>the maximum size of a data frame that will be read in, measured by the number of rows times the number of columns.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If the numer of rows times the number of columns being extracted from the .xdf file exceeds this, a warning will be reported and a smaller number of rows will be read in than requested.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`maxRowsByCols`</ph> is set to be too large, you may experience problems  from loading a huge data frame into memory.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>To extract a subset of rows  and/or columns from an .xdf file, use <bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxDataStep.md)</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>read data by blocks.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>This argument is deprecated.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>list of information sent to C++ interpreter.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>if <ph id="ph1">`returnDataFrame`</ph> is <ph id="ph2">`TRUE`</ph>, a data frame is returned.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Otherwise a list is returned.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxImport<ept id="p1">](rxImport.md)</ept>, <bpt id="p2">[</bpt>rxDataStep<ept id="p2">](rxDataStep.md)</ept>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>