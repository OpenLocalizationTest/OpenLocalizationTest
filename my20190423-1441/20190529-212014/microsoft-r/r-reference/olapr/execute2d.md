<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="execute2d.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b37aa95d506f0cea626fbd727504beeb05c389b4c3.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">7aa95d506f0cea626fbd727504beeb05c389b4c3</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\olapr\execute2d.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>execute2D function (olapR) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Takes a Query object or an MDX string, and returns the result as a data frame.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(olapR), execute2D</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>execute2D: olapR execute2D Methods</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Takes a Query object or an MDX string, and returns the result as a data frame.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Object of class "OlapConnection" returned by</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Object of class "Query" returned by</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>String specifying a valid MDX query</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If a query is provided: <ph id="ph1">`execute2D`</ph> validates a query object (optional), generates an mdx query string from the query object, executes the mdx query across, and returns the result as a data frame.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If an MDX string is provided: <ph id="ph1">`execute2D`</ph> executes the mdx query, and returns the result as a data frame.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>A data frame if the MDX command returned a result-set.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>and a warning if the query returned no data.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>An error if the query is invalid</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Multi-dimensional query results are flattened to 2D using a standard flattening algorithm.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Creating a Demo OLAP Cube (the same as the one used in the examples): <bpt id="p1">[</bpt><ph id="ph1">`https://msdn.microsoft.com/en-us/library/ms170208.aspx`</ph><ept id="p1">](https://msdn.microsoft.com/en-us/library/ms170208.aspx)</ept></source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Query<ept id="p1">](Query.md)</ept><ph id="ph1">`, `</ph><bpt id="p2">[</bpt>OlapConnection<ept id="p2">](OlapConnection.md)</ept><ph id="ph2">`, `</ph><bpt id="p3">[</bpt>executeMD<ept id="p3">](ExecuteMD.md)</ept><ph id="ph3">`, `</ph><bpt id="p4">[</bpt>explore<ept id="p4">](Explore.md)</ept><ph id="ph4">`, `</ph>data.frame</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>