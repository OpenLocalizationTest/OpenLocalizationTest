<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="pemacompute.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18cfa0d333d1bb8c2e5747aa5ecf5c1c77c612bbadc.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">fa0d333d1bb8c2e5747aa5ecf5c1c77c612bbadc</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revopemar\pemacompute.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Comute PEMA</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Use a PemaBaseClass reference class object to perform a Parallel External Memory Algorithm computation.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RevoPemaR, pemaCompute, models</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>pemaCompute:  Compute PEMA</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Applies to version 8.0.3 of package RevoPemaR.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Use a PemaBaseClass reference class object to perform a Parallel External Memory Algorithm (PEMA) computation.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>pemaObj</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt>PemaBaseClass<ept id="p1">](pemabaseclass.md)</ept> reference class object containing the methods for the analysis.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>A data frame or <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> data source object.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>outData</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>An <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> data source object that has write capabilities, such as an .xdf file.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Not used by all <bpt id="p1">[</bpt>PemaBaseClass<ept id="p1">](pemabaseclass.md)</ept> reference class objects.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>overwrite</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outFile`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>append</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>either <ph id="ph1">`"none"`</ph> to create a new file, <ph id="ph2">`"rows"`</ph> to append rows to an existing file, or <ph id="ph3">`"cols"`</ph> to append columns to an existing file.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outFile`</ph> exists and <ph id="ph2">`append`</ph> is <ph id="ph3">`"none"`</ph>,  the <ph id="ph4">`overwrite`</ph> argument must be set to <ph id="ph5">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Ignored when <ph id="ph1">`outData`</ph> is not specified or not relevant.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>You cannot append to <ph id="ph1">`RxTextData`</ph> or <ph id="ph2">`RxTeradata`</ph> data sources,  and appending is not supported for composite .xdf files or when using the <ph id="ph3">`RxHadoopMR`</ph> compute context.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>computeContext</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or a <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> compute context object.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>initPema</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> the <ph id="ph2">`initialize`</ph> method for the <ph id="ph3">`pemaObj`</ph> object will be called before performing computations.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>...</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Other fields in the <ph id="ph1">`PemaBaseClass`</ph> class to be utilized in the analysis.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`pemaCompute`</ph> function provides a framework for writing parallel, external memory algorithms (PEMAs) that can be run serially on a single computer, and will be automatically parallelized when run on cluster supported by <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The value returned that returned by the <ph id="ph1">`PemaBaseClass`</ph> <ph id="ph2">`processResults`</ph> method.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Note that the reference class <ph id="ph1">`PemaBaseClass`</ph> will be reinitialized at the beginning of the analysis unless <ph id="ph2">`initPema`</ph> is set to <ph id="ph3">`TRUE`</ph>, and will contain updated values upon completion.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>PemaBaseClass<ept id="p1">](pemabaseclass.md)</ept>, <bpt id="p2">[</bpt>PemaMean<ept id="p2">](pemamean.md)</ept>, <bpt id="p3">[</bpt>setPemaClass<ept id="p3">](setpemaclass.md)</ept></source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>