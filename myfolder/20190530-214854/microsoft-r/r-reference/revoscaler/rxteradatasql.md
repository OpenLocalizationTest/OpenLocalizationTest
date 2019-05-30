<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxteradatasql.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3ee2af4f974b2eb183373dd7809a2df04ac327d67e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">e2af4f974b2eb183373dd7809a2df04ac327d67e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxteradatasql.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxTeradataSql function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Execute an arbitrary SQL statement that does not return data in a Teradata data base.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxTeradataSql, rxTeradataTableExists, rxTeradataDropTable, file</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxTeradataSql:  rxTeradataSql</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Execute an arbitrary SQL statement that does not return data in a Teradata data base.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>character string specifying valid SQL statement that does not return data</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>One of the following:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>a character string specifying a table name, in the form <ph id="ph1">`"tablename"`</ph> or<ph id="ph2">`"database.tablename"`</ph>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>(In Teradata, each user is a database; the user database can be specified as <ph id="ph1">`"username.tablename"`</ph>.)</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>an <bpt id="p1">[</bpt>RxTeradata<ept id="p1">](RxTeradata.md)</ept> data source that has the <ph id="ph1">`table`</ph> specified</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>an <bpt id="p1">[</bpt>RxOdbcData<ept id="p1">](RxOdbcData.md)</ept> data source that has the <ph id="ph1">`table`</ph> specified.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>or character string specifying the connection string.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the connection string from the currently  active compute context will be used if available.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed through.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>An SQL query is passed to the Teradata ODBC driver.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>is executed for the side effects and returns <ph id="ph1">`NULL`</ph> invisibly.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>returns <ph id="ph1">`TRUE`</ph> is the table exists, <ph id="ph2">`FALSE`</ph> otherwise.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The database searched for the table is determined as follows:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`table`</ph> argument is a character string and specifies a database, that is, if the <ph id="ph2">`table`</ph> argument is specified as <ph id="ph3">`"database.tablename"`</ph>, the specified database is searched for the table.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If the containing database does not exist, an error is returned.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`table`</ph> argument is a character string and does not specify a database, that is, if the <ph id="ph2">`table`</ph> argument is specified as <ph id="ph3">`"tablename"`</ph>,the database specified in the <ph id="ph4">`connectionString`</ph> is searched.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`connectionString`</ph> is missing, the connection string in the current compute context object is used.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`table`</ph> argument is an <bpt id="p1">[</bpt>RxTeradata<ept id="p1">](RxTeradata.md)</ept> or <bpt id="p2">[</bpt>RxOdbcData<ept id="p2">](RxOdbcData.md)</ept> data source, the table name specified in the data source is searched for in the database specified in the data source.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>returns <ph id="ph1">`TRUE`</ph> is the table is successfully dropped, <ph id="ph2">`FALSE`</ph> otherwise (for example, if the table did not exist).</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>RxTeradata</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>