<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxsyncpackages.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338aef35fa314ab8bb4dc29a70ebba9a89b5c4fbeece.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">ef35fa314ab8bb4dc29a70ebba9a89b5c4fbeece</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxsyncpackages.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxSyncPackages function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Synchronizes all R packages installed in a database with the packages on the files system.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>The packages contained in the database are also installed on the file system so they can be loaded by R.  You might need to use rxSyncPackages if you rebuilt a server instance or restored SQL Server databases on a new machine, or if you think an R package on the file system is corrupted.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxSyncPackages, sync, synchronize, use, packages, sql</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>rxSyncPackages: Synchronize Packages for Compute Context</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Synchronizes all R packages installed in a database with the packages on the files system.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The packages contained in the database are also installed on the file system so they can be loaded by R. You might need to use rxSyncPackages if you rebuilt a server instance or restored SQL Server databases on a new machine, or if you think an R package on the file system is corrupted.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>an <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept> or equivalent character string or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If set to the default of <ph id="ph1">`NULL`</ph>, the currently active compute context is used.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Supported compute contexts are <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>character vector containing either <ph id="ph1">`"shared"`</ph> or <ph id="ph2">`"private"`</ph> or both.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>synchronizes the packages on a per-database shared location on SQL Server, which in turn can be used (referred) by multiple different users.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>synchronizes the packages on per-database, per-user private location on SQL Server which is only accessible to the single user.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>By default both <ph id="ph1">`"shared"`</ph> and <ph id="ph2">`"private"`</ph> are set, which will synchronize  the entire table of packages for all scopes and users.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>character vector.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Should be either empty <ph id="ph1">`''`</ph> or a vector of valid SQL database user account names.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Only users in <ph id="ph1">`'db_owner'`</ph> role for a database can specify this value to install packages on  behalf of other users.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, "progress report" is given during installation of given packages.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>For a <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context, the user specified as part of connection string is considered the package owner if the <ph id="ph1">`owner`</ph> argument is empty.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>To call this function, a user must be granted permissions by a database owner, making the user a member of either <ph id="ph1">`'rpkgs-shared'`</ph> or <ph id="ph2">`'rpkgs-private'`</ph> database role.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Members of the <ph id="ph1">`'rpkgs-shared'`</ph> role can install packages to <ph id="ph2">`"shared"`</ph> location and <ph id="ph3">`"private"`</ph> location.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Members of the <ph id="ph1">`'rpkgs-private'`</ph> role can only install packages in a <ph id="ph2">`"private"`</ph> location for their own use.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>To use the packages installed on the SQL Server, a user must be at least a member of <ph id="ph1">`'rpkgs-users'`</ph> role.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>See the help file for additional details.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Invisible</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxInstallPackages<ept id="p1">](rxInstallPackages.md)</ept>, <bpt id="p2">[</bpt>rxPackage<ept id="p2">](rxPackage.md)</ept>, install.packages, <bpt id="p3">[</bpt>rxFindPackage<ept id="p3">](rxFindPackage.md)</ept>, <bpt id="p4">[</bpt>rxInstalledPackages<ept id="p4">](rxInstalledPackages.md)</ept>, <bpt id="p5">[</bpt>rxRemovePackages<ept id="p5">](rxRemovePackages.md)</ept>, <bpt id="p6">[</bpt>rxSqlLibPaths<ept id="p6">](rxSqlLibPaths.md)</ept>,</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>require</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>