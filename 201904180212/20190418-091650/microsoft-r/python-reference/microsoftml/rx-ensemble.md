<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-ensemble.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b43cbcc25e34ac547a1ef4cf7cc3c153ad7dd5d94c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">3cbcc25e34ac547a1ef4cf7cc3c153ad7dd5d94c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\rx-ensemble.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_ensemble: Ensembles</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Train an ensemble of models</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>ensemble</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.rx_ensemble<ept id="p1">*</ept>: Combine models into a single one</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Train an ensemble of models.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rx_ensemble`</ph> is a function that trains a number of models of various kinds to obtain better predictive performance than could be obtained from a single model.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>formula</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>A symbolic or mathematical formula in valid Python syntax, enclosed in double quotes.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>A symbolic formula might reference objects in the data source, such as <ph id="ph1">`"creditScore ~ yearsEmploy"`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Interaction terms (<ph id="ph1">`creditScore * yearsEmploy`</ph>) and expressions (<ph id="ph2">`creditScore == 1`</ph>) are not currently supported.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>A data source object or a character string specifying a <bpt id="p1">*</bpt>.xdf<ept id="p1">*</ept> file or a data frame object.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Alternatively, it can be a list of data sources indicating each model should be trained using one of the data sources in the list.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>In this case, the length of the data list must be equal to <bpt id="p1">*</bpt>model_count<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>trainers</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>A list of trainers with their arguments.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The trainers are created by using <ph id="ph1">`FastTrees`</ph>, <ph id="ph2">`FastForest`</ph>, <ph id="ph3">`FastLinear`</ph>, <ph id="ph4">`LogisticRegression`</ph>, <ph id="ph5">`NeuralNetwork`</ph>, or <ph id="ph6">`OneClassSvm`</ph>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>method</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>A character string that specifies the type of ensemble: <ph id="ph1">`"anomaly"`</ph> for Anomaly Detection, <ph id="ph2">`"binary"`</ph> for Binary Classification, <ph id="ph3">`multiClass`</ph> for Multiclass Classification, or <ph id="ph4">`"regression"`</ph> for Regression.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>random_seed</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Specifies the random seed.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`None`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>model_count</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Specifies the number of models to train.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If this number is greater than the length of the trainers list, the trainers list is duplicated to match <ph id="ph1">`model_count`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>replace</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>A logical value specifying if the sampling of observations should be done with or without replacement.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`False`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>samp_rate</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>A scalar of positive value specifying the percentage of observations to sample for each trainer.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The default is <ph id="ph1">`1.0`</ph> for sampling with replacement (i.e., <ph id="ph2">`replace=True`</ph>) and <ph id="ph3">`0.632`</ph> for sampling without replacement (i.e., <ph id="ph4">`replace=False`</ph>).</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>When <ph id="ph1">`split_data`</ph> is <ph id="ph2">`True`</ph>, the default of <ph id="ph3">`samp_rate`</ph> is <ph id="ph4">`1.0`</ph> (no sampling is done before splitting).</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>split_data</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>A logical value specifying whether or not to train the base models on non-overlapping partitions.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The default is <ph id="ph1">`False`</ph>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>It is available only for <ph id="ph1">`RxSpark`</ph> compute context and ignored for others.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>combine_method</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Specifies the method used to combine the models:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Median"`</ph>: to compute the median of the individual model outputs,</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Average"`</ph>: to compute the average of the individual model outputs and</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Vote"`</ph>: to compute (pos-neg) / the total number of models, where ‘pos’</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>max_calibration</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Specifies the maximum number of examples to use for calibration.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>This argument is ignored for all tasks other than binary classification.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>ml_transforms</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Specifies a list of MicrosoftML transforms to be performed on the data before training or <bpt id="p1">*</bpt>None<ept id="p1">*</ept> if no transforms are to be performed.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Transforms that require an additional pass over the data (such as <ph id="ph1">`featurize_text`</ph>, <ph id="ph2">`categorical`</ph> are not allowed.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>These transformations are performed after any specified R transformations.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>ml_transform_vars</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Specifies a character vector of variable names to be used in <bpt id="p1">*</bpt>ml_transforms<ept id="p1">*</ept> or <bpt id="p2">*</bpt>None<ept id="p2">*</ept> if none are to be used.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>row_selection</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Specifies the rows (observations) from the data set that are to be used by the model with the name of a logical variable from the data set (in quotes) or with a logical expression using variables in the data set.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rowSelection = "old"`</ph> will only use observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`True`</ph>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rowSelection = (age &gt; 20) &amp; (age &lt; 65) &amp; (log(income) &gt; 10)`</ph> only uses observations in which the value of the <ph id="ph2">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph3">`log`</ph> of the <ph id="ph4">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transform_func`</ph>).</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`row_selection`</ph> can be defined outside of the function call using the <ph id="ph2">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>transforms</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>An expression of the form that represents the first round of variable transformations.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`row_selection`</ph>) can be defined outside of the function call using the <ph id="ph3">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>transform_objects</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>A named list that contains objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transform_function`</ph>, and <ph id="ph3">`row_selection`</ph>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>transform_function</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>The variable transformation function.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>transform_variables</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>A character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>transform_packages</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>A character vector specifying additional Python packages (outside of those specified in <ph id="ph1">`RxOptions.get_option("transform_packages")`</ph>) to be made available and preloaded for use in variable transformation functions.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>For example, those explicitly defined in <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../revoscalepy/revoscalepy-package.md)</ept> functions via their <ph id="ph1">`transforms`</ph> and <ph id="ph2">`transform_function`</ph> arguments or those defined implicitly via their <ph id="ph3">`formula`</ph> or <ph id="ph4">`row_selection`</ph> arguments.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transform_packages`</ph> argument may also be <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, indicating that no packages outside <ph id="ph2">`RxOptions.get_option("transform_packages")`</ph> are preloaded.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>transform_environment</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>A user-defined environment to serve as a parent to all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transform_environment = None`</ph>, a new “hash” environment with parent <ph id="ph2">`revoscalepy.baseenv`</ph> is used instead.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Specifies the number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the level of reporting on the row processing progress:</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the amount of output wanted.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Integer values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Sets the context in which computations are executed, specified with a valid <ph id="ph1">`revoscalepy.RxComputeContext`</ph>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Currently local and <bpt id="p1">[</bpt>revoscalepy.RxSpark<ept id="p1">](../revoscalepy/RxSpark.md)</ept> compute contexts are supported.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>When <bpt id="p1">[</bpt>revoscalepy.RxSpark<ept id="p1">](../revoscalepy/RxSpark.md)</ept> is specified, the training of the models is done in a distributed way, and the ensembling is done locally.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Note that the compute context cannot be non-waiting.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>A <ph id="ph1">`rx_ensemble`</ph> object with the trained ensemble model.</source>
        </trans-unit></group></body></file></xliff>