<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxfindpackage.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86ccbd6a268518f8fd2ccfb94944f54773708ecf7e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">ccbd6a268518f8fd2ccfb94944f54773708ecf7e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxfindpackage.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxFindPackage function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Find the path for one or more packages for a compute context.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxFindPackage, packages, sql, install, uninstall, remove, use</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxFindPackage: Find Packages for Compute Context</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Find the path for one or more packages for a compute context.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>character vector of name(s) of packag(es).</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>an <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept> or equivalent character string or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If set to the default of <ph id="ph1">`NULL`</ph>, the currently active compute context is used.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Supported compute contexts are <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> and <bpt id="p2">[</bpt>RxLocalSeq<ept id="p2">](RxLocalSeq.md)</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>logical</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>a character vector describing the location of R library trees to search through, or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The default value of <ph id="ph1">`NULL`</ph> corresponds to checking the loaded namespace, then all libraries currently known in  <ph id="ph2">`.libPaths()`</ph>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> only <ph id="ph1">`NULL`</ph> is supported.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, warnings or an error is given if the package is not found.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, additional diagnostics are printed if available.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This is a wrapper for find.package.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>See the help file for additional details.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>A character vector of paths of package directories.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If using a distributed compute context with the <ph id="ph1">`allNodes`</ph> set to <ph id="ph2">`TRUE`</ph>, a list of lists with a character vector of paths from each node will be returned.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxPackage<ept id="p1">](rxPackage.md)</ept>, find.package, <bpt id="p2">[</bpt>rxInstalledPackages<ept id="p2">](rxInstalledPackages.md)</ept>, <bpt id="p3">[</bpt>rxInstallPackages<ept id="p3">](rxInstallPackages.md)</ept>,</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxRemovePackages<ept id="p1">](rxRemovePackages.md)</ept>, <bpt id="p2">[</bpt>rxSyncPackages<ept id="p2">](rxSyncPackages.md)</ept>, <bpt id="p3">[</bpt>rxSqlLibPaths<ept id="p3">](rxSqlLibPaths.md)</ept>,</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>require</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>