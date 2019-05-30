<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxsummary.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3ef76ce744466840341632f015b21ac878ec991d30.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">f76ce744466840341632f015b21ac878ec991d30</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxsummary.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxSummary function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Produce univariate summaries of objects in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxSummary, univar</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxSummary: Object Summaries</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Produce univariate summaries of objects in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>formula, as described in <bpt id="p1">[</bpt>rxFormula<ept id="p1">](rxFormula.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The formula typically does not contain a response variable, i.e. it should be of the form <ph id="ph1">`~ terms`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`~.`</ph> is used as the formula, summary statistics will be computed for all  non-character variables.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If a numeric variable is interacted with a factor variable, summary statistics will be computed for each category of the factor.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>either a data source object, a character string specifying a .xdf file, or a data frame object to summarize.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>NULL, a character string or vector of character strings  specifying .xdf file names(s), or an RxXdfData object or list of RxXdfData objects.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If not NULL, and the formula includes computations by factor, the by-group summary results will be  written out to one or more .xdf files.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If more than one <ph id="ph1">`.xdf`</ph> file is created and a single character string is specified, an integer will be appended to the base byGroupOutFile name  for additional file names.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The resulting RxXdfData objects will be listed in  the <ph id="ph1">`categorical`</ph> component of the output object.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>is not supported when using distributed compute contexts such as RxHadoopMR.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>a character vector containing one or more of the following  values:  "Mean", "StdDev", "Min", "Max", "ValidObs", "MissingObs", "Sum".</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>logical variable.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, missings will be removed  by term (by variable or by interaction expression) before computing  summary statistics.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, observations with missings in any  term will be removed before computations.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as frequency weights for the observations.</source>
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
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>character vector defining additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and  preloaded for use in variable transformation functions, e.g., those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments or those  defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>user-defined environment to serve as a parent to  all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`byGroupOutFile`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>is ignored <ph id="ph1">`byGroupOutFile`</ph> is <ph id="ph2">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, sparse cube is used.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, rows with no observations will be removed from the output for counts of categorical data.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>By default, it has the same value as <ph id="ph1">`useSparseCube`</ph>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>For large summary computation, this should be set to <ph id="ph1">`TRUE`</ph>, otherwise R may run out of memory even if the internal C++ computation succeeds.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>maximum number of rows to write to each block in the  <ph id="ph1">`byGroupOutFile`</ph> (if it is not <ph id="ph2">`NULL`</ph>).</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, additional summary information is printed.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>a valid <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`RxSpark`</ph>,  and <ph id="ph2">`RxHadoopMR`</ph> compute  contexts distribute the computation among the nodes specified by the  compute context; for other compute contexts, the  computation is distributed if possible on the local computer.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Revolution Compute Engine.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Special function <ph id="ph1">`F()`</ph> can be used in formula to force a variable to be interpreted as factors.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>If the formula contains a single dependent or response variable, summary statistics are computed for the interaction between that variable and the first term of the independent variables.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>(Multiple response variables are not permitted.) For example, using the formula <ph id="ph1">`y ~ xfac`</ph> will give the same results as using the formula <ph id="ph2">`~y:xfac`</ph>, where <ph id="ph3">`y`</ph> is a continuous variable and <ph id="ph4">`xfac`</ph> is a factor.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Summary statistics for <ph id="ph1">`y`</ph> are computed for each factor level of <ph id="ph2">`x`</ph>.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>This facilitates using the same formula in <ph id="ph1">`rxSummary`</ph> as in, for example, <ph id="ph2">`rxCube`</ph> or <ph id="ph3">`rxLinMod`</ph>.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>an rxSummary object containing the following elements:</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>number of valid observations.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>number of missing observations.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>data frame containing summaries for continuous variables.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>list of summaries for categorical variables.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>types of categorical summaries: can be "counts", or "cube" (for crosstab counts) or "none" (if there is no categorical summaries).</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>formula used to obtain the summary.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>rxTransform</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>