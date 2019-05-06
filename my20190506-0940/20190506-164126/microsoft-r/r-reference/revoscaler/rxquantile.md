<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxquantile.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc775063e2f6b1b254b0adabc6708c902ae7c5a39d36a7.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">63e2f6b1b254b0adabc6708c902ae7c5a39d36a7</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxquantile.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxQuantile function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Quickly computes approximate quantiles (without sorting)</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxQuantile, univar</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxQuantile:  Approximate Quantiles for .xdf Files and Data Frames</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Quickly computes approximate quantiles (without sorting)</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A character string containing the name of the numeric variable for which to compute the quantiles.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>data frame, character string containing an .xdf file name (with path), or  <bpt id="p1">[</bpt>RxDataSource-class<ept id="p1">](RxDataSource-class.md)</ept> object representing the data set.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as frequency weights for the observations.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>numeric vector of probabilities with values in the [0,1] range.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>logical; if <ph id="ph1">`TRUE`</ph>, the result has a <ph id="ph2">`names`</ph> attribute.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>integer.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The maximum number of integer bins to use for integer data.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>For exact results, this should be larger than the range of data.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>However, larger values may increase memory requirements and computational time.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>numeric value to multiply data values by before computing integer bins.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, do not use integer approximations for bins.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>integer.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The number of breaks to use in computing numeric bins. Ignored if <ph id="ph1">`numericBins`</ph> is <ph id="ph2">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from an <ph id="ph1">`.xdf`</ph> data source.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, additional computational information may be printed.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>rxQuantiles computes approximate quantiles by counting binned data, then computing a linear interpolation of the empirical cdf for continuous data or the inverse of empirical distribution function for integer data.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If the binned data are integers, or can be converted to integers by multiplication, the computation is exact when integral bins are used.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The size of the bins can be controlled by using the <ph id="ph1">`multiple`</ph> function if desired.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Missing values are removed before computing the quantiles.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>A vector the length of <ph id="ph1">`probs`</ph> is returned; if <ph id="ph2">`names = TRUE`</ph>, it has a names attribute.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>quantile, <bpt id="p1">[</bpt>rxCube<ept id="p1">](rxCube.md)</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>