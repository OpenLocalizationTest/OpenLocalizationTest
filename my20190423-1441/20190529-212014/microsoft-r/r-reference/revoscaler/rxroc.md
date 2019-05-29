<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxroc.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3850e996fe66f05753cfe57b9e5e95f8c0b939e03.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">850e996fe66f05753cfe57b9e5e95f8c0b939e03</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxroc.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxRoc function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Compute and plot an ROC curve using actual and predicted values from binary classifier system</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxRoc, rxRocCurve, rxAuc, as.data.frame.rxRoc, plot.rxRoc, rxAuc.rxRoc, hplot</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxRoc:  Receiver Operating Characteristic (ROC) computations and plot</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Compute and plot an ROC curve using actual and predicted values from binary classifier system</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A character string with the name of the variable containing actual (observed) binary values.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>A character string or vector of character strings with the name(s) of the variable  containing predicted values in the [0,1] interval.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>data frame, character string containing an .xdf file name (with path), or  <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object representing an .xdf file containing the actual and observed variables.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>integer specifying the number of breaks to use to determine thresholds for computing the true and false positive rates.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>logical; if <ph id="ph1">`TRUE`</ph>, rows containing duplicate entries for sensitivity and specificity will be removed from the returned data frame.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If performing computations for more than one prediction variable, this implies that there may be a different number of rows for each prediction variable.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the AUC is computed for each prediction variable and printed  in the subtitle or legend text.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>main title for the plot.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Alternatively <ph id="ph1">`main`</ph> can be used.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> a default title will be created.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>subtitle (at the bottom) for the plot.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> and <ph id="ph2">`computeAuc`</ph> is <ph id="ph3">`TRUE`</ph>, the AUC for a single prediction variable will be computed and printed in the subtitle.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>title for the X axis.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Alternatively <ph id="ph1">`xlab`</ph> can be used.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, a default X axis title will be used.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>title for the Y axis.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Alternatively <ph id="ph1">`ylab`</ph> can be used.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, a default Y axis title will be used.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> and more than one prediction variable is specified, a legend is is created.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`computeAuc`</ph> is <ph id="ph2">`TRUE`</ph>, the AUC is computed for each prediction variable and printed in the legend text.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, a grid line from (0,0) to (1,1) is added to represent a pure chance model.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>an rxRoc object.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>an integer or character string specifying the prediction variable for which to extract data frame containing the ROC computations.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If an integer is specified, it will use that as an index to an alphabetized list of <ph id="ph1">`predictionVarNames`</ph>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, all of the computed data will be returned in a data frame.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to an underlying function.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>For plotting functions, these are passed to the  xyplot function.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>computes the sensitivity (true positive rate) and specificity (true negative rate) using a variable containing actual (observed) zero and one values and a variable containing predicted values in the unit interval as the discrimination threshold is varied.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The thresholds are determined by the <ph id="ph1">`numBreaks`</ph> argument.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The computations are done on chunks of data, so that they can be performed on very large data sets.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>If more than one prediction variable is specified, the computations will be performed for each prediction variable.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Observations that have a missing value for the actual value or any of the prediction values are removed before computations are performed.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>and the S3 <ph id="ph1">`plot`</ph> method for an <ph id="ph2">`rxRoc`</ph> object plot the computed sensitivity (true positive rate) versus 1 - specificity (false positive rate).</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>ROC curves were first used during World War II for detecting enemy objects in battle fields.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>returns a data frame of class <ph id="ph1">`"rxRoc"`</ph> containing four variables: <ph id="ph2">`threshold`</ph>, <ph id="ph3">`sensitivity`</ph>, <ph id="ph4">`specificity`</ph>, and <ph id="ph5">`predVarName`</ph> (a factor variable containing the prediction variable name).</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxAuc`</ph> S3 method for an <ph id="ph2">`rxRoc`</ph> object returns the AUC (area under the curve) summary statistic.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxPredict<ept id="p1">](rxPredict.md)</ept>, <bpt id="p2">[</bpt>rxLogit<ept id="p2">](rxLogit.md)</ept>, <bpt id="p3">[</bpt>rxGlm<ept id="p3">](rxGLM.md)</ept>, <bpt id="p4">[</bpt>rxLinePlot<ept id="p4">](rxLinePlot.md)</ept>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>