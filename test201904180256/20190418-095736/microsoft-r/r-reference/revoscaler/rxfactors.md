<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxfactors.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c7bf4e2b60d3ae37f2e11aafb3eb0d3df1672ff10.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">7bf4e2b60d3ae37f2e11aafb3eb0d3df1672ff10</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxfactors.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxFactors function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Recodes a factor variable by mapping one set of factor levels and indices to a new set.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Can also be used to convert non-factor variable into a factor.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxFactors, manip, category</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>rxFactors:  Factor Variable Recoding</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Recodes a factor variable by mapping one set of factor levels and indices to a new set.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Can also be used to convert non-factor variable into a factor.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>either an RxXdfData object, a character string specifying the .xdf file, or a data frame.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>character vector of variable names,a list of named variable information lists, or empty or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`sortLevels`</ph> is set to <ph id="ph2">`TRUE`</ph>, the levels of the variables named in the character vector will  all be sorted; if <ph id="ph3">`sortLevels`</ph> is <ph id="ph4">`TRUE`</ph> and <ph id="ph5">`factorInfo`</ph> is empty or <ph id="ph6">`NULL`</ph>, all   factors will be sorted.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If a <ph id="ph1">`factorInfo`</ph> list is provided, each variable information list contains one or more of the   named elements given below.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Currently available properties for a column information list are:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`levels`</ph> - optional vector, containing values to match in converting non-factor data to factor levels.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`levels = NULL`</ph>, all of the unique values in the data are converted to levels.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>in the order encountered.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>However, the user can  override this behavior and sort the resulting levels alphabetically by setting <ph id="ph1">`sortLevels = TRUE`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The user may also specify a subset of the data to convert to levels.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>In this case, if <ph id="ph1">`otherLevel = NULL`</ph>,  all data values <bpt id="p1">*</bpt>not<ept id="p1">*</ept> found in the <ph id="ph2">`levels`</ph> subset will be converted to missing (<ph id="ph3">`NA`</ph>) values.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>For example, if a variable <ph id="ph1">`x`</ph> is comprised of integer data <ph id="ph2">`1`</ph>, <ph id="ph3">`2`</ph>, <ph id="ph4">`3`</ph>, <ph id="ph5">`4`</ph>, <ph id="ph6">`5`</ph>, then</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>`` - <ph id="ph1">`factorInfo = list(x = list(levels = 2:4, otherLevel = NULL))`</ph></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>will convert <ph id="ph1">`x`</ph> into a factor with data <ph id="ph2">`NA`</ph>, <ph id="ph3">`"2"`</ph>, <ph id="ph4">`"3"`</ph>, <ph id="ph5">`"4"`</ph>, <ph id="ph6">`NA`</ph> with levels <ph id="ph7">`"2"`</ph>,<ph id="ph8">`"3"`</ph>,<ph id="ph9">`"4"`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Alternatively, the user may wish to place all of those unspecified values into a single category, say <ph id="ph1">`"other"`</ph>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>In that case, use <ph id="ph1">`otherLevel = "other"`</ph> along with the subset <ph id="ph2">`levels`</ph> specification.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Note that the <ph id="ph1">`levels`</ph> vector may be any type, e.g., 'integer', 'numeric', 'character'.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>However, behind the scenes,  it is always converted to type 'character', as are the data values being converted.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The resulting strings are matched  with those of the data to populate the categories.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`otherLevel`</ph> - character string defining the level to assign to all factor values that  are not listed in the <ph id="ph2">`newLevels`</ph> field, if <ph id="ph3">`newLevels`</ph> is specified.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`otherLevel = NULL`</ph>,  the default, the factor levels that are not listed in <ph id="ph2">`newLevels`</ph> will be left unchanged and in their original  order.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If specified, the value set here overrides the default argument of the same in the primary argument list.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`sortLevels`</ph> - logical scalar.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the resulting levels will be sorted alphabetically.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If the input variable is not a factor and levels are not specified, this will be ignored and levels will be in the order in which they are encountred.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`varName`</ph> - character string defining the name of an existing data variable to recode.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If this field is left unspecified, then the name of the corresponding list element in <ph id="ph1">`factorInfo`</ph> will be used.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>For example, all of the following are acceptable and equivalent <ph id="ph1">`factorInfo`</ph> specifications for alphabetically  sorting the levels of an existing factor variable named <ph id="ph2">`"myFacVar"`</ph>:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>`` - <ph id="ph1">`factorInfo = list( myFacVar = list( sortLevels = TRUE ) )`</ph></source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>`` - <ph id="ph1">`factorInfo = list( list( sortLevels = TRUE, varName = "myFacVar" ) )`</ph></source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>`` - <ph id="ph1">`factorInfo = list( myFacVar = list( sortLevels = TRUE, varName = "myFacVar" ) )`</ph></source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>However, if you wish to rename a variable after conversion (keeping the old variable in tact),  there is only one acceptable format: the variable to be recoded must appear in the <ph id="ph1">`varName`</ph> field while the new variable name for the converted data must appear as the name of the corresponding list element.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>For example, to sort the levels of an existing factor variable <ph id="ph1">`"myFacVar"`</ph> and store the result in a new variable <ph id="ph2">`"myNewVar"`</ph>, you would issue:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>`` - <ph id="ph1">`factorInfo = list( myNewFacVar = list( sortLevels = TRUE, varName = "myFacVar" ) )`</ph></source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`newLevels`</ph> - a character vector or list, possibly with named elements, used to rename the levels of a factor.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>While <ph id="ph1">`levels`</ph> provides a means of filtering the data the user wishes to import and convert to factor levels, <ph id="ph2">`newLevels`</ph> is used to alter converted or existing levels by renaming, collapsing, or sorting them.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>See the Examples section below for typical use cases of <ph id="ph1">`newLevels`</ph>.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`description`</ph> - character string defining a description for the recoded variable.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>the default value to use for the <ph id="ph1">`sortLevels`</ph> field in the <ph id="ph2">`factorInfo`</ph> list.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>the default value to use for the <ph id="ph1">`otherLevel`</ph> field in the <ph id="ph2">`factorInfo`</ph> list.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>either an RxXdfData object, a character string specifying the .xdf file, or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outFile = NULL`</ph>, a data frame is returned.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>When writing to HDFS, <ph id="ph1">`outFile`</ph> must be an <ph id="ph2">`RxXdfData`</ph> object representing a new composite XDF.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>character vector of variable names to include in the data file.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToDrop`</ph>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>character vector of variable names to not include in the data file.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToKeep`</ph>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outFile`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Ignored if a dataframe is returned.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>this argument is used only when  <ph id="ph1">`inData`</ph> is referring to an .xdf file  (character string defining a path to an existing .xdf file or an RxXdfData object) and we wish to return the output as a data frame (<ph id="ph2">`outFile = NULL`</ph>).</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>In this case, and behind the scenes, the output is written to a temporary .xdf file and <ph id="ph1">`rxDataStep`</ph> is subsequently called to convert the output into a data frame.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`maxRowsByCols`</ph> argument is passed directly in the <ph id="ph2">`rxDataStep`</ph> call, giving the user some control over the conversion.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxDataStep.md)</ept> for more details on the <ph id="ph1">`maxRowsByCols`</ph> argument.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`data`</ph> and <ph id="ph2">`outFile`</ph> are the same file, blocksPerRead must be 1.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, additional summary information is printed.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>integer in the range of -1 to 9.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the  amount of compression - resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>If  <ph id="ph1">`xdfCompressionLevel`</ph> is set to 0, there will be no compression and files will be compatible  with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression  will be used.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Microsoft R Services Compute Engine.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Factors are variables that represent categories.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>An example is a variable named <ph id="ph1">`"state"`</ph> whose values are the levels <ph id="ph2">`"Alabama"`</ph>, <ph id="ph3">`"Alaska"`</ph>, ..., <ph id="ph4">`"Wyoming"`</ph>.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>There are two parts to a factor variable:</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>1 a vector of N (number of observations) integer indexes with values in the range of <ph id="ph1">`1:K`</ph>, where K is the number of categories.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>1 a vector of K strings (characters) that are used when the vector is displayed and in some other situations.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>For instance, when state levels are alphabetical, all observations for which <ph id="ph1">`state == "Alabama"`</ph> will have the index <ph id="ph2">`1`</ph>,  <ph id="ph3">`state == "Washington"`</ph> values correspond to index <ph id="ph4">`47`</ph>, and so on.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Recoding a factor means changing from one set of indices to another.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>For instance, if the levels for <ph id="ph1">`"state"`</ph> are currently arranged in the order in which they were encountered when importing a .csv file, and it is desired to put them in alphabetical order, then it is necessary to change the index for every observation.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>If numeric data is converted to a factor, a maximum precision of 6 is used.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>So, for example, the values 7.123456 and 7.12346 would be placed in the same category.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>To recode a categorical or factor variable into a continuous variable within a formula use <ph id="ph1">`N()`</ph>.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>To recode continuous variable to a categorical or factor variable within a formula use <ph id="ph1">`F()`</ph>.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxFormula<ept id="p1">](rxFormula.md)</ept>.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>To rename the levels of a factor variable in an .xdf file (without change the levels themselves), use <bpt id="p1">[</bpt>rxSetVarInfoXdf<ept id="p1">](rxSetVarInfoXdf.md)</ept>.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>if <ph id="ph1">`outFile`</ph> is <ph id="ph2">`NULL`</ph>, then a data frame is returned.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Otherwise, the results are written to the specified <ph id="ph1">`outFile`</ph> file and an RxXdfData object is returned <bpt id="p1">*</bpt>invisibly<ept id="p1">*</ept> corresponding to the output file.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxFormula<ept id="p1">](rxFormula.md)</ept>, <bpt id="p2">[</bpt>rxSetVarInfoXdf<ept id="p2">](rxSetVarInfoXdf.md)</ept>, <bpt id="p3">[</bpt>rxImport<ept id="p3">](rxImport.md)</ept>, <bpt id="p4">[</bpt>rxDataStep<ept id="p4">](rxDataStep.md)</ept>.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>