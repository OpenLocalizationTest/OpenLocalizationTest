<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="query.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef0690673356cbe7ea731d91fca1ec9aca7987c981aaf0cd216.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">6cbe7ea731d91fca1ec9aca7987c981aaf0cd216</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\olapr\query.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Query function (olapR) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Query constructs a Query object.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Set functions are used to build and modify the Query axes and cube name.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(olapR), Query</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Query: olapR Query Construction</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`Query`</ph> constructs a "Query" object.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Set functions are used to build and modify the Query axes and cube name.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>A logical (TRUE, FALSE, NA) specifying whether the Query should be validated during execution</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>An object of class "Query" returned by <ph id="ph1">`Query`</ph></source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>A string specifying the name of the cube to query</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A vector of strings specifying an axis.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>See example below.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>An integer representing the axis number to be set.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>axis(qry, 1) == columns(qry), axis(qry, 2) == pages(qry), etc.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`Query`</ph> is the constructor for the Query object.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Set functions are used to specify what the Query should return.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Queries are passed to the <ph id="ph1">`Execute2D`</ph> and <ph id="ph2">`ExecuteMD`</ph> functions.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`compose`</ph> takes the Query object and generates an MDX string equivalent to the one that the Execute functions would generate and use.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`Query`</ph> returns an object of type "Query".</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`cube`</ph> returns a string.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`columns`</ph> returns a vector of strings.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rows`</ph> returns a vector of strings.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`pages`</ph> returns a vector of strings.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`sections`</ph> returns a vector of strings.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`axis`</ph> returns a vector of strings.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`slicers`</ph> returns a vector of strings.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`compose`</ph> returns a string.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`is.Query`</ph> returns a boolean.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>A Query object is not as powerful as pure MDX.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If the Query API is not sufficient, try using an MDX Query string with one of the Execute functions.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>execute2D<ept id="p1">](Execute2D.md)</ept> or <bpt id="p2">[</bpt>executeMD<ept id="p2">](ExecuteMD.md)</ept> for references.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>execute2D<ept id="p1">](Execute2D.md)</ept>, <bpt id="p2">[</bpt>executeMD<ept id="p2">](ExecuteMD.md)</ept>, <bpt id="p3">[</bpt>OlapConnection<ept id="p3">](OlapConnection.md)</ept><ph id="ph1">`, `</ph><bpt id="p4">[</bpt>explore<ept id="p4">](Explore.md)</ept></source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>