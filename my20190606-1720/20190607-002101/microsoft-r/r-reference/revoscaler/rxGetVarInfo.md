<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxGetVarInfo.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c377efe56c0c0078b3cac027e51d2db6042d771d0b3.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">7efe56c0c0078b3cac027e51d2db6042d771d0b3</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxGetVarInfo.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxGetVarInfo function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Get variable information for a RevoScaleR data source or data frame, including variable names, descriptions, and value labels</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxGetVarInfo, attribute</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxGetVarInfo: Get Variable Information for a Data Source</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Get variable information for a RevoScaleR data source or data frame, including variable names, descriptions, and value labels</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>a data frame, a character string specifying the .xdf file, or an <bpt id="p1">[</bpt>RxDataSource<ept id="p1">](RxDataSource.md)</ept> object.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If a local compute context is being used,  this argument may also be a list of data sources,  in which case the output will be returned in a named list.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>See the details section for more information.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, value labels (including factor  levels) are included in the output if present.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>character vector of variable names for which information is returned.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToDrop`</ph>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>character vector of variable names for which information is not returned.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, argument is ignored.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Cannot be used with <ph id="ph1">`varsToKeep`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>,  variable information  (e.g., high/low values) for non-xdf data sources will be computed  by reading through the data set.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Ignored if the active <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>compute context is local.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Otherwise, if <ph id="ph1">`TRUE`</ph>, a list containing the variable information for the data set on each node in the active compute context will be returned.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, only information on the data set on the master node will be returned.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Will also give partial information for lists and matrices.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If a local compute context is being used, the <ph id="ph1">`data`</ph> and <ph id="ph2">`file`</ph> arguments may be a list of data source objects, e.g., <ph id="ph3">`data = list(iris, airquality, attitude)`</ph>, in which case a named list of results are returned.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxGetVarInfo`</ph>, a mix of supported data sources is allowed.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If the <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept> is distributed, <ph id="ph1">`rxGetVarInfo`</ph> will request information from the compute context nodes.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>list with named elements corresponding to the variables in the data set.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Each list element is also a list with with following possible elements:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>character string specifying the variable description</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>character string specifying the variable type</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>character string specifying the storage type</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>numeric giving the low values, possibly generated through a temporary factor transformation</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>numeric giving the high values, possibly generated through a temporary factor transformation</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>(factor only) a character vector containing the factor levels</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>character vector of value codes, for informational  purposes only</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>character vector of value labels that is the same length as <ph id="ph1">`valueInfoCodes`</ph>, used for informational purposes only</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxSetVarInfo<ept id="p1">](rxSetVarInfoXdf.md)</ept>, <bpt id="p2">[</bpt>rxDataStep<ept id="p2">](rxDataStep.md)</ept>.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>