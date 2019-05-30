<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-data-odbc.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3eb12bf3be1f642dca82a7b74ad2a3dd93a402c66f.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">b12bf3be1f642dca82a7b74ad2a3dd93a402c66f</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-data-odbc.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Import relational data using ODBC (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to import relational data using ODBC and rxImport in RevoScaleR in Machine Learning Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Import relational data using ODBC</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RevoScaleR allows you to read or write data from virtually any database for which you can obtain an ODBC driver, a standard software interface for accessing relational data.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>ODBC connections are enabled through drivers and a driver manager.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Drivers handle the translation of requests from an application to the database.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The ODBC Driver Manager sets up and manages the connection between them.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Both drivers and an ODBC Driver Manager must be installed on the computer running Microsoft R. On Windows, the driver manager is built in.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>On Linux systems, RevoScaleR supports <bpt id="p1">[</bpt>unixODBC<ept id="p1">](http://www.unixodbc.org/)</ept>, which you will need to install.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Once the manager is installed, you can proceed to install individual database drivers for all of the data sources you need to support.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>To import data from a relational database management system, do the following:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Install an ODBC Driver Manager (Linux only)</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Install ODBC drivers</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Create an <bpt id="p1">**</bpt>RxOdbcData<ept id="p1">**</ept> data source</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>For read operations, use <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> to read data</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>For write operations, use <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> to write data back to the data source</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>About ODBC in Microsoft R</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>In Microsoft R, an ODBC and <bpt id="p1">**</bpt>RxOdbcData<ept id="p1">**</ept> dependency exists for data imported from relational database systems like Oracle, PostgreSQL, and MySQL, to name a few.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>ODBC is primarily required for <bpt id="p1">**</bpt>RxOdbcData<ept id="p1">**</ept> data sources, but it is also used internally for DBMS-specific connections to SQL Server.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If you delete the ODBC driver for SQL Server and then try to use <bpt id="p1">**</bpt>RxSqlServerData<ept id="p1">**</ept>, the connection fails.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Although ODBC drivers exist for text data, Microsoft R does not use ODBC for sources accessed as file-based reads.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>To be specific, it's not used for accessing text files, SPSS database files, or SAS database files.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>For SQL Server, you can use <bpt id="p1">**</bpt>RxSqlServerData<ept id="p1">**</ept> or <bpt id="p2">**</bpt>RxOdbcData<ept id="p2">**</ept> interchangeably, unless you are accessing <bpt id="p3">[</bpt>R objects stored in a SQL Server table<ept id="p3">](https://docs.microsoft.com/sql/advanced-analytics/r/save-and-load-r-objects-from-sql-server-using-odbc)</ept>, in which case <bpt id="p4">**</bpt>RxOdbcData<ept id="p4">**</ept> is required.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>For examples and instructions on using SQL Server data in Microsoft R, see <bpt id="p1">[</bpt>Import SQL data from Azure SQL Database and SQL Server<ept id="p1">](how-to-revoscaler-data-sql.md)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>How to configure ODBC for relational data access</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Follow these steps to configure ODBC for loading data from an external relational database.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>1 - Install unixODBC</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Linux only</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>An ODBC Driver Manager manages communication between applications and drivers.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>On Linux, an ODBC Driver Manager is not typically bundled in a Linux distribution.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Although several driver managers are available, Microsoft R supports the <bpt id="p1">[</bpt>unixODBC Driver Manager<ept id="p1">](http://www.unixodbc.org/)</ept>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>To first check whether unixODBC is installed, do the following:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>On RHEL:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>On Ubuntu:</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>On SLES:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If unixODBC is not installed, issue the following commands to add it:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>On RHEL:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>On Ubuntu:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>On SLES:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>For more information, SQL Server documentation provides in-depth instructions for <bpt id="p1">[</bpt>installing unixODBC<ept id="p1">](https://docs.microsoft.com/sql/connect/odbc/linux/installing-the-driver-manager)</ept> on a variety of Linux operating systems.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Alternatively, you can go to the <bpt id="p1">[</bpt>unixODBC web site<ept id="p1">](http://www.unixodbc.org/)</ept>, download the software, and follow instructions on the site.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>2 - Install drivers</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>ODBC drivers must be installed on the machine running Machine Learning Server or R Client.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>You will need a driver that corresponds to the database version you plan to use.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>To check which drivers are installed, use the instructions below.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>On Linux</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>To list existing drivers:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Driver version information is in the odbcinst.ini file.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>To find the location of that file:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Typically, driver information is in /etc/odbcinst.ini.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>To view its contents:</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>You can also list any existing ODBC data sources already on the system:</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>On Windows</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Search for <bpt id="p1">*</bpt>odbc data sources<ept id="p1">*</ept> to find the ODBC Data Source Administrator (64-bit) application.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>In ODBC Data Source Administrator &gt; Drivers tab, review the currently installed drivers.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>If the driver you need is missing, download and install the driver using instructions provided by the vendor.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>A partial list of download links is provided below.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>ODBC download sites for commonly used databases</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Drivers for commonly used databases might be pre-installed with the operating system or database management system, but if not, most can be downloaded from database vendor web sites.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The following table provides links to download pages for several data platforms.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Data platform</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Driver download pages and instructions</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>SQL Server on Linux</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Installing the Microsoft ODBC Driver for SQL Server on Linux</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Oracle Instant Client</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Oracle Instant Client Downloads</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>MySQL</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Download Connector/ODBC</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>PostgreSQL</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>psqlODBC</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Cloudera</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Cloudera ODBC Driver for Hive</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>3 - Connect and import</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>This step uses examples to illustrate connection strings, query strings, <bpt id="p1">**</bpt>RxOdbcData<ept id="p1">**</ept> data source objects, XDF objects, and import commands for various platform configurations.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Query strings must consist of data extraction queries (SELECT and SHOW statements) that populate a single data frame or .xdf file.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>As long as a single extracted table is produced, you can use queries linked by AND, OR, and multiple FROM clauses.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Unsupported syntax includes INSERT queries or multiple query strings separated by a semicolon.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Recall that <bpt id="p1">**</bpt>RxOdbcData<ept id="p1">**</ept> provides local compute context only, which means that when you create the object, any read or write operations are executed by Machine Learning Server on the local machine.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Using SQL Server</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>This example uses a connection string to connect to a local SQL Server instance and the <bpt id="p1">[</bpt>RevoClaimsDB database<ept id="p1">](sample-built-in-data.md)</ept>.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>For simplicity, the connection is further scoped to a single table, but you could write T-SQL to select a more interesting data set.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>This returns the following:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>If you are selecting an entire table or view, a simpler alternative for the query string is just the name of that object specified as an argument on <bpt id="p1">**</bpt>RxOdbcData<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>For example: <ph id="ph1">`sDS &lt;-RxOdbcData(tabble=dbo.claims, connectionString=sConnectStr)`</ph>.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>With this shortcut, you can omit the sQuery object from your script.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>By amending the <bpt id="p1">**</bpt>RxOdbcData<ept id="p1">**</ept> object with additional arguments, you can use <bpt id="p2">*</bpt>colClasses<ept id="p2">*</ept> to recast numeric "character" data as integers or float, and use <bpt id="p3">*</bpt>stringsAsFactors<ept id="p3">*</ept> to convert all unspecified character variables to factors:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Data values for age and car.age are expressed as ranges in the original data, so those columns (as well as the type column) are appropriately converted to factors through the <bpt id="p1">*</bpt>stringsAsFactors<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Retaining the character data type for cost is also appropriate for the existing data.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>While cost has mostly numeric values, it also has multiple instances of "NA".</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>After re-import, variable metadata should be as follows:</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Using Oracle Express</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Oracle Express is a free version of the popular Oracle database management system intended for evaluation and education.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>It uses the same ODBC drivers as the commercial offerings.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>The follow example demonstrates an Oracle SQL statement to show all the tables in a database (this differs from standard SQL implementations):</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>This yields a list of tables similar to the following (showing partial results for brevity, with the first 10 tables):</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Using MySQL on Red Hat Enterprise Linux</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>As a first step, specify the name of your DSN.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>On Linux, this is the same name specified for the ODBC configuration.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Next Steps</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Continue on to the following data import articles to learn more about XDF, data source objects, and other data formats:</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Import SQL data</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Import text data</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Import and consume data on HDFS</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>XDF files</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Data Sources</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>RevoScaleR Functions</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Tutorial: data import and exploration<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept> <bpt id="p2">[</bpt>Tutorial: data manipulation and statistical analysis<ept id="p2">](tutorial-revoscaler-data-model-analysis.md)</ept></source>
        </trans-unit></group></body></file></xliff>