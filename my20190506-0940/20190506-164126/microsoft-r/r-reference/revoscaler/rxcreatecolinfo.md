<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxcreatecolinfo.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc77502fb609dfc55b3b3ddfa4abd5d895ae0d9530bfa4.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">2fb609dfc55b3b3ddfa4abd5d895ae0d9530bfa4</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxcreatecolinfo.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxCreateColInfo function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Generates a colInfo list from a data source that can be used in rxImport or an RxDataSource constructor.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxCreateColInfo, file, connection</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxCreateColInfo:  Function to generate a 'colInfo' list from a data source</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Generates a <ph id="ph1">`colInfo`</ph> list from a data source that can be used in <ph id="ph2">`rxImport`</ph> or an <ph id="ph3">`RxDataSource`</ph> constructor.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>An <bpt id="p1">[</bpt>RxDataSource<ept id="p1">](RxDataSource.md)</ept> object, a character string containing an .xdf file name, or a data frame.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>An object returned from <bpt id="p1">[</bpt>rxGetVarInfo<ept id="p1">](rxGetVarInfo.md)</ept> is also supported.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the low/high values will be included in the <ph id="ph2">`colInfo`</ph> object.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Note that this will override any actual low/high values in the data set if the <ph id="ph1">`colInfo`</ph> object is applied to a different data source.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, only column information for factor variables will be included in the output.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>to include all variables, or character vector of variables to include.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, factor levels will be sorted.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If factor levels represent integers, they will be put in numeric order.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, a pass through the data will be taken for non-xdf data sources in order to compute factor levels and low/high values.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the <ph id="ph2">`factorIndex`</ph> variable type will be used instead of <ph id="ph3">`factor`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>This function can be used to ensure consistent factor levels when importing a series of text files to xdf.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>It is also useful for repeated analysis on non-xdf data sources.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>A <ph id="ph1">`colInfo`</ph> list that can be used as input for <bpt id="p1">[</bpt>rxImport<ept id="p1">](rxImport.md)</ept> and in data sources such as <bpt id="p2">[</bpt>RxTextData<ept id="p2">](RxTextData.md)</ept> and <bpt id="p3">[</bpt>RxSqlServerData<ept id="p3">](RxSqlServerData.md)</ept>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxDataSource-class<ept id="p1">](RxDataSource-class.md)</ept>, <bpt id="p2">[</bpt>RxTextData<ept id="p2">](RxTextData.md)</ept>, <bpt id="p3">[</bpt>RxSqlServerData<ept id="p3">](RxSqlServerData.md)</ept>, <bpt id="p4">[</bpt>RxSpssData<ept id="p4">](RxSpssData.md)</ept>, <bpt id="p5">[</bpt>RxSasData<ept id="p5">](RxSasData.md)</ept>, <bpt id="p6">[</bpt>RxOdbcData<ept id="p6">](RxOdbcData.md)</ept>, <bpt id="p7">[</bpt>RxTeradata<ept id="p7">](RxTeradata.md)</ept>, <bpt id="p8">[</bpt>RxXdfData<ept id="p8">](RxXdfData.md)</ept>, <bpt id="p9">[</bpt>rxImport<ept id="p9">](rxImport.md)</ept>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>