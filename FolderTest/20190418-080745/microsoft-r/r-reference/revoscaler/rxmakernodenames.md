<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxmakernodenames.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef0690673357612799283eb2b2ef4e50016b6f18e69a5fb4b4c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">7612799283eb2b2ef4e50016b6f18e69a5fb4b4c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxmakernodenames.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxMakeRNodeNames function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Converts valid computer names into valid R variable names.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Should only be used when you want to guarantee that host  names are usable as variable names.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxMakeRNodeNames, IO</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>rxMakeRNodeNames:  Converts valid computer names into valid R variable names.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Converts valid computer names into valid R variable names.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Should only be used when you want to guarantee that host names are usable as variable names.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>character vector of node names to be converted.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>rxMakeRNodeNames will preform the following transformations on each element of the character vector passed:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>1 Perform <ph id="ph1">`toupper`</ph> on the name.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>1 Remove all white space from the name.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>1 If one exists, removes the first dot and all characters following it from the name.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>(This has the effect of stripping the domain name off, if one exists.)</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>1 Changes any '-' (dash) characters to '_' (underscore) characters so that node names used as variables do not have to be quoted.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The names returned by this function are valid R names, that is, symbols, but they may no longer be valid computer node names.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Do <bpt id="p1">**</bpt>not<ept id="p1">**</ept> use these names, or this function, in any context where the name may be used to query or control the actual computer; use the original computer name for that.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>This function is intended to be used only to generate R variable names for processing or storing distributed computing results from the associated computer.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Note also that once a host name has been converted into a guaranteed acceptable R variable name, it is impossible to guarantee the reverse conversion.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>