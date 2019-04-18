<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-fast-linear.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4a4c86ff7968611f8c7d2c4e0b7e00a654a62ff16.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a4c86ff7968611f8c7d2c4e0b7e00a654a62ff16</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\rx-fast-linear.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_fast_linear: Fast Linear Model - Stochastic Dual Coordinate Ascent</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>A Stochastic Dual Coordinate Ascent (SDCA) optimization trainer for linear binary classification and regression.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>models, linear, SDCA, stochastic, classification, regression</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.rx_fast_linear<ept id="p1">*</ept>: Linear Model with Stochastic Dual Coordinate Ascent</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>A Stochastic Dual Coordinate Ascent (SDCA) optimization trainer for linear binary classification and regression.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rx_fast_linear`</ph> is a trainer based on the Stochastic Dual Coordinate Ascent (SDCA) method, a state-of-the-art optimization technique for convex objective functions.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The algorithm can be scaled for use on large out-of-memory data sets due to a semi-asynchronized implementation that supports multi-threading.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Convergence is underwritten by periodically enforcing synchronization between primal and dual updates in a separate thread.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Several choices of loss functions are also provided.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The SDCA method combines several of the best properties and capabilities of logistic regression and SVM algorithms.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>For more information on SDCA, see the citations in the reference section.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Traditional optimization algorithms, such as stochastic gradient descent (SGD), optimize the empirical loss function directly.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The SDCA chooses a different approach that optimizes the dual problem instead.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The dual loss function is parametrized by per-example weights.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>In each iteration, when a training example from the training data set is read, the corresponding example weight is adjusted so that the dual loss function is optimized with respect to the current example.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>No learning rate is needed by SDCA to determine step size as is required by various gradient descent methods.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rx_fast_linear`</ph> supports binary classification with three types of loss functions currently: Log loss, hinge loss, and smoothed hinge loss.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Linear regression also supports with squared loss function.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Elastic net regularization can be specified by the <ph id="ph1">`l2_weight`</ph> and <ph id="ph2">`l1_weight`</ph> parameters.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Note that the <ph id="ph1">`l2_weight`</ph> has an effect on the rate of convergence.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>In general, the larger the <ph id="ph1">`l2_weight`</ph>, the faster SDCA converges.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Note that <ph id="ph1">`rx_fast_linear`</ph> is a stochastic and streaming optimization algorithm.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The results depend on the order of the training data.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>For reproducible results, it is recommended that one sets <ph id="ph1">`shuffle`</ph> to <ph id="ph2">`False`</ph> and <ph id="ph3">`train_threads`</ph> to <ph id="ph4">`1`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>formula</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The formula described in revoscalepy.rx_formula.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Interaction terms and <ph id="ph1">`F()`</ph> are not currently supported in <bpt id="p1">[</bpt>microsoftml<ept id="p1">](microsoftml-package.md)</ept>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>A data source object or a character string specifying a <bpt id="p1">*</bpt>.xdf<ept id="p1">*</ept> file or a data frame object.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>method</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Specifies the model type with a character string: <ph id="ph1">`"binary"`</ph> for the default binary classification or <ph id="ph2">`"regression"`</ph> for linear regression.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>loss_function</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Specifies the empirical loss function to optimize.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>For binary classification, the following choices are available:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`log_loss`</ph><ept id="p1">](log-loss.md)</ept>: The log-loss.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>This is the default.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`hinge_loss`</ph><ept id="p1">](hinge-loss.md)</ept>: The SVM hinge loss.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Its parameter represents the margin size.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`smooth_hinge_loss`</ph>: The smoothed hinge loss.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Its parameter represents the smoothing constant.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>For linear regression, squared loss <bpt id="p1">[</bpt><ph id="ph1">`squared_loss`</ph><ept id="p1">](squared-loss.md)</ept> is currently supported.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>When this parameter is set to <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, its default value depends on the type of learning:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`log_loss`</ph><ept id="p1">](log-loss.md)</ept> for binary classification.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`squared_loss`</ph><ept id="p1">](squared-loss.md)</ept> for linear regression.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The following example changes the loss_function to <bpt id="p1">[</bpt><ph id="ph1">`hinge_loss`</ph><ept id="p1">](hinge-loss.md)</ept>: <ph id="ph2">`rx_fast_linear(..., loss_function=hinge_loss())`</ph>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>l1_weight</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Specifies the L1 regularization weight.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The value must be either non-negative or <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>None<ept id="p1">*</ept> is specified, the actual value is automatically computed based on data set.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>None<ept id="p1">*</ept> is the default value.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>l2_weight</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Specifies the L2 regularization weight.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>The value must be either non-negative or <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>None<ept id="p1">*</ept> is specified, the actual value is automatically computed based on data set.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>None<ept id="p1">*</ept> is the default value.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>train_threads</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Specifies how many concurrent threads can be used to run the algorithm.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>When this parameter is set to <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, the number of threads used is determined based on the number of logical processors available to the process as well as the sparsity of data.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Set it to <ph id="ph1">`1`</ph> to run the algorithm in a single thread.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>convergence_tolerance</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Specifies the tolerance threshold used as a convergence criterion.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>It must be between 0 and 1.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`0.1`</ph>.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The algorithm is considered to have converged if the relative duality gap, which is the ratio between the duality gap and the primal loss, falls below the specified convergence tolerance.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>max_iterations</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Specifies an upper bound on the number of training iterations.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>This parameter must be positive or <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>None<ept id="p1">*</ept> is specified, the actual value is automatically computed based on data set.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Each iteration requires a complete pass over the training data.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Training terminates after the total number of iterations reaches the specified upper bound or when the loss function converges, whichever happens earlier.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>shuffle</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Specifies whether to shuffle the training data.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Set <ph id="ph1">`True`</ph> to shuffle the data; <ph id="ph2">`False`</ph> not to shuffle.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`True`</ph>.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>SDCA is a stochastic optimization algorithm.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>If shuffling is turned on, the training data is shuffled on each iteration.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>check_frequency</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>The number of iterations after which the loss function is computed and checked to determine whether it has converged.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>The value specified must be a positive integer or <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, the actual value is automatically computed based on data set.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Otherwise, for example, if <ph id="ph1">`checkFrequency = 5`</ph> is specified, then the loss function is computed and convergence is checked every 5 iterations.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>The computation of the loss function requires a separate complete pass over the training data.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>normalize</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Specifies the type of automatic normalization used:</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Auto"`</ph>: if normalization is needed, it is performed automatically.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>This is the default choice.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"No"`</ph>: no normalization is performed.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Yes"`</ph>: normalization is performed.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Warn"`</ph>: if normalization is needed, a warning message is displayed, but normalization is not performed.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Normalization rescales disparate data ranges to a standard scale.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Feature scaling insures the distances between data points are proportional and enables various optimization methods such as gradient descent to converge much faster.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>If normalization is performed, a <ph id="ph1">`MaxMin`</ph> normalizer is used.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>It normalizes values in an interval [a, b] where <ph id="ph1">`-1 &lt;= a &lt;= 0`</ph> and <ph id="ph2">`0 &lt;= b &lt;= 1`</ph> and <ph id="ph3">`b - a = 1`</ph>.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>This normalizer preserves sparsity by mapping zero to zero.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>ml_transforms</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Specifies a list of MicrosoftML transforms to be performed on the data before training or <bpt id="p1">*</bpt>None<ept id="p1">*</ept> if no transforms are to be performed.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt><ph id="ph1">`featurize_text`</ph><ept id="p1">](featurize-text.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`categorical`</ph><ept id="p2">](categorical.md)</ept>, and <bpt id="p3">[</bpt><ph id="ph3">`categorical_hash`</ph><ept id="p3">](categorical-hash.md)</ept>, for transformations that are supported.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>These transformations are performed after any specified Python transformations.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>ml_transform_vars</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Specifies a character vector of variable names to be used in <ph id="ph1">`ml_transforms`</ph> or <bpt id="p1">*</bpt>None<ept id="p1">*</ept> if none are to be used.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>row_selection</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Specifies the rows (observations) from the data set that are to be used by the model with the name of a logical variable from the data set (in quotes) or with a logical expression using variables in the data set.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`row_selection = "old"`</ph> will only use observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`True`</ph>.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`row_selection = (age &gt; 20) &amp; (age &lt; 65) &amp; (log(income) &gt; 10)`</ph> only uses observations in which the value of the <ph id="ph2">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph3">`log`</ph> of the <ph id="ph4">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transform_function`</ph>).</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`row_selection`</ph> can be defined outside of the function call using the <ph id="ph2">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>transforms</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>An expression of the form that represents the first round of variable transformations.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`row_selection`</ph>) can be defined outside of the function call using the <ph id="ph3">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>transform_objects</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>A named list that contains objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transform_function`</ph>, and <ph id="ph3">`row_selection`</ph>.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>transform_function</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>The variable transformation function.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>transform_variables</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>A character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>transform_packages</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>A character vector specifying additional Python packages (outside of those specified in <ph id="ph1">`RxOptions.get_option("transform_packages")`</ph>) to be made available and preloaded for use in variable transformation functions.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>For example, those explicitly defined in <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../revoscalepy/revoscalepy-package.md)</ept> functions via their <ph id="ph1">`transforms`</ph> and <ph id="ph2">`transform_function`</ph> arguments or those defined implicitly via their <ph id="ph3">`formula`</ph> or <ph id="ph4">`row_selection`</ph> arguments.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transform_packages`</ph> argument may also be <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, indicating that no packages outside <ph id="ph2">`RxOptions.get_option("transform_packages")`</ph> are preloaded.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>transform_environment</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>A user-defined environment to serve as a parent to all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transform_environment = None`</ph>, a new “hash” environment with parent revoscalepy.baseenv is used instead.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Specifies the number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the level of reporting on the row processing progress:</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the amount of output wanted.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Integer values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Sets the context in which computations are executed, specified with a valid revoscalepy.RxComputeContext.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Currently local and <bpt id="p1">[</bpt>revoscalepy.RxInSqlServer<ept id="p1">](../revoscalepy/RxInSqlServer.md)</ept> compute contexts are supported.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>ensemble</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Control parameters for ensembling.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt><ph id="ph1">`FastLinear`</ph><ept id="p1">](learners-object.md)</ept> object with the trained model.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>This algorithm is multi-threaded and will not attempt to load the entire dataset into memory.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`hinge_loss`</ph><ept id="p1">](hinge-loss.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`log_loss`</ph><ept id="p2">](log-loss.md)</ept>, <bpt id="p3">[</bpt><ph id="ph3">`smoothed_hinge_loss`</ph><ept id="p3">](smoothed-hinge-loss.md)</ept>, <bpt id="p4">[</bpt><ph id="ph4">`squared_loss`</ph><ept id="p4">](squared-loss.md)</ept>, <bpt id="p5">[</bpt><ph id="ph5">`rx_predict`</ph><ept id="p5">](rx-predict.md)</ept></source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Scaling Up Stochastic Dual Coordinate Ascent<ept id="p1">](https://research.microsoft.com/en-us/um/people/mbilenko/papers/15-sasdca.pdf)</ept></source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Stochastic Dual Coordinate Ascent Methods for Regularized Loss Minimization<ept id="p1">](http://www.jmlr.org/papers/volume14/shalev-shwartz13a/shalev-shwartz13a.pdf)</ept></source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>loss functions</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><bpt id="p2">*</bpt>microsoftml.hinge_loss<ept id="p2">*</ept>: Hinge loss function<ept id="p1">](hinge-loss.md)</ept></source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><bpt id="p2">*</bpt>microsoftml.log_loss<ept id="p2">*</ept>: Log loss function<ept id="p1">](log-loss.md)</ept></source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><bpt id="p2">*</bpt>microsoftml.smoothed_hinge_loss<ept id="p2">*</ept>: Smoothed hinge loss function<ept id="p1">](smoothed-hinge-loss.md)</ept></source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><bpt id="p2">*</bpt>microsoftml.squared_loss<ept id="p2">*</ept>: Squared loss function<ept id="p1">](squared-loss.md)</ept></source>
        </trans-unit></group></body></file></xliff>