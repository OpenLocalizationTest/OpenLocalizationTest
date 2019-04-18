<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxoneclasssvm.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4611c7f3bf606dfbc596c2a23ad477bac779370a6.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">611c7f3bf606dfbc596c2a23ad477bac779370a6</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\rxoneclasssvm.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxOneClassSvm function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Machine Learning One Class Support Vector Machines</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), rxOneClassSvm, anomaly, detection, models</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxOneClassSvm: OneClass SVM</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Machine Learning One Class Support Vector Machines</source>
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
          <source>The maximal size in MB of the cache that stores the training data.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Increase this for large training sets.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The default value is 100 MB.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>A character string representing the kernel used for computing inner products.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>maKernel<ept id="p1">](kernel.md)</ept>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The following choices are available:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rbfKernel()`</ph>: Radial basis function kernel.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Its parameter  represents<ph id="ph1">`gamma`</ph> in the term <ph id="ph2">`exp(-gamma|x-y|^2`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If not  specified, it defaults to <ph id="ph1">`1`</ph> divided by the number of features used.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rbfKernel(gamma = .1)`</ph>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This is the default value.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`linearKernel()`</ph>: Linear kernel.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`polynomialKernel()`</ph>: Polynomial kernel with parameter names <ph id="ph2">`a`</ph>,  <ph id="ph3">`bias`</ph>, and <ph id="ph4">`deg`</ph> in the term <ph id="ph5">`(a*&lt;x,y&gt; + bias)^deg`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The  <ph id="ph1">`bias`</ph>, defaults to <ph id="ph2">`0`</ph>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The degree, <ph id="ph1">`deg`</ph>, defaults to  <ph id="ph2">`3`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`a`</ph> is not specified, it is set to <ph id="ph2">`1`</ph> divided by the number of features.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`maKernelPoynomial(bias = 0, deg = ``  3)`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`sigmoidKernel()`</ph>: Sigmoid kernel with parameter names  <ph id="ph2">`gamma`</ph> and <ph id="ph3">`coef0`</ph> in the term <ph id="ph4">`tanh(gamma*&lt;x,y&gt; + coef0)`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`gamma`</ph>, defaults to <ph id="ph2">`1`</ph> divided by the number of features.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The  parameter <ph id="ph1">`coef0`</ph> defaults to <ph id="ph2">`0`</ph>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>For example,  <ph id="ph1">`sigmoidKernel(gamma = .1, coef0 = 0)`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The threshold for optimizer convergence.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If the  improvement between iterations is less than the threshold, the algorithm  stops and returns the current model.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The value must be greater than or equal to <ph id="ph1">`.Machine$double.eps`</ph>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The default value is 0.001.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The trade-off between the fraction of outliers and the number of support vectors (represented by the Greek letter nu).</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Must be between 0 and 1, typically between 0.1 and 0.5.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The default value is 0.1.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Uses the shrinking heuristic if <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>In this case, some samples will be "shrunk" during the training procedure, which may speed up training.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Specifies the type of automatic normalization used:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"auto"`</ph>: if normalization is needed, it is performed  automatically.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>This is the default choice.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"no"`</ph>: no normalization is performed.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"yes"`</ph>: normalization is performed.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"warn"`</ph>: if normalization is needed, a warning  message is displayed, but normalization is not performed.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Normalization rescales disparate data ranges to a standard scale.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Feature scaling insures the distances between data points are proportional and  enables various optimization methods such as gradient descent to converge  much faster.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If normalization is performed, a <ph id="ph1">`MaxMin`</ph> normalizer is  used.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>It normalizes values in an interval [a, b] where <ph id="ph1">`-1 &lt;= a &lt;= 0`</ph>and <ph id="ph2">`0 &lt;= b &lt;= 1`</ph> and <ph id="ph3">`b - a = 1`</ph>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>This normalizer preserves  sparsity by mapping zero to zero.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Specifies a list of MicrosoftML transforms to be performed on the data before training or <ph id="ph1">`NULL`</ph> if no transforms are  to be performed.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>featurizeText<ept id="p1">](featurizeText.md)</ept>, <bpt id="p2">[</bpt>categorical<ept id="p2">](categorical.md)</ept>, and <bpt id="p3">[</bpt>categoricalHash<ept id="p3">](categoricalHash.md)</ept>, for transformations that are supported.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>These transformations are performed after any specified R transformations.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Specifies a character vector of variable names to be used in <ph id="ph1">`mlTransforms`</ph> or <ph id="ph2">`NULL`</ph> if none are to be used.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Specifies the rows (observations) from the data set that are to be used by the model with the name of a logical variable from the  data set (in quotes) or with a logical expression using variables in the    data set.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will only use observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rowSelection = (age &gt; 20) &amp; (age &lt; 65) &amp; (log(income) &gt; 10)`</ph> only uses observations in which the value of the <ph id="ph2">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph3">`log`</ph> of the <ph id="ph4">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>An expression of the form <ph id="ph1">`list(name = expression, ``...)`</ph> that represents the first round of variable transformations.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>As with  all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>) can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>A named list that contains objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The variable transformation function.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>See rxTransform for details.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>A character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>See rxTransform for details.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>A character vector specifying additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and preloaded for use in variable transformation functions.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>For example, those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph1">`transforms`</ph> and <ph id="ph2">`transformFunc`</ph> arguments or those defined implicitly via their <ph id="ph3">`formula`</ph> or <ph id="ph4">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>, indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> are preloaded.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>A user-defined environment to serve as a parent to all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Specifies the number of blocks to read for each chunk  of data read from the data source.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the level of reporting on the row processing progress:</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the amount of output wanted.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Integer  values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Sets the context in which computations are executed, specified with a valid RxComputeContext.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Currently local and RxInSqlServer compute contexts are supported.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Control parameters for ensembling.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed directly to the Microsoft Compute Engine.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>detection is to identify outliers that do not belong to some target class.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>This type of SVM is one-class because the training set contains only examples from the target class.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>It infers what properties are normal for the objects in the target class and from these properties predicts which examples are unlike the normal examples.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>This is useful for anomaly detection because the scarcity of training examples is the defining character of anomalies: typically there are very few examples of network intrusion, fraud, or other types of anomalous behavior.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxOneClassSvm`</ph>: A <ph id="ph2">`rxOneClassSvm`</ph> object with the trained model.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`OneClassSvm`</ph>: A learner specification object of class <ph id="ph2">`maml`</ph> for the OneClass Svm trainer.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>This algorithm is single-threaded and will always attempt to load the entire dataset into memory.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rbfKernel<ept id="p1">](kernel.md)</ept>, <bpt id="p2">[</bpt>linearKernel<ept id="p2">](kernel.md)</ept>, <bpt id="p3">[</bpt>polynomialKernel<ept id="p3">](kernel.md)</ept>, <bpt id="p4">[</bpt>sigmoidKernel<ept id="p4">](kernel.md)</ept><ph id="ph1">
</ph><bpt id="p5">[</bpt>rxFastTrees<ept id="p5">](rxFastTrees.md)</ept>, <bpt id="p6">[</bpt>rxFastForest<ept id="p6">](rxFastForest.md)</ept>, <bpt id="p7">[</bpt>rxFastLinear<ept id="p7">](rxFastLinear.md)</ept>, <bpt id="p8">[</bpt>rxLogisticRegression<ept id="p8">](rxLogisticRegression.md)</ept>, <bpt id="p9">[</bpt>rxNeuralNet<ept id="p9">](rxNeuralNet.md)</ept>, <bpt id="p10">[</bpt>featurizeText<ept id="p10">](featurizeText.md)</ept>, <bpt id="p11">[</bpt>categorical<ept id="p11">](categorical.md)</ept>, <bpt id="p12">[</bpt>categoricalHash<ept id="p12">](categoricalHash.md)</ept>, <bpt id="p13">[</bpt>rxPredict.mlModel<ept id="p13">](rxPredict.md)</ept>.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>