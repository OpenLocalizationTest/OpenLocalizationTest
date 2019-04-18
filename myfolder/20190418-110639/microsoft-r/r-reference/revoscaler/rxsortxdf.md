<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxsortxdf.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f768198ac1abc03a661e71b1a551c1175fd903bbc.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">768198ac1abc03a661e71b1a551c1175fd903bbc</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxsortxdf.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxSort function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Efficient multi-key sorting of the variables in an .xdf file or data frame in a local compute context.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxSort, file</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxSort:  Variable sorting of an .xdf file or data frame.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Efficient multi-key sorting of the variables in an .xdf file or data frame in a local compute context.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>a data frame, a character string denoting the path to an existing .xdf file, or an RxXdfData object.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>either an RxXdfData object or a character string denoting the path to an existing .xdf file.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>an .xdf path to store the sorted output.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, a data frame with the sorted output  will be returned from <ph id="ph2">`rxSort`</ph>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>character vector containing the names of the variables to use for sorting.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If multiple variables are used, the first <ph id="ph1">`sortByVars`</ph> variable is sorted and common values are grouped.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The second variable is then sorted within the first variable groups.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The third variable is then sorted within groupings formed by the first two variables, and so on.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>a logical scalar or vector defining the whether or not the <ph id="ph1">`sortByVars`</ph> variables are  to be sorted in decreasing or increasing order.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If a vector, the length <ph id="ph1">`decreasing`</ph> must be that of <ph id="ph2">`sortByVars`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If a logical scalar, the value of <ph id="ph1">`decreasing`</ph> is replicated to the length <ph id="ph2">`sortByVars`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>a character string defining the sorting method to use.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`"auto"`</ph> automatically determines the sort method based on the amount of memory required for sorting.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If possible, all of the data will be sorted in memory.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`"mergeSort"`</ph> uses a merge sort method, where chunks of data are pre-sorted, then merged together.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`"varByVar"`</ph> uses a variable-by-variable sort method,  which assumes that the <ph id="ph2">`sortByVars`</ph> variables and the calculated sorted index variable can be held in memory simultaneously.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`type="varByVar"`</ph>, the variables in the sorted data are re-ordered so that the variables named in <ph id="ph2">`sortByVars`</ph> come first, followed by any remaining variables.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>a logical scalar for controlling the treatment of missing values.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, missing values  in the data are treated as the lowest value; if <ph id="ph2">`FALSE`</ph>, they are treated as the highest value.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>a logical scalar.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, case sensitive sorting is performed for character data.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, only the first observation will be   kept when duplicate values of the key (<ph id="ph2">`sortByVars`</ph>) are encountered.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The sort  <ph id="ph1">`type`</ph> must be set to <ph id="ph2">`"auto"`</ph> or <ph id="ph3">`"mergeSort"`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>character vector defining variables to keep when writing the output to file.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, this argument is ignored.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>This argument takes precedence over <ph id="ph1">`varsToDrop`</ph> if both are specified, i.e., both are not <ph id="ph2">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If both <ph id="ph1">`varsToKeep`</ph> and <ph id="ph2">`varsToDrop`</ph> are <ph id="ph3">`NULL`</ph> then all variables are  written to the data source.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>character vector of variable names to exclude when writing the output data file.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, this argument is ignored.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If both <ph id="ph1">`varsToKeep`</ph> and <ph id="ph2">`varsToDrop`</ph> are <ph id="ph3">`NULL`</ph> then all variables are  written to the data source.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>character string denoting name of new variable for frequency counts if <ph id="ph1">`removeDupKeys`</ph> is set to <ph id="ph2">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Ignored if <ph id="ph1">`removeDupKeys`</ph> is set to <ph id="ph2">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, a new variable for frequency counts will not be created.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outFile`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>the maximum size of a data frame that will be returned if <ph id="ph1">`outFile`</ph> is set to <ph id="ph2">`NULL`</ph> and <ph id="ph3">`inData`</ph> is an .xdf file , measured by the number of rows times the number of columns.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If the number of rows times the number of columns being created from the .xdf file exceeds this, a warning will be reported and the number of rows in the returned data frame will be truncated.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`maxRowsByCols`</ph> is set to be too large, you may experience problems  from loading a huge data frame into memory.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>integer specifying the maximum size of the memory buffer (in Mb)  to use in sorting when <ph id="ph1">`type`</ph> is set to <ph id="ph2">`"auto"`</ph>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The default value of <ph id="ph1">`bufferLimit = -1`</ph> will attempt to  determine an appropriate buffer limit based on system memory.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, additional summary information is printed.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>integer in the range of -1 to 9.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the  amount of compression for the output file - resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>If  <ph id="ph1">`xdfCompressionLevel`</ph> is set to 0, there will be no compression and the output file will be compatible  with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression  will be used.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>deprecated argument.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>It will be ignored.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Revolution Compute Engine.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Using <ph id="ph1">`sortbyVars`</ph>, multiple keys can be specified to perform an iterative, within-category sorting of the variables in the <ph id="ph2">`inData`</ph> or <ph id="ph3">`inFile`</ph> .xdf file.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The argument <ph id="ph1">`varsToKeep`</ph> (or alternatively <ph id="ph2">`varsToDrop`</ph>) is used to define the set of sorted variables to store in the specified <ph id="ph3">`outFile`</ph> file or the returned data frame if <ph id="ph4">`outData`</ph> is <ph id="ph5">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`sortbyVars`</ph> variables are automatically prepended to the set of output variables defined by <ph id="ph2">`varsToKeep`</ph> or <ph id="ph3">`varsToDrop`</ph>.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>If an <ph id="ph1">`outFile`</ph> is not specified, a data frame with the sorted data is returned.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>If an <ph id="ph1">`outFile`</ph> is specified, an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> data source is returned that can be used in subsequent RevoScaleR analysis.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>If sorting is unsuccessful, <ph id="ph1">`FALSE`</ph> is returned.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>sort</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>