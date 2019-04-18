<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-sql-server.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18cdc7578d81b81a0034a4792eef2d280041fbe2b51.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">dc7578d81b81a0034a4792eef2d280041fbe2b51</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-sql-server.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Use RevoScaleR with SQL Server (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Overview and tutorial to using RevoScaleR in SQL Server databases.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Using RevoScaleR with SQL Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>By using the <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions in your R solutions, you can create high-performance big data analytics that use SQL Server data, or that run in the context of a SQL Server database server.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>This introduction provides general knowledge that you need to get started with analyzing SQL Server data, or moving your models into production in SQL Server 2016.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>It is primarily intended for users who are already have a basic familiarity with the R language and would like to understand more about how to use the <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> package with SQL Server.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>We recommend that you read this introduction to understand the requirements and basic workflows, and refer to SQL Server Books Online.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>In particular, the walkthrough that was previously included in this guide is now published as a tutorial for <bpt id="p1">**</bpt>SQL Server R Services<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Data Science End-to-End Walkthrough<ept id="p1">](https://msdn.microsoft.com/library/mt612857.aspx)</ept>: Load, explore, and analyze the New York City taxi dataset.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Build models and deploy them to SQL Server for production.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Using the RevoScaleR Packages<ept id="p1">](https://msdn.microsoft.com/library/mt637368.aspx)</ept>: Deep dive on the anaytical sunctions provided by the <bpt id="p2">**</bpt>RevoScaleR<ept id="p2">**</ept> package.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Demonstrates how to create and use compute contexts, how to move data between local and server compute contexts using XDF files, and creates a simulation using R code that runs in SQL Server.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Data Science Scenarios and Solution Templates<ept id="p1">](https://msdn.microsoft.com/en-us/library/mt693423.aspx)</ept>: Includes all the R and T-SQL code you need for fraud detection, churn analysis, predictive maintenance, and demand forecasting.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>All tutorials include sample code, along with explanations of how to work with SQL and R.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Basic Operations</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> package is included when you install <bpt id="p2">**</bpt>SQL Server R Services<ept id="p2">**</ept> on an instance of SQL Server 2016.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> is also included in all installations of <bpt id="p2">**</bpt>Machine Learning Server<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Development</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>You can develop your R solutions in any R IDE you prefer.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>We recommend that you use a standalone R IDE when testing your code and exploring your data, rather than trying to write R code inside of T-SQL.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>For R Services in particular, <bpt id="p1">[</bpt>R Tools for Visual Studio<ept id="p1">](https://www.visualstudio.com/features/rtvs-vs.aspx)</ept> is a good choice, because it has strong support for both R code and integration with SQL Server, but you can use any IDE that supports database connectivity.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>To run R code within the context of SQL Server, you have two options:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Run code from your laptop or any remote workstation, but set the compute context to SQL Server..</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Copy R code into the <ph id="ph1">@script</ph> argument of a special SQL stored procedure, <bpt id="p1">[</bpt>sp_execute_external_script<ept id="p1">](https://msdn.microsoft.com/library/mt604368.aspx)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>You can provide input data as a parameter of the stored procedure, call the stored procedure from any application that supports SQL calls, and easily export results to any application that can consume SQL data.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Getting SQL Server Data</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>To work with SQL Server data in R, you must create a SQL Server data source in your R code.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>to do this, use the <ph id="ph1">`RxSqlServerData`</ph> function, which defines the connection string and the data you want to use.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The data source is saved as a variable that points to the data.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The data is not actually loaded or moved until you use a function that uses the data, such as the <ph id="ph1">`rxDataStep`</ph> (which can work with multiple data sources) or <ph id="ph2">`rxGetVarInfo`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The ability to save the data source object in a variable makes it very easy to re-use connection information with different functions, create multiple variables for different tables in a single source, and so forth.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Most of the rx functions also support moving or analyzing data in chunks.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Additionally, with SQL Server data you can stream data, sending a predefined number of rows in each batch, or, if the function supports it, process the data in parallel.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>In contrast, when you read data from a database using RODBC, all the data is read into memory, making it difficult to work with large datasets.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Using SQL Server as a Compute Context</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>A defining feature of the <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> package is that most of its functions support execution of R code in different compute contexts.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>To run your R code on the SQL Server computer:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Define a compute context that points to the database server.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Change the <bpt id="p1">*</bpt>active compute context<ept id="p1">*</ept> to use the SQL Server computer.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>To switch back to local execution, reset the compute context to the default.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If you run R code within T-SQL code, the server is always used as the compute context.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>In this scenario, your code will call the R libraries installed on the SQL Server instance, and use secure connections to get data from the database.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>You can also save models in a database table, load models from a table to use for scoring, and save your results ot a databse table, all without leaving the context of SQL Server.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>For more information, see SQL Server 2016 Books Online:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Data Exploration and Predictive Modeling with R<ept id="p1">](https://msdn.microsoft.com/library/mt590947.aspx)</ept></source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>R Interoperability in SQL Server R Services<ept id="p1">](https://docs.microsoft.com/en-us/sql/advanced-analytics/r/r-interoperability-in-sql-server)</ept></source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Deploying, Managing, and Optimizing Solutions</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>One of the primary goals of providing R Services in SQL Server is to make it easier to deploy R code in production.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Typically you'll deploy your R code to production by wrapping it in a stored procedure.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Stored procedures in SQL Server support parameterization, making it easy to pass in a SQL query as input, and save the results to the database.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Because the syntax for calling stored procedures is supported by many applications, you do not need to write any extra code to call your R code from an external application -- just pass in the data and handle the results that are returned.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>You can also generate visualizations and archive them locally, export them to other applications such as Reporting Services or Power BI, or send them back to your local workstation for review.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Finally, because R Services is integrated with SQL Server, you can use database server tools for monitoring code execution and managing and balancing resources.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>For more information, see SQL Server 2016 Books Online:</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Operationalizing Your R Code<ept id="p1">](https://msdn.microsoft.com/library/mt590864.aspx)</ept></source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Resource Governance for R Services<ept id="p1">](https://msdn.microsoft.com/library/mt703708.aspx)</ept></source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SQL Server R Services Performance Tuning<ept id="p1">](https://msdn.microsoft.com/en-us/library/mt723573.aspx)</ept></source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Related Guides</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>For information on other distributed computing compute contexts, see:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to use RevoScaleR on Hadoop MapReduce<ept id="p1">](how-to-revoscaler-hadoop.md)</ept></source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to use RevoScaleR on Spark<ept id="p1">](how-to-revoscaler-spark.md)</ept></source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>More information on <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> can be found here:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Tutorial: Data Import<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept></source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR Function Reference<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept></source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Distributed Computing<ept id="p1">](how-to-revoscaler-distributed-computing.md)</ept></source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR ODBC Data Import<ept id="p1">](how-to-revoscaler-data-odbc.md)</ept></source>
        </trans-unit></group></body></file></xliff>