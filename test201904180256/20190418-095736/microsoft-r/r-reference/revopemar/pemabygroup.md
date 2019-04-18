<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="pemabygroup.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c90dbd84460907531354ee4be6d3c861b775f1c5d.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">90dbd84460907531354ee4be6d3c861b775f1c5d</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revopemar\pemabygroup.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Generator for an PemaByGroup reference class object</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Generator for an PemaByGroup reference class object to be used with pemaCompute.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This will compute arbitrary statistics by a grouping variable in a data set.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RevoPemaR, PemaByGroup,  models</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>PemaByGroup:  Generator for an PemaByGroup reference class object</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Applies to version 8.0.3 of package RevoPemaR.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Generator for an PemaByGroup reference class object to be used with pemaCompute.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>This will compute arbitrary statistics by a grouping variable in a data set.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>...</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Arguments used in the constructor.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>See Details section.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>This is an example of a parallel external memory algorithm for use with <bpt id="p1">[</bpt>pemaCompute<ept id="p1">](pemacompute.md)</ept>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>User-specified arguments for the <ph id="ph1">`initalize`</ph> method are:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>groupByVar = "character", computeVars = "character", fnList = "ANY", sep = "character",</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`groupByVar`</ph>: character string containing name of grouping variable.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>It can be a factor, character, or integer vector.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`computeVars`</ph>: character vector containing the name of one or more variables on which to compute the by-group statistics.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`fnList`</ph>: a named list of lists specifying functions and argument values.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The first element of each function list should be the function.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The second element of the function list should be named the name of the argument for the data vector or list of data vectors to process.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The value should be set to <ph id="ph1">`NULL`</ph> or the names of additional variables to be included in an input data list.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`sep`</ph>: the separator to use in creating the variable name(s) for the computed statistic(s).</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>It will take the form of <ph id="ph1">`varName.fnName`</ph> where the <ph id="ph2">`.`</ph> is replaced by <ph id="ph3">`sep`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>An <ph id="ph1">`PemaByGroup`</ph> reference class object.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>setRefClass, <bpt id="p1">[</bpt>PemaBaseClass<ept id="p1">](pemabaseclass.md)</ept></source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>