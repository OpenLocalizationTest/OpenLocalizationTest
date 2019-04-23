<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxlineplot.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca8602d907cd1620f89e897e025ed7a6e701f6cbd244.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">02d907cd1620f89e897e025ed7a6e701f6cbd244</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxlineplot.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxLinePlot function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Line or scatter plot using data from an .xdf file or data frame - a wrapper function for xyplot.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxLinePlot, hplot</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxLinePlot: Line Plot</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Line or scatter plot using data from an .xdf file or data frame - a wrapper function for xyplot.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>formula for plot, taking the form of <ph id="ph1">`y~x|g1 + g2`</ph>where <ph id="ph2">`g1`</ph> and <ph id="ph3">`g2`</ph> are optional conditioning factor variables.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>either an RxXdfData object, a character string specifying the .xdf file, or a data frame containing the data to plot.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>name of a logical variable in the data set (in quotes) or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>will use only observations in which the value of the <ph id="ph1">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph2">`log`</ph> of the <ph id="ph3">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations  (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function  call using the expression function.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>an expression of the form <ph id="ph1">`list(name = expression, ...)`</ph> representing variable transformations required for the formula or rowSelection.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>)  can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>a named list containing objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>variable transformation function.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>character vector defining additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and  preloaded for use in variable transformation functions, e.g., those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments or those  defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>user-defined environment to serve as a parent to  all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from  the data source.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>character vector specifying the type of plot.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`"l"`</ph> for line, <ph id="ph2">`"p"`</ph> for points, <ph id="ph3">`"b"`</ph> for both, <ph id="ph4">`"smooth"`</ph> for a  loess fit, <ph id="ph5">`"s"`</ph> for stair steps, or <ph id="ph6">`"r"`</ph> for a regression line.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>main title for the plot.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Alternatively <ph id="ph1">`main`</ph> can be used.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>subtitle (at the bottom) for the plot.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Alternatively <ph id="ph1">`sub`</ph> can be used.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>title for the X axis.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Alternatively <ph id="ph1">`xlab`</ph> can be used.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>title for the Y axis.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Alternatively <ph id="ph1">`ylab`</ph> can be used.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>number of tick marks for numeric X axis.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>number of tick marks for numeric Y axis.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> and more than one line or set of symbols is plotted, a legend is is created.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>character or integer vector specifying line colors for the plot.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>See colors for a list of available colors.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>line style for line plot: <ph id="ph1">`"blank"`</ph>, <ph id="ph2">`"solid"`</ph>, <ph id="ph3">`"dashed"`</ph>, <ph id="ph4">`"dotted"`</ph>, <ph id="ph5">`"dotdash"`</ph>, <ph id="ph6">`"longdash"`</ph>, or <ph id="ph7">`"twodash"`</ph>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Specify <ph id="ph1">`"blank"`</ph> for no line, or set <ph id="ph2">`type`</ph> to <ph id="ph3">`"p"`</ph>.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>a positive number specifiying the line width for line plot.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The interpretation is device-specific.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>character or integer vector denoting the symbol colors.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>See colors for a list of available colors.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>character or integer vector denoting the symbol style(s): <ph id="ph1">`"circle"`</ph>, <ph id="ph2">`"solid circle"`</ph>, <ph id="ph3">`"square"`</ph>, <ph id="ph4">`"solid square"`</ph>, <ph id="ph5">`"triangle"`</ph>, <ph id="ph6">`"solid triangle"`</ph>, <ph id="ph7">`"diamond"`</ph>, <ph id="ph8">`"solid diamond"`</ph>, <ph id="ph9">`"plus"`</ph> (3), <ph id="ph10">`"cross"`</ph> (4), <ph id="ph11">`"down triangle"`</ph> (6), <ph id="ph12">`"square x"`</ph> (7), <ph id="ph13">`"star"`</ph> (8), <ph id="ph14">`"diamond +"`</ph> (9), <ph id="ph15">`"circle +"`</ph> (10), <ph id="ph16">`"up down triangle"`</ph> (11), <ph id="ph17">`"square +"`</ph> (12), <ph id="ph18">`"circle x"`</ph> (13), or any single character.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>numerical value giving the amount by which symbols should be magnified.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>background color for the plot area and legend.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>color for grid lines.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>See colors for a list of available colors.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>line width for grid lines.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>line style for grid lines: <ph id="ph1">`"blank"`</ph>, <ph id="ph2">`"solid"`</ph>, <ph id="ph3">`"dashed"`</ph>, <ph id="ph4">`"dotted"`</ph>, <ph id="ph5">`"dotdash"`</ph>, <ph id="ph6">`"longdash"`</ph>, or <ph id="ph7">`"twodash"`</ph>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the plot is printed.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, and the <bpt id="p1">**</bpt>lattice<ept id="p1">**</ept> package is loaded, an xyplot object is returned invisibly and can be printed later.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Note that the printing of the legend or key will depend on the trellis.par.getsettings at the time of printing.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the underlying xyplot function if loaded.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>is enhanced by the recommended <bpt id="p1">**</bpt>lattice<ept id="p1">**</ept> package.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>an xyplot object if the <bpt id="p1">**</bpt>lattice<ept id="p1">**</ept> is loaded.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Otherwise <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>xyplot, <bpt id="p1">[</bpt>rxHistogram<ept id="p1">](rxHistogram.md)</ept>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>