<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxPredict.rxNaiveBayes.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b31c688d7ec25dc4cf499a7fff9a8cd50c8df539ea.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1c688d7ec25dc4cf499a7fff9a8cd50c8df539ea</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxPredict.rxNaiveBayes.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxPredict.rxNaiveBayes function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxPredict.rxNaiveBayes, models, tree, classif, classification</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>rxPredict.rxNaiveBayes: Prediction for Large Data Naive Bayes Classifiers</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Calculate predicted or fitted values for a data set from an rxNaiveBayes object.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>object returned from a call to <bpt id="p1">[</bpt>rxNaiveBayes<ept id="p1">](rxNaiveBayes.md)</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>either a data source object, a character string  specifying a .xdf file, or a data frame object.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>file or existing data frame to store predictions;  can be same as the input file or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If not <ph id="ph1">`NULL`</ph>, must be an .xdf file if <ph id="ph2">`data`</ph> is an .xdf file  or a data frame if <ph id="ph3">`data`</ph> is a data frame.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>character string specifying the type of predicted values to be returned.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Supported choices are</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>-  a vector of predicted classes.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>-  a matrix of predicted class probabilities whose columns are the probability of the first, second, etc. class.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>a vector of prior probabilities.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If unspecified, the class proportions of the data counts in the training set are used.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If present, they should be specified in the order of the factor levels of the response and they must be all non-negative and sum to 1.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>character vector specifying name(s) to give to the prediction results.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, and the output file is different from the input file,  variables in the model will be written to the output file in addition to the predictions.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If variables from the input data set are transformed in the model,  the transformed variables will also be written out.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>or character vector of additional variables names from the input data to include in the <ph id="ph1">`outData`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`writeModelVars`</ph> is <ph id="ph2">`TRUE`</ph>,  model variables will be included as well.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the factor levels for the data  will be verified against factor levels in the model.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Setting to <ph id="ph1">`FALSE`</ph> can speed up computations if using lots of factors.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to <bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxDataStep.md)</ept> such as <ph id="ph1">`removeMissingsOnRead`</ph>, <ph id="ph2">`overwrite`</ph>,  <ph id="ph3">`blocksPerRead`</ph>, <ph id="ph4">`reportProgress`</ph>, <ph id="ph5">`xdfCompressionLevel`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Prediction for large data models requires both a fitted model object and a data set, either the original data (to obtain fitted values and residuals) or a new data set containing the same set of variables as the original fitted model.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Notice that this is different from the behavior of <ph id="ph1">`predict`</ph>, which can usually work on the original data simply by referencing the fitted model.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Depending on the form of <ph id="ph1">`data`</ph>, this function variously returns a data frame or a data source representing a .xdf file.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Naive Bayes classifier <bpt id="p1">[</bpt><ph id="ph1">`https://en.wikipedia.org/wiki/Naive_Bayes_classifier`</ph><ept id="p1">](https://en.wikipedia.org/wiki/Naive_Bayes_classifier)</ept></source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxNaiveBayes<ept id="p1">](rxNaiveBayes.md)</ept>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>