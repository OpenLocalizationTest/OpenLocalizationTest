<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-neural-network.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b35423ed1eb392b4d64d108d51bad61d8aafab8bc9.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5423ed1eb392b4d64d108d51bad61d8aafab8bc9</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\rx-neural-network.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_neural_network: Neural Net</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Neural networks for regression modeling and for Binary and multi-class classification.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>models, classification, regression, neural network, dnn</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.rx_neural_network<ept id="p1">*</ept>: Neural Network</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Neural networks for regression modeling and for Binary and multi-class classification.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A neural network is a class of prediction models inspired by the human brain.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>A neural network can be represented as a weighted directed graph.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Each node in the graph is called a neuron.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The neurons in the graph are arranged in layers, where neurons in one layer are connected by a weighted edge (weights can be 0 or positive numbers) to neurons in the next layer.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The first layer is called the input layer, and each neuron in the input layer corresponds to one of the features.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The last layer of the function is called the output layer.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>So in the case of binary neural networks it contains two output neurons, one for each class, whose values are the probabilities of belonging to each class.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The remaining layers are called hidden layers.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The values of the neurons in the hidden layers and in the output layer are set by calculating the weighted sum of the values of the neurons in the previous layer and applying an activation function to that weighted sum.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>A neural network model is defined by the structure of its graph (namely, the number of hidden layers and the number of neurons in each hidden layer), the choice of activation function, and the weights on the graph edges.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The neural network algorithm tries to learn the optimal weights on the edges based on the training data.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Although neural networks are widely known for use in deep learning and modeling complex problems such as image recognition, they are also easily adapted to regression problems.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Any class of statistical models can be considered a neural network if they use adaptive weights and can approximate non-linear functions of their inputs.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Neural network regression is especially suited to problems where a more traditional regression model cannot fit a solution.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>formula</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The formula as described in revoscalepy.rx_formula.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Interaction terms and <ph id="ph1">`F()`</ph> are not currently supported in <bpt id="p1">[</bpt>microsoftml<ept id="p1">](microsoftml-package.md)</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>A data source object or a character string specifying a <bpt id="p1">*</bpt>.xdf<ept id="p1">*</ept> file or a data frame object.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>method</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>A character string denoting Fast Tree type:</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>for the default binary classification neural network.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>for multi-class classification neural network.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>for a regression neural network.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>num_hidden_nodes</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The default number of hidden nodes in the neural net.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The default value is 100.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>num_iterations</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The number of iterations on the full training set.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The default value is 100.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>optimizer</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>A list specifying either the <ph id="ph1">`sgd`</ph> or <ph id="ph2">`adaptive`</ph> optimization algorithm.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>This list can be created using <bpt id="p1">[</bpt><ph id="ph1">`sgd_optimizer`</ph><ept id="p1">](sgd-optimizer.md)</ept> or <bpt id="p2">[</bpt><ph id="ph2">`adadelta_optimizer`</ph><ept id="p2">](adadelta-optimizer.md)</ept>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`sgd`</ph>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>net_definition</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The Net# definition of the structure of the neural network.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>For more information about the Net# language, see <bpt id="p1">[</bpt>Reference Guide<ept id="p1">](https://azure.microsoft.com/documentation/articles/machine-learning-azure-ml-netsharp-reference-guide/)</ept></source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>init_wts_diameter</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Sets the initial weights diameter that specifies the range from which values are drawn for the initial learning weights.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The weights are initialized randomly from within this range.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The default value is 0.1.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>max_norm</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Specifies an upper bound to constrain the norm of the incoming weight vector at each hidden unit.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>This can be very important in max out neural networks as well as in cases where training produces unbounded weights.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>acceleration</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Specifies the type of hardware acceleration to use.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Possible values are “sse_math” and “gpu_math”.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>For GPU acceleration, it is recommended to use a miniBatchSize greater than one.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If you want to use the GPU acceleration, there are additional manual setup steps are required:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Download and install NVidia CUDA Toolkit 6.5 (<bpt id="p1">[</bpt>CUDA Toolkit<ept id="p1">](https://developer.nvidia.com/cuda-toolkit-65)</ept>).</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Download and install NVidia cuDNN v2 Library (<bpt id="p1">[</bpt>cudnn Library<ept id="p1">](https://developer.nvidia.com/rdp/cudnn-archive)</ept>).</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Find the libs directory of the microsoftml package by calling <ph id="ph1">`import microsoftml, os`</ph>, <ph id="ph2">`os.path.join(microsoftml.__path__[0], "mxLibs")`</ph>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Copy <bpt id="p1">*</bpt>cublas64_65.dll<ept id="p1">*</ept>, <bpt id="p2">*</bpt>cudart64_65.dll<ept id="p2">*</ept> and <bpt id="p3">*</bpt>cusparse64_65.dll<ept id="p3">*</ept> from the CUDA Toolkit 6.5 into the libs directory of the microsoftml package.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Copy <bpt id="p1">*</bpt>cudnn64_65.dll<ept id="p1">*</ept> from the cuDNN v2 Library into the libs directory of the microsoftml package.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>mini_batch_size</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Sets the mini-batch size.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Recommended values are between 1 and 256.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>This parameter is only used when the acceleration is GPU.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Setting this parameter to a higher value improves the speed of training, but it might negatively affect the accuracy.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The default value is 1.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>normalize</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Specifies the type of automatic normalization used:</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>: if normalization is needed, it is performed automatically.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>This is the default choice.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>: no normalization is performed.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>: normalization is performed.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>: if normalization is needed, a warning message is displayed, but normalization is not performed.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Normalization rescales disparate data ranges to a standard scale.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Feature scaling insures the distances between data points are proportional and enables various optimization methods such as gradient descent to converge much faster.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>If normalization is performed, a <ph id="ph1">`MaxMin`</ph> normalizer is used.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>It normalizes values in an interval [a, b] where <ph id="ph1">`-1 &lt;= a &lt;= 0`</ph> and <ph id="ph2">`0 &lt;= b &lt;= 1`</ph> and <ph id="ph3">`b - a = 1`</ph>.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>This normalizer preserves sparsity by mapping zero to zero.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>ml_transforms</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Specifies a list of MicrosoftML transforms to be performed on the data before training or <bpt id="p1">*</bpt>None<ept id="p1">*</ept> if no transforms are to be performed.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt><ph id="ph1">`featurize_text`</ph><ept id="p1">](featurize-text.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`categorical`</ph><ept id="p2">](categorical.md)</ept>, and <bpt id="p3">[</bpt><ph id="ph3">`categorical_hash`</ph><ept id="p3">](categorical-hash.md)</ept>, for transformations that are supported.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>These transformations are performed after any specified Python transformations.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>ml_transform_vars</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Specifies a character vector of variable names to be used in <ph id="ph1">`ml_transforms`</ph> or <bpt id="p1">*</bpt>None<ept id="p1">*</ept> if none are to be used.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>row_selection</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Specifies the rows (observations) from the data set that are to be used by the model with the name of a logical variable from the data set (in quotes) or with a logical expression using variables in the data set.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>will only use observations in which the value of the variable <ph id="ph1">`old`</ph> is <ph id="ph2">`True`</ph>.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>only uses observations in which the value of the <ph id="ph1">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph2">`log`</ph> of the <ph id="ph3">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transform_function`</ph>).</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`row_selection`</ph> can be defined outside of the function call using the <ph id="ph2">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>transforms</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>An expression of the form that represents the first round of variable transformations.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`row_selection`</ph>) can be defined outside of the function call using the <ph id="ph3">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>transform_objects</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>A named list that contains objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transform_function`</ph>, and <ph id="ph3">`row_selection`</ph>.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>transform_function</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>The variable transformation function.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>transform_variables</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>A character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>transform_packages</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>A character vector specifying additional Python packages (outside of those specified in <ph id="ph1">`RxOptions.get_option("transform_packages")`</ph>) to be made available and preloaded for use in variable transformation functions.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>For example, those explicitly defined in <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../revoscalepy/revoscalepy-package.md)</ept> functions via their <ph id="ph1">`transforms`</ph> and <ph id="ph2">`transform_function`</ph> arguments or those defined implicitly via their <ph id="ph3">`formula`</ph> or <ph id="ph4">`row_selection`</ph> arguments.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transform_packages`</ph> argument may also be <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, indicating that no packages outside <ph id="ph2">`RxOptions.get_option("transform_packages")`</ph> are preloaded.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>transform_environment</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>A user-defined environment to serve as a parent to all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transform_environment = None`</ph>, a new “hash” environment with parent revoscalepy.baseenvis used instead.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Specifies the number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the level of reporting on the row processing progress:</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the amount of output wanted.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Integer values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Sets the context in which computations are executed, specified with a valid revoscalepy.RxComputeContext.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Currently local and <bpt id="p1">[</bpt>revoscalepy.RxInSqlServer<ept id="p1">](../revoscalepy/RxInSqlServer.md)</ept> compute contexts are supported.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>ensemble</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Control parameters for ensembling.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt><ph id="ph1">`NeuralNetwork`</ph><ept id="p1">](learners-object.md)</ept> object with the trained model.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>This algorithm is single-threaded and will not attempt to load the entire dataset into memory.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`adadelta_optimizer`</ph><ept id="p1">](adadelta-optimizer.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`sgd_optimizer`</ph><ept id="p2">](sgd-optimizer.md)</ept>, <bpt id="p3">[</bpt><ph id="ph3">`avx_math`</ph><ept id="p3">](avx-math.md)</ept>, <bpt id="p4">[</bpt><ph id="ph4">`clr_math`</ph><ept id="p4">](clr-math.md)</ept>, <bpt id="p5">[</bpt><ph id="ph5">`gpu_math`</ph><ept id="p5">](gpu-math.md)</ept>, <bpt id="p6">[</bpt><ph id="ph6">`mkl_math`</ph><ept id="p6">](mkl-math.md)</ept>, <bpt id="p7">[</bpt><ph id="ph7">`sse_math`</ph><ept id="p7">](sse-math.md)</ept>, <bpt id="p8">[</bpt><ph id="ph8">`rx_predict`</ph><ept id="p8">](rx-predict.md)</ept>.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Wikipedia: Artificial neural network</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>optimizers</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.adadelta_optimizer<ept id="p1">*</ept>: Adaptive learning rate method</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.sgd_optimizer<ept id="p1">*</ept>: Stochastic gradient descent</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>math</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.avx_math<ept id="p1">*</ept>: Acceleration with AVX instructions</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.clr_math<ept id="p1">*</ept>: Acceleration with .NET math</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.gpu_math<ept id="p1">*</ept>: Acceleration with NVidia CUDA</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.mkl_math<ept id="p1">*</ept>: Acceleration with Intel MKL</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.sse_math<ept id="p1">*</ept>: Acceleration with SSE instructions</source>
        </trans-unit></group></body></file></xliff>