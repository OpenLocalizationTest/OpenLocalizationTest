<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="mlmodel.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3f801904ef6e54c045767a861f7458934da72649e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">f801904ef6e54c045767a861f7458934da72649e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\mlmodel.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>summary.mlModel function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Summary of a Microsoft R Machine Learning model.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), summary.mlModel, coef.mlModel, file, manip</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>summary.mlModel: Summary of a Microsoft R Machine Learning model.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Summary of a Microsoft R Machine Learning model.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A model object returned from a <bpt id="p1">**</bpt>MicrosoftML<ept id="p1">**</ept> analysis.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Specifies the count of top coefficients to show in the summary for linear models such as <bpt id="p1">[</bpt>rxLogisticRegression<ept id="p1">](rxLogisticRegression.md)</ept> and  <bpt id="p2">[</bpt>rxFastLinear<ept id="p2">](rxFastLinear.md)</ept>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The bias appears first, followed by other weights, sorted by their absolute values in descending order.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If set to <ph id="ph1">`NULL`</ph>,  all non-zero coefficients are shown.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Otherwise, only the first <ph id="ph1">`top`</ph>coefficients are shown.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed to the summary method.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Provides summary information about the original function call, the</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>data set used to train the model, and statistics for coefficients in the model.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`summary`</ph> method of the <bpt id="p1">**</bpt>MicrosoftML<ept id="p1">**</ept> analysis objects returns a list that includes the original function call and the underlying parameters used.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`coef`</ph> method returns a named vector of weights, processing information from the model object.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">[</bpt>rxLogisticRegression<ept id="p1">](rxLogisticRegression.md)</ept>, the following statistics may also present in the summary when <ph id="ph1">`showTrainingStats`</ph> is set to <ph id="ph2">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The size, in terms of row count, of the data set used to train the model.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The model deviance is given by <ph id="ph1">`-2 * ln(L)`</ph> where <ph id="ph2">`L`</ph> is the likelihood of obtaining the observations with all features incorporated in the model.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The null deviance is given by <ph id="ph1">`-2 * ln(L0)`</ph> where <ph id="ph2">`L0`</ph> is the likelihood of obtaining the observations with no effect from the features.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The null model includes the bias if there is one in the model.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The AIC (Akaike Information Criterion) is defined as <ph id="ph1">`2 * k ``+ deviance`</ph>, where <ph id="ph2">`k`</ph> is the number of coefficients of the model.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The bias counts as one of the coefficients.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The AIC is a measure of the relative quality of the model.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>It deals with the trade-off between the goodness of fit of the model (measured by deviance) and the complexity of the model (measured by number of coefficients).</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>This is a data frame containing the statistics for each coefficient in the model.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>For each coefficient, the following statistics are shown.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The bias appears in the first row, and the remaining coefficients in the ascending order of p-value.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>EstimateThe estimated coefficient value of the model.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Std ErrorThis is the square root of the large-sample variance of the estimate of the coefficient.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>z-ScoreWe can test against the null hypothesis, which states that the coefficient should be zero, concerning the significance of the coefficient by calculating the ratio of its estimate and its standard error.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Under the null hypothesis, if there is no regularization applied, the estimate of the concerning coefficient follows a normal distribution with mean 0 and a standard deviation equal to the standard error computed above.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The z-score outputs the ratio between the estimate of a coefficient and the standard error of the coefficient.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Pr(&gt;|z|) This is the corresponding p-value for the two-sided test of the z-score.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Based on the significance level, a significance indicator is appended to the p-value.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`F(x)`</ph> is the CDF of the standard normal distribution <ph id="ph2">`N(0, 1)`</ph>, then <ph id="ph3">`P(&gt;|z|) = 2 - ``2 * F(|z|)`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxFastTrees<ept id="p1">](rxFastTrees.md)</ept>, <bpt id="p2">[</bpt>rxFastForest<ept id="p2">](rxFastForest.md)</ept>, <bpt id="p3">[</bpt>rxFastLinear<ept id="p3">](rxFastLinear.md)</ept>, <bpt id="p4">[</bpt>rxOneClassSvm<ept id="p4">](rxOneClassSvm.md)</ept>, <bpt id="p5">[</bpt>rxNeuralNet<ept id="p5">](rxNeuralNet.md)</ept>, <bpt id="p6">[</bpt>rxLogisticRegression<ept id="p6">](rxLogisticRegression.md)</ept>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>