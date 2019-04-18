<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxinstalledpackages.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c89cfc3e2492405df24b5e8ccffaf6b6b96a431e6.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">89cfc3e2492405df24b5e8ccffaf6b6b96a431e6</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxinstalledpackages.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxInstalledPackages function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Find (or retrieve) details of installed packages for a compute context.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxInstalledPackages, packages, sql, install, uninstall, remove, use</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxInstalledPackages: Installed Packages for Compute Context</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Find (or retrieve) details of installed packages for a compute context.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>an <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept> or equivalent character string or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If set to the default of <ph id="ph1">`NULL`</ph>, the currently active compute context is used.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Supported compute contexts are <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> and <bpt id="p2">[</bpt>RxLocalSeq<ept id="p2">](RxLocalSeq.md)</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>a character vector describing the location of R library  trees to search through, or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The default value of <ph id="ph1">`NULL`</ph> corresponds to checking the loaded namespace,  then all libraries currently known in  <ph id="ph2">`.libPaths()`</ph>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> only <ph id="ph1">`NULL`</ph> is supported.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>character vector or <ph id="ph1">`NULL`</ph> (default).</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If non-null, used to select packages;  <ph id="ph1">`"high"`</ph> is equivalent to <ph id="ph2">`c("base", "recommended")`</ph>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>To select all packages without an assigned priority use priority = <ph id="ph1">`"NA"`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, do not use cached information, nor cache it.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>a character vector giving the fields to extract from each package's DESCRIPTION file,  or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the following fields are used: <ph id="ph2">`"Package"`</ph>, <ph id="ph3">`"LibPath"`</ph>, <ph id="ph4">`"Version"`</ph>, <ph id="ph5">`"Priority"`</ph>, <ph id="ph6">`"Depends"`</ph>,  <ph id="ph7">`"Imports"`</ph>, <ph id="ph8">`"LinkingTo"`</ph>, <ph id="ph9">`"Suggests"`</ph>, <ph id="ph10">`"Enhances"`</ph>,  <ph id="ph11">`"License"`</ph>, <ph id="ph12">`"License_is_FOSS"`</ph>, <ph id="ph13">`"License_restricts_use"`</ph>,  <ph id="ph14">`"OS_type"`</ph>, <ph id="ph15">`"MD5sum"`</ph>, <ph id="ph16">`"NeedsCompilation"`</ph>, and <ph id="ph17">`"Built"`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Unavailable fields result in <ph id="ph1">`NA`</ph> values.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>character string or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If non-null and non-empty, used to select packages  which are installed for that sub-architecture.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>This is a wrapper for installed.packages.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>See the help file for additional details.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Note that <ph id="ph1">`rxInstalledPackages`</ph> treats the <ph id="ph2">`field`</ph> argument differently, only returning the <ph id="ph3">`fields`</ph> specified in the argument.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>By default, a character vector of installed packages is returned.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`fields`</ph> is not set to <ph id="ph2">`"Package"`</ph>, a matrix with one row per package is returned.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The row names are the package names and the possible column names are <ph id="ph1">`"Package"`</ph>, <ph id="ph2">`"LibPath"`</ph>, <ph id="ph3">`"Version"`</ph>, <ph id="ph4">`"Priority"`</ph>, <ph id="ph5">`"Depends"`</ph>, <ph id="ph6">`"Imports"`</ph>, <ph id="ph7">`"LinkingTo"`</ph>, <ph id="ph8">`"Suggests"`</ph>, <ph id="ph9">`"Enhances"`</ph>, <ph id="ph10">`"License"`</ph>, <ph id="ph11">`"License_is_FOSS"`</ph>, <ph id="ph12">`"License_restricts_use"`</ph>, <ph id="ph13">`"OS_type"`</ph>, <ph id="ph14">`"MD5sum"`</ph>, <ph id="ph15">`"NeedsCompilation"`</ph>, and <ph id="ph16">`"Built"`</ph> (the R version the package was built under).</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Additional columns can be specified using the fields argument.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If using a distributed compute context with the <ph id="ph1">`allNodes`</ph> set to <ph id="ph2">`TRUE`</ph>, a list of matrices from each node will be returned.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context multiple rows for a package will be returned if different versions of the same package is installed in different <ph id="ph1">`"system"`</ph>, <ph id="ph2">`"shared"`</ph> and <ph id="ph3">`"private"`</ph> scopes.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxPackage<ept id="p1">](rxPackage.md)</ept>, installed.packages, <bpt id="p2">[</bpt>rxFindPackage<ept id="p2">](rxFindPackage.md)</ept>, <bpt id="p3">[</bpt>rxInstallPackages<ept id="p3">](rxInstallPackages.md)</ept>,</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxRemovePackages<ept id="p1">](rxRemovePackages.md)</ept>, <bpt id="p2">[</bpt>rxSyncPackages<ept id="p2">](rxSyncPackages.md)</ept>, <bpt id="p3">[</bpt>rxSqlLibPaths<ept id="p3">](rxSqlLibPaths.md)</ept>,</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>require</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>