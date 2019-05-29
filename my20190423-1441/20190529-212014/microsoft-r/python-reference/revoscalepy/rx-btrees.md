<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-btrees.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3536bb7d1c96721a52630700e5af018744c5e0965.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">536bb7d1c96721a52630700e5af018744c5e0965</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-btrees.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_btrees: Fits stochastic gradient boosted decision trees (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Fit stochastic gradient boosted decision trees on an .xdf file or data frame for small or large data using parallel external memory algorithm.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>learner, tree</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rx_btrees</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Fit stochastic gradient boosted decision trees on an .xdf file or data frame for small or large data using parallel external memory algorithm.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>formula</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Statistical model using symbolic formulas.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Either a data source object, a character string specifying a ‘.xdf’ file, or a data frame object.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If a Spark compute context is being used, this argument may also be an RxHiveData, RxOrcData, RxParquetData or RxSparkDataFrame object or a Spark data frame object from pyspark.sql.DataFrame.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>output_file</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Either an RxXdfData data source object or a character string specifying the ‘.xdf’ file for storing the resulting node indices.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If None, then no node indices are stored to disk.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If the input data is a data frame, the node indices are returned automatically.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>write_model_vars</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If True, and the output file is different from the input file, variables in the model will be written to the output file in addition to the node numbers.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If variables from the input data set are transformed in the model, the transformed variables will also be written out.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>overwrite</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If True, an existing output_file with an existing column named outColName will be overwritten.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>pweights</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Character string specifying the variable of numeric values to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>fweights</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Character string specifying the variable of integer values to use as frequency weights for the observations.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>method</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Character string specifying the splitting method.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Currently, only “class” or “anova” are supported.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The default is “class” if the response is a factor, otherwise “anova”.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>parms</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Optional list with components specifying additional parameters for the “class” splitting method, as follows:</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>prior: A vector of prior probabilities.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The priors must be positive and sum to 1.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The default priors are proportional to the data counts.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>loss: A loss matrix, which must have zeros on the diagonal and positive off-diagonal elements.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>By default, the off-diagonal elements are set to 1.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>split: The splitting index, either gini (the default) or information.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If parms is specified, any of the components can be specified or omitted.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The defaults will be used for missing components.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>cost</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>A vector of non-negative costs, containing one element for each variable in the model.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Defaults to one for all variables.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>When deciding which split: to choose, the improvement on splitting on a variable is divided by its cost.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>min_split</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The minimum number of observations that must exist in a node before a split is attempted.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>By default, this is sqrt(num of obs).</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>For non-XDF data sources, as (num of obs) is unknown in advance, it is wisest to specify this argument directly.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>min_bucket</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The minimum number of observations in a terminal node (or leaf).</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>By default, this is min_split/3.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>cp</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Numeric scalar specifying the complexity parameter.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Any split that does not decrease overall lack-of-fit by at least cp is not attempted.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>max_compete</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The maximum number of competitor splits retained in the output.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>These are useful model diagnostics, as they allow you to compare splits in the output with the alternatives.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>max_surrogate</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The maximum number of surrogate splits retained in the output.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>See the Details for a description of how surrogate splits are used in the model fitting.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Setting this to 0 can greatly improve the performance of the algorithm; in some cases almost half the computation time is spent in computing surrogate splits.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>use_surrogate</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>An integer specifying how surrogates are to be used in the splitting process: 0: Display-only; observations with a missing value for the primary</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>1: Use surrogates, in order, to split observations missing the primary split variable.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>If all surrogates are missing, the observation is not split.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>2: Use surrogates, in order, to split observations missing the primary split variable.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>If all surrogates are missing or max_surrogate=0, send the observation in the majority direction.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The 0 value corresponds to the behavior of the tree function, and 2 (the default) corresponds to the recommendations of Breiman et al.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>surrogate_style</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>An integer controlling selection of a best surrogate.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>The default, 0, instructs the program to use the total number of correct classifications for a potential surrogate, while 1 instructs the program to use the percentage of correct classification over the non-missing values of the surrogate.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Thus, 0 penalizes potential surrogates with a large number of missing values.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>n_tree</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>A positive integer specifying the number of trees to grow.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>m_try</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>A positive integer specifying the number of variables to sample as split candidates at each tree node.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>The default values are sqrt(num of vars) for classification and (num of vars)/3 for regression.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>replace</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>A bool value specifying if the sampling of observations should be done with or without replacement.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>cutoff</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>(Classification only) A vector of length equal to the number of classes specifying the dividing factors for the class votes.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>The default is 1/(num of classes).</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>strata</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>A character string specifying the (factor) variable to use for stratified sampling.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>sample_rate</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>A scalar or a vector of positive values specifying the percentage(s) of observations to sample for each tree: for unstratified sampling: A scalar of positive value specifying the</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>for stratified sampling: A vector of positive values of length equal to the number of strata specifying the percentages of observations to sample from the strata for each tree.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>importance</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>A bool value specifying if the importance of predictors should be assessed.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>seed</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>An integer that will be used to initialize the random number generator.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>The default is random.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>For reproducibility, you can specify the random seed either using set.seed or by setting this seed argument as part of your call.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>compute_oob_error</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>An integer specifying whether and how to compute the prediction error for out-of-bag samples: &lt;0: never.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>This option may reduce the computation time.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>=0: only once for the entire forest.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>0: once for each addition of a tree.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>This is the default.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>loss_function</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Character string specifying the name of the loss function to use.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>The following options are currently supported: “gaussian”: Regression: for numeric responses.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>“bernoulli”: Regression: for 0-1 responses.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>“multinomial”: Classification: for categorical responses with two or more levels.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>learning_rate</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Numeric scalar specifying the learning rate of the boosting procedure.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>max_num_bins</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>The maximum number of bins to use to cut numeric data.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>The default is min(1001, max(101, sqrt(num of obs))).</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>For non-XDF data sources, as (num of obs) is unknown in advance, it is wisest to specify this argument directly.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>If set to 0, unit binning will be used instead of cutting.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>See the ‘Details’ section for more information.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>max_unordered_levels</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>The maximum number of levels allowed for an unordered factor predictor for multiclass (&gt;2) classification.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>remove_missings</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>If True, rows with missing values are removed and will not be included in the output data.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>use_sparse_cube</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>If True, sparse cube is used.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>find_splits_in_parallel</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>bool value.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>If True, optimal splits for each node are determined using parallelization methods; this will typically speed up computation as the number of nodes on the same level is increased.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>row_selection</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>transforms</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>transform_objects</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>transform_function</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Variable transformation function.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>The variables used in the transformation function must be specified in transform_variables if they are not variables used in the model.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>transform_variables</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>List of strings of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>transform_packages</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>integer value with options: 0: No progress is reported.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>1: The number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>2: Rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>3: Rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Integer value.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>If 0, no additional output is printed.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>If 1, additional summary information is printed.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>A RxComputeContext object for prediction.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>kwargs</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Additional parameters</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>A RxDForestResults object of dtree model.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`rx_predict`</ph><ept id="p1">](rx-predict.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`rx_predict_rx_dforest`</ph><ept id="p2">](rx-predict-rx-dforest.md)</ept>.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>