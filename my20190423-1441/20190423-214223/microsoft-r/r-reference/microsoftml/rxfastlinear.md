<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxfastlinear.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca861ca7c2bb615d8b37c2f6466ed2e629eb31478466.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1ca7c2bb615d8b37c2f6466ed2e629eb31478466</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\rxfastlinear.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxFastLinear function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>A Stochastic Dual Coordinate Ascent (SDCA) optimization trainer  for linear binary classification and regression.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxFastLinear is a trainer based on the Stochastic Dual Coordinate Ascent (SDCA) method, a state-of-the-art optimization technique for convex objective functions.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>The algorithm can be scaled for use on large out-of-memory data  sets due to a semi-asynchronized implementation that supports multi-threading.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>primal and dual updates in a separate thread.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Several choices of loss functions are also provided.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>The SDCA method combines several of the  best properties and capabilities of logistic regression and SVM algorithms.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>For more information on SDCA, see the citations in the reference section.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Traditional optimization algorithms, such as stochastic gradient descent  (SGD), optimize the empirical loss function directly.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>The SDCA chooses a different approach that optimizes the dual problem instead.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>The dual loss function is parametrized by per-example weights.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>In each iteration, when a training example from the training data set is read, the corresponding example weight is adjusted so that the dual loss function is optimized with respect to the current example.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>No learning rate is needed by SDCA to  determine step size as is required by various gradient descent methods.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxFastLinear supports binary classification with three types of loss functions currently: Log loss, hinge loss, and smoothed hinge loss.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Linear regression also supports with squared loss function.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Elastic net regularization can be specified by the l2Weight and l1Weight parameters.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Note that the l2Weight has an effect on the rate of convergence.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>In general, the larger the l2Weight, the faster  SDCA converges.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Note that rxFastLinear is a stochastic and streaming optimization algorithm.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>The results depends on the order of the training data.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>For reproducible results, it is recommended that one sets shuffle to FALSE and trainThreads to 1.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), rxFastLinear, classification, fast, linear, regression, sdca, stochastic</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>rxFastLinear: Fast Linear Model -- Stochastic Dual Coordinate Ascent</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>A Stochastic Dual Coordinate Ascent (SDCA) optimization trainer for linear binary classification and regression.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>is a trainer based on the Stochastic Dual Coordinate Ascent (SDCA) method, a state-of-the-art optimization technique for convex objective functions.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The algorithm can be scaled for use on large out-of-memory data sets due to a semi-asynchronized implementation that supports multi-threading.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>primal and dual updates in a separate thread.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Several choices of loss functions are also provided.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The SDCA method combines several of the best properties and capabilities of logistic regression and SVM algorithms.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>For more information on SDCA, see the citations in the reference section.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Traditional optimization algorithms, such as stochastic gradient descent (SGD), optimize the empirical loss function directly.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The SDCA chooses a different approach that optimizes the dual problem instead.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The dual loss function is parametrized by per-example weights.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>In each iteration, when a training example from the training data set is read, the corresponding example weight is adjusted so that the dual loss function is optimized with respect to the current example.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>No learning rate is needed by SDCA to determine step size as is required by various gradient descent methods.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>supports binary classification with three types of loss functions currently: Log loss, hinge loss, and smoothed hinge loss.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Linear regression also supports with squared loss function.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Elastic net regularization can be specified by the <ph id="ph1">`l2Weight`</ph> and <ph id="ph2">`l1Weight`</ph> parameters.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Note that the <ph id="ph1">`l2Weight`</ph> has an effect on the rate of convergence.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>In general, the larger the <ph id="ph1">`l2Weight`</ph>, the faster SDCA converges.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Note that <ph id="ph1">`rxFastLinear`</ph> is a stochastic and streaming optimization algorithm.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The result depends on the order of the training data.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>For reproducible results, it is recommended that one sets <ph id="ph1">`shuffle`</ph> to <ph id="ph2">`FALSE`</ph> and <ph id="ph3">`trainThreads`</ph> to <ph id="ph4">`1`</ph>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The formula described in rxFormula.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Interaction terms and <ph id="ph1">`F()`</ph> are currently not supported in <bpt id="p1">**</bpt>MicrosoftML<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>A data source object or a character string specifying a .xdf file or a data frame object.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Specifies the model type with a character string: <ph id="ph1">`"binary"`</ph> for the default binary classification or <ph id="ph2">`"regression"`</ph> for linear  regression.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Specifies the empirical loss function to optimize.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>For binary classification, the following choices are available:</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>logLoss<ept id="p1">](loss.md)</ept>: The log-loss.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>This is the default.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>hingeLoss<ept id="p1">](loss.md)</ept>: The SVM hinge loss.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Its parameter represents the margin size.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>smoothHingeLoss<ept id="p1">](loss.md)</ept>: The smoothed hinge loss.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Its parameter represents the smoothing constant.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>For linear regression, squared loss <bpt id="p1">[</bpt>squaredLoss<ept id="p1">](loss.md)</ept> is currently supported.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>When this parameter is set to <ph id="ph1">`NULL`</ph>, its default value depends on the type of learning:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>logLoss<ept id="p1">](loss.md)</ept> for binary classification.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>squaredLoss<ept id="p1">](loss.md)</ept> for linear regression.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Specifies the L2 regularization weight.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>The value must be either non-negative or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> is specified, the  actual value is automatically computed based on data set.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>is the default value.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Specifies the L1 regularization weight.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The value must be either non-negative or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> is specified, the  actual value is automatically computed based on data set.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>is the default value.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Specifies how many concurrent threads can be used to run the algorithm.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>When this parameter is set to <ph id="ph1">`NULL`</ph>, the number of threads used is determined based on the number of logical processors available to the process as well as the sparsity of data.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Set it to <ph id="ph1">`1`</ph> to run the algorithm in a single thread.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Specifies the tolerance threshold used as a  convergence criterion.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>It must be between 0 and 1.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`0.1`</ph>.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The algorithm is considered to have converged if the relative  duality gap, which is the ratio between the duality gap and the primal loss,  falls below the specified convergence tolerance.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Specifies an upper bound on the number of training iterations.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>This parameter must be positive or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> is specified, the actual value is automatically computed based on data set.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Each iteration requires a complete pass over the training data.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Training  terminates after the total number of iterations reaches the specified   upper bound or when the loss function converges, whichever happens earlier.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Specifies whether to shuffle the training data.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Set <ph id="ph1">`TRUE`</ph> to shuffle the data; <ph id="ph2">`FALSE`</ph> not to shuffle.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>SDCA is a stochastic optimization algorithm.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>If shuffling is turned on, the training data is shuffled on each iteration.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>The number of iterations after which the loss function is computed and checked to determine whether it has converged.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>The value  specified must be a positive integer or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the actual value is automatically computed based on data set.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Otherwise,  for example, if <ph id="ph1">`checkFrequency = 5`</ph> is specified, then the loss function is computed and convergence is checked every 5 iterations.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>The computation of the loss function requires a separate complete pass over the training data.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Specifies the type of automatic normalization used:</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>: if normalization is needed, it is automatically  performed.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>This is the default value.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>: no normalization is performed.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>: normalization is performed.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>: if normalization is needed, a warning message is   displayed, but normalization is not performed.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Normalization rescales disparate data ranges to a standard scale.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Feature scaling insures the distances between data points are proportional and  enables various optimization methods such as gradient descent to converge  much faster.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>If normalization is performed, a <ph id="ph1">`MaxMin`</ph> normalizer is  used.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>It normalizes values in an interval [a, b] where <ph id="ph1">`-1 &lt;= a &lt;= 0`</ph>and <ph id="ph2">`0 &lt;= b &lt;= 1`</ph> and <ph id="ph3">`b - a = 1`</ph>.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>This normalizer preserves  sparsity by mapping zero to zero.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Specifies a list of MicrosoftML transforms to be performed on the data before training or <ph id="ph1">`NULL`</ph> if no transforms are  to be performed.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>featurizeText<ept id="p1">](featurizeText.md)</ept>, <bpt id="p2">[</bpt>categorical<ept id="p2">](categorical.md)</ept>, and <bpt id="p3">[</bpt>categoricalHash<ept id="p3">](categoricalHash.md)</ept>, for transformations that are supported.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>These transformations are performed after any specified R transformations.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Specifies a character vector of variable names to be used in <ph id="ph1">`mlTransforms`</ph> or <ph id="ph2">`NULL`</ph> if none are to be used.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Specifies the rows (observations) from the data set that are to be used by the model with the name of a logical variable from the  data set (in quotes) or with a logical expression using variables in the    data set.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will only use observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>only uses observations in which the value of the <ph id="ph1">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph2">`log`</ph> of the <ph id="ph3">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>An expression of the form <ph id="ph1">`list(name = expression, ``...)`</ph> that represents the first round of variable transformations.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>As with  all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>) can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>A named list that contains objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>The variable transformation function.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>See rxTransform for details.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>A character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>See rxTransform for details.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>A character vector specifying additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and preloaded for use in variable transformation functions.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>For example, those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph1">`transforms`</ph> and <ph id="ph2">`transformFunc`</ph> arguments or those defined implicitly via their <ph id="ph3">`formula`</ph> or <ph id="ph4">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>, indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> are preloaded.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>A user-defined environment to serve as a parent to all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Specifies the number of blocks to read for each chunk  of data read from the data source.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the level of reporting on the row processing progress:</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the amount of output wanted.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Integer  values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Sets the context in which computations are executed, specified with a valid RxComputeContext.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Currently local and RxInSqlServer compute contexts are supported.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Control parameters for ensembling.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed directly to the Microsoft Compute Engine.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>: A <ph id="ph1">`rxFastLinear`</ph> object with the trained model.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`FastLinear`</ph>: A learner specification object of class <ph id="ph2">`maml`</ph> for the Fast Linear trainer.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>This algorithm is multi-threaded and will not attempt to load the entire dataset into memory.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>logLoss<ept id="p1">](loss.md)</ept>, <bpt id="p2">[</bpt>hingeLoss<ept id="p2">](loss.md)</ept>, <bpt id="p3">[</bpt>smoothHingeLoss<ept id="p3">](loss.md)</ept>, <bpt id="p4">[</bpt>squaredLoss<ept id="p4">](loss.md)</ept>, <bpt id="p5">[</bpt>rxFastTrees<ept id="p5">](rxFastTrees.md)</ept>, <bpt id="p6">[</bpt>rxFastForest<ept id="p6">](rxFastForest.md)</ept>, <bpt id="p7">[</bpt>rxLogisticRegression<ept id="p7">](rxLogisticRegression.md)</ept>, <bpt id="p8">[</bpt>rxNeuralNet<ept id="p8">](rxNeuralNet.md)</ept>, <bpt id="p9">[</bpt>rxOneClassSvm<ept id="p9">](rxOneClassSvm.md)</ept>, <bpt id="p10">[</bpt>featurizeText<ept id="p10">](featurizeText.md)</ept>, <bpt id="p11">[</bpt>categorical<ept id="p11">](categorical.md)</ept>, <bpt id="p12">[</bpt>categoricalHash<ept id="p12">](categoricalHash.md)</ept>, <bpt id="p13">[</bpt>rxPredict.mlModel<ept id="p13">](rxPredict.md)</ept>.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>