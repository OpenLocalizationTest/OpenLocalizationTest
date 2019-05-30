<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxlocatefile.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e5e82b115f0df713c31e432f5b3b686ee36d511d1.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5e82b115f0df713c31e432f5b3b686ee36d511d1</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxlocatefile.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxLocateFile function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Obtain the normalized absolute path to the first occurrence of the specified input file  in the specified set of paths.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxLocateFile, IO</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxLocateFile:  Find File on a Given Data Path</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Obtain the normalized absolute path to the first occurrence of the specified input file in the specified set of paths.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Character string defining path to a file or a data source containing a file name.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>character vector of search paths.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the search path  determined by <ph id="ph2">`isOutFile`</ph> is used.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Only the paths listed are searched;  the list is not recursive.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>, character string or <bpt id="p1">[</bpt>RxFileSystem<ept id="p1">](RxFileSystem.md)</ept> object indicating type of file system;  <ph id="ph1">`"native"`</ph>or <ph id="ph2">`RxNativeFileSystem`</ph> object can be used for the local operating system, or an <ph id="ph3">`RxHdfsFileSystem`</ph> object for the Hadoop file system.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the active compute context will be checked for a valid file system.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If not available, <ph id="ph1">`rxGetOption("fileSystem")`</ph> will be used to obtain the file system.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`file`</ph> is a data source containing a file system, that file system will take precedent.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, search using <ph id="ph2">`outDataPath`</ph> instead of <ph id="ph3">`dataPath`</ph> in <bpt id="p1">[</bpt>rxOptions<ept id="p1">](rxOptions.md)</ept> or in the local compute context (e.g.,<bpt id="p2">[</bpt>RxLocalSeq<ept id="p2">](RxLocalSeq.md)</ept>).</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>character string containing default extension to use if extension is missing from <ph id="ph1">`file`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, information on the file to be located is printed.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`file`</ph> path may be relative, for example, <ph id="ph2">`"one/two/myfile.xdf"`</ph> or absolute, for example, <ph id="ph3">`"C:/one/two/myfile.xdf"`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`file`</ph> is an absolute path, the existence of the file is verified and, if found, the absolute path is returned in normalized form.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`file`</ph> is a relative path, the current working directory and then any paths specified in <ph id="ph2">`pathsToSearch`</ph> are prepended to <ph id="ph3">`file`</ph> and a search for the file along the concatenated paths is performed.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The first path where the file is found is returned in normalized form.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If the file does not exist an error is thrown.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>