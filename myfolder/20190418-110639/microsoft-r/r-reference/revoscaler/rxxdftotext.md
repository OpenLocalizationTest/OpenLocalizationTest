<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxxdftotext.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f04ca33866f6b57f267f37b81340b4952ee538fa4.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04ca33866f6b57f267f37b81340b4952ee538fa4</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxxdftotext.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxXdfToText function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Write .xdf file content to a delimited text file.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxDataStep recommended.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxXdfToText, file, connection</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>rxXdfToText: Export .xdf File to Delimited Text File</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Write .xdf file content to a delimited text file.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxDataStep`</ph> recommended.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>either an RxXdfData object or a character string specifying the input .xdf file.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>character string specifying the output delimited text file.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>character vector of variable names to include when reading from <ph id="ph1">`inFile`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToDrop`</ph>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>character vector of variable names to exclude when reading from <ph id="ph1">`inFile`</ph>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToKeep`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>name of a logical variable in the data set (in quotes) or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rowSelection = (age &gt; 20) &amp; (age &lt; 65) &amp; (log(income) &gt; 10)`</ph> will use only observations in which the value of the <ph id="ph2">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph3">`log`</ph> of the <ph id="ph4">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations  (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function  call using the expression function.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>an expression of the form <ph id="ph1">`list(name = expression, ...)`</ph> representing the first round of variable transformations.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>)  can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>a named list containing objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>variable transformation function.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>character vector specifying additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and  preloaded for use in variable transformation functions, both those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments and those  defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>user-defined environment to serve as a parent to  all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the existing <ph id="ph2">`outFile`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>character(s) specifying the separator between columns.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>logical value or numeric vector.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, any character or factor columns will be surrounded by double quotes.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>If a numeric vector, its elements are taken as the indices of columns to quote.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>In both cases, row and column names are quoted if they are written.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, nothing is quoted.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>character string to use for missing values in the data.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>character(s) to print at the end of each line (row).</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`eol = "\r\n"`</ph> will produce Windows' line endings on a Unix-alike OS, and <ph id="ph2">`eol = "\r"`</ph> will produce files as expected by Mac OS Excel 2004.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>a logical value indicating whether the column names in the <ph id="ph1">`inFile`</ph> should be written as the first row in the output text file.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>additional arguments passed to the write.table function.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>For most purposes, the more general <bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxDataStep.md)</ept> is preferred for writing to text files.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>An <bpt id="p1">[</bpt>RxTextData<ept id="p1">](RxTextData.md)</ept> object representing the output text file.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxDataStep.md)</ept>, <bpt id="p2">[</bpt>rxImport<ept id="p2">](rxImport.md)</ept>, write.table, <bpt id="p3">[</bpt>rxSplit<ept id="p3">](rxSplitXdf.md)</ept>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>