<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-fast-trees.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca863752255648fc3a4572e6d325f1c2920a5b8d1631.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">3752255648fc3a4572e6d325f1c2920a5b8d1631</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\rx-fast-trees.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_fast_trees: Fast Tree</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Machine Learning Fast Tree</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>models, classification, regression</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.rx_fast_trees<ept id="p1">*</ept>: Boosted Trees</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Machine Learning Fast Tree</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>rx_fast_trees is an implementation of FastRank.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>FastRank is an efficient implementation of the MART gradient boosting algorithm.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Gradient boosting is a machine learning technique for regression problems.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>It builds each regression tree in a step-wise fashion, using a predefined loss function to measure the error for each step and corrects for it in the next.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>So this prediction model is actually an ensemble of weaker prediction models.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>In regression problems, boosting builds a series of such trees in a step-wise fashion and then selects the optimal tree using an arbitrary differentiable loss function.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>MART learns an ensemble of regression trees, which is a decision tree with scalar values in its leaves.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>A decision (or regression) tree is a binary tree-like flow chart, where at each interior node one decides which of the two child nodes to continue to based on one of the feature values from the input.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>At each leaf node, a value is returned.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>In the interior nodes, the decision is based on the test <ph id="ph1">`"x &lt;= v"`</ph>, where <ph id="ph2">`x`</ph> is the value of the feature in the input sample and <ph id="ph3">`v`</ph> is one of the possible values of this feature.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The functions that can be produced by a regression tree are all the piece-wise constant functions.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The ensemble of trees is produced by computing, in each step, a regression tree that approximates the gradient of the loss function, and adding it to the previous tree with coefficients that minimize the loss of the new tree.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The output of the ensemble produced by MART on a given instance is the sum of the tree outputs.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>In case of a binary classification problem, the output is converted to a probability by using some form of calibration.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>In case of a regression problem, the output is the predicted value of the function.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>In case of a ranking problem, the instances are ordered by the output value of the ensemble.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`method`</ph> is set to <ph id="ph2">`"regression"`</ph>, a regression version of FastTree is used.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If set to <ph id="ph1">`"ranking"`</ph>, a ranking version of FastTree is used.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>In the ranking case, the instances should be ordered by the output of the tree ensemble.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The only difference in the settings of these versions is in the calibration settings, which are needed only for classification.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>formula</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The formula as described in revoscalepy.rx_formula.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Interaction terms and <ph id="ph1">`F()`</ph> are not currently supported in <bpt id="p1">[</bpt>microsoftml<ept id="p1">](microsoftml-package.md)</ept>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>A data source object or a character string specifying a <bpt id="p1">*</bpt>.xdf<ept id="p1">*</ept> file or a data frame object.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>method</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>A character string that specifies the type of Fast Tree: <ph id="ph1">`"binary"`</ph> for the default Fast Tree Binary Classification or <ph id="ph2">`"regression"`</ph> for Fast Tree Regression.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>num_trees</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Specifies the total number of decision trees to create in the ensemble.By creating more decision trees, you can potentially get better coverage, but the training time increases.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The default value is 100.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>num_leaves</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The maximum number of leaves (terminal nodes) that can be created in any tree.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Higher values potentially increase the size of the tree and get better precision, but risk overfitting and requiring longer training times.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The default value is 20.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>learning_rate</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Determines the size of the step taken in the direction of the gradient in each step of the learning process.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>This determines how fast or slow the learner converges on the optimal solution.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If the step size is too big, you might overshoot the optimal solution.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If the step size is too small, training takes longer to converge to the best solution.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>min_split</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Minimum number of training instances required to form a leaf.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>That is, the minimal number of documents allowed in a leaf of a regression tree, out of the sub-sampled data.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>A ‘split’ means that features in each level of the tree (node) are randomly divided.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The default value is</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Only the number of instances is counted even if instances are weighted.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>example_fraction</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The fraction of randomly chosen instances to use for each tree.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>The default value is 0.7.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>feature_fraction</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>The fraction of randomly chosen features to use for each tree.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The default value is 1.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>split_fraction</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The fraction of randomly chosen features to use on each split.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>The default value is 1.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>num_bins</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Maximum number of distinct values (bins) per feature.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>If the feature has fewer values than the number indicated, each value is placed in its own bin.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>If there are more values, the algorithm creates <ph id="ph1">`numBins`</ph> bins.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>first_use_penalty</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The feature first use penalty coefficient.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>This is a form of regularization that incurs a penalty for using a new feature when creating the tree.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Increase this value to create trees that don’t use many features.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>The default value is 0.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>gain_conf_level</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Tree fitting gain confidence requirement (should be in the range [0,1)).</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>The default value is 0.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>unbalanced_sets</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`True`</ph>, derivatives optimized for unbalanced sets are used.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Only applicable when <ph id="ph1">`type`</ph> equal to <ph id="ph2">`"binary"`</ph>.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`False`</ph>.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>train_threads</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>The number of threads to use in training.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>The default value is 8.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>random_seed</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Specifies the random seed.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>ml_transforms</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Specifies a list of MicrosoftML transforms to be performed on the data before training or <bpt id="p1">*</bpt>None<ept id="p1">*</ept> if no transforms are to be performed.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt><ph id="ph1">`featurize_text`</ph><ept id="p1">](featurize-text.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`categorical`</ph><ept id="p2">](categorical.md)</ept>, and <bpt id="p3">[</bpt><ph id="ph3">`categorical_hash`</ph><ept id="p3">](categorical-hash.md)</ept>, for transformations that are supported.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>These transformations are performed after any specified Python transformations.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>ml_transform_vars</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Specifies a character vector of variable names to be used in <ph id="ph1">`ml_transforms`</ph> or <bpt id="p1">*</bpt>None<ept id="p1">*</ept> if none are to be used.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>row_selection</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Specifies the rows (observations) from the data set that are to be used by the model with the name of a logical variable from the data set (in quotes) or with a logical expression using variables in the data set.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>will only use observations in which the value of the variable <ph id="ph1">`old`</ph> is <ph id="ph2">`True`</ph>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>only uses observations in which the value of the <ph id="ph1">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph2">`log`</ph> of the <ph id="ph3">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transform_function`</ph>).</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`row_selection`</ph> can be defined outside of the function call using the <ph id="ph2">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>transforms</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>An expression of the form  that represents the first round of variable transformations.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`row_selection`</ph>) can be defined outside of the function call using the <ph id="ph3">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>transform_objects</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>A named list that contains objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transform_function`</ph>, and <ph id="ph3">`row_selection`</ph>.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>transform_function</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>The variable transformation function.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>transform_variables</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>A character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>transform_packages</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>A character vector specifying additional Python packages (outside of those specified in <ph id="ph1">`RxOptions.get_option("transform_packages")`</ph>) to be made available and preloaded for use in variable transformation functions.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>For example, those explicitly defined in <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../revoscalepy/revoscalepy-package.md)</ept> functions via their <ph id="ph1">`transforms`</ph> and <ph id="ph2">`transform_function`</ph> arguments or those defined implicitly via their <ph id="ph3">`formula`</ph> or <ph id="ph4">`row_selection`</ph> arguments.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transform_packages`</ph> argument may also be <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, indicating that no packages outside <ph id="ph2">`RxOptions.get_option("transform_packages")`</ph> are preloaded.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>transform_environment</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>A user-defined environment to serve as a parent to all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transform_environment = None`</ph>, a new “hash” environment with parent revoscalepy.baseenv is used instead.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Specifies the number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the level of reporting on the row processing progress:</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the amount of output wanted.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Integer values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Sets the context in which computations are executed, specified with a valid revoscalepy.RxComputeContext.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Currently local and <bpt id="p1">[</bpt>revoscalepy.RxInSqlServer<ept id="p1">](../revoscalepy/RxInSqlServer.md)</ept> compute contexts are supported.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>ensemble</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Control parameters for ensembling.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt><ph id="ph1">`FastTrees`</ph><ept id="p1">](learners-object.md)</ept> object with the trained model.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>This algorithm is multi-threaded and will always attempt to load the entire dataset into memory.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`rx_fast_forest`</ph><ept id="p1">](rx-fast-forest.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`rx_predict`</ph><ept id="p2">](rx-predict.md)</ept></source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Wikipedia: Gradient boosting (Gradient tree boosting)</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Greedy function approximation: A gradient boosting machine.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit></group></body></file></xliff>