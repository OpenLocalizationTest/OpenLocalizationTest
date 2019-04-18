<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxdforest.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926eac77e32cdd93b9b00cd32734caf07cd4572f7e5.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eac77e32cdd93b9b00cd32734caf07cd4572f7e5</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxdforest.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxDForest function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxDForest, plot.rxDForest, print.rxDForest, models, tree, classif, regression, classification</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>rxDForest: Parallel External Memory Algorithm for Classification and Regression Decision Forests</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Fit classification and regression decision forests on an .xdf file or data frame for small or large data using parallel external memory algorithm.</source>
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
          <source>either an RxXdfData data source object or a character string  specifying the .xdf file for storing the resulting OOB predictions.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> or the input data is a data frame, then no OOB predictions are stored to disk.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`rowSelection`</ph> is specified and not <ph id="ph2">`NULL`</ph>,  then <ph id="ph3">`outFile`</ph> cannot be the same as the <ph id="ph4">`data`</ph>since the resulting set of OOB predictions will generally not  have the same number of rows as the original data source.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, and the output file is different from the input file,  variables in the model will be written to the output file in addition to the OOB predictions.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If variables from the input data set are transformed in the model,  the transformed variables will also be written out.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outFile`</ph>with an existing column named <ph id="ph3">`outColName`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>character string specifying the variable  to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>character string specifying the variable  to use as frequency weights for the observations.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>character string specifying the splitting method.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Currently, only <ph id="ph1">`"class"`</ph> or <ph id="ph2">`"anova"`</ph> are supported.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The default is <ph id="ph1">`"class"`</ph> if the response is a factor, otherwise <ph id="ph2">`"anova"`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>optional list with components specifying additional parameters for the <ph id="ph1">`"class"`</ph> splitting method, as follows:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`prior`</ph> - a vector of prior probabilities.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The priors must be positive and sum to 1.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The default  priors are proportional to the data counts.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`loss`</ph> - a loss matrix, which must have zeros on the diagonal and positive off-diagonal elements.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>By default, the off-diagonal elements are set to 1.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`split`</ph> - the splitting index, either <ph id="ph2">`gini`</ph> (the default) or <ph id="ph3">`information`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`parms`</ph> is specified, any of the components can be specified or omitted.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The defaults will be used for missing components.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>a vector of non-negative costs, containing one element for each variable in the model.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Defaults to one for all variables.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>When deciding which split   to choose, the improvement on splitting on a variable is divided by its cost.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>the minimum number of observations that must exist in a node before a split is attempted.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>By default, this is <ph id="ph1">`sqrt(num of obs)`</ph>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>For non-XDF data sources, as <ph id="ph1">`(num of obs)`</ph> is unknown in advance, it is wisest to specify this argument directly.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>the minimum number of observations in a terminal node (or leaf).</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>By default, this is <ph id="ph1">`minSplit`</ph>/3.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>the maximum depth of any tree node.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The computations take much longer at greater depth, so lowering <ph id="ph1">`maxDepth`</ph> can greatly speed up computation time.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>numeric scalar specifying the complexity parameter.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Any split that does not decrease overall lack-of-fit by at  least <ph id="ph1">`cp`</ph> is not attempted.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>the maximum number of competitor splits retained in the output.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>These are useful model diagnostics, as they allow you to compare splits in the output with the alternatives.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>the maximum number of surrogate splits retained in the output.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>See the Details for a description of how surrogate splits are used in the model fitting.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Setting this to 0 can greatly improve the performance of the algorithm; in some cases almost half the computation time is spent in computing surrogate splits.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>an integer specifying how surrogates are to be used in the splitting process:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph> - display-only; observations with a missing value for the primary split variable are not sent further down the tree.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph> - use surrogates,in order, to split observations missing the primary split variable.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If all surrogates are missing, the  observation is not split.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph> - use surrogates, in order, to split observations missing the primary split variable.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If all surrogates are missing or <ph id="ph1">`maxSurrogate=0`</ph>, send the observation in the majority direction.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`0`</ph> value corresponds to the behavior of the <ph id="ph2">`tree`</ph> function, and <ph id="ph3">`2`</ph> (the default) corresponds to the recommendations of Breiman et al.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>an integer controlling selection of a best surrogate.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The default, <ph id="ph1">`0`</ph>, instructs the program to use the total number of correct classifications for a potential surrogate, while <ph id="ph2">`1`</ph> instructs the program to use the percentage of correct classification over  the non-missing values of the surrogate.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Thus, <ph id="ph1">`0`</ph> penalizes potential surrogates with a large number of missing values.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>a positive integer specifying the number of trees to grow.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>a positive integer specifying the number of variables to sample as split candidates at each tree node.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The default values is <ph id="ph1">`sqrt(num of vars)`</ph> for classification and <ph id="ph2">`(num of vars)/3`</ph> for regression.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>a logical value specifying if the sampling of observations should be done with or without replacement.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>(Classification only) a vector of length equal to the number of classes specifying the dividing factors for the class votes.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The default is <ph id="ph1">`1/(num of classes)`</ph>.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>a character string specifying the (factor) variable to use for stratified sampling.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>a scalar or a vector of positive values specifying the percentage(s) of observations to sample for each tree:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>for unstratified sampling:  a scalar of positive value specifying the percentage of observations to sample for each tree.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The default is 1.0 for sampling with replacement (i.e., <ph id="ph1">`replace=TRUE`</ph>) and  0.632 for sampling without replacement (i.e., <ph id="ph2">`replace=FALSE`</ph>).</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>for stratified sampling:  a vector of positive values of length equal to the number of strata specifying  the percentages of observations to sample from the strata for each tree.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>a logical value specifying if the importance of predictors should be assessed.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>an integer that will be used to initialize the random number generator.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>The default is random.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>For reproducibility, you can specify the random seed either using set.seed or by setting this <ph id="ph1">`seed`</ph> argument as part of your call.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>an integer specifying whether and how to compute the prediction error for out-of-bag samples:</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`&lt;0`</ph> - never.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>This option may reduce the computation time.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`=0`</ph> - only once for the entire forest.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`&gt;0`</ph> - once for each addition of a tree.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>This is the default.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>the maximum number of bins to use to cut numeric data.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>The default is <ph id="ph1">`min(1001, max(101, sqrt(num of obs)))`</ph>.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>For non-XDF data sources, as <ph id="ph1">`(num of obs)`</ph> is unknown in advance, it is wisest to specify this argument directly.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>If set to <ph id="ph1">`0`</ph>, unit binning will be used instead of cutting.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>See the 'Details' section for more information.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>the maximum number of levels allowed for an unordered factor predictor for multiclass (&gt;2) classification.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, rows with missing values are removed and  will not be included in the output data.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, sparse cube is used.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, optimal splits for each node are determined using parallelization methods;  this will typically speed up computation as the number of nodes on the same level is increased.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Note that when it is <ph id="ph1">`TRUE`</ph>, the number of nodes being processed in parallel is also  printed to the console, interleaved with the number of rows read from the input data set.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>EXPERIMENTAL.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, rxDForest will be run with <bpt id="p1">[</bpt>rxExec<ept id="p1">](rxExec.md)</ept>, which submits only one job to the scheduler and thus can speed up computation on small data sets particularly in the RxHadoopMR compute context.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>name of a logical variable in the data set (in quotes) or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rowSelection = (age &gt; 20) &amp; (age &lt; 65) &amp; (log(income) &gt; 10)`</ph> will use only observations in which the value of the <ph id="ph2">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph3">`log`</ph> of the <ph id="ph4">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations  (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function  call using the expression function.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>an expression of the form <ph id="ph1">`list(name = expression, ...)`</ph>representing the first round of variable transformations.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>)  can be defined outside of the function call  using the expression function.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>a named list containing objects that can be referenced by  <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>variable transformation function.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>The ".rxSetLowHigh" attribute must be set for transformed variables if they are to be used in <ph id="ph1">`formula`</ph>.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>character vector of input data set variables  needed for the transformation function.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>character vector defining additional R packages  (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>)  to be made available and preloaded for use in variable transformation functions,  e.g., those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions  via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments  or those defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>user-defined environment to serve as a parent to all environments  developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>,  a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data  read from the data source.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Integer values from <ph id="ph1">`1`</ph> to <ph id="ph2">`2`</ph> provide increasing amounts of information are provided.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>a valid <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`RxSpark`</ph> and <ph id="ph2">`RxHadoopMR`</ph> compute contexts distribute the computation among the nodes specified by the compute context; for other compute contexts, the computation is distributed if possible on the local computer.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>integer in the range of -1 to 9 indicating the compression level for the output data  if written to an <ph id="ph1">`.xdf`</ph> file.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the amount of compression -  resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`xdfCompressionLevel`</ph> is set to 0, there will be no compression and  files will be compatible with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression will be used.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Microsoft R Services Compute Engine and to <bpt id="p1">[</bpt>rxExec<ept id="p1">](rxExec.md)</ept> when <ph id="ph1">`scheduleOnce`</ph> is set to <ph id="ph2">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>an object of class <ph id="ph1">`rxDForest`</ph>.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>see plot.default for details.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxDForest`</ph> is a parallel external memory decision forest algorithm targeted for very large data sets.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>It is modeled on the random forest ideas of Leo Breiman and Adele Cutler and the randomForest package of Andy Liaw and Matthew Weiner, using the tree-fitting algorithm introduced in <bpt id="p1">[</bpt>rxDTree<ept id="p1">](rxDTree.md)</ept>.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>In a decision forest, a number of decision trees are fit to bootstrap samples of the original data.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Observations omitted from a given bootstrap sample are termed "out-of-bag" observations.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>For a given observation, the decision forest prediction is determined by the result of sending the observation through all the trees for which it is out-of-bag.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>For classification, the prediction is the class to which a majority assigned the observation, and for regression, the prediction is the mean of the predictions.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>For each tree, the out-of-bag observations are fed through the tree to estimate out-of-bag error estimates.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>The reported out-of-bag error estimates are cumulative (that is, the <bpt id="p1">*</bpt>i<ept id="p1">*</ept>th element represents the out-of-bag error estimate for all trees through the <bpt id="p2">*</bpt>i<ept id="p2">*</ept>th).</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>an object of class <ph id="ph1">`"rxDForest"`</ph>.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>It is a list with the following components, similar to those of class <ph id="ph1">`"randomForest"`</ph>:</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>The number of trees.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>The number of variables tried at each split.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>One of <ph id="ph1">`"class"`</ph> (for classification) or <ph id="ph2">`"anova"`</ph> (for regression).</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>a list containing the entire forest.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>a data frame containing the out-of-bag error estimate.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>For classification forests, this includes the OOB error estimate, which represents the proportion of times the predicted class is  not equal to the true class, and the cumulative number of out-of-bag observations for the forest.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>For   regression forests, this includes the OOB error estimate, which here represents the sum of squared  residuals of the out-of-bag observations divided by the number of out-of-bag observations, the number  of out-of-bag observations, the out-of-bag variance, and the "pseudo-R-Squared", which is 1 minus the quotient of the <ph id="ph1">`oob.err`</ph> and <ph id="ph2">`oob.var`</ph>.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>(classification only) the confusion matrix of the prediction (based  on out-of-bag data).</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>(classification only) The cutoff vector.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>The input parameters passed to the underlying code.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>The input formula.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>The original call to <ph id="ph1">`rxDForest`</ph>.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Like <bpt id="p1">[</bpt>rxDTree<ept id="p1">](rxDTree.md)</ept>, <ph id="ph1">`rxDForest`</ph> requires multiple passes over the data set and the maximum number of passes can be computed as follows:</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>quantile computation:  <ph id="ph1">`1`</ph> pass for computing the quantiles for all continuous variables,</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>recursive partition:  <ph id="ph1">`maxDepth + 1`</ph> passes per tree for building the tree on the entire dataset,</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>out-of-bag prediction:  <ph id="ph1">`1`</ph> pass per tree for computing the out-of-bag error estimates.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxDForest`</ph> uses random streams and RNGs in parallel computation for sampling.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Different threads on different nodes will be using different random streams so that different but equivalent results might be obtained for different number of threads.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>Breiman, L. (2001) Random Forests.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Machine Learning<ept id="p1">*</ept> <bpt id="p2">**</bpt>45(1)<ept id="p2">**</ept>, 5--32.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Liaw, A., and Weiner, M. (2002).</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>Classification and Regression by randomForest.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>R News 2(3), 18--22.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Intel Math Kernel Library, Vector Statistical Library Notes<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>See section <bpt id="p1">**</bpt>Random Streams and RNGs in Parallel Computation<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxDTree<ept id="p1">](rxDTree.md)</ept>, <bpt id="p2">[</bpt>rxPredict.rxDForest<ept id="p2">](rxPredict.rxDForest.md)</ept>, <bpt id="p3">[</bpt>rxDForestUtils<ept id="p3">](rxDForestUtils.md)</ept>, <bpt id="p4">[</bpt>rxRngNewStream<ept id="p4">](rxRng.md)</ept>.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>