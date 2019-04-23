<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-featurize.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca8684b8ca8f567d33b4db0d012162e1c3b244e82ce8.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">84b8ca8f567d33b4db0d012162e1c3b244e82ce8</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\rx-featurize.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_featurize: Data Transformation for revoscalepy data sources</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Transforms data from an input data set to an output data set.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>transform, featurizer</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.rx_featurize<ept id="p1">*</ept>: Data transformation for data sources</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Transforms data from an input data set to an output data set.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../revoscalepy/revoscalepy-package.md)</ept> data source object, a data frame, or the path to a <ph id="ph1">`.xdf`</ph> file.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>output_data</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Output text or xdf file name or an <ph id="ph1">`RxDataSource`</ph> with write capabilities in which to store transformed data.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, a data frame is returned.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>overwrite</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`True`</ph>, an existing <ph id="ph2">`output_data`</ph> is overwritten; if <ph id="ph3">`False`</ph> an existing <ph id="ph4">`output_data`</ph> is not overwritten.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`False`</ph>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>data_threads</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>An integer specifying the desired degree of parallelism in the data pipeline.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, the number of threads used is determined internally.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>random_seed</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Specifies the random seed.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>max_slots</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Max slots to return for vector valued columns (&lt;=0 to return all).</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>ml_transforms</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Specifies a list of MicrosoftML transforms to be performed on the data before training or <bpt id="p1">*</bpt>None<ept id="p1">*</ept> if no transforms are to be performed.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt><ph id="ph1">`featurize_text`</ph><ept id="p1">](featurize-text.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`categorical`</ph><ept id="p2">](categorical.md)</ept>, and <bpt id="p3">[</bpt><ph id="ph3">`categorical_hash`</ph><ept id="p3">](categorical-hash.md)</ept>, for transformations that are supported.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>These transformations are performed after any specified Python transformations.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>ml_transform_vars</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Specifies a character vector of variable names to be used in <ph id="ph1">`ml_transforms`</ph> or <bpt id="p1">*</bpt>None<ept id="p1">*</ept> if none are to be used.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>row_selection</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Specifies the rows (observations) from the data set that are to be used by the model with the name of a logical variable from the data set (in quotes) or with a logical expression using variables in the data set.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>will only use observations in which the value of the variable <ph id="ph1">`old`</ph> is <ph id="ph2">`True`</ph>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>only uses observations in which the value of the <ph id="ph1">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph2">`log`</ph> of the <ph id="ph3">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transform_function`</ph>).</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`row_selection`</ph> can be defined outside of the function call using the <ph id="ph2">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>transforms</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>An expression of the form that represents the first round of variable transformations.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`row_selection`</ph>) can be defined outside of the function call using the <ph id="ph3">`expression`</ph> function.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>transform_objects</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>A named list that contains objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transform_function`</ph>, and <ph id="ph3">`row_selection`</ph>.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>transform_function</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The variable transformation function.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>transform_variables</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>A character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>transform_packages</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>A character vector specifying additional Python packages (outside of those specified in <ph id="ph1">`RxOptions.get_option("transform_packages")`</ph>) to be made available and preloaded for use in variable transformation functions.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>For example, those explicitly defined in <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../revoscalepy/revoscalepy-package.md)</ept> functions via their <ph id="ph1">`transforms`</ph> and <ph id="ph2">`transform_function`</ph> arguments or those defined implicitly via their <ph id="ph3">`formula`</ph> or <ph id="ph4">`row_selection`</ph> arguments.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transform_packages`</ph> argument may also be <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, indicating that no packages outside <ph id="ph2">`RxOptions.get_option("transform_packages")`</ph> are preloaded.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>transform_environment</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>NOT SUPPORTED.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>A user-defined environment to serve as a parent to all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transform_environment = None`</ph>, a new “hash” environment with parent revoscalepy.baseenv is used instead The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Specifies the number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the level of reporting on the row processing progress:</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`1`</ph>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the amount of output wanted.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Integer values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`1`</ph>.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Sets the context in which computations are executed, specified with a valid revoscalepy.RxComputeContext.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Currently local and <bpt id="p1">[</bpt>revoscalepy.RxInSqlServer<ept id="p1">](../revoscalepy/RxInSqlServer.md)</ept> compute contexts are supported.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>A data frame or an <bpt id="p1">[</bpt>revoscalepy.RxDataSource<ept id="p1">](../revoscalepy/RxDataSource.md)</ept> object representing the created output data.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`rx_predict`</ph><ept id="p1">](rx-predict.md)</ept>, <bpt id="p2">[</bpt>revoscalepy.rx_data_step<ept id="p2">](../revoscalepy/rx-data-step.md)</ept>, <bpt id="p3">[</bpt>revoscalepy.rx_import<ept id="p3">](../revoscalepy/rx-import.md)</ept>.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit></group></body></file></xliff>