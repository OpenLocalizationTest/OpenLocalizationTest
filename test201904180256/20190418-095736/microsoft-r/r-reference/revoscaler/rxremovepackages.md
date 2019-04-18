<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxremovepackages.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18ce97c5dcdbd1b90a74946c9e3eaafe4abdfae6c56.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">e97c5dcdbd1b90a74946c9e3eaafe4abdfae6c56</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxremovepackages.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxRemovePackages function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Removes installed packages from a compute context.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxRemovePackages, remove, uninstall, packages, sql</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxRemovePackages: Remove Packages from Compute Context</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Removes installed packages from a compute context.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>a <ph id="ph1">`character`</ph> vector of names of the packages to be removed.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>a <ph id="ph1">`character`</ph> vector  identifying library path from where the package needs to be removed.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>This argument is not supported in <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Only valid for a local compute context.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Applicable only for <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, does dependency resolution of the packages being removed and removes the dependent packages also if the dependent packages aren't referenced by other packages outside the dependency closure.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Applicable only for <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, verifies there are no references to the dependent packages by other packages outside the dependency closure.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, "progress report" is given during removal of given packages.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>character.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Applicable only for <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Should be either <ph id="ph1">`"shared"`</ph> or <ph id="ph2">`"private"`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"shared"`</ph> removes the packages from a per-database shared location on SQL Server which in turn could have been used (referred) by multiple different users.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"private"`</ph> removes the packages from a per-database, per-user private location on SQL Server which is only accessible to the single user.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>character.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Applicable only for <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>This is generally empty <ph id="ph1">`''`</ph> value.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Should be either empty <ph id="ph1">`''`</ph> or a valid SQL database user account name.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Only users in <ph id="ph1">`'db_owner'`</ph> role for a database can specify this value to remove packages on  behalf of other users.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>an <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept> or equivalent character string or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If set to the default of <ph id="ph1">`NULL`</ph>, the currently active compute context is used.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Supported compute contexts are <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept>, <bpt id="p2">[</bpt>RxLocalSeq<ept id="p2">](RxLocalSeq.md)</ept>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>This is a simple wrapper for remove.packages.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context, the user specified as part of connection string is used for removing the packages if <ph id="ph1">`owner`</ph> argument is empty.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The user calling this function needs to be granted permissions by database owner by making them member of either <ph id="ph1">`'rpkgs-shared'`</ph> or <ph id="ph2">`'rpkgs-private'`</ph> database role.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Users in <ph id="ph1">`'rpkgs-shared'`</ph> role can remove packages from <ph id="ph2">`"shared"`</ph> location and their own <ph id="ph3">`"private"`</ph> location.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Users in <ph id="ph1">`'rpkgs-private'`</ph> role can only remove packages from their own <ph id="ph2">`"private"`</ph> location.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Invisible <ph id="ph1">`NULL`</ph></source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxPackage<ept id="p1">](rxPackage.md)</ept>, remove.packages, <bpt id="p2">[</bpt>rxFindPackage<ept id="p2">](rxFindPackage.md)</ept>, <bpt id="p3">[</bpt>rxInstalledPackages<ept id="p3">](rxInstalledPackages.md)</ept>, <bpt id="p4">[</bpt>rxInstallPackages<ept id="p4">](rxInstallPackages.md)</ept>,</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxSyncPackages<ept id="p1">](rxSyncPackages.md)</ept>, <bpt id="p2">[</bpt>rxSqlLibPaths<ept id="p2">](rxSqlLibPaths.md)</ept>,</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>require</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>