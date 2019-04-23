<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxdtree.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca8631a99238e5497f80f572f14530fdd0a29cd1e905.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31a99238e5497f80f572f14530fdd0a29cd1e905</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxdtree.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxDTree function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxDTree, print.rxDTree, models, tree, classif, regression, classification</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>rxDTree: Parallel External Memory Algorithm for Classification and Regression Trees</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Fit classification and regression trees on an .xdf file or data frame for small or large data using parallel external memory algorithm.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>formula as described in <bpt id="p1">[</bpt>rxFormula<ept id="p1">](rxFormula.md)</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Currently, formula functions are not supported.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>either a data source object, a character string  specifying a .xdf file, or a data frame object.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>either an RxXdfData data source object or a character string  specifying the .xdf file for storing the resulting node indices.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, then no node indices are stored to disk.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If the input data is a data frame,  the node indices are returned automatically.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`rowSelection`</ph> is specified and not <ph id="ph2">`NULL`</ph>,  then <ph id="ph3">`outFile`</ph> cannot be the same as the <ph id="ph4">`data`</ph>since the resulting set of node indices will generally not  have the same number of rows as the original data source.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>character string to be used as a column name  for the resulting node indices if <ph id="ph1">`outFile`</ph> is not <ph id="ph2">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Note that make.names is used on <ph id="ph1">`outColName`</ph>to ensure that the column name is valid.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`outFile`</ph> is an <ph id="ph2">`RxOdbcData`</ph> source, dots are first converted to underscores.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Thus, the default <ph id="ph1">`outColName`</ph> becomes <ph id="ph2">`"X_rxNode"`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, and the output file is different from the input file,  variables in the model will be written to the output file in addition to the node numbers.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If variables from the input data set are transformed in the model,  the transformed variables will also be written out.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>or character vector of additional variables names from the input data or transforms to include in the <ph id="ph1">`outFile`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`writeModelVars`</ph> is <ph id="ph2">`TRUE`</ph>, model variables will be included as well.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outFile`</ph>with an existing column named <ph id="ph3">`outColName`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>character string specifying the variable of numeric values to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>character string specifying the variable of integer values to use as frequency weights for the observations.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>character string specifying the splitting method.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Currently, only <ph id="ph1">`"class"`</ph> or <ph id="ph2">`"anova"`</ph> are supported.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The default is <ph id="ph1">`"class"`</ph> if the response is a factor, otherwise <ph id="ph2">`"anova"`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>optional list with components specifying additional parameters for the <ph id="ph1">`"class"`</ph> splitting method, as follows:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>- a vector of prior probabilities.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The priors must be positive and sum to 1.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The default  priors are proportional to the data counts.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>- a loss matrix, which must have zeros on the diagonal and positive off-diagonal elements.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>By default, the off-diagonal elements are set to 1.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>- the splitting index, either <ph id="ph1">`gini`</ph> (the default) or <ph id="ph2">`information`</ph>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`parms`</ph> is specified, any of the components can be specified or omitted.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The defaults will be used for missing components.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>a vector of non-negative costs, containing one element for each variable in the model.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Defaults to one for all variables.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>When deciding which split   to choose, the improvement on splitting on a variable is divided by its cost.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>the minimum number of observations that must exist in a node before a split is attempted.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>By default, this is <ph id="ph1">`sqrt(num of obs)`</ph>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>For non-XDF data sources, as <ph id="ph1">`(num of obs)`</ph> is unknown in advance, it is wisest to specify this argument directly.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>the minimum number of observations in a terminal node (or leaf).</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>By default, this is <ph id="ph1">`minSplit`</ph>/3.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>numeric scalar specifying the complexity parameter.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Any split that does not decrease overall lack-of-fit by at  least <ph id="ph1">`cp`</ph> is not attempted.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>the maximum number of competitor splits retained in the output.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>These are useful model diagnostics, as they allow you to compare splits in the output with the alternatives.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>the maximum number of surrogate splits retained in the output.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>See the Details for a description of how surrogate splits are used in the model fitting.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Setting this to 0 can greatly improve the performance of the algorithm; in some cases almost half the computation time is spent in computing surrogate splits.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>an integer specifying how surrogates are to be used in the splitting process:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>- display-only; observations with a missing value for the primary split variable are not sent further down the tree.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>- use surrogates,in order, to split observations missing the primary split variable.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If all surrogates are missing, the  observation is not split.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>- use surrogates, in order, to split observations missing the primary split variable.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>If all surrogates are missing or <ph id="ph1">`maxSurrogate=0`</ph>, send the observation in the majority direction.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`0`</ph> value corresponds to the behavior of the <ph id="ph2">`tree`</ph> function, and <ph id="ph3">`2`</ph> (the default) corresponds to the recommendations of Breiman et al.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>the number of cross-validations to be performed along with the model building.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Currently, <ph id="ph1">`1:xVal`</ph> is repeated and used to identify the folds.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If not zero, the <ph id="ph1">`cptable`</ph> component of the resulting model will contain both the mean (xerror) and standard deviation (xstd) of the cross-validation errors,  which can be used to select the optimal cost-complexity pruning of the fitted tree.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Set it to zero if external cross-validation will be used to evaluate the fitted model because a value of k increases the compute time to (k+1)-fold over a value of zero.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>an integer controlling selection of a best surrogate.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The default, <ph id="ph1">`0`</ph>, instructs the program to use the total number of correct classifications for a potential surrogate, while <ph id="ph2">`1`</ph> instructs the program to use the percentage of correct classification over  the non-missing values of the surrogate.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Thus, <ph id="ph1">`0`</ph> penalizes potential surrogates with a large number of missing values.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>the maximum depth of any tree node.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The computations take much longer at greater depth, so lowering <ph id="ph1">`maxDepth`</ph> can greatly speed up computation time.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>the maximum number of bins to use to cut numeric data.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>The default is <ph id="ph1">`min(1001, max(101, sqrt(num of obs)))`</ph>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>For non-XDF data sources, as <ph id="ph1">`(num of obs)`</ph> is unknown in advance, it is wisest to specify this argument directly.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>If set to <ph id="ph1">`0`</ph>, unit binning will be used instead of cutting.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>See the 'Details' section for more information.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>the maximum number of levels allowed for an unordered factor predictor for multiclass (&gt;2) classification.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, rows with missing values are removed and  will not be included in the output data.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>logical value or NULL.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the tree node IDs for all the observations are computed and returned.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the IDs are computed for data.frame with less than 1000 observations  and are returned as the <ph id="ph2">`where`</ph> component in the fitted <ph id="ph3">`rxDTree`</ph> object.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, sparse cube is used.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, optimal splits for each node are determined using parallelization methods;  this will typically speed up computation as the number of nodes on the same level is increased.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Note that when it is <ph id="ph1">`TRUE`</ph>, the number of nodes being processed in parallel is also  printed to the console, interleaved with the number of rows read from the input data set.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Optional complexity parameter for pruning.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`pruneCp &gt; 0`</ph>, <ph id="ph2">`prune.rxDTree`</ph> is  called on the completed tree with the specified <ph id="ph3">`pruneCp`</ph> and the pruned tree is returned.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>This contrasts with the <ph id="ph1">`cp`</ph> parameter that determines which splits are considered in <bpt id="p1">*</bpt>growing<ept id="p1">*</ept> the tree.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The option <ph id="ph1">`pruneCp="auto"`</ph> causes <ph id="ph2">`rxDTree`</ph> to call the function <ph id="ph3">`rxDTreeBestCp`</ph> on the completed tree, then use its return value as the cp value for <ph id="ph4">`prune.rxDTree`</ph>.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>name of a logical variable in the data set (in quotes) or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>will use only observations in which the value of the <ph id="ph1">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph2">`log`</ph> of the <ph id="ph3">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations  (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function  call using the expression function.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>an expression of the form <ph id="ph1">`list(name = expression, ...)`</ph>representing the first round of variable transformations.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>)  can be defined outside of the function call  using the expression function.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>a named list containing objects that can be referenced by  <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>variable transformation function.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>The ".rxSetLowHigh" attribute must be set for transformed variables if they are to be used in <ph id="ph1">`formula`</ph>.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>character vector of input data set variables  needed for the transformation function.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>character vector defining additional R packages  (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>)  to be made available and preloaded for use in variable transformation functions,  e.g., those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions  via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments  or those defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>user-defined environment to serve as a parent to all environments  developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>,  a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data  read from the data source.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Integer values from <ph id="ph1">`1`</ph> to <ph id="ph2">`2`</ph> provide increasing amounts of information are provided.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>a valid <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`RxSpark`</ph> and <ph id="ph2">`RxHadoopMR`</ph> compute contexts distribute the computation among the nodes specified by the compute context; for other compute contexts, the computation is distributed if possible on the local computer.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>integer in the range of -1 to 9 indicating the compression level for the output data  if written to an <ph id="ph1">`.xdf`</ph> file.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the amount of compression -  resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`xdfCompressionLevel`</ph> is set to 0, there will be no compression and  files will be compatible with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression will be used.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Microsoft R Services Compute Engine.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>is a parallel external memory decision tree algorithm targeted for very large data sets.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>It is modeled after rpart (Version 4.1-0) and inspired by the algorithm proposed by Yael Ben-Haim and Elad Tom-Tov (2010).</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>It uses a histogram as the approximate compressed representation of the data and builds the tree in a breadth-first fashion using horizontal parallelism.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>specifies the maximum number of bins for the histogram of each continuous independent variable and thus controls the accuracy of the algorithm.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Also, rxDTree builds histograms with roughly equal number of observations in each bin and checks only the boundaries of the bins as candidate splits to find the best split.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>So it is possible that a suboptimal split is chosen if <ph id="ph1">`maxNumBins`</ph> is too small.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>This may cause the tree to be different from one constructed by a standard algorithm.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Increasing <ph id="ph1">`maxNumBins`</ph> allows more accurate results but with increased time and memory usage..</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Surrogate splits may be used to assign observations for which the primary split variable is missing.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Surrogate splits compare the groups produced by the remaining predictor variables to the groups produced by the primary split variable, and the predictors are ranked by how well their groups match the primary predictor.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>The best match is used as the surrogate split.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>an object of class <ph id="ph1">`"rxDTree"`</ph> representing the fitted tree.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>It is a list with components similar to those of class <ph id="ph1">`"rpart"`</ph> with the following distinctions:</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>-  A vector of integers indicating the node to which each point is allocated.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>This information is always returned if the data source is a data frame.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>If the data source is not a data frame and <ph id="ph1">`outFile`</ph> is specified.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>i.e., not <ph id="ph1">`NULL`</ph>, the node indices are written/appended to  the specified file with a column name as defined by <ph id="ph2">`outColName`</ph>.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>For other components, see rpart.object for details.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>rxDTree requires multiple passes over the data set and the maximum number of passes can be computed as follows:</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>quantile computation:  <ph id="ph1">`1`</ph> pass for computing the quantiles for all continuous variables,</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>recursive partition:  <ph id="ph1">`maxDepth + 1`</ph> passes for building the tree on the entire dataset,</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>tree node assignment:  <ph id="ph1">`1`</ph> pass for computing the id of the leaf node that each observation falls into.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>If cross validation is specified (i.e., <ph id="ph1">`xVal&gt;0`</ph>), additional passes will be needed for each fold:</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>recursive partition:  <ph id="ph1">`maxDepth + 1`</ph> passes for building the tree on the other folds,</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>tree node assignment:  <ph id="ph1">`1`</ph> pass for predicting on the current fold.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>resulting in <ph id="ph1">`xVal * ((maxDepth + 1) + 1)`</ph> additional passes for cross validation.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>Breiman, L., Friedman, J. H., Olshen, R. A.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>and Stone, C. J.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>(1984) <bpt id="p1">*</bpt>Classification and Regression Trees<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Wadsworth.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Therneau, T. M.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>and Atkinson, E. J.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>(2011) <bpt id="p1">*</bpt>An Introduction to Recursive Partitioning Using the RPART Routines<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Yael Ben-Haim and Elad Tom-Tov (2010) A streaming parallel decision tree algorithm.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Journal of Machine Learning Research<ept id="p1">*</ept> <bpt id="p2">**</bpt>11<ept id="p2">**</ept>, 849--872.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>rpart, rpart.control, rpart.object, <bpt id="p1">[</bpt>rxPredict.rxDTree<ept id="p1">](rxPredict.rxDTree.md)</ept>, <bpt id="p2">[</bpt>rxAddInheritance<ept id="p2">](rxAddInheritance.md)</ept>, <bpt id="p3">[</bpt>rxDForestUtils<ept id="p3">](rxDForestUtils.md)</ept>.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>