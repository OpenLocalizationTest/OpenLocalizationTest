<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-predict.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b391375993ed850d29d29fda3b234179fc452c44ac.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">91375993ed850d29d29fda3b234179fc452c44ac</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\rx-predict.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_predict: Scores using a Microsoft ML Machine Learning model</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Reports per-instance scoring results in a data frame or revoscalepy data source using a trained Microsoft ML Machine Learning model with arevoscalepydata source.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>models, prediction</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.rx_predict<ept id="p1">*</ept>: Scores using a Microsoft machine learning model</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Reports per-instance scoring results in a data frame or revoscalepy data source using a trained Microsoft ML Machine Learning model with arevoscalepydata source.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The following items are reported in the output by default: scoring on three variables for the binary classifiers: PredictedLabel, Score, and Probability; the Score for oneClassSvm and regression classifiers; PredictedLabel for Multi-class classifiers, plus a variable for each category prepended by the Score.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>model</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>A model information object returned from a microsoftml model.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>For example, an object returned from <ph id="ph1">`rx_fast_trees`</ph> or <ph id="ph2">`rx_logistic_regression`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../revoscalepy/index.md)</ept> data source object, a data frame, or the path to a <ph id="ph1">`.xdf`</ph> file.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>output_data</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Output text or xdf file name or an <ph id="ph1">`RxDataSource`</ph> with write capabilities in which to store transformed data.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, a data frame is returned.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>write_model_vars</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`True`</ph>, variables in the model are written to the output data set in addition to the scoring variables.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If variables from the input data set are transformed in the model, the transformed variables are also included.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`False`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>extra_vars_to_write</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>or character vector of additional variables names from the input data to include in the <ph id="ph1">`output_data`</ph>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`write_model_vars`</ph> is <ph id="ph2">`True`</ph>, model variables are included as well.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`None`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>suffix</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>A character string specifying suffix to append to the created scoring variable(s) or <ph id="ph1">`None`</ph> in there is no suffix.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`None`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>overwrite</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`True`</ph>, an existing <ph id="ph2">`output_data`</ph> is overwritten; if <ph id="ph3">`False`</ph> an existing <ph id="ph4">`output_data`</ph> is not overwritten.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`False`</ph>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>data_threads</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>An integer specifying the desired degree of parallelism in the data pipeline.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>None<ept id="p1">*</ept>, the number of threads used is determined internally.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Specifies the number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the level of reporting on the row processing progress:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`1`</ph>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the amount of output wanted.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Integer values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`1`</ph>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Sets the context in which computations are executed, specified with a valid revoscalepy.RxComputeContext.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Currently local and <bpt id="p1">[</bpt>revoscalepy.RxInSqlServer<ept id="p1">](../revoscalepy/RxInSqlServer.md)</ept> compute contexts are supported.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>kargs</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Additional arguments sent to compute engine.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>A data frame or an <bpt id="p1">[</bpt>revoscalepy.RxDataSource<ept id="p1">](../revoscalepy/RxDataSource.md)</ept> object representing the created output data.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>By default, output from scoring binary classifiers include three variables: <ph id="ph1">`PredictedLabel`</ph>, <ph id="ph2">`Score`</ph>, and <ph id="ph3">`Probability`</ph>; <ph id="ph4">`rx_oneclass_svm`</ph> and regression include one variable: <ph id="ph5">`Score`</ph>; and multi-class classifiers include <ph id="ph6">`PredictedLabel`</ph> plus a variable for each category prepended by <ph id="ph7">`Score`</ph>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>If a <ph id="ph1">`suffix`</ph> is provided, it is added to the end of these output variable names.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`rx_featurize`</ph><ept id="p1">](rx-featurize.md)</ept>, <bpt id="p2">[</bpt>revoscalepy.rx_data_step<ept id="p2">](../revoscalepy/rx-data-step.md)</ept>, <bpt id="p3">[</bpt>revoscalepy.rx_import<ept id="p3">](../revoscalepy/rx-import.md)</ept>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit></group></body></file></xliff>