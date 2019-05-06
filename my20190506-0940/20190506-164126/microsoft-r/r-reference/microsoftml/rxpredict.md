<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxpredict.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc77504a5e33a88bb66a9eb3525b1a8178e3af99ddbc2b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">4a5e33a88bb66a9eb3525b1a8178e3af99ddbc2b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\rxpredict.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxPredict.mlModel function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Reports per-instance scoring results in a data frame or RevoScaleR data source using a trained Microsoft R Machine Learning model with a RevoScaleR data source.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), rxPredict.mlModel, manip</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxPredict.mlModel: Score using a Microsoft R Machine Learning model</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Reports per-instance scoring results in a data frame or RevoScaleR data source using a trained Microsoft R Machine Learning model with a RevoScaleR data source.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A model information object returned from a MicrosoftML model.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>For example, an object returned from <bpt id="p1">[</bpt>rxFastTrees<ept id="p1">](rxFastTrees.md)</ept> or <bpt id="p2">[</bpt>rxLogisticRegression<ept id="p2">](rxLogisticRegression.md)</ept>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> data source object, a data frame, or the path to a <ph id="ph1">`.xdf`</ph> file.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Output text or xdf file name or an <ph id="ph1">`RxDataSource`</ph> with write capabilities in which to store predictions.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, a data frame is returned.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, variables in the model are written to the output data set in addition to the scoring variables.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If variables from the input data set are transformed in the model, the transformed variables are also included.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>or character vector of additional variables names from the input data to include in the <ph id="ph1">`outData`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`writeModelVars`</ph> is <ph id="ph2">`TRUE`</ph>, model variables are included as well.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>A character string specifying suffix to append to the created  scoring variable(s) or <ph id="ph1">`NULL`</ph> in there is no suffix.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The default  value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outData`</ph> is overwritten; if <ph id="ph3">`FALSE`</ph> an existing <ph id="ph4">`outData`</ph> is not overwritten.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The default  value is <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>An integer specifying the desired degree of parallelism in the data pipeline.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the number of threads used is determined internally.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Specifies the number of blocks to read for each chunk  of data read from the data source.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the level of reporting  on the row processing progress:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`1`</ph>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>An integer value that specifies the amount of output wanted.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Integer  values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`1`</ph>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Sets the context in which computations are executed, specified with a valid RxComputeContext.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Currently local and RxInSqlServer compute contexts are supported.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed directly to the Microsoft Compute Engine.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The following items are reported in the output by default: scoring on three variables for the binary classifiers: PredictedLabel, Score, and Probability; the Score for oneClassSvm and regression classifiers; PredictedLabel for Multi-class classifiers, plus a variable for each category prepended by the Score.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>A data frame or an RxDataSource object representing the created output data.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>By default, output from scoring binary classifiers include three variables: <ph id="ph1">`PredictedLabel`</ph>, <ph id="ph2">`Score`</ph>, and <ph id="ph3">`Probability`</ph>; <ph id="ph4">`rxOneClassSvm`</ph> and regression include one variable: <ph id="ph5">`Score`</ph>; and multi-class classifiers include <ph id="ph6">`PredictedLabel`</ph> plus a variable for each category prepended by <ph id="ph7">`Score`</ph>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If a <ph id="ph1">`suffix`</ph> is provided, it is added to the end of these output variable names.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxFastTrees<ept id="p1">](rxFastTrees.md)</ept>, <bpt id="p2">[</bpt>rxFastForest<ept id="p2">](rxFastForest.md)</ept>, <bpt id="p3">[</bpt>rxLogisticRegression<ept id="p3">](rxLogisticRegression.md)</ept>, <bpt id="p4">[</bpt>rxNeuralNet<ept id="p4">](rxNeuralNet.md)</ept>, <bpt id="p5">[</bpt>rxOneClassSvm<ept id="p5">](rxOneClassSvm.md)</ept>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>