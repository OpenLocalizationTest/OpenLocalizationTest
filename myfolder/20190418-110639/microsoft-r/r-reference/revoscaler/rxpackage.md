<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxpackage.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907fd025aea7d87ce0be060ef3f03b63951a9f23d0c3.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d025aea7d87ce0be060ef3f03b63951a9f23d0c3</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxpackage.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxPackage function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This article explains how to enable and disable R package management on SQL Server Machine Learning Services (in-database), as well as installation, usage, and removal of individual packages.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> provides the necessary rx functions for these tasks.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxPackage, packages, sql, install, uninstall, remove, use</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>rxPackage: R Package Management in SQL Server</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>This article explains how to enable and disable R package management on SQL Server Machine Learning Services (in-database), as well as installation, usage, and removal of individual packages.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> provides the necessary rx functions for these tasks.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>SQL Server Machine Learning Services and the previous version, SQL Server R Services, support install and uninstall of R packages on SQL Server.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>A database administrator (in <ph id="ph1">`db_owner`</ph> role) must grant permissions to allow access to package functions at both the database and instance level.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>R package management functions are part of the base distribution.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>These functions allows packages to be installed from a local or remote repository into a local library (folder).</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>R provides the following core functions for managing local libraries:</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>available.packages() - enumerate packages available in a repository for installation</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>installed.packages() - enumerate installed packages in a library</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>install.packages() - install packages, including dependency resolution, from a repository into a library</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>remove.packages() - remove installed packages from a library</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>library() - load the installed package and access its functions</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>RevoScaleR also provides package management functions, which is especially useful for managing packages in a SQL Server compute context in a client session.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Packages in the database are reflected back on the file system, in a secure location.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Access is controlled through database roles, which determine whether you can install packages from a local or remote repository into a database.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>RevoScaleR provides the following core client functions for managing libraries in a database on a remote SQL server:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxInstalledPackages<ept id="p1">](rxInstalledPackages.md)</ept>() - enumerate installed packages in a database on SQL Server</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxInstallPackages<ept id="p1">](rxInstallPackages.md)</ept>() - install packages, including dependency resolution, from a repository onto a library in a database.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Simultaneously install the same packages on the file system using per-database and per-user profile locations.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxRemovePackages<ept id="p1">](rxRemovePackages.md)</ept>() - remove installed packages from a library in a database and further uninstall the packages from secured per-database, per-user location on SQL server</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxSqlLibPaths<ept id="p1">](rxSqlLibPaths.md)</ept>() - get secured library paths for the given user to refer to the installed packages for SQL Server to then use it in .libPaths() to refer to the packages</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>library() - same as R equivalent; used to load the installed package and access its functions</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxSyncPackages<ept id="p1">](rxSyncPackages.md)</ept>() - synchronize packages from a database on SQL Server to the file system used by R</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Ther are two scopes for installation and usage of packages in a particular database in SQL Server:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`Shared scope`</ph> - Share the packages with other users of the same database.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`Private scope`</ph> - Isolate a packge in a per-user private location, accessible only to the user installing the package.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Both scopes can be used to design different secure deployment models of packages.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For example, using a <ph id="ph1">`shared`</ph> scope, data scientist department heads can be granted permissions to install packages, which can then be used by all other data scientists in the group.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>In another deployment model, the data scientists can be granted <ph id="ph1">`private`</ph> scope permissions to install and use their private packages without affecting other data scientists using the same server.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Database roles are used to secure package installation and access:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rpkgs-users`</ph> - allows users to use shared packages installed by users belong to <ph id="ph2">`rpkgs-shared`</ph> role</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rpkgs-private`</ph> - allows all permissions as <ph id="ph2">`rpkgs-users`</ph> role and also allows users to install, remove and use private packages</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rpkgs-shared`</ph> - allows all permissions as <ph id="ph2">`rpkgs-private`</ph> role and also allows users to install, remove shared packages</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`db_owner`</ph> - allows all permissions as <ph id="ph2">`rpkgs-shared`</ph> role and also allows users to install &amp; remove shared and private packages for other users for management</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Enable R package management on SQL Server<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>By default, R package management is turned off at the instance level.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>To use this functionality, the administrator must do the following:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Enable package management on the SQL Server instance.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Enable package management on the SQL database.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt><ph id="ph1">`RegisterRExt.exe`</ph><ept id="p1">**</ept> command line utility, which ships with RevoScaleR, allows administrators to enable package management for instances and specific databases.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>You can find RegisterRExt.exe at <ph id="ph1">`&lt;SQLInstancePath&gt;\R_SERVICES\library\RevoScaleR\rxLibs\x64\RegisterRExt.exe`</ph>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>To enable R package management at instance level, open an elevated command prompt and run the following command:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>This command creates some package-related, instance-level artifacts on the SQL Server machine.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Next, enable R package management at database level using an elevated command prompt and the following command:</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>This command creates database artifacts, including <ph id="ph1">`rpkgs-users`</ph>, <ph id="ph2">`rpkgs-private`</ph> and <ph id="ph3">`rpkgs-shared`</ph> database roles to control user permissions who can install, uninstall, and use packages.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Disable R package management on a SQL Server<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>To disable R package management on a SQL server, the administrator must do the following:</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Disable package management on the database.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Disable package management on the SQL Server instance.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">**</bpt><ph id="ph1">`RegisterRExt.exe`</ph><ept id="p1">**</ept> command line utility located at <ph id="ph2">`&lt;SQLInstancePath&gt;\R_SERVICES\library\RevoScaleR\rxLibs\x64\RegisterRExt.exe`</ph>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>To disable R package management at the database level, open an elevated command prompt and run the following command:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>This command removes the package-related database artifacts from the database, as well as the packages in the secured file system location.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>After disabling package management at the database level, disable package management at instance level by running the following command at an elevated command prompt:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>This command removes the package-related, per-instance artifacts from the SQL Server.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxSqlLibPaths<ept id="p1">](rxSqlLibPaths.md)</ept>, <bpt id="p2">[</bpt>rxInstalledPackages<ept id="p2">](rxInstalledPackages.md)</ept>, <bpt id="p3">[</bpt>rxInstallPackages<ept id="p3">](rxInstallPackages.md)</ept>,</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxRemovePackages<ept id="p1">](rxRemovePackages.md)</ept>, <bpt id="p2">[</bpt>rxFindPackage<ept id="p2">](rxFindPackage.md)</ept>, library require</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>