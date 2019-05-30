<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxnew.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3ef661800ec465764cb848051f1f1edbcfc1c0cd97.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">f661800ec465764cb848051f1f1edbcfc1c0cd97</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxnew.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxNewDataSource function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This is the main generator for RxDataSource S4 classes.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxNewDataSource, rxNewDataSource,character-method, file, connection</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxNewDataSource: RevoScaleR Data Sources: Class Generator</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This is the main generator for RxDataSource S4 classes.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>character name of the specific class to instantiate.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>any other arguments are passed to the class generator <ph id="ph1">`name`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>This is a wrapper to specific class generator functions for the RCE data source classes.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>For example, the RxXdfData class uses function <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> as a generator.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Therefore either <ph id="ph1">`RxXdfData(...)`</ph> or <ph id="ph2">`rxNewDataSource("RxXdfData", ...)`</ph> will create an RxXdfData instance.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>RxDataSource data source object.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>This object may be used to open and close the actual RevoScaleR data sources.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Side Effects</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>This function creates the data source instance in the Microsoft R Services Compute Engine, but does not actually open the data.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The methods <bpt id="p1">[</bpt>rxOpen<ept id="p1">](rxOpen-methods.md)</ept> and <bpt id="p2">[</bpt>rxClose<ept id="p2">](rxOpen-methods.md)</ept> will open and close the data.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept>, <bpt id="p2">[</bpt>RxTextData<ept id="p2">](RxTextData.md)</ept>, <bpt id="p3">[</bpt>RxSasData<ept id="p3">](RxSasData.md)</ept>, <bpt id="p4">[</bpt>RxSpssData<ept id="p4">](RxSpssData.md)</ept>, <bpt id="p5">[</bpt>RxOdbcData<ept id="p5">](RxOdbcData.md)</ept>, <bpt id="p6">[</bpt>RxTeradata<ept id="p6">](RxTeradata.md)</ept>, <bpt id="p7">[</bpt>rxOpen<ept id="p7">](rxOpen-methods.md)</ept>, <bpt id="p8">[</bpt>rxReadNext<ept id="p8">](rxOpen-methods.md)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>