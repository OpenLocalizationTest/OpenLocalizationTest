<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxsqllibpaths.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef0690673357ac58ca27959cc6925c57e904d957619acbdf85b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">7ac58ca27959cc6925c57e904d957619acbdf85b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxsqllibpaths.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxSqlLibPaths function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Gets the search path for the library trees for packages while executing inside the SQL Server, using <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context or using T-SQL script with sp_execute_external_script stored procedure with embedded R script.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxSqlLibPaths, use, packages, sql, install, uninstall, remove</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxSqlLibPaths: Search Paths for Packages in SQL compute context</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Gets the search path for the library trees for packages while executing inside the SQL Server, using <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context or using T-SQL script with sp_execute_external_script stored procedure with embedded R script.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>a <ph id="ph1">`character`</ph> connection string for the SQL Server.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>This should be a local connection string (external connection strings are not supported while executing on a SQL Server).</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>You can also specify <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context object for input, from which the connection string will be extracted and used.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context, a user specified on the connection string must be a member of one of the following roles <ph id="ph1">`'db_owner'`</ph> <ph id="ph2">`'rpkgs-shared'`</ph>,  <ph id="ph3">`'rpkgs-private'`</ph> or <ph id="ph4">`'rpkgs-private'`</ph> in the database.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>When rxExec() function is called from a client machine with <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> compute context to execute the rx function on SQL Server, the <ph id="ph1">`.libPaths()`</ph> is automatically updated to include the library paths returned by this <bpt id="p2">[</bpt>rxSqlLibPaths<ept id="p2">](rxSqlLibPaths.md)</ept> function.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>A character vector of the library paths containing both <ph id="ph1">`"shared"`</ph> or <ph id="ph2">`"private"`</ph> scope of the packages if the user specified in the connection string is allowed access.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>On access denied, it returns an empty character vector.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxPackage<ept id="p1">](rxPackage.md)</ept>, .libPaths, <bpt id="p2">[</bpt>rxFindPackage<ept id="p2">](rxFindPackage.md)</ept>, <bpt id="p3">[</bpt>rxInstalledPackages<ept id="p3">](rxInstalledPackages.md)</ept>, <bpt id="p4">[</bpt>rxInstallPackages<ept id="p4">](rxInstallPackages.md)</ept>,</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxRemovePackages<ept id="p1">](rxRemovePackages.md)</ept>, <bpt id="p2">[</bpt>rxSyncPackages<ept id="p2">](rxSyncPackages.md)</ept>, require</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>