<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-admin-r-package-management.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c887a1e6c1ec093708355ced89ed74bf6ed6488b1.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">887a1e6c1ec093708355ced89ed74bf6ed6488b1</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-admin-r-package-management.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Package Management Guide - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Managing R Packages in DeployR - for DeployR administrators</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>r packages, DeployR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>R Package Management Guide</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Introduction</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>As the DeployR administrator, one of your responsibilities is to ensure the R code that runs on the DeployR server has access to the R package dependencies declared within that code.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The following sections discuss R package management in this context.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>By adopting one or both of the R package management approaches described below, your data scientists can avoid issues where a script they've tested locally now fails due to missing package dependencies when executed in the DeployR server environment.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Guideline:<ept id="p1">**</ept> Assign the appropriate permissions for packaging installations and/or install the packages on behalf of your users with <ph id="ph1">`deployrPackage()`</ph>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Centralized Management</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>One option is to install a fixed set of default packages across the DeployR grid on behalf of your users.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>This can be done in a number of ways.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>One such approach is to use a master R script that contains all required package dependency declarations for the DeployR server as follows:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>In your local environment:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Install <ph id="ph1">`deployrUtils`</ph> locally <bpt id="p1">[</bpt>from GitHub<ept id="p1">](https://github.com/Microsoft/deployrUtils/releases)</ept> using your IDE, R console, or terminal window with the following commands:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Create a master R script that you'll use to install the package dependencies across the DeployR grid.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>At the top of that script, declare each package dependency individually using <ph id="ph1">`deployrPackage()`</ph>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>For the full function help, use <ph id="ph1">`library(help="deployrUtils")`</ph> in your IDE.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>In your remote DeployR server environment:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Manually run this R script on a DeployR grid node.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Repeat previous step by running the master script manually on every grid node machine.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Running this script on each grid node ensures the full set of packages is installed and available on each node.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>You will have to update and manually rerun this script on each node on the DeployR grid whenever a new package needs to be added to the server environment.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Decentralized Management</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Another option is to <bpt id="p1">[</bpt>assign permissions<ept id="p1">](deployr-admin-console-permissions-with-roles.md#viewing-editing-and-assigning-roles)</ept> for R package installation to select users.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Then, these select users can install the packages they need directly within their code.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>When you've explicitly assigned the <ph id="ph1">`PACKAGE_MANAGER`</ph> role to users, they are granted permissions to install R packages via <ph id="ph2">`deployrUtils::deployrPackage()`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Login</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Also note that the <ph id="ph1">`ADMINISTRATOR`</ph> and <ph id="ph2">`POWER_USER`</ph> roles have implicit <ph id="ph3">`PACKAGE_MANAGER`</ph> rights, while <ph id="ph4">`BASIC_USER`</ph> does not.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Read more on default roles...<ept id="p1">](deployr-admin-console-permissions-with-roles.md#predefined-system-roles)</ept></source>
        </trans-unit></group></body></file></xliff>