<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxinstallpackages.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335839558b0307fafc1c7de9a1c4ad1b17eb713a0cf.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">839558b0307fafc1c7de9a1c4ad1b17eb713a0cf</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxinstallpackages.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxInstallPackages function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install R packages from repositories or install local files for the current session.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxInstallPackages, install, use, packages, sql</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxInstallPackages: Install Packages for Compute Context</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Install R packages from repositories or install local files for the current session.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`character`</ph> vector of the names of packages whose current versions should be downloaded from the repositories.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If repos = NULL, a character vector of file paths of .zip files containing binary builds of packages.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>(http:// and file:// URLs are also accepted and the files will be downloaded and installed from local copies.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If you specify .zip files with repos = <ph id="ph1">`NULL`</ph> with <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept> compute context the .zip file paths should already be present on a folder.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Applicable only for <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, skips missing dependent packages for which otherwise an error is generated.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>character vector, the base URL(s) of the repositories to use.Can be NULL to install from local files, directories.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>logical.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, "progress report" is given during installation of given packages.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>character.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Applicable only for <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Should be either <ph id="ph1">`"shared"`</ph> or <ph id="ph2">`"private"`</ph>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"shared"`</ph> installs the packages on per database shared location on SQL server which in turn can be used (referred) by multiple different users.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"private"`</ph> installs the packages on per database, per user private location on SQL server which is only accessible to the single user.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>character.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Applicable only for <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>This is generally empty <ph id="ph1">`''`</ph> value.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Should be either empty <ph id="ph1">`''`</ph> or a valid SQL database user account name.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Only users in <ph id="ph1">`'db_owner'`</ph> role for a database can specify this value to install packages on  behalf of other users.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>an <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept> or equivalent character string or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If set to the default of <ph id="ph1">`NULL`</ph>, the currently active compute context is used.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Supported compute contexts are <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept>, <bpt id="p2">[</bpt>RxLocalSeq<ept id="p2">](RxLocalSeq.md)</ept>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>This is a simple wrapper for install.packages.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context the user specified as part of connection string is used for installing the packages if <ph id="ph1">`owner`</ph> argument is empty.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The user calling this function needs to be granted permissions by database owner by making them member of either <ph id="ph1">`'rpkgs-shared'`</ph> or <ph id="ph2">`'rpkgs-private'`</ph> database role.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Users in <ph id="ph1">`'rpkgs-shared'`</ph> role can install packages to <ph id="ph2">`"shared"`</ph> location and <ph id="ph3">`"private"`</ph> location.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Users in <ph id="ph1">`'rpkgs-private'`</ph> role can only install packages <ph id="ph2">`"private"`</ph> location for their own use.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>To use the packages installed on the SQL server a user needs to be a member of at least the <ph id="ph1">`'rpkgs-users'`</ph> role.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>See the help file for additional details.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Invisible <ph id="ph1">`NULL`</ph></source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxPackage<ept id="p1">](rxPackage.md)</ept>, install.packages, <bpt id="p2">[</bpt>rxFindPackage<ept id="p2">](rxFindPackage.md)</ept>, <bpt id="p3">[</bpt>rxInstalledPackages<ept id="p3">](rxInstalledPackages.md)</ept>, <bpt id="p4">[</bpt>rxRemovePackages<ept id="p4">](rxRemovePackages.md)</ept>, <bpt id="p5">[</bpt>rxSyncPackages<ept id="p5">](rxSyncPackages.md)</ept>, <bpt id="p6">[</bpt>rxSqlLibPaths<ept id="p6">](rxSqlLibPaths.md)</ept>,</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>require</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>