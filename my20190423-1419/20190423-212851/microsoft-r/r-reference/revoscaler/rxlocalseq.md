<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxlocalseq.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a506861fdf72e6d75005717ee8ee707d3285c15e6.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">506861fdf72e6d75005717ee8ee707d3285c15e6</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxlocalseq.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxLocalSeq function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Creates a local compute context object.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This is the main generator for S4 class RxLocalSeq.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Computations using rxExec will be processed sequentially.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This is the default compute context.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), RxLocalSeq, IO</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>RxLocalSeq: Generate Local Compute Context</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Creates a local compute context object.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>This is the main generator for S4 class RxLocalSeq.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Computations using rxExec will be processed sequentially.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>This is the default compute context.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>a compute context object.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`object`</ph> has slots for   <ph id="ph2">`dataPath`</ph> and/or <ph id="ph3">`outDataPath`</ph>, they will be copied to the  equivalent slots for the new <ph id="ph4">`RxLocalSeq`</ph> object.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Explicit specifications  of the <ph id="ph1">`dataPath`</ph> and/or outDataPath arguments will override this.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>or character vector defining the search path(s) for the input data source(s).</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If not <ph id="ph1">`NULL`</ph>, it overrides any specification for <ph id="ph2">`dataPath`</ph> in <bpt id="p1">[</bpt>rxOptions<ept id="p1">](rxOptions.md)</ept></source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>or character vector defining the search path(s) for  new output data file(s).</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If not <ph id="ph1">`NULL`</ph>, this overrides any specification for <ph id="ph2">`dataPath`</ph>in <bpt id="p1">[</bpt>rxOptions<ept id="p1">](rxOptions.md)</ept></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>A job is associated with the compute context in effect at the time the job was submitted.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If the compute context subsequently changes, the compute context of the job is not affected.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Note that <ph id="ph1">`dataPath`</ph> and <ph id="ph2">`outDataPath`</ph> are only utiltized by data sources used in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> analyses.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>They do not alter the working directory for other R functions that read from or write to files.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>object of class RxLocalSeq.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxSetComputeContext<ept id="p1">](rxSetComputeContext.md)</ept>, <bpt id="p2">[</bpt>rxExec<ept id="p2">](rxExec.md)</ept>, <bpt id="p3">[</bpt>rxOptions<ept id="p3">](rxOptions.md)</ept>, <bpt id="p4">[</bpt>RxComputeContext<ept id="p4">](RxComputeContext.md)</ept>, <bpt id="p5">[</bpt>RxLocalParallel<ept id="p5">](RxLocalParallel.md)</ept>, <bpt id="p6">[</bpt>RxLocalSeq-class<ept id="p6">](RxLocalSeq-class.md)</ept>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>