<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxlogisticregression.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335b50e1dfa49059640c9233023ec40b261d8b8ce24.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">b50e1dfa49059640c9233023ec40b261d8b8ce24</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\rxlogisticregression.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxLogisticRegression function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Machine Learning Logistic Regression</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), rxLogisticRegression, classification, models</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxLogisticRegression: Logistic Regression</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Machine Learning Logistic Regression</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The formula as described in rxFormula.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Interaction terms and <ph id="ph1">`F()`</ph> are not currently supported in the <bpt id="p1">**</bpt>MicrosoftML<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>A data source object or a character string specifying a .xdf file or a data frame object.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>A character string that specifies the type of Logistic Regression:  <ph id="ph1">`"binary"`</ph> for the default binary classification logistic regression or <ph id="ph2">`"multi"`</ph> for multinomial logistic regression.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The L2 regularization weight.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Its value must be greater than  or equal to <ph id="ph1">`0`</ph> and the default value is set to <ph id="ph2">`1`</ph>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The L1 regularization weight.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Its value must be greater than  or equal to <ph id="ph1">`0`</ph> and the default value is set to <ph id="ph2">`1`</ph>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Threshold value for optimizer convergence.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If the improvement between iterations is less than the threshold, the algorithm stops and returns the current model.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Smaller values are slower, but more accurate.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`1e-07`</ph>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Memory size for L-BFGS, specifying the number of past positions and gradients to store for the computation of the next step.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This optimization parameter limits the amount of memory that is used to compute the magnitude and direction of the next step.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>When you specify less memory,  training is faster but less accurate.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Must be greater than or equal to  <ph id="ph1">`1`</ph> and the default value is <ph id="ph2">`20`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Sets the initial weights diameter that specifies  the range from which values are drawn for the initial weights.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>These   weights are initialized randomly from within this range.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>For  example, if the diameter is specified to be <ph id="ph1">`d`</ph>, then the weights  are uniformly distributed between <ph id="ph2">`-d/2`</ph> and <ph id="ph3">`d/2`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`0`</ph>, which specifies that all the  weights are  initialized to <ph id="ph2">`0`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Sets the maximum number of iterations.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>After this number  of steps, the algorithm stops even if it has not satisfied convergence criteria.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Specify <ph id="ph1">`TRUE`</ph> to show the statistics of  training data and the trained model; otherwise, <ph id="ph2">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The  default value is <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>For additional information about model  statistics, see <bpt id="p1">[</bpt>summary.mlModel<ept id="p1">](mlModel.md)</ept>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Set to a number greater than 0 to use Stochastic Gradient Descent (SGD) to find the initial parameters.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>A non-zero value  set specifies the tolerance SGD uses to determine convergence.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`0`</ph> specifying that SGD is not used.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The number of threads to use in training the model.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>This should be set to the number of cores on the machine.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Note that  L-BFGS multi-threading attempts to load dataset into memory.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>In case of out-of-memory issues, set <ph id="ph1">`trainThreads`</ph> to <ph id="ph2">`1`</ph> to turn off multi-threading.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> the number of threads to use is determined internally.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, forces densification of the internal optimization vectors.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, enables the logistic regression  optimizer use sparse or dense internal states as it finds appropriate.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Setting <ph id="ph1">`denseOptimizer`</ph> to <ph id="ph2">`TRUE`</ph> requires the internal  optimizer to use a dense internal state, which may help alleviate load  on the garbage collector for some varieties of larger problems.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Specifies the type of automatic normalization used:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"auto"`</ph>: if normalization is needed, it is performed  automatically.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>This is the default choice.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"no"`</ph>: no normalization is performed.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"yes"`</ph>: normalization is performed.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"warn"`</ph>: if normalization is needed, a warning  message is displayed, but normalization is not performed.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Normalization rescales disparate data ranges to a standard scale.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Feature scaling insures the distances between data points are proportional and  enables various optimization methods such as gradient descent to converge  much faster.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>If normalization is performed, a <ph id="ph1">`MaxMin`</ph> normalizer is  used.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>It normalizes values in an interval [a, b] where <ph id="ph1">`-1 &lt;= a &lt;= 0`</ph>and <ph id="ph2">`0 &lt;= b &lt;= 1`</ph> and <ph id="ph3">`b - a = 1`</ph>.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>This normalizer preserves  sparsity by mapping zero to zero.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Specifies a list of MicrosoftML transforms to be performed on the data before training or <ph id="ph1">`NULL`</ph> if no transforms are  to be performed.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>featurizeText<ept id="p1">](featurizeText.md)</ept>, <bpt id="p2">[</bpt>categorical<ept id="p2">](categorical.md)</ept>, and <bpt id="p3">[</bpt>categoricalHash<ept id="p3">](categoricalHash.md)</ept>, for transformations that are supported.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>These transformations are performed after any specified R transformations.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Specifies a character vector of variable names to be used in <ph id="ph1">`mlTransforms`</ph> or <ph id="ph2">`NULL`</ph> if none are to be used.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Specifies the rows (observations) from the data set that are to be used by the model with the name of a logical variable from the  data set (in quotes) or with a logical expression using variables in the    data set.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will only use observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rowSelection = (age &gt; 20) &amp; (age &lt; 65) &amp; (log(income) &gt; 10)`</ph> only uses observations in which the value of the <ph id="ph2">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph3">`log`</ph> of the <ph id="ph4">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>An expression of the form <ph id="ph1">`list(name = expression, ``...)`</ph> that represents the first round of variable transformations.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>As with  all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>) can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>A named list that contains objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>The variable transformation function.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>See rxTransform for details.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>A character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>See rxTransform for details.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>A character vector specifying additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and preloaded for use in variable transformation functions.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>For example, those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph1">`transforms`</ph> and <ph id="ph2">`transformFunc`</ph> arguments or those defined implicitly via their <ph id="ph3">`formula`</ph> or <ph id="ph4">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>, indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> are preloaded.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>A user-defined environment to serve as a parent to all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Specifies the number of blocks to read for each chunk  of data read from the data source.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the level of reporting on the row processing progress:</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the amount of output wanted.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Integer  values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Sets the context in which computations are executed, specified with a valid RxComputeContext.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Currently local and RxInSqlServer compute contexts are supported.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Control parameters for ensembling.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed directly to the Microsoft Compute Engine.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Logistic Regression is a classification method used to predict the value of a categorical dependent variable from its relationship to one or more independent variables assumed to have a logistic distribution.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>If the dependent variable has only two possible values (success/failure), then the logistic regression is binary.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>If the dependent variable has more than two possible values (blood type given diagnostic test results), then the logistic regression is multinomial.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>The optimization technique used for <ph id="ph1">`rxLogisticRegression`</ph> is the limited memory Broyden-Fletcher-Goldfarb-Shanno (L-BFGS).</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Both the L-BFGS and regular BFGS algorithms use quasi-Newtonian methods to estimate the computationally intensive Hessian matrix in the equation used by Newton's method to calculate steps.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>But the L-BFGS approximation uses only a limited amount of memory to compute the next step direction, so that it is especially suited for problems with a large number of variables.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`memorySize`</ph> parameter specifies the number of past positions and gradients to store for use in the computation of the next step.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>This learner can use elastic net regularization: a linear combination of L1 (lasso) and L2 (ridge) regularizations.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Regularization is a method that can render an ill-posed problem more tractable by imposing constraints that provide information to supplement the data and that prevents overfitting by penalizing models with extreme coefficient values.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>This can improve the generalization of the model learned by selecting the optimal complexity in the bias-variance tradeoff.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Regularization works by adding the penalty that is associated with coefficient values to the error of the hypothesis.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>An accurate model with extreme coefficient values would be penalized more, but a less accurate model with more conservative values would be penalized less.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>L1 and L2 regularization have different effects and uses that are complementary in certain respects.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`l1Weight`</ph>: can be applied to sparse models, when working with high-dimensional data.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>It pulls small weights associated features that are relatively unimportant towards 0.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`l2Weight`</ph>: is preferable for data that is not sparse.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>It pulls large weights towards zero.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Adding the ridge penalty to the regularization overcomes some of lasso's</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>limitations.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>It can improve its predictive accuracy, for example, when the number of predictors is greater than the sample size.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`x = l1Weight`</ph> and <ph id="ph2">`y = l2Weight`</ph>, <ph id="ph3">`ax + by = c`</ph> defines the linear span of the regularization terms.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>The default values of x and y are both <ph id="ph1">`1`</ph>.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>An aggressive regularization can harm predictive capacity by excluding important variables out of the model.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>So choosing the optimal values for the regularization parameters is important for the performance of the logistic regression model.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxLogisticRegression`</ph>: A <ph id="ph2">`rxLogisticRegression`</ph> object with the trained model.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`LogisticReg`</ph>: A learner specification object of class <ph id="ph2">`maml`</ph> for the Logistic Reg trainer.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>This algorithm will attempt to load the entire dataset into memory when <ph id="ph1">`trainThreads &gt; 1`</ph> (multi-threading).</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxFastTrees<ept id="p1">](rxFastTrees.md)</ept>, <bpt id="p2">[</bpt>rxFastForest<ept id="p2">](rxFastForest.md)</ept>, <bpt id="p3">[</bpt>rxFastLinear<ept id="p3">](rxFastLinear.md)</ept>, <bpt id="p4">[</bpt>rxNeuralNet<ept id="p4">](rxNeuralNet.md)</ept>, <bpt id="p5">[</bpt>rxOneClassSvm<ept id="p5">](rxOneClassSvm.md)</ept>, <bpt id="p6">[</bpt>featurizeText<ept id="p6">](featurizeText.md)</ept>, <bpt id="p7">[</bpt>categorical<ept id="p7">](categorical.md)</ept>, <bpt id="p8">[</bpt>categoricalHash<ept id="p8">](categoricalHash.md)</ept>, <bpt id="p9">[</bpt>rxPredict.mlModel<ept id="p9">](rxPredict.md)</ept>.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>