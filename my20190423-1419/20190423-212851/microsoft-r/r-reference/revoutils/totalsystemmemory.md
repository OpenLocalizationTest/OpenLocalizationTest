<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="totalsystemmemory.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a10a65eadcc627d776cb9e0fa64b2666e7ae1168c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">10a65eadcc627d776cb9e0fa64b2666e7ae1168c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoutils\totalsystemmemory.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Obtain Total System Memory</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Uses operating system tools to return total system memory.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>, totalSystemMemory,  sysdata</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>totalSystemMemory:  Obtain Total System Memory</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Uses operating system tools to return total system memory.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>On Unix-alikes, checks the <ph id="ph1">`/proc/meminfo`</ph> file for the total memory.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If the system call returns an error, the function returns <ph id="ph1">`NA`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>On Windows systems, uses <ph id="ph1">`wmic`</ph> to obtain the <ph id="ph2">`TotalVisibleMemorySize`</ph>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>A numeric value representing total system memory in kBytes, or <ph id="ph1">`NA`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>