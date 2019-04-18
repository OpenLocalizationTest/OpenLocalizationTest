<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxresultsdf.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f9bbdead225b22b5758f46f1802f149a1acad3033.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9bbdead225b22b5758f46f1802f149a1acad3033</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxresultsdf.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxResultsDF function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Obtain a counts, sums, or means data frame from an analysis object.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxResultsDF, rxResultsDF.rxCrossTabs, rxResultsDF.rxCube, rxResultsDF.rxLinMod, rxResultsDF.rxLogit, rxResultsDF.rxSummary, category, models</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxResultsDF: Crosstab Counts or Sums Data Frame</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Obtain a counts, sums, or means data frame from an analysis object.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>object of class rxCrossTabs, rxCube, rxLinMod, rxLogit, or rxSummary.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>character string specifying the type of output to display.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Typically this is <ph id="ph1">`"counts"`</ph>, or for <ph id="ph2">`rxSummary`</ph> <ph id="ph3">`"stats"`</ph>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If there is a  dependent variable in the <ph id="ph1">`rxCrossTabs`</ph> formula, <ph id="ph2">`"sums"`</ph> and <ph id="ph3">`"means"`</ph>can be used.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>integer specifying the element number from the object list to extract.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Currently only <ph id="ph1">`1`</ph> is supported.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>logical scalar or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the  first column of the returned data frame will be converted to integers.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, it will be a factor column.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, it will be returned as an integer column if it was wrapped in an <ph id="ph2">`F()`</ph> in the formula.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the  counts or sums in the returned data frame will be converted to integers.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, they will be numeric doubles.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the names of the variables for  which there are results will be put into the row names for the data frame   rather than in a separate <ph id="ph2">`Names`</ph> variable.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the underlying print method for the output list object.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Method to access counts, sums, and means data frames from RevoScaleR analysis objects.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>a data frame containing the computed counts, sums, or means.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxCrossTabs<ept id="p1">](rxCrossTabs.md)</ept><ph id="ph1">
</ph><bpt id="p2">[</bpt>rxCube<ept id="p2">](rxCube.md)</ept><ph id="ph2">
</ph><bpt id="p3">[</bpt>rxLinMod<ept id="p3">](rxLinMod.md)</ept><ph id="ph3">
</ph><bpt id="p4">[</bpt>rxLogit<ept id="p4">](rxLogit.md)</ept><ph id="ph4">
</ph><bpt id="p5">[</bpt>rxSummary<ept id="p5">](rxSummary.md)</ept><ph id="ph5">
</ph><bpt id="p6">[</bpt>rxMarginals<ept id="p6">](rxMarginals.md)</ept></source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>