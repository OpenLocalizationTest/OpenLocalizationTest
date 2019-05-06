<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="setpemaclass.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc775079e3766da8d3345b2ef9f108a60bd63ee2e29491.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">79e3766da8d3345b2ef9f108a60bd63ee2e29491</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revopemar\setpemaclass.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>PEMA classes</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Returns a generator function for creating analysis reference class objects to use in pemaCompute.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RevoPemaR, setPemaClass, methods</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>setPemaClass:  PEMA classes</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Applies to version 8.0.3 of package RevoPemaR.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Returns a generator function for creating analysis reference class objects to use in pemaCompute.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Class</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>character string name for the class.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>fields</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>either a character vector of field names or a named list of the fields.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>contains</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>optional vector of super reference classes for this class.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The fields  and class-based methods will be inherited.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>methods</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>a named list of function definitions that can be invoked on objects from this class.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>where</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>the environment in which to store the class definition.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>includeMethods</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, methods (including those of parent classes) will be included when serializing.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>...</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>other arguments to be passed to setRefClass.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>See setRefClass for more information on arguments and using reference classes.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`setPemaCLass`</ph> generator provides a framework for writing parallel, external memory algorithms (PEMAs) that can be run serially on a single computer, and will be automatically parallelized when run on cluster supported by <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>returns a generator function suitable for creating objects from the class, invisibly.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>PemaBaseClass<ept id="p1">](pemabaseclass.md)</ept>, setRefClass, <bpt id="p2">[</bpt>PemaMean<ept id="p2">](pemamean.md)</ept>, <bpt id="p3">[</bpt>pemaCompute<ept id="p3">](pemacompute.md)</ept></source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>