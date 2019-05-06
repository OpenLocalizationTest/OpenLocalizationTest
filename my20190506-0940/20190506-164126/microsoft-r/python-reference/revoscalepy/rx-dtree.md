<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-dtree.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750efd55d566d01f2dc8f52f5b9737ba6585d62be39.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">efd55d566d01f2dc8f52f5b9737ba6585d62be39</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-dtree.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_dtree: Fits classification and regression trees (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Fit classification and regression trees on an .xdf file or data frame for small or large data using parallel external memory algorithm.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>learner, tree</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rx_dtree</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Fit classification and regression trees on an .xdf file or data frame for small or large data using parallel external memory algorithm.</source>
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
          <source>output_column_name</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Character string to be used as a column name for the resulting node indices if output_file is not None.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Note that make.names is used on outColName to ensure that the column name is valid.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If the output_file is an RxOdbcData source, dots are first converted to underscores.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Thus, the default outColName becomes “X_rxNode”.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>write_model_vars</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If True, and the output file is different from the input file, variables in the model will be written to the output file in addition to the node numbers.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If variables from the input data set are transformed in the model, the transformed variables will also be written out.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>extra_vars_to_write</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>None or list of strings of additional variables names from the input data or transforms to include in the output_file.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If writeModelVars is True, model variables will be included as well.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>overwrite</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If True, an existing output_file with an existing column named outColName will be overwritten.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>pweights</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Character string specifying the variable of numeric values to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>fweights</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Character string specifying the variable of integer values to use as frequency weights for the observations.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>method</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Character string specifying the splitting method.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Currently, only “class” or “anova” are supported.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The default is “class” if the response is a factor, otherwise “anova”.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>parms</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Optional list with components specifying additional parameters for the “class” splitting method, as follows:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>prior: A vector of prior probabilities.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The priors must be positive and sum to 1.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The default priors are proportional to the data counts.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>loss: A loss matrix, which must have zeros on the diagonal and positive off-diagonal elements.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>By default, the off-diagonal elements are set to 1.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>split: The splitting index, either gini (the default) or information.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>If parms is specified, any of the components can be specified or omitted.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The defaults will be used for missing components.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>cost</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>A vector of non-negative costs, containing one element for each variable in the model.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Defaults to one for all variables.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>When deciding which split to choose, the improvement on splitting on a variable is divided by its cost.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>min_split</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The minimum number of observations that must exist in a node before a split is attempted.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>By default, this is sqrt(num of obs).</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>For non-XDF data sources, as (num of obs) is unknown in advance, it is wisest to specify this argument directly.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>min_bucket</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The minimum number of observations in a terminal node (or leaf).</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>By default, this is min_split/3.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>cp</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Numeric scalar specifying the complexity parameter.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Any split that does not decrease overall lack-of-fit by at least cp is not attempted.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>max_compete</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>The maximum number of competitor splits retained in the output.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>These are useful model diagnostics, as they allow you to compare splits in the output with the alternatives.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>max_surrogate</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The maximum number of surrogate splits retained in the output.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Setting this to 0 can greatly improve the performance of the algorithm; in some cases almost half the computation time is spent in computing surrogate splits.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>use_surrogate</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>An integer specifying how surrogates are to be used in the splitting process: 0: Display-only; observations with a missing value for the primary</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>1: Use surrogates, in order, to split observations missing the primary split variable.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>If all surrogates are missing, the observation is not split.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>2: Use surrogates, in order, to split observations missing the primary split variable.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>If all surrogates are missing or max_surrogate=0, send the observation in the majority direction.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The 0 value corresponds to the behavior of the tree function, and 2 (the default) corresponds to the recommendations of Breiman et al.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>x_val</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>The number of cross-validations to be performed along with the model building.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Currently, 1:x_val is repeated and used to identify the folds.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>If not zero, the cptable component of the resulting model will contain both the mean (xerror) and standard deviation (xstd) of the cross-validation errors, which can be used to select the optimal cost-complexity pruning of the fitted tree.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Set it to zero if external cross-validation will be used to evaluate the fitted model because a value of k increases the compute time to (k+1)-fold over a value of zero.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>surrogate_style</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>An integer controlling selection of a best surrogate.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>The default, 0, instructs the program to use the total number of correct classifications for a potential surrogate, while 1 instructs the program to use the percentage of correct classification over the non-missing values of the surrogate.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Thus, 0 penalizes potential surrogates with a large number of missing values.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>max_depth</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>The maximum depth of any tree node.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>The computations take much longer at greater depth, so lowering max_depth can greatly speed up computation time.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>max_num_bins</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>The maximum number of bins to use to cut numeric data.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>The default is min(1001, max(101, sqrt(num of obs))).</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>For non-XDF data sources, as (num of obs) is unknown in advance, it is wisest to specify this argument directly.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>If set to 0, unit binning will be used instead of cutting.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>max_unordered_levels</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>The maximum number of levels allowed for an unordered factor predictor for multiclass (&gt;2) classification.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>remove_missings</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>If True, rows with missing values are removed and will not be included in the output data.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>compute_obs_node_id</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Bool value or None.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>If True, the tree node IDs for all the observations are computed and returned.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>If None, the IDs are computed for data.frame with less than 1000 observations and are returned as the where component in the fitted rxDTree object.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>use_sparse_cube</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>If True, sparse cube is used.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>find_splits_in_parallel</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>If True, optimal splits for each node are determined using parallelization methods; this will typically speed up computation as the number of nodes on the same level is increased.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>prune_cp</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Optional complexity parameter for pruning.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>If prune_cp &gt; 0, prune.rxDTree is called on the completed tree with the specified prune_cp and the pruned tree is returned.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>This contrasts with the cp parameter that determines which splits are considered in growing the tree.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>The option prune_cp=”auto” causes rxDTree to call the function rxDTreeBestCp on the completed tree, then use its return value as the cp value for prune.rxDTree.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>row_selection</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>transform_objects</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>A dictionary of variables besides the data that are used in the transform function.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>See rx_data_step for examples.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>transform_function</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Name of the function that will be used to modify the data before the model is built.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>The variables used in the transformation function must be specified in transform_objects.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>See rx_data_step for examples.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>transform_variables</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>List of strings of the column names needed for the transform function.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>transform_packages</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Integer value with options: 0: No progress is reported.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>1: The number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>2: Rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>3: Rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Integer value.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>If 0, no additional output is printed.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>If 1, additional summary information is printed.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>A RxComputeContext object for prediction.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>kwargs</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Additional parameters</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>A RxDTreeResults object of dtree model.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`rx_predict`</ph><ept id="p1">](rx-predict.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`rx_predict_rx_dtree`</ph><ept id="p2">](rx-predict-rx-dtree.md)</ept>.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>