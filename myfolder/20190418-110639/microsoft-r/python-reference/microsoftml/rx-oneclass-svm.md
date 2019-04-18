<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-oneclass-svm.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907fb5a4099beda8ff058c026be5bf5a7d6aa01ead8c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">b5a4099beda8ff058c026be5bf5a7d6aa01ead8c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\rx-oneclass-svm.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_oneclass_svm: OneClass SVM</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Machine Learning One Class Support Vector Machines</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>models, anomaly, detection</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.rx_oneclass_svm<ept id="p1">*</ept>: Anomaly Detection</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Machine Learning One Class Support Vector Machines</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>One-class SVM is an algorithm for anomaly detection.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The goal of anomaly detection is to identify outliers that do not belong to some target class.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>This type of SVM is one-class because the training set contains only examples from the target class.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>It infers what properties are normal for the objects in the target class and from these properties predicts which examples are unlike the normal examples.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>This is useful for anomaly detection because the scarcity of training examples is the defining character of anomalies: typically there are very few examples of network intrusion, fraud, or other types of anomalous behavior.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>formula</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The formula as described in revoscalepy.rx_formula.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Interaction terms and <ph id="ph1">`F()`</ph> are not currently supported in <bpt id="p1">[</bpt>microsoftml<ept id="p1">](microsoftml-package.md)</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>A data source object or a character string specifying a <bpt id="p1">*</bpt>.xdf<ept id="p1">*</ept> file or a data frame object.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>cache_size</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The maximal size in MB of the cache that stores the training data.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Increase this for large training sets.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The default value is 100 MB.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>kernel</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>A character string representing the kernel used for computing inner products.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>For more information, see <ph id="ph1">`ma_kernel()`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The following choices are available:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rbf_kernel`</ph>: Radial basis function kernel.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Its parameter represents<ph id="ph1">``gamma``</ph> in the term <ph id="ph2">`exp(-gamma|x-y|^2`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If not specified, it defaults to <ph id="ph1">`1`</ph> divided by the number of features used.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rbf_kernel(gamma = .1)`</ph>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>This is the default value.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`linear_kernel`</ph>: Linear kernel.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`polynomial_kernel`</ph>: Polynomial kernel with parameter names <ph id="ph2">`a`</ph>, <ph id="ph3">`bias`</ph>, and <ph id="ph4">`deg`</ph> in the term <ph id="ph5">`(a*&lt;x,y&gt; + bias)^deg`</ph>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`bias`</ph>, defaults to <ph id="ph2">`0`</ph>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The degree, <ph id="ph1">`deg`</ph>, defaults to <ph id="ph2">`3`</ph>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`a`</ph> is not specified, it is set to <ph id="ph2">`1`</ph> divided by the number of features.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`sigmoid_kernel`</ph>: Sigmoid kernel with parameter names <ph id="ph2">`gamma`</ph> and <ph id="ph3">`coef0`</ph> in the term <ph id="ph4">`tanh(gamma*&lt;x,y&gt; + coef0)`</ph>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`gamma`</ph>, defaults to <ph id="ph2">`1`</ph> divided by the number of features.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The parameter <ph id="ph1">`coef0`</ph> defaults to <ph id="ph2">`0`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`sigmoid_kernel(gamma = .1, coef0 = 0)`</ph>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>epsilon</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The threshold for optimizer convergence.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>If the improvement between iterations is less than the threshold, the algorithm stops and returns the current model.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The value must be greater than or equal to <ph id="ph1">`numpy.finfo(double).eps`</ph>.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The default value is 0.001.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>nu</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The trade-off between the fraction of outliers and the number of support vectors (represented by the Greek letter nu).</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Must be between 0 and 1, typically between 0.1 and 0.5.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The default value is 0.1.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>shrink</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Uses the shrinking heuristic if <ph id="ph1">`True`</ph>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>In this case, some samples will be “shrunk” during the training procedure, which may speed up training.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`True`</ph>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>normalize</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Specifies the type of automatic normalization used:</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Auto"`</ph>: if normalization is needed, it is performed automatically.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>This is the default choice.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"No"`</ph>: no normalization is performed.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Yes"`</ph>: normalization is performed.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Warn"`</ph>: if normalization is needed, a warning message is displayed, but normalization is not performed.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Normalization rescales disparate data ranges to a standard scale.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Feature scaling insures the distances between data points are proportional and enables various optimization methods such as gradient descent to converge much faster.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If normalization is performed, a <ph id="ph1">`MaxMin`</ph> normalizer is used.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>It normalizes values in an interval [a, b] where <ph id="ph1">`-1 &lt;= a &lt;= 0`</ph> and <ph id="ph2">`0 &lt;= b &lt;= 1`</ph> and <ph id="ph3">`b - a = 1`</ph>.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>This normalizer preserves sparsity by mapping zero to zero.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>ml_transforms</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Specifies a list of MicrosoftML transforms to be performed on the data before training or <bpt id="p1">*</bpt>None<ept id="p1">*</ept> if no transforms are to be performed.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt><ph id="ph1">`featurize_text`</ph><ept id="p1">](featurize-text.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`categorical`</ph><ept id="p2">](categorical.md)</ept>, and <bpt id="p3">[</bpt><ph id="ph3">`categorical_hash`</ph><ept id="p3">](categorical-hash.md)</ept>, for transformations that are supported.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>These transformations are performed after any specified Python transformations.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>ml_transform_vars</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Specifies a character vector of variable names to be used in <ph id="ph1">`ml_transforms`</ph> or <bpt id="p1">*</bpt>None<ept id="p1">*</ept> if none are to be used.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>row_selection</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Specifies the rows (observations) from the data set that are to be used by the model with the name of a logical variable from the data set (in quotes) or with a logical expression using variables in the data set.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`row_selection = "old"`</ph> will only use observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`True`</ph>.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`row_selection = (age &gt; 20) &amp; (age &lt; 65) &amp; (log(income) &gt; 10)`</ph> only uses observations in which the value of the <ph id="ph2">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph3">`log`</ph> of the <ph id="ph4">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transform_function`</ph>).</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`row_selection`</ph> can be defined outside of the function call using the <ph id="ph2">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>transforms</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>An expression of the form that represents the first round of variable transformations.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`row_selection`</ph>) can be defined outside of the function call using the <ph id="ph3">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>transform_objects</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>A named list that contains objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transform_function`</ph>, and <ph id="ph3">`row_selection`</ph>.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>transform_function</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>The variable transformation function.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>transform_variables</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>A character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>transform_packages</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>A character vector specifying additional Python packages (outside of those specified in <ph id="ph1">`RxOptions.get_option("transform_packages")`</ph>) to be made available and preloaded for use in variable transformation functions.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>For example, those explicitly defined in <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../revoscalepy/revoscalepy-package.md)</ept> functions via their <ph id="ph1">`transforms`</ph> and <ph id="ph2">`transform_function`</ph> arguments or those defined implicitly via their <ph id="ph3">`formula`</ph> or <ph id="ph4">`row_selection`</ph> arguments.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transform_packages`</ph> argument may also be <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, indicating that no packages outside <ph id="ph2">`RxOptions.get_option("transform_packages")`</ph> are preloaded.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>transform_environment</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>A user-defined environment to serve as a parent to all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transform_environment = None`</ph>, a new “hash” environment with parent revoscalepy.baseenv is used instead.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Specifies the number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the level of reporting on the row processing progress:</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the amount of output wanted.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Integer values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Sets the context in which computations are executed, specified with a valid revoscalepy.RxComputeContext.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Currently local and <bpt id="p1">[</bpt>revoscalepy.RxInSqlServer<ept id="p1">](../revoscalepy/RxInSqlServer.md)</ept> compute contexts are supported.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>ensemble</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Control parameters for ensembling.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt><ph id="ph1">`OneClassSvm`</ph><ept id="p1">](learners-object.md)</ept> object with the trained model.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>This algorithm is single-threaded and will always attempt to load the entire dataset into memory.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`linear_kernel`</ph>, <ph id="ph2">`polynomial_kernel`</ph>, <ph id="ph3">`rbf_kernel`</ph>, <ph id="ph4">`sigmoid_kernel`</ph>, <bpt id="p1">[</bpt><ph id="ph5">`rx_predict`</ph><ept id="p1">](rx-predict.md)</ept>.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Wikipedia: Anomaly detection<ept id="p1">](https://en.wikipedia.org/wiki/Anomaly_detection)</ept></source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Microsoft Azure Machine Learning Studio: One-Class Support Vector Machine<ept id="p1">](https://msdn.microsoft.com/library/azure/dn913103.aspx)</ept></source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Estimating the Support of a High-Dimensional Distribution<ept id="p1">](https://research.microsoft.com/pubs/69731/tr-99-87.pdf)</ept></source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>New Support Vector Algorithms<ept id="p1">](http://www.stat.purdue.edu/~yuzhu/stat598m3/Papers/NewSVM.pdf)</ept></source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>LIBSVM: A Library for Support Vector Machines<ept id="p1">](https://www.csie.ntu.edu.tw/~cjlin/papers/libsvm.pdf)</ept></source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit></group></body></file></xliff>