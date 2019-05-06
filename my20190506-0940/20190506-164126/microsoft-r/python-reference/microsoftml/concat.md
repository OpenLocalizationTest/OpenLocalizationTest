<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="concat.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750606793467d5f6ab4dc9f77f78e5011944c769291.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">606793467d5f6ab4dc9f77f78e5011944c769291</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\concat.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>concat: Machine Learning Concat Transform</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Combines several columns into a single vector-valued column.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>transform, schema</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.concat<ept id="p1">*</ept>: Concatenates multiple columns into a single vector</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Combines several columns into a single vector-valued column.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>creates a single vector-valued column from multiple columns.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>It can be performed on data before training a model.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The concatenation can significantly speed up the processing of data when the number of columns is as large as hundreds to thousands.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>cols</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A character dict or list of variable names to transform.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`dict`</ph>, the keys represent the names of new variables to be created.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Note that all the input variables must be of the same type.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>It is possible to produce multiple output columns with the concatenation transform.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>In this case, you need to use a list of vectors to define a one-to-one mapping between input and output variables.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>For example, to concatenate columns InNameA and InNameB into column OutName1 and also columns InNameC and InNameD into column OutName2, use the dict: dict(OutName1 = [InNameA, InNameB], outName2 = [InNameC, InNameD])</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>kargs</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Additional arguments sent to the compute engine.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>An object defining the concatenation transform.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`drop_columns`</ph><ept id="p1">](drop-columns.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`select_columns`</ph><ept id="p2">](select-columns.md)</ept>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit></group></body></file></xliff>