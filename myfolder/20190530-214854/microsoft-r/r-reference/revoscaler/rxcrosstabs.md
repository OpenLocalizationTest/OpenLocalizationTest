<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxcrosstabs.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e60558705b6673d747a1f666d381d06aab65d5c01.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">60558705b6673d747a1f666d381d06aab65d5c01</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxcrosstabs.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxCrossTabs function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Use rxCrossTabs to create contingency tables from cross- classifying factors using a formula interface.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>It performs equivalent computations to the <bpt id="p1">[</bpt>rxCube<ept id="p1">](rxCube.md)</ept> function, but returns its results in a different way.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxCrossTabs, print.rxCrossTabs, summary.rxCrossTabs, mean.rxCrossTabs, as.list.rxCrossTabs, category, models</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>rxCrossTabs: Cross Tabulation</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`rxCrossTabs`</ph> to create contingency tables from cross- classifying factors using a formula interface.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>It performs equivalent computations to the <bpt id="p1">[</bpt>rxCube<ept id="p1">](rxCube.md)</ept> function, but returns its results in a different way.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>formula as described in <bpt id="p1">[</bpt>rxFormula<ept id="p1">](rxFormula.md)</ept> with the categorical cross-classifying variables (separated by <ph id="ph1">`:`</ph>) on the right hand side.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>either a data source object, a character string specifying a .xdf file, or a data frame object containing the cross-classifying variables.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as frequency weights for the observations.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the mean values of the contingency table are also stored in the output object along with the sums and counts.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>By default, if the mean values are stored, the <ph id="ph1">`print`</ph> and <ph id="ph2">`summary`</ph> methods display them.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>However, the <ph id="ph1">`output`</ph> argument in those methods can be used to override this behavior by setting <ph id="ph2">`output`</ph> equal to <ph id="ph3">`"sums"`</ph> or <ph id="ph4">`"counts"`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, a list of marginal table values is stored as an attribute named <ph id="ph2">`"marginals"`</ph> for each of the contingency tables.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Each marginals list contains entries for the row, column and grand totals or means, depending on the type of data table.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>To access them directly, use the <bpt id="p1">[</bpt>rxMarginals<ept id="p1">](rxMarginals.md)</ept> function.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the C++ cube functionality is called.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>name of a logical variable in the data set (in quotes) or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>will use only observations in which the value of the <ph id="ph1">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph2">`log`</ph> of the <ph id="ph3">`income`</ph> variable is greater than 10.</source>
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
          <source>If <ph id="ph1">`TRUE`</ph>, sparse cube is used.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>For large crosstab computation, R may run out of memory due to the resulting expanded contingency tables  even if the internal C++  computation succeeds.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>In which cases, try to use <ph id="ph1">`rxCube`</ph> instead.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, rows with no observations will be removed from the contingency tables.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>By default, it has the same value as <ph id="ph1">`useSparseCube`</ph>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Please note this affects only those zeroed counts in the final contingency table for which there are no observations in the input data.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>However, if the input data contains a row with <bpt id="p1">*</bpt>frequency<ept id="p1">*</ept> zero it will be reported in the final contingency table.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>This should be set to <ph id="ph1">`TRUE`</ph> if the total number of combinations of factor values on the right-hand side of the <ph id="ph2">`formula`</ph> is significant and as a result R might run out of memory when handling the resulting large contingency table.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an object of class xtabs is returned.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Note that the only difference between the structures of an equivalent <ph id="ph1">`xtabs`</ph> call output and the output of <ph id="ph2">`rxCrossTabs(..., returnXtabs = TRUE)`</ph> is that they will contain different <ph id="ph3">`"call"`</ph> attributes.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Note also that <ph id="ph1">`xtabs`</ph> expects the cross-classifying variables in the <ph id="ph2">`formula`</ph> to be separated by plus (+) symbols whereas <ph id="ph3">`rxCrossTabs`</ph> expects them to be separated by a colon (:) symbols.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, <ph id="ph2">`NA`</ph> values are removed when calculating the marginal means of the contingency tables.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>integer value:  Options are:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, additional summary information is printed.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>a valid <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`RxSpark`</ph>  and <ph id="ph2">`RxHadoopMR`</ph> compute  contexts distribute the computation among the nodes specified by the  compute context; for other compute contexts, the  computation is distributed if possible on the local computer.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>for <ph id="ph1">`rxCrossTabs`</ph>, additional arguments to be passed directly to the base computational function.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>objects of class rxCrossTabs.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>character string used to specify the type of output to display.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Choices are <ph id="ph1">`"sums"`</ph>, <ph id="ph2">`"counts"`</ph> and <ph id="ph3">`"means"`</ph>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, header information is printed.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>character string used to specify the summary to create.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Choices are <ph id="ph1">`"%"`</ph> or <ph id="ph2">`"percentages"`</ph> and <ph id="ph3">`"chisquare"`</ph> to summarize the cross-tabulation results with percentages or performs a chi-squared test for independence of factors, respectively.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The output is returned in a list and the <ph id="ph1">`print`</ph> and <ph id="ph2">`summary`</ph> methods can be used to display and summarize the contingency table(s) contained in each element of the output list.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`print`</ph> method produces an output similar to that of the xtabs function.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`summary`</ph> method produces a summary table for each output contingency table and displays the column, row, and total table percentages as well as the counts.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>an object of class rxCrossTabs that contains a list of elements described as follows:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>list of contingency tables whose values are cross-tabulation sums.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>This object is NULL if there are no dependent variables specified in the formula<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>The names of the list objects are built using the dependent variables specified in the formula (if they exist) along with the independent variable factor levels corresponding to each contingency table.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`z &lt;- rxCrossTabs(ncontrols ~ agegp + alcgp + tobgp, esoph); names(z$sums)`</ph> will return the character vector with elements <ph id="ph2">`"ncontrols, tobgp = 0-9g/day"`</ph>, <ph id="ph3">`"ncontrols, tobgp = 10-19"`</ph>, <ph id="ph4">`"ncontrols, tobgp = 20-29"`</ph>, <ph id="ph5">`"ncontrols, tobgp = 30+"`</ph>.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Typically, the user should rely on the <ph id="ph1">`print`</ph> or <ph id="ph2">`summary`</ph> methods to display the cross tabulation results but you can also directly access an individual contingency table using its name in R's standard list data access methods.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>For example, to access the "ncontrols, tobgp = 10-19" table containing cross tabulation summations you would use <ph id="ph1">`z$sums[["ncontrols, tobgp = 10-19"]]`</ph> or equivalently <ph id="ph2">`z$sums[[2]]`</ph>.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>To print the entire list of cross-tabulation summations one would issue <ph id="ph1">`print(z, output="sums")`</ph>.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>list of contingency tables whose values are cross-tabulation counts.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>The names of the list objects are equivalent to those of the 'sums' output list.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>list of contingency tables containing cross tabulation mean values.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>This object is NULL if there are no dependent variables specified in the formula<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>The 'means' list is returned only if the user has specified <ph id="ph1">`means=TRUE`</ph> in the call to rxCrossTabs.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`means=FALSE`</ph> in the call, mean values still may be calculated and returned using the <ph id="ph2">`print`</ph> and <ph id="ph3">`summary`</ph> methods with an <ph id="ph4">`output="means"`</ph> argument.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>In this case, the mean values are calculated dynamically.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>If you wish to have quick access to the means, use <ph id="ph1">`means=TRUE`</ph> in the call to rxCrossTabs.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>The names of the list objects are equivalent to those of the 'sums' output list.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>original call to the underlying <ph id="ph1">`rxCrossTabs.formula`</ph> method.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>list of chi-square tests, one for each cross-tabulation table.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Each entry contains the results of a chi-squared test for independence of factors as used in the summary method for the xtabs function.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>The names of the list objects are equivalent to those of the 'sums' output list.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>formula used in the <ph id="ph1">`rxCrossTabs`</ph> call.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>character vector of dependent variable names as extracted from the formula.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>xtabs, <bpt id="p1">[</bpt>rxMarginals<ept id="p1">](rxMarginals.md)</ept>, <bpt id="p2">[</bpt>rxCube<ept id="p2">](rxCube.md)</ept>, <bpt id="p3">[</bpt>as.xtabs<ept id="p3">](as.xtabs.md)</ept>, <bpt id="p4">[</bpt>rxChiSquaredTest<ept id="p4">](rxChiSquaredTest.md)</ept>, <bpt id="p5">[</bpt>rxFisherTest<ept id="p5">](rxChiSquaredTest.md)</ept>, <bpt id="p6">[</bpt>rxKendallCor<ept id="p6">](rxChiSquaredTest.md)</ept>, <bpt id="p7">[</bpt>rxPairwiseCrossTab<ept id="p7">](rxPairwiseCrosstab.md)</ept>, <bpt id="p8">[</bpt>rxRiskRatio<ept id="p8">](rxRiskRatio.md)</ept>, <bpt id="p9">[</bpt>rxOddsRatio<ept id="p9">](rxRiskRatio.md)</ept>, <bpt id="p10">[</bpt>rxTransform<ept id="p10">](rxTransform.md)</ept>.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>