<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="revoscaler-sql-server-functions.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc775049459e0dbeb50ed697a46bf38ef092bd124615f2.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">49459e0dbeb50ed697a46bf38ef092bd124615f2</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\revoscaler-sql-server-functions.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>SQL Server RevoScaleR functions (Machine Learning Server and Microsoft R)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RevoScaleR functions for a SQL Server compute context</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>RevoScaleR Functions for a SQL Server compute context</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>This article provides an overview of the main RevoScaleR functions for use with SQL Server, along with comments on their syntax.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Functions for working with SQL Server Data Sources</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>The following functions let you define a SQL Server data source.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>A data source object is a container that specifies a connection string together with the set of data that you want, defined either as a table, view, or query.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Stored procedure calls are not supported.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>In addition to defining a data source, you can execute DDL statements from R, if you have the necessary permissions on the instance and database.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxSqlServerData<ept id="p1">](rxsqlserverdata.md)</ept> - Define a SQL Server  data source object</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxSqlServerDropTable<ept id="p1">](rxsqlserverdroptable.md)</ept> - Drop a SQL Server  table</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxSqlServerTableExists<ept id="p1">](rxsqlserverdroptable.md)</ept> - Check for the existence of a database table or object</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxExecuteSQLDDL<ept id="p1">](rxexecutesqlddl.md)</ept> - Execute a command to define, manipulate, or control SQL data, but not return data</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Functions for Defining or Managing a Compute Context</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The following functions let you define a new compute context, switch compute contexts, or identify the current compute context.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](rxcomputecontext.md)</ept> - Create a compute context.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxInSqlServer<ept id="p1">](rxinsqlserver.md)</ept> - Generate a SQL Server compute context that lets <bpt id="p2">**</bpt>RevoScaleR<ept id="p2">**</ept> functions run in SQL Server R Services.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxGetComputeContext<ept id="p1">](rxsetcomputecontext.md)</ept> - Get the current compute context.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxSetComputeContext<ept id="p1">](rxsetcomputecontext.md)</ept> - Specify which compute context to use.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The local compute context is available by default, or you can specify the keyword <bpt id="p1">**</bpt>local<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Functions for Using a Data Source</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>After you have created a data source object, you can open it to get data, or write new data to it.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Depending on the size of the data in the source, you can also define the batch size as part of the data source and move data in chunks.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxIsOpen<ept id="p1">](rxopen-methods.md)</ept> - Check whether a data source is available</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxOpen<ept id="p1">](rxopen-methods.md)</ept> - Open a data source for reading</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxReadNext<ept id="p1">](rxopen-methods.md)</ept> - Read data from a source</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxWriteNext<ept id="p1">](rxopen-methods.md)</ept> - Write data to the target</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxClose<ept id="p1">](rxopen-methods.md)</ept> - Close a data source</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Functions that work with XDF Files</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The following functions can be used to create a local data cache in the XDF format.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>This file can be useful when working with more data than can be transferred from the database in one batch, or more data than can fit in memory.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If you regularly move large amounts of data from a database to a local workstation, rather than query the database repeatedly for each R operation, you can use the XDF file to save the data locally and then work with it in your R workspace, using the XDF file as the cache.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>- Move data from an ODBC source to the XDF file</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>- Create an XDF data object</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>- Read data from XDF int a data frame</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Comparison of RevoScaleR and CRAN R Functions</source>
        </trans-unit></group></body></file></xliff>