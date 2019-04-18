<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxcomputecontext.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c12261ff4f038e83714acd7479b0071dc890602ed.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">12261ff4f038e83714acd7479b0071dc890602ed</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxcomputecontext.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxComputeContext function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This is the main generator for RxComputeContext S4 classes.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), RxComputeContext, file, connection</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RxComputeContext: RevoScaleR Compute Contexts: Class Generator</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This is the main generator for RxComputeContext S4 classes.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>character string specifying class name or description of the specific  class to instantiate, or an existing <ph id="ph1">`RxComputeContext`</ph> object.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Choices include: "RxLocalSeq" or "local", "RxLocalParallel" or "localpar", "RxSpark" or "spark",  "RxHadoopMR" or "hadoopmr", "RxInSqlServer" or "sqlserver", and "RxForeachDoPar" or "dopar".</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>any other arguments are passed to the class generator determined from <ph id="ph1">`context`</ph>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>This is a wrapper to specific class generator functions for the RevoScaleR compute context classes.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>For example, the RxInSqlServer class uses function <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> as a generator.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Therefore either <ph id="ph1">`RxInSqlServer(...)`</ph> or <ph id="ph2">`RxComputeContext("RxInSqlServer", ...)`</ph> will create an RxInSqlServer instance.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>A type of RxComputeContext compute context object.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>This object may be used to in <bpt id="p1">[</bpt>rxSetComputeContext<ept id="p1">](rxSetComputeContext.md)</ept> or <bpt id="p2">[</bpt>rxOptions<ept id="p2">](rxOptions.md)</ept> to set the compute context.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxComputeContext-class<ept id="p1">](RxComputeContext-class.md)</ept>, <bpt id="p2">[</bpt>RxHadoopMR<ept id="p2">](RevoScaleR-deprecated.md)</ept>, <bpt id="p3">[</bpt>RxSpark<ept id="p3">](RxSpark.md)</ept>, <bpt id="p4">[</bpt>RxInSqlServer<ept id="p4">](RxInSqlServer.md)</ept>, <bpt id="p5">[</bpt>RxLocalSeq<ept id="p5">](RxLocalSeq.md)</ept>, <bpt id="p6">[</bpt>RxLocalParallel<ept id="p6">](RxLocalParallel.md)</ept>, <bpt id="p7">[</bpt>RxForeachDoPar<ept id="p7">](RxForeachDoPar.md)</ept>, <bpt id="p8">[</bpt>rxSetComputeContext<ept id="p8">](rxSetComputeContext.md)</ept>, <bpt id="p9">[</bpt>rxOptions<ept id="p9">](rxOptions.md)</ept>, <bpt id="p10">[</bpt>rxExec<ept id="p10">](rxExec.md)</ept>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>