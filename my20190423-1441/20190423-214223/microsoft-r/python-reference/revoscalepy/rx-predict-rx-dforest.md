<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-predict-rx-dforest.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86afd760c636a853ee9f51176ad2e8b2063c64508a.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">afd760c636a853ee9f51176ad2e8b2063c64508a</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-predict-rx-dforest.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_predict_rx_dforest: Prediction for Large Data Classification and Regression Forests (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Calculate predicted or fitted values for a data set from an rx_dforest or rx_btrees object.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>predict</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rx_predict_rx_dforest</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Calculate predicted or fitted values for a data set from an rx_dforest or rx_btrees object.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>model_object</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>object returned from a call to rx_dtree.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>a data frame or an RxXdfData data source object to be used for predictions.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If a Spark compute context is being used, this argument may also be an RxHiveData, RxOrcData, RxParquetData or RxSparkDataFrame object or a Spark data frame object from pyspark.sql.DataFrame.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>output_data</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>an RxXdfData data source object or existing data frame to store predictions.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>predict_var_names</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>list of strings specifying name(s) to give to the prediction results</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>write_model_vars</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>bool value.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If True, and the output data set is different from the input data set, variables in the model will be written to the output data set in addition to the predictions (and residuals, standard errors, and confidence bounds, if requested).</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If variables from the input data set are transformed in the model, the transformed variables will also be included.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>extra_vars_to_write</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>None or list of strings of additional variables names from the input data or transforms to include in the output_data.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If write_model_vars is True, model variables will be included as well.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>append</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>either “none” to create a new file or “rows” to append rows to an existing file.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If output_data exists and append is “none”, the overwrite argument must be set to True.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>overwrite</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>bool value.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>If True, an existing output_data will be overwritten.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>overwrite is ignored if appending rows.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>type</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>the type of prediction desired.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Supported choices are: “response”, “prob”, and “vote”.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>cutoff</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>(Classification only) a vector of length equal to the number of classes specifying the dividing factors for the class votes.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The default is the one used when the decision forest is built.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>remove_missings</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>bool value.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>If True, rows with missing values are removed.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>compute_residuals</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>bool value.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>If True, residuals are computed.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>residual_type</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Indicates the type of residual desired.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>residual_var_names</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>list of strings specifying name(s) to give to the residual results.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If the data and output_data are the same file, blocks_per_read must be 1.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>integer value with options: 0: no progress is reported.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>1: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>2: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>3: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>If 0, no additional output is printed.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>If 1, additional summary information is printed.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>xdf_compression_level</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>integer in the range of -1 to 9 indicating the compression level for the output data if written to an .xdf file.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>a RxComputeContext object for prediction.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>kwargs</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>additional parameters</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>a data frame or a data source object of prediction results.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`rx_predict`</ph><ept id="p1">](rx-predict.md)</ept>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>