<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxfindfileinpath.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335039fdfff296ea2bad2ea3c109e485e3784eab8e5.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">039fdfff296ea2bad2ea3c109e485e3784eab8e5</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxfindfileinpath.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxFindFileInPath function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Sequentially checks the entries in a delimited path string for a provided file name.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxFindFileInPath, IO</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxFindFileInPath:  Finds where in a given path a file is.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Sequentially checks the entries in a delimited path string for a provided file name.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>character vector, compute context or job object.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>This is a required parameter.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If a compute context is provided, the <ph id="ph1">`dataPath`</ph> from that context (assuming it has one ) will be used;  if a job object is provided, that job object's compute context's <ph id="ph2">`dataPath`</ph> will be used.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If a character vector is provided, each element of the vector should contain one directory path.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If a character scalar is supplied, multiple directory paths can be contained by using the standard system  delimiters (":" for Linux and ";") to separate the entries within the path.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This allows system PATH's to  be parsed using this function.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>logical scalar.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>This is a required parameter.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The name of the file being sought along the <ph id="ph1">`path`</ph>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>This function will sequentially check the locations (directories) provided in the <ph id="ph1">`path`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Thus, if there exists more than one instance of a file with the same <ph id="ph1">`fileName`</ph>, the first instance of a directory in the path containing the file will be the one returned.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Returns NULL if the target file is not found in any of the possible locations, or the path to the file (not including the file name) if it is found.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>