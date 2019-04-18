<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-logistic-regression.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef06906733552581a5a7b3cf07dfc19ba62892a3e75114f1faa.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">52581a5a7b3cf07dfc19ba62892a3e75114f1faa</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\rx-logistic-regression.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_logistic_regression: Logistic Regression</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Machine Learning Logistic Regression</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>models, classification</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.rx_logistic_regression<ept id="p1">*</ept>: Logistic Regression</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Machine Learning Logistic Regression</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Logistic Regression is a classification method used to predict the value of a categorical dependent variable from its relationship to one or more independent variables assumed to have a logistic distribution.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If the dependent variable has only two possible values (success/failure), then the logistic regression is binary.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If the dependent variable has more than two possible values (blood type given diagnostic test results), then the logistic regression is multinomial.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The optimization technique used for <ph id="ph1">`rx_logistic_regression`</ph> is the limited memory Broyden-Fletcher-Goldfarb-Shanno (L-BFGS).</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Both the L-BFGS and regular BFGS algorithms use quasi-Newtonian methods to estimate the computationally intensive Hessian matrix in the equation used by Newton’s method to calculate steps.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>But the L-BFGS approximation uses only a limited amount of memory to compute the next step direction, so that it is especially suited for problems with a large number of variables.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`memory_size`</ph> parameter specifies the number of past positions and gradients to store for use in the computation of the next step.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>This learner can use elastic net regularization: a linear combination of L1 (lasso) and L2 (ridge) regularizations.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Regularization is a method that can render an ill-posed problem more tractable by imposing constraints that provide information to supplement the data and that prevents overfitting by penalizing models with extreme coefficient values.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>This can improve the generalization of the model learned by selecting the optimal complexity in the bias-variance tradeoff.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Regularization works by adding the penalty that is associated with coefficient values to the error of the hypothesis.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>An accurate model with extreme coefficient values would be penalized more, but a less accurate model with more conservative values would be penalized less.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>L1 and L2 regularization have different effects and uses that are complementary in certain respects.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`l1_weight`</ph>: can be applied to sparse models, when working with high-dimensional data.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>It pulls small weights associated features that are relatively unimportant towards 0.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`l2_weight`</ph>: is preferable for data that is not sparse.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>It pulls large weights towards zero.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Adding the ridge penalty to the regularization overcomes some of lasso’s limitations.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>It can improve its predictive accuracy, for example, when the number of predictors is greater than the sample size.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`x = l1_weight`</ph> and <ph id="ph2">`y = l2_weight`</ph>, <ph id="ph3">`ax + by = c`</ph> defines the linear span of the regularization terms.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The default values of x and y are both <ph id="ph1">`1`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>An aggressive regularization can harm predictive capacity by excluding important variables out of the model.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>So choosing the optimal values for the regularization parameters is important for the performance of the logistic regression model.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>formula</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The formula as described in revoscalepy.rx_formula Interaction terms and <ph id="ph1">`F()`</ph> are not currently supported in <bpt id="p1">[</bpt>microsoftml<ept id="p1">](microsoftml-package.md)</ept>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>A data source object or a character string specifying a <bpt id="p1">*</bpt>.xdf<ept id="p1">*</ept> file or a data frame object.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>method</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>A character string that specifies the type of Logistic Regression: <ph id="ph1">`"binary"`</ph> for the default binary classification logistic regression or <ph id="ph2">`"multiClass"`</ph> for multinomial logistic regression.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>l2_weight</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The L2 regularization weight.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Its value must be greater than or equal to <ph id="ph1">`0`</ph> and the default value is set to <ph id="ph2">`1`</ph>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>l1_weight</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The L1 regularization weight.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Its value must be greater than or equal to <ph id="ph1">`0`</ph> and the default value is set to <ph id="ph2">`1`</ph>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>opt_tol</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Threshold value for optimizer convergence.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If the improvement between iterations is less than the threshold, the algorithm stops and returns the current model.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Smaller values are slower, but more accurate.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`1e-07`</ph>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>memory_size</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Memory size for L-BFGS, specifying the number of past positions and gradients to store for the computation of the next step.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>This optimization parameter limits the amount of memory that is used to compute the magnitude and direction of the next step.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>When you specify less memory, training is faster but less accurate.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Must be greater than or equal to <ph id="ph1">`1`</ph> and the default value is <ph id="ph2">`20`</ph>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>max_iterations</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Sets the maximum number of iterations.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>After this number of steps, the algorithm stops even if it has not satisfied convergence criteria.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>show_training_stats</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Specify <ph id="ph1">`True`</ph> to show the statistics of training data and the trained model; otherwise, <ph id="ph2">`False`</ph>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`False`</ph>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>For additional information about model statistics, see <ph id="ph1">`summary.ml_model()`</ph>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>sgd_init_tol</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Set to a number greater than 0 to use Stochastic Gradient Descent (SGD) to find the initial parameters.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>A non-zero value set specifies the tolerance SGD uses to determine convergence.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`0`</ph> specifying that SGD is not used.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>init_wts_diameter</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Sets the initial weights diameter that specifies the range from which values are drawn for the initial weights.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>These weights are initialized randomly from within this range.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>For example, if the diameter is specified to be <ph id="ph1">`d`</ph>, then the weights are uniformly distributed between <ph id="ph2">`-d/2`</ph> and <ph id="ph3">`d/2`</ph>.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`0`</ph>, which specifies that all the  weights are initialized to <ph id="ph2">`0`</ph>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>train_threads</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>The number of threads to use in training the model.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>This should be set to the number of cores on the machine.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Note that L-BFGS multi-threading attempts to load dataset into memory.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>In case of out-of-memory issues, set <ph id="ph1">`train_threads`</ph> to <ph id="ph2">`1`</ph> to turn off multi-threading.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>None<ept id="p1">*</ept> the number of threads to use is determined internally.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>dense_optimizer</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`True`</ph>, forces densification of the internal optimization vectors.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`False`</ph>, enables the logistic regression optimizer use sparse or dense internal states as it finds appropriate.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Setting <ph id="ph1">`denseOptimizer`</ph> to <ph id="ph2">`True`</ph> requires the internal optimizer to use a dense internal state, which may help alleviate load on the garbage collector for some varieties of larger problems.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>normalize</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Specifies the type of automatic normalization used:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Auto"`</ph>: if normalization is needed, it is performed automatically.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>This is the default choice.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"No"`</ph>: no normalization is performed.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Yes"`</ph>: normalization is performed.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Warn"`</ph>: if normalization is needed, a warning message is displayed, but normalization is not performed.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Normalization rescales disparate data ranges to a standard scale.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Feature scaling insures the distances between data points are proportional and enables various optimization methods such as gradient descent to converge much faster.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>If normalization is performed, a <ph id="ph1">`MaxMin`</ph> normalizer is used.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>It normalizes values in an interval [a, b] where <ph id="ph1">`-1 &lt;= a &lt;= 0`</ph> and <ph id="ph2">`0 &lt;= b &lt;= 1`</ph> and <ph id="ph3">`b - a = 1`</ph>.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>This normalizer preserves sparsity by mapping zero to zero.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>ml_transforms</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Specifies a list of MicrosoftML transforms to be performed on the data before training or <bpt id="p1">*</bpt>None<ept id="p1">*</ept> if no transforms are to be performed.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt><ph id="ph1">`featurize_text`</ph><ept id="p1">](featurize-text.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`categorical`</ph><ept id="p2">](categorical.md)</ept>, and <bpt id="p3">[</bpt><ph id="ph3">`categorical_hash`</ph><ept id="p3">](categorical-hash.md)</ept>, for transformations that are supported.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>These transformations are performed after any specified Python transformations.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>ml_transform_vars</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Specifies a character vector of variable names to be used in <ph id="ph1">`ml_transforms`</ph> or <bpt id="p1">*</bpt>None<ept id="p1">*</ept> if none are to be used.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>row_selection</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Specifies the rows (observations) from the data set that are to be used by the model with the name of a logical variable from the data set (in quotes) or with a logical expression using variables in the data set.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`row_selection = "old"`</ph> will only use observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`True`</ph>.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`row_selection = (age &gt; 20) &amp; (age &lt; 65) &amp; (log(income) &gt; 10)`</ph> only uses observations in which the value of the <ph id="ph2">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph3">`log`</ph> of the <ph id="ph4">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transform_function`</ph>).</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`row_selection`</ph> can be defined outside of the function call using the <ph id="ph2">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>transforms</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>An expression of the form that represents the first round of variable transformations.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`row_selection`</ph>) can be defined outside of the function call using the <ph id="ph3">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>transform_objects</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>A named list that contains objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transform_function`</ph>, and <ph id="ph3">`row_selection`</ph>.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>transform_function</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>The variable transformation function.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>transform_variables</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>A character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>transform_packages</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>A character vector specifying additional Python packages (outside of those specified in <ph id="ph1">`RxOptions.get_option("transform_packages")`</ph>) to be made available and preloaded for use in variable transformation functions.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>For example, those explicitly defined in <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../revoscalepy/index.md)</ept> functions via their <ph id="ph1">`transforms`</ph> and <ph id="ph2">`transform_function`</ph> arguments or those defined implicitly via their <ph id="ph3">`formula`</ph> or <ph id="ph4">`row_selection`</ph> arguments.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transform_packages`</ph> argument may also be <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, indicating that no packages outside <ph id="ph2">`RxOptions.get_option("transform_packages")`</ph> are preloaded.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>transform_environment</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>A user-defined environment to serve as a parent to all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transform_environment = None`</ph>, a new “hash” environment with parent revoscalepy.baseenv is used instead.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Specifies the number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the level of reporting on the row processing progress:</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the amount of output wanted.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Integer values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Sets the context in which computations are executed, specified with a valid revoscalepy.RxComputeContext.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Currently local and <bpt id="p1">[</bpt>revoscalepy.RxInSqlServer<ept id="p1">](../revoscalepy/RxInSqlServer.md)</ept> compute contexts are supported.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>ensemble</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Control parameters for ensembling.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt><ph id="ph1">`LogisticRegression`</ph><ept id="p1">](learners-object.md)</ept> object with the trained model.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>This algorithm will attempt to load the entire dataset into memory when <ph id="ph1">`train_threads &gt; 1`</ph> (multi-threading).</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Wikipedia: L-BFGS<ept id="p1">](https://en.wikipedia.org/wiki/L-BFGS)</ept></source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Wikipedia: Logistic regression<ept id="p1">](https://en.wikipedia.org/wiki/Logistic_regression)</ept></source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Scalable Training of L1-Regularized Log-Linear Models<ept id="p1">](https://research.microsoft.com/apps/pubs/default.aspx?id=78900)</ept></source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Test Run - L1 and L2 Regularization for Machine Learning<ept id="p1">](https://msdn.microsoft.com/en-us/magazine/dn904675.aspx)</ept></source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit></group></body></file></xliff>