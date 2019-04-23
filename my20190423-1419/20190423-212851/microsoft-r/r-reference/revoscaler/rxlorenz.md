<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxlorenz.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a6bf44e8a02865b2efb54f8af9189e7cb6d781c42.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">6bf44e8a02865b2efb54f8af9189e7cb6d781c42</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxlorenz.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxLorenz function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Compute and plot an empirical Lorenz curve from a variable in a data set, optionally specifiying a separate variable from which to compute the y-values for the curve.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Compute the Gini Coefficient from the Lorenz curve data.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Appropriate for big data sets since data is binned with computations performed in one pass, rather than sorting the data as part of the computation process.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxLorenz, rxGini, rxGini.rxLorenz, plot.rxLorenz,  univar</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>rxLorenz:  Lorenz Curve and Gini Coefficient</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Compute and plot an empirical Lorenz curve from a variable in a data set, optionally specifiying a separate variable from which to compute the y-values for the curve.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Compute the Gini Coefficient from the Lorenz curve data.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Appropriate for big data sets since data is binned with computations performed in one pass, rather than sorting the data as part of the computation process.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>A character string with the name of the variable to use in computing approximate quantiles.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A character string with the name of the variable to use to compute the mean values per quantile.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Can be the same as <ph id="ph1">`orderVarName`</ph>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>data frame, character string containing an .xdf file name (with path), or  <bpt id="p1">[</bpt>RxDataSource-class<ept id="p1">](RxDataSource-class.md)</ept> object representing a data set containing the actual and observed variables.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>integer specifiying the number of breaks to use in comuting approximate quantiles.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as frequency weights for the observations.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, additional information is printed as summary statistics are computed.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>output object from rxLorenz function.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>main title for the plot.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>subtitle (at the bottom) for the plot.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>title for the X axis.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>title for the Y axis.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>character or integer vector specifying line color for the Lorenz curve.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>See colors for a list of available colors.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>line style for line plot: <ph id="ph1">`"blank"`</ph>, <ph id="ph2">`"solid"`</ph>, <ph id="ph3">`"dashed"`</ph>, <ph id="ph4">`"dotted"`</ph>, <ph id="ph5">`"dotdash"`</ph>, <ph id="ph6">`"longdash"`</ph>, or <ph id="ph7">`"twodash"`</ph>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Specify <ph id="ph1">`"blank"`</ph> for no line, or set <ph id="ph2">`type`</ph> to <ph id="ph3">`"p"`</ph>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>a positive number specifiying the line width for line plot.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The interpretation is device-specific.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, a diagonal grid line will be drawn representing complete equality.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>character or integer vector specifying line color for the equality grid line.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the color of other grid lines will be used.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>line style for the equality grid line: <ph id="ph1">`"blank"`</ph>, <ph id="ph2">`"solid"`</ph>, <ph id="ph3">`"dashed"`</ph>, <ph id="ph4">`"dotted"`</ph>, <ph id="ph5">`"dotdash"`</ph>, <ph id="ph6">`"longdash"`</ph>, or <ph id="ph7">`"twodash"`</ph>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the style of other gride lines will be used.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>a positive number specifiying the line width for line plot.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the width of other grid lines will be used.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed to <ph id="ph1">`xyplot`</ph>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>computes the cumulative percentage values of the variable specified in <ph id="ph1">`valueVarName`</ph> for groups binned by the <ph id="ph2">`orderVarname`</ph>.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The size of the bins is determined by <ph id="ph1">`numBreaks`</ph>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>When plotted, the cumulative percentage values are plotted against the quantile percentages.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The Gini coefficient is computed by estimating the ratio of the area between the line of equality and the Lorenz curve to the total area under the line of equality (using trapezoidal integration).</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The Gini coefficient can range from 0 to 1, with 0 representing perfect equality.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Precision can be increased by increasing <ph id="ph1">`numBreaks`</ph>.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>returns a data frame of class <ph id="ph1">`"rxLorenz"`</ph> containing two variables: <ph id="ph2">`cumVals`</ph> and <ph id="ph3">`percent`</ph>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>It also may have a <ph id="ph1">`"description"`</ph> attribute containing the value variable name or description.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>returns a numeric vector of length one containing the approximate Gini coefficient.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxPredict<ept id="p1">](rxPredict.md)</ept>, <bpt id="p2">[</bpt>rxLogit<ept id="p2">](rxLogit.md)</ept>, <bpt id="p3">[</bpt>rxGlm<ept id="p3">](rxGLM.md)</ept>, <bpt id="p4">[</bpt>rxLinePlot<ept id="p4">](rxLinePlot.md)</ept>, <bpt id="p5">[</bpt>rxQuantile<ept id="p5">](rxQuantile.md)</ept>, <bpt id="p6">[</bpt>rxRoc<ept id="p6">](rxRoc.md)</ept>.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>