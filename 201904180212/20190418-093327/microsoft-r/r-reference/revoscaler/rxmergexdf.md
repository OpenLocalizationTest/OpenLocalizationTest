<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxmergexdf.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b487d7b4bdcd4393ee5f48659048fbb38f3cb2435b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">87d7b4bdcd4393ee5f48659048fbb38f3cb2435b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxmergexdf.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxMerge function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Merge (join) two data sources on one or more match variables.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>The rxMerge function is multi-threaded.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>In local compute context, the data sources may be sorted .xdf files or data frames.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>In <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context, the data sources may be <bpt id="p2">[</bpt>RxParquetData<ept id="p2">](RxSparkData.md)</ept>, <bpt id="p3">[</bpt>RxHiveData<ept id="p3">](RxSparkData.md)</ept>, <bpt id="p4">[</bpt>RxOrcData<ept id="p4">](RxSparkData.md)</ept>, <bpt id="p5">[</bpt>RxXdfData<ept id="p5">](RxXdfData.md)</ept> or <bpt id="p6">[</bpt>RxTextData<ept id="p6">](RxTextData.md)</ept>.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxMerge, rxMergeXdf, file</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>rxMerge:  Merge two data sources</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Merge (join) two data sources on one or more match variables.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The rxMerge function is multi-threaded.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>In local compute context, the data sources may be sorted .xdf files or data frames.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context, the data sources may be <bpt id="p2">[</bpt>RxParquetData<ept id="p2">](RxSparkData.md)</ept>, <bpt id="p3">[</bpt>RxHiveData<ept id="p3">](RxSparkData.md)</ept>, <bpt id="p4">[</bpt>RxOrcData<ept id="p4">](RxSparkData.md)</ept>, <bpt id="p5">[</bpt>RxXdfData<ept id="p5">](RxXdfData.md)</ept> or <bpt id="p6">[</bpt>RxTextData<ept id="p6">](RxTextData.md)</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>the first data set to merge.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>In local compute context, a data frame, a character string denoting the path to an  existing .xdf file, or an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If a list of <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> objects is provided, they will be merged sequentially.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context, an <bpt id="p2">[</bpt>RxParquetData<ept id="p2">](RxSparkData.md)</ept>, <bpt id="p3">[</bpt>RxHiveData<ept id="p3">](RxSparkData.md)</ept>, <bpt id="p4">[</bpt>RxOrcData<ept id="p4">](RxSparkData.md)</ept>, <bpt id="p5">[</bpt>RxXdfData<ept id="p5">](RxXdfData.md)</ept> or <bpt id="p6">[</bpt>RxTextData<ept id="p6">](RxTextData.md)</ept> data source.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If a list of data source objects is provided, they will be merged sequentially.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>the first data set to merge; either a character string denoting the path to an  existing .xdf file or an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>the second data set to merge.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>In local compute context, a data frame, a character string denoting the path  to an existing .xdf file, or an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Can be <ph id="ph1">`NULL`</ph> if a list of <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> objects is provided for <ph id="ph2">`inData1`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context, an <bpt id="p2">[</bpt>RxParquetData<ept id="p2">](RxSparkData.md)</ept>, <bpt id="p3">[</bpt>RxHiveData<ept id="p3">](RxSparkData.md)</ept>, <bpt id="p4">[</bpt>RxOrcData<ept id="p4">](RxSparkData.md)</ept>, <bpt id="p5">[</bpt>RxXdfData<ept id="p5">](RxXdfData.md)</ept> or <bpt id="p6">[</bpt>RxTextData<ept id="p6">](RxTextData.md)</ept> data source.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Can be <ph id="ph1">`NULL`</ph> if a list of data source objects is provided for <ph id="ph2">`inData1`</ph>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>the second data set to merge; either a character string denoting the path  to an existing .xdf file or an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>in local compute context, an .xdf path to store the merged output.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`outFile`</ph> already exists, <ph id="ph2">`overwrite`</ph> must be set to <ph id="ph3">`TRUE`</ph> to overwrite the file.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, a data frame containing the merged data will be returned.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context, an <bpt id="p2">[</bpt>RxParquetData<ept id="p2">](RxSparkData.md)</ept>, <bpt id="p3">[</bpt>RxHiveData<ept id="p3">](RxSparkData.md)</ept>, <bpt id="p4">[</bpt>RxOrcData<ept id="p4">](RxSparkData.md)</ept> or <bpt id="p5">[</bpt>RxXdfData<ept id="p5">](RxXdfData.md)</ept> data source.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>character vector containing the names of the variables to match for merging.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>In local compute context, the data sets MUST BE presorted in the same order by these variables, unless <ph id="ph1">`autoSort`</ph> is set to <ph id="ph2">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxSort<ept id="p1">](rxSortXdf.md)</ept>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Not required for <ph id="ph1">`type`</ph> equal to <ph id="ph2">`"union"`</ph> or <ph id="ph3">`"oneToOne"`</ph>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>a character string defining the merge method to use:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"inner"`</ph> compares each row of <ph id="ph2">`inData1`</ph> with each row of <ph id="ph3">`inData2`</ph> to  find all pairs of rows in which the values of the <ph id="ph4">`matchVars`</ph> are the same.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"oneToOne"`</ph> appends columns from <ph id="ph2">`inData1`</ph> to <ph id="ph3">`inData2`</ph>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Not supported in <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"left"`</ph> includes all rows that match (as in <ph id="ph2">`"inner"`</ph>) plus rows from <ph id="ph3">`inData1`</ph> that no not have matches.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NA`</ph>'s will be used for the values for variables from <ph id="ph2">`inData2`</ph> that are not matched.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"right"`</ph> includes all rows that match (as in <ph id="ph2">`"inner"`</ph>) plus rows from <ph id="ph3">`inData2`</ph> that no not have matches.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NA`</ph>'s will be used for the values for variables from <ph id="ph2">`inData1`</ph> that are not matched.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"full"`</ph> is a combination of both <ph id="ph2">`"left"`</ph> and <ph id="ph3">`"right"`</ph> merge.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"union"`</ph> append rows from <ph id="ph2">`inData2`</ph> to <ph id="ph3">`inData1`</ph>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Not supported in <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The two input files must have the same number of columns with the same data types.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>a logical scalar for controlling the treatment of missing values.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, missing values  in the data are treated as the lowest value; if <ph id="ph2">`FALSE`</ph>, they are treated as the highest value.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Not supported in <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>a logical scalar for controlling whether or not to sort the input data sets by the <ph id="ph1">`matchVars`</ph> before merging.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the data sets are sorted before merging; if <ph id="ph2">`FALSE`</ph>,  it is assumed that the data sets are already sorted by the <ph id="ph3">`matchVars`</ph>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Not supported in <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>a character vector of length two containing the extensions to be used for handling duplicate variable names in the two input data sets.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>These extensions are not applied to matching variables.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, file or data frame names will be used as the extension.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>If the names are the same,  the extensions <ph id="ph1">`1`</ph> and <ph id="ph2">`2`</ph> will be used (unless there are other variables with those names.)  For example, if <ph id="ph3">`duplicateVarExt = c("One", "Two")`</ph> and <ph id="ph4">`inData1`</ph> and <ph id="ph5">`inData2`</ph> both have the variable <ph id="ph6">`y`</ph>, the output data set will contain the variables <ph id="ph7">`y.One`</ph> and <ph id="ph8">`y.Two`</ph>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>character vector of variable names to include from the <ph id="ph1">`inData1`</ph>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToDrop1`</ph>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>character vector of variable names to exclude  from <ph id="ph1">`inData1`</ph>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToKeep1`</ph>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>a named character vector of new names for variables from <ph id="ph1">`inData1`</ph> when writing them to <ph id="ph2">`outData`</ph>.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>For example, specifying <ph id="ph1">`c(x = "newx", y = "newy"`</ph> would give the input variables <ph id="ph2">`x`</ph> and <ph id="ph3">`y`</ph> the names <ph id="ph4">`newx`</ph> and <ph id="ph5">`newy`</ph> in the output data.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>character vector of variable names to include from the <ph id="ph1">`inData2`</ph>.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToDrop2`</ph>.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>character vector of variable names to exclude  from <ph id="ph1">`inData2`</ph>.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToKeep2`</ph>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>a named character vector of new names for variables from <ph id="ph1">`inData2`</ph> when writing them to <ph id="ph2">`outData`</ph>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>For example, specifying <ph id="ph1">`c(x = "newx", y = "newy"`</ph> would give the input variables <ph id="ph2">`x`</ph> and <ph id="ph3">`y`</ph> the names <ph id="ph4">`newx`</ph> and <ph id="ph5">`newy`</ph> in the output data.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>an integer specifying how many rows should be written out to each block in the output .xdf file.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>If set to -1, the smaller of the two average block sizes of the input data sets will be used.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Ignored if <ph id="ph1">`outData`</ph> is <ph id="ph2">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Not supported in <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>a logical scalar specifying whether or not the <ph id="ph1">`matchVars`</ph> variables were  sorted in decreasing or increasing order.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The input data must be sorted in the  same order.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outFile`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Ignored if <ph id="ph1">`outData`</ph> is <ph id="ph2">`NULL`</ph></source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>the maximum size of a data frame that will be returned if <ph id="ph1">`outFile`</ph> is set to <ph id="ph2">`NULL`</ph> and <ph id="ph3">`inData`</ph> is an .xdf file , measured by the number of rows times the number of columns.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>If the number of rows times the number of columns being created from the .xdf file exceeds this, a warning will be reported and the number of rows in the returned data frame will be truncated.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`maxRowsByCols`</ph> is set to be too large, you may experience problems  from loading a huge data frame into memory.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Not supported in <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>integer specifiying the maximum size of the memory buffer (in Mb)  to use in merging.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>The default value of <ph id="ph1">`bufferLimit = -1`</ph> will attempt to  determine an appropriate buffer limit based on system memory.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Not supported in <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Not supported in <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, additional summary information is printed.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>integer in the range of -1 to 9.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the  amount of compression for the output file - resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>If  <ph id="ph1">`xdfCompressionLevel`</ph> is set to 0, there will be no compression and the output file will be compatible  with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression  will be used.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Microsoft R Server Compute Engine.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>The arguments <ph id="ph1">`varsToKeep1`</ph> (or alternatively <ph id="ph2">`varsToDrop1`</ph>) and <ph id="ph3">`varsToKeep2`</ph> (or alternatively <ph id="ph4">`varsToDrop2`</ph>) are used to define the set of variables from the input files that will be stored in the specified merged <ph id="ph5">`outFile`</ph> file.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`matchVars`</ph> must be included in the variables read from the input files.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>A single copy of the <ph id="ph1">`matchVars`</ph> variables will be saved in the <ph id="ph2">`outFile`</ph> file.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxMerge`</ph>: If an <ph id="ph2">`outFile`</ph> is not specified, a data frame with the merged data is returned.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>If an <ph id="ph1">`outFile`</ph> is specified, a data source object is returned that can be used in subsequent RevoScaleR analysis.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxMergeXdf`</ph>: If merging is successful, <ph id="ph2">`TRUE`</ph> is returned; otherwise <ph id="ph3">`FALSE`</ph> is returned.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>sort</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>