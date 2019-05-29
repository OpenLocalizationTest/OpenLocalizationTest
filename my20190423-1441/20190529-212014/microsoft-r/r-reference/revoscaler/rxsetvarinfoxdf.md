<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxsetvarinfoxdf.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3a06eb0c8a516fe3c399aa6b0011c194334405adb.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a06eb0c8a516fe3c399aa6b0011c194334405adb</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxsetvarinfoxdf.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxSetVarInfo function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Set the variable information for an .xdf file, including variable names, descriptions, and value labels, or set attributes for variables in a data frame</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxSetVarInfo, rxSetVarInfoXdf, attribute</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxSetVarInfo: Set Variable Information for .xdf File or Data Frame</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Set the variable information for an .xdf file, including variable names, descriptions, and value labels, or set attributes for variables in a data frame</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>list containing lists of variable information for variables in the XDF data source or data frame.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>a data frame, a character string specifying the .xdf file, or an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>character string specifying the .xdf file or   an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The list for each variable contained in <ph id="ph1">`varInfo`</ph> can have the following elements:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>: integer indicating the position of the variable in the data set.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If present, will be used instead of the list name.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>: character string giving a new name for the variable.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>: character string giving a description of the variable.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>: numeric value specifying the low value used in <bpt id="p1">*</bpt>on the fly<ept id="p1">*</ept> factor conversions using the <ph id="ph1">`F()`</ph> transformation.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>: numeric value specifying the high value used in <bpt id="p1">*</bpt>on the fly<ept id="p1">*</ept> factor conversions using the <ph id="ph1">`F()`</ph> transformation.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>: character vector of factor levels.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>This will re-label an existing factor, but not change the underlying values.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>: character vector of value codes for informational purposes only.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>: character vector of value labels the same length as valueInfoCodes, used for informational purposes only.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>: character string giving <ph id="ph1">`tzone`</ph> attribute for a POSIXct variable.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If the input data is a data frame, a data frame is returned containing variables with the new attributes.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If the input data represents an .xdf file or composite file, an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object representing the modified file is returned.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>and <ph id="ph1">`rxSetVarInfo`</ph> do not change the underlying data so the user cannot set the variable type and storage type using this function, or recode the levels of a factor variable.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>To recode factors, use <bpt id="p1">[</bpt>rxFactors<ept id="p1">](rxFactors.md)</ept>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>is not supported for single .xdf files in HDFS.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxDataStep<ept id="p1">](rxDataStep.md)</ept>, <bpt id="p2">[</bpt>rxFactors<ept id="p2">](rxFactors.md)</ept>,</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>