<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-predict.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c720c92c1d190a2a8c26ac717d2095e9cab9f6118.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">720c92c1d190a2a8c26ac717d2095e9cab9f6118</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-predict.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_predict: Predicted Values and Residuals for rx_lin_mod, rx_logit, rx_dtree, (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Generic function to compute predicted values and residuals using rx_lin_mod, rx_logit, rx_dtree, rx_dforest and rx_btrees objects.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>predict</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rx_predict</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Generic function to compute predicted values and residuals using rx_lin_mod, rx_logit, rx_dtree, rx_dforest and rx_btrees objects.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>model_object</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>object returned from a call to rx_lin_mod, rx_logit, rx_dtree, rx_dforest and rx_btrees.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Objects with multiple dependent variables are not supported.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>a data frame or an RxXdfData data source object to be used for predictions.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If a Spark compute context is being used, this argument may also be an RxHiveData, RxOrcData, RxParquetData or RxSparkDataFrame object or a Spark data frame object from pyspark.sql.DataFrame.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>output_data</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>an RxXdfData data source object or existing data frame to store predictions.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>kwargs</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>additional parameters</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>a data frame or a data source object of prediction results.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`rx_predict_default`</ph><ept id="p1">](rx-predict-default.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`rx_predict_rx_dtree`</ph><ept id="p2">](rx-predict-rx-dtree.md)</ept>, <bpt id="p3">[</bpt><ph id="ph3">`rx_predict_rx_dforest`</ph><ept id="p3">](rx-predict-rx-dforest.md)</ept>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Note: Function <bpt id="p1">*</bpt>rx_predict<ept id="p1">*</ept> does not run predictions but chooses the appropriate function <bpt id="p2">[</bpt><ph id="ph1">`rx_predict_default`</ph><ept id="p2">](rx-predict-default.md)</ept>, <bpt id="p3">[</bpt><ph id="ph2">`rx_predict_rx_dtree`</ph><ept id="p3">](rx-predict-rx-dtree.md)</ept>, or <bpt id="p4">[</bpt><ph id="ph3">`rx_predict_rx_dforest`</ph><ept id="p4">](rx-predict-rx-dforest.md)</ept> based on the model which was given to it.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Each of them has a different set of parameters described by their documentation.</source>
        </trans-unit></group></body></file></xliff>