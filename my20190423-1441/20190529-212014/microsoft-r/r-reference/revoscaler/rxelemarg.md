<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxelemarg.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b32dc07d4fe98018f450ec5273e4b3cd1d6f2fa331.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">2dc07d4fe98018f450ec5273e4b3cd1d6f2fa331</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxelemarg.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxElemArg function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Allows different argument values to be passed to different (named and unnamed) nodes or cores through the elipsis argument for rxExec.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>A vector or list of the argument values is used.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxElemArg, IO</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>rxElemArg:  Helper function for rxExec arguments</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Allows different argument values to be passed to different (named and unnamed) nodes or cores through the elipsis argument for rxExec.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>A vector or list of the argument values is used.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The list or vector to be applied across the set of computations.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>This function is designed for use only within a call to <bpt id="p1">[</bpt>rxExec<ept id="p1">](rxExec.md)</ept>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxExec<ept id="p1">](rxExec.md)</ept> allows for the processing of a user function on multiple nodes or cores.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Arguments for the user function can be passed directly through the call to <bpt id="p1">[</bpt>rxExec<ept id="p1">](rxExec.md)</ept>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>By default, the same argument value will be passed to each of the nodes or cores.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If instead, a vector or list of argument values is wrapped in a call to <ph id="ph1">`rxElemArg`</ph>, a distinct argument value will be passed to each node or core.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`timesToRun`</ph> is specified for <bpt id="p1">[</bpt>rxExec<ept id="p1">](rxExec.md)</ept>, the length of the vector or list within <ph id="ph2">`rxElemsArg`</ph> must have a length equalto <ph id="ph3">`timesToRun`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`timesToRun`</ph> is not specified and the <ph id="ph2">`elemType`</ph> is set to <ph id="ph3">`"cores"`</ph>, the length of the vector or list will determine the <ph id="ph4">`timesToRun`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`elemArgs`</ph> is used in addition to the <ph id="ph2">`rxElemArg`</ph> function, the length of both lists/vectors must be the same.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>x is returned with attributes modified for use by rxExec.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>rxExec</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>