<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxcube.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4c8581d0f1265e35d03422033706025fdda6da746.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">c8581d0f1265e35d03422033706025fdda6da746</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxcube.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxCube function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Use rxCube to create efficiently represented contingency tables from cross-classifying factors using a formula interface.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>It performs equivalent calculations to the rxCrossTabs function, but returns its results in a different way.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxCube, print.rxCube, summary.rxCube, as.data.frame.rxCube, subset.rxCube, [.rxCube, category, models</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>rxCube: Cross Tabulation</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`rxCube`</ph> to create efficiently represented contingency tables from cross-classifying factors using a formula interface.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>It performs equivalent calculations to the <ph id="ph1">`rxCrossTabs`</ph> function, but returns its results in a different way.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>formula as described in <bpt id="p1">[</bpt>rxFormula<ept id="p1">](rxFormula.md)</ept> with the cross-classifying variables (separated by <ph id="ph1">`:`</ph>) on the right hand side.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Independent variables must be factors.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If present, the dependent variable must be numeric.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>either a data source object, a character string specifying a .xdf file, or a data frame object containing the cross-classifying variables.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph>, a character string specifying a .xdf file, or an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If not NULL, the cube results will be written out to an .xdf file and an <ph id="ph1">`RxXdfData`</ph> object will be returned.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`outFile`</ph> is not supported when using distributed compute contexts.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as frequency weights for the observations.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> (default), the mean values of the dependent variable are returned.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Otherwise, the variable summations are returned.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the C++ cube functionality is called.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>name of a logical variable in the data set (in quotes) or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rowSelection = (age &gt; 20) &amp; (age &lt; 65) &amp; (log(income) &gt; 10)`</ph> will use only observations in which the value of the <ph id="ph2">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph3">`log`</ph> of the <ph id="ph4">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations  (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function  call using the expression function.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>an expression of the form <ph id="ph1">`list(name = expression, ...)`</ph> representing the first round of variable transformations.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>)  can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>a named list containing objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>variable transformation function.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The variables used in the  transformation function must be specified in <ph id="ph1">`transformVars`</ph> if they are not variables used in the model.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>character vector defining additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and  preloaded for use in variable transformation functions, e.g., those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments or those  defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>user-defined environment to serve as a parent to  all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outFile`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`overwrite`</ph> is ignored <ph id="ph2">`outFile`</ph> is <ph id="ph3">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, sparse cube is used.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, rows with no observations will be removed from the output.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>By default, it has the same value as <ph id="ph1">`useSparseCube`</ph>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>For large cube computation, this should be set to <ph id="ph1">`TRUE`</ph>, otherwise R may run out of memory even if the internal C++ computation succeeds.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, a data frame is returned, otherwise a list is returned.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Ignored if <ph id="ph1">`outFile`</ph> is specified and is not <ph id="ph2">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>See the Details section for more information.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>maximum number of rows to write to each block in the  <ph id="ph1">`outFile`</ph> (if it is not <ph id="ph2">`NULL`</ph>).</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, additional summary information is printed.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>a valid <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`RxSpark`</ph> and <ph id="ph2">`RxHadoopMR`</ph> compute  contexts distribute the computation among the nodes specified by the  compute context; for other compute contexts, the  computation is distributed if possible on the local computer.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Revolution Compute Engine.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>output objects from rxCube function.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, header information is printed.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>the <ph id="ph1">`row.names`</ph> argument passed unaltered to the underlying <ph id="ph2">`as.data.frame.list`</ph> function.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>the <ph id="ph1">`optional`</ph> argument passed unaltered to the underlying <ph id="ph2">`as.data.frame.list`</ph> function.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>The output of the <ph id="ph1">`rxCube`</ph> function is essentially the same as that produced by <bpt id="p1">[</bpt>rxCrossTabs<ept id="p1">](rxCrossTabs.md)</ept> except that it is presented in a different format.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>While the <ph id="ph1">`rxCrossTabs`</ph> function produces lists of contingency tables (where each table is a matrix), the <ph id="ph2">`rxCube`</ph> function outputs a single list (or data frame, or .xdf file) containing one column for each variable specified in the formula, plus a <ph id="ph3">`"Counts"`</ph> column.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The columns corresponding to <bpt id="p1">*</bpt>independent<ept id="p1">*</ept> variables contain the factor levels of that variable, replicated as necessary.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>If a dependent variable is specified in the formula, an output column of the same name is produced and contains the mean values of the categories defined by the interaction of the independent/categorical variables.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`"Counts"`</ph> column contains the counts of the interactions used to form the corresponding means.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`outFile`</ph> is not NULL: an <ph id="ph2">`RxXdfData`</ph> object representing the output .xdf file.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>In this case, the value for <ph id="ph1">`returnDataFrame`</ph> is ignored.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`returnDataFrame = FALSE`</ph>: an object of class rxCube that is also of class <ph id="ph2">`"list"`</ph>.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>This is the default.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`returnDataFrame = TRUE`</ph>: an object of class <ph id="ph2">`"data.frame"`</ph>.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>In all cases, the names of the output columns are those of the variables defined in the formula plus a <ph id="ph1">`"Counts"`</ph> column.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>See the Details section for more information regarding the content of these columns.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>xtabs, <bpt id="p1">[</bpt>rxCrossTabs<ept id="p1">](rxCrossTabs.md)</ept>, <bpt id="p2">[</bpt>as.xtabs<ept id="p2">](as.xtabs.md)</ept>, <bpt id="p3">[</bpt>rxTransform<ept id="p3">](rxTransform.md)</ept>.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>