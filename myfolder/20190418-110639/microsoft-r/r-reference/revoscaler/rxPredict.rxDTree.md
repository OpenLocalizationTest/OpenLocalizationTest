<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxPredict.rxDTree.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f710776345aa145cf9eb819b50c0625bc9a6c6620.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">710776345aa145cf9eb819b50c0625bc9a6c6620</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxPredict.rxDTree.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxPredict.rxDTree function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxPredict.rxDTree, models, tree, classif, regression, classification</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>rxPredict.rxDTree: Prediction for Large Data Classification and Regression Trees</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Calculate predicted or fitted values for a data set from an rxDTree object.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>object returned from a call to <ph id="ph1">`rxDTree`</ph>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>either a data source object, a character string  specifying a .xdf file, or a data frame object.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>file or existing data frame to store predictions;  can be same as the input file or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If not <ph id="ph1">`NULL`</ph>, must be an .xdf file if <ph id="ph2">`data`</ph> is an .xdf file  or a data frame if <ph id="ph3">`data`</ph> is a data frame.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>character vector specifying name(s) to give to the prediction results.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, and the output file is different from the input file,  variables in the model will be written to the output file in addition to the predictions.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If variables from the input data set are transformed in the model,  the transformed variables will also be written out.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or character vector of additional variables names from the input data or transforms to include in the <ph id="ph2">`outData`</ph>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`writeModelVars`</ph> is <ph id="ph2">`TRUE`</ph>, model variables will be included as well.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>either <ph id="ph1">`"none"`</ph> to create a new files or <ph id="ph2">`"rows"`</ph> to append rows to an existing file.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outData`</ph> exists and <ph id="ph2">`append`</ph> is <ph id="ph3">`"none"`</ph>, the <ph id="ph4">`overwrite`</ph> argument must be set to <ph id="ph5">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>You can append only to <bpt id="p1">[</bpt>RxTeradata<ept id="p1">](RxTeradata.md)</ept> data source.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outData`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`overwrite`</ph> is ignored if appending rows.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>see predict.rpart for details.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, rows with missing values are removed and  will not be included in the output data.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, residuals are computed.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>see residuals.rpart for details.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>character vector specifying name(s) to give to the residual results.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data  read from the data source.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Integer values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information are provided.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>integer in the range of -1 to 9 indicating the compression level for the output data if written to an <ph id="ph1">`.xdf`</ph> file.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the amount of compression - resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`xdfCompressionLevel`</ph> is set to 0, there will be no compression and files will be compatible with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression will be used.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Microsoft R Services Compute Engine.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Prediction for large data models requires both a fitted model object and a data set, either the original data (to obtain fitted values and residuals) or a new data set containing the same set of variables as the original fitted model.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Notice that this is different from the behavior of <ph id="ph1">`predict`</ph>, which can usually work on the original data simply by referencing the fitted model.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Depending on the form of <ph id="ph1">`data`</ph>, this function variously returns a data frame or a data source representing a .xdf file.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Breiman, L., Friedman, J. H., Olshen, R. A.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>and Stone, C. J.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>(1984) <bpt id="p1">*</bpt>Classification and Regression Trees<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Wadsworth.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Therneau, T. M.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>and Atkinson, E. J.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>(2011) <bpt id="p1">*</bpt>An Introduction to Recursive Partitioning Using the RPART Routines<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Yael Ben-Haim and Elad Tom-Tov (2010) A streaming parallel decision tree algorithm.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Journal of Machine Learning Research<ept id="p1">*</ept> <bpt id="p2">**</bpt>11<ept id="p2">**</ept>, 849--872.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>rpart, rpart.control, rpart.object, <bpt id="p1">[</bpt>rxDTree<ept id="p1">](rxDTree.md)</ept>.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>