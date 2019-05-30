<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxgetinfoxdf.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e34154b9bad8413ac559d6eb1a528305f42499759.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">34154b9bad8413ac559d6eb1a528305f42499759</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxgetinfoxdf.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxGetInfo function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Get basic information about an RevoScaleR data source or data frame</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxGetInfo, attribute</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxGetInfo: Get Data Source Information</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Get basic information about an RevoScaleR data source or data frame</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>a data frame, a character string specifying an .xdf, or an <bpt id="p1">[</bpt>RxDataSource<ept id="p1">](RxDataSource.md)</ept> object.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If a local compute context is being used,  this argument may also be a list of data sources,  in which case the output will be returned in a named list.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>See the details section for more information.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, variable information is returned.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, block sizes are returned in the output for an .xdf file, and when printed the first 10 block sizes are shown.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> and <ph id="ph2">`getVarInfo`</ph> is <ph id="ph3">`TRUE`</ph> or <ph id="ph4">`NULL`</ph>, factor value labels are included in the output.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>character vector of variable names for which information is returned.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> or <ph id="ph2">`getVarInfo`</ph> is <ph id="ph3">`FALSE`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToDrop`</ph>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>character vector of variable names for which information is not returned.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> or <ph id="ph2">`getVarInfo`</ph> is <ph id="ph3">`FALSE`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToKeep`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>starting row for retrieval of data if a data frame or .xdf file.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>number of rows of data to retrieve if a data frame or .xdf file.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, and <ph id="ph2">`getVarInfo`</ph> is <ph id="ph3">`TRUE`</ph>, variable information  (e.g., high/low values) for non-xdf data sources will be computed  by reading through the data set.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, and <ph id="ph2">`getVarInfo`</ph> is <ph id="ph3">`FALSE`</ph>, the number of variables will be gotten from from non-xdf data sources  (but not the number of rows).</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Ignored if the active <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept> compute context is local or <ph id="ph1">`RxForeachDoPar`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Otherwise, if <ph id="ph1">`TRUE`</ph>, a list containing the information for the data set on each node in the active compute context will be returned.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, only information on the data set on the master node will be returned.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Note that the determination of the master node is not controlled by the end user.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">*</bpt>RevoScaleR Distributed Computing Guide<ept id="p1">*</ept> for more information on master node computations.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, additional summary information is printed for an .xdf file.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If a local compute context is being used, the <ph id="ph1">`data`</ph> and <ph id="ph2">`file`</ph> arguments may be a list of data source objects, e.g., <ph id="ph3">`data = list(iris, airquality, attitude)`</ph>, in which case a named list of results are returned.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxGetInfo`</ph>, a mix of supported data sources is allowed.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Note that data frames should not be specified in quotes because, in that case, they will be interpreted as .xdf data paths.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>If the <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept> is distributed, <ph id="ph1">`rxGetInfo`</ph> will request information from the compute context nodes.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>list containing the following possible elements:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>character string containing the file name and path (if an .xdf file).</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>character string containing object name (if not an .xdf file).</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>class of the object if an R object.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>length of the object if it is not an .xdf file or data frame.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>number of composite data files(if a composite .xdf file).</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>number of rows in the data set.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>number of variables in the data set.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>number of blocks in the data set.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>list of variable information where each element is a list describing a variable.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>(See return value of <bpt id="p1">[</bpt>rxGetVarInfo<ept id="p1">](rxGetVarInfo.md)</ept> for more information.)</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>integer vector containing number of rows in each block (if <ph id="ph1">`getBlockSizes`</ph> is set to <ph id="ph2">`TRUE`</ph>).</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Set to <ph id="ph1">`NULL`</ph> if <ph id="ph2">`data`</ph> is a data frame.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>data frame containing the data (if <ph id="ph1">`numRows &gt; 0`</ph>)</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If using a distributed compute context with the <ph id="ph1">`allNodes`</ph> set to <ph id="ph2">`TRUE`</ph>, a list of lists with information on the data from each node will be returned.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxDataStep.md)</ept>, <bpt id="p2">[</bpt>rxGetVarInfo<ept id="p2">](rxGetVarInfo.md)</ept>, <bpt id="p3">[</bpt>rxSetVarInfo<ept id="p3">](rxSetVarInfoXdf.md)</ept>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>