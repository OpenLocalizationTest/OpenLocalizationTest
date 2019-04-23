<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxfastforest.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86cdc3a0757fbcf16eda1c22e84f2c112b18a15c84.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">cdc3a0757fbcf16eda1c22e84f2c112b18a15c84</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\rxfastforest.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxFastForest function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Machine Learning Fast Forest</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), rxFastForest, classification, models, regression</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxFastForest: Fast Forest</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Machine Learning Fast Forest</source>
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
          <source>A character string denoting Fast Tree type:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>for the default Fast Tree Binary Classification or</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>for Fast Tree Regression.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Specifies the total number of decision trees to create in  the ensemble.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>By creating more decision trees, you can potentially get  better coverage, but the training time increases.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The default value is 100.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The maximum number of leaves (terminal nodes) that can be created in any tree.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Higher values potentially increase the size of the tree and get better precision, but risk overfitting and requiring longer training times.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The default value is 20.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Minimum number of training instances required to form a leaf.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>That is, the minimal number of documents allowed in a leaf of a regression tree, out of the sub-sampled data.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>A 'split' means that features in each level of the tree (node) are randomly divided.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The default value is 10.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The fraction of randomly chosen instances to use for each tree.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The default value is 0.7.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The fraction of randomly chosen features to use for each tree.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The default value is 0.7.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The fraction of randomly chosen features to use on each split.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The default value is 0.7.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Maximum number of distinct values (bins) per feature.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The default value is 255.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The feature first use penalty coefficient.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The default  value is 0.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Tree fitting gain confidence requirement (should be in the range [0,1)).</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The default value is 0.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The number of threads to use in training.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>is specified, the number of threads to use is determined internally.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Specifies the random seed.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Specifies a list of MicrosoftML transforms to be performed on the data before training or <ph id="ph1">`NULL`</ph> if no transforms are  to be performed.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>featurizeText<ept id="p1">](featurizeText.md)</ept>, <bpt id="p2">[</bpt>categorical<ept id="p2">](categorical.md)</ept>, and <bpt id="p3">[</bpt>categoricalHash<ept id="p3">](categoricalHash.md)</ept>, for transformations that are supported.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>These transformations are performed after any specified R transformations.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Specifies a character vector of variable names to be used in <ph id="ph1">`mlTransforms`</ph> or <ph id="ph2">`NULL`</ph> if none are to be used.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Specifies the rows (observations) from the data set that are to be used by the model with the name of a logical variable from the  data set (in quotes) or with a logical expression using variables in the    data set.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will only use observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>only uses observations in which the value of the <ph id="ph1">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph2">`log`</ph> of the <ph id="ph3">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>An expression of the form <ph id="ph1">`list(name = expression, ``...)`</ph> that represents the first round of variable transformations.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>As with  all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>) can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>A named list that contains objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The variable transformation function.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>See rxTransform for details.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>A character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>See rxTransform for details.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>A character vector specifying additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and preloaded for use in variable transformation functions.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>For example, those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph1">`transforms`</ph> and <ph id="ph2">`transformFunc`</ph> arguments or those defined implicitly via their <ph id="ph3">`formula`</ph> or <ph id="ph4">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>, indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> are preloaded.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>A user-defined environment to serve as a parent to all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Specifies the number of blocks to read for each chunk  of data read from the data source.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the level of reporting on the row processing progress:</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the amount of output wanted.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Integer  values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Sets the context in which computations are executed, specified with a valid RxComputeContext.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Currently local and RxInSqlServer compute contexts are supported.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Control parameters for ensembling.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed directly to the Microsoft Compute Engine.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Decision trees are non-parametric models that perform a sequence</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>of simple tests on inputs.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>This decision procedure maps them to outputs found in the training dataset whose inputs were similar to the instance being processed.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>A decision is made at each node of the binary tree data structure based on a measure of similarity that maps each instance recursively through the branches of the tree until the appropriate leaf node is reached and the output decision returned.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Decision trees have several advantages:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>They are efficient in both computation and memory usage during training and prediction.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>They can represent non-linear decision boundaries.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>They perform integrated feature selection and classification.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>They are resilient in the presence of noisy features.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Fast forest regression is a random forest and quantile regression forest implementation using the regression tree learner in <bpt id="p1">[</bpt>rxFastTrees<ept id="p1">](rxFastTrees.md)</ept>.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>The model consists of an ensemble of decision trees.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Each tree in a decision forest outputs a Gaussian distribution by way of prediction.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>An aggregation is performed over the ensemble of trees to find a Gaussian distribution closest to the combined distribution for all trees in the model.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>This decision forest classifier consists of an ensemble of decision trees.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Generally, ensemble models provide better coverage and accuracy than single decision trees.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Each tree in a decision forest outputs a Gaussian distribution by way of prediction.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>An aggregation is performed over the ensemble of trees to find a Gaussian distribution closest to the combined distribution for all trees in the model.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>: A <ph id="ph1">`rxFastForest`</ph> object with the trained model.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`FastForest`</ph>: A learner specification object of class <ph id="ph2">`maml`</ph> for the Fast Forest trainer.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>This algorithm is multi-threaded and will always attempt to load the entire dataset into memory.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxFastTrees<ept id="p1">](rxFastTrees.md)</ept>, <bpt id="p2">[</bpt>rxFastLinear<ept id="p2">](rxFastLinear.md)</ept>, <bpt id="p3">[</bpt>rxLogisticRegression<ept id="p3">](rxLogisticRegression.md)</ept>, <bpt id="p4">[</bpt>rxNeuralNet<ept id="p4">](rxNeuralNet.md)</ept>, <bpt id="p5">[</bpt>rxOneClassSvm<ept id="p5">](rxOneClassSvm.md)</ept>, <bpt id="p6">[</bpt>featurizeText<ept id="p6">](featurizeText.md)</ept>, <bpt id="p7">[</bpt>categorical<ept id="p7">](categorical.md)</ept>, <bpt id="p8">[</bpt>categoricalHash<ept id="p8">](categoricalHash.md)</ept>, <bpt id="p9">[</bpt>rxPredict.mlModel<ept id="p9">](rxPredict.md)</ept>.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>