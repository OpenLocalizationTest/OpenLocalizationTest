<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="olapr.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b428e0e5a1c4c11eda2e401d8c9bd0487969f7d180.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">28e0e5a1c4c11eda2e401d8c9bd0487969f7d180</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\olapr\olapr.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>OlapR package for R (Microsoft R Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Function help reference for the olapR R package of Microsoft R Server, used to import data from OLAP cubes stored in SQL Server Analysis Services into R.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>olapR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>olapR package</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>olapR<ept id="p1">**</ept> library provides R functions for importing data from OLAP cubes stored in SQL Server Analysis Services into a data frame.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This package is available on premises, on Windows only.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Package details</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Current version:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>1.0.0</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Built on:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>R 3.4.3</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Package distribution:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server for Windows<ept id="p1">](../../what-is-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>R Client (Windows)<ept id="p1">](../../r-client/what-is-microsoft-r-client.md)</ept></source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>R Server 9.1<ept id="p1">](../../what-is-microsoft-r-server.md)</ept></source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SQL Server 2017 Machine Learning Services (Windows only) and SQL Server 2016 R Services<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/getting-started-with-machine-learning-services)</ept></source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>How to use olapR</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>olapR<ept id="p1">**</ept> library provides a simple R style API for generating and validating MDX queries against an Analysis Services cube.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>olapR<ept id="p1">**</ept> does not provide APIs for all MDX scenarios, but it does cover the most use cases including slice, dice, drilldown, rollup, and pivot scenarios in N dimensions.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>You can also input a direct MDX query to Analysis Services for queries that cannot be constructed using the olapR APIs.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Workflow for using olapR<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Load the library.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Create a connection string pointing to a MOLAP cube on Analysis Services.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Verify you have read access on the cube</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Use the connection string on a connection.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Verify the connection using the explore function.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Set up a query by submitting an MDX query string or by building a query structure.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Execute the query and verify the result.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>To execute an MDX query on an OLAP Cube, you need to first create a connection string (<ph id="ph1">`olapCnn`</ph>) and validate using the function <ph id="ph2">`OlapConnection(connectionString)`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The connection string must have a Data Source (such as localhost) and a Provider (MSOLAP).</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>After the connection is established, you can either pass in a fully defined MDX query, or you can construct the query using the <ph id="ph1">`Query()`</ph> object, setting the query details using cube(), axis(), columns(), slicers(), and so forth.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Finally, pass the <ph id="ph1">`olapCnn`</ph> and query into either <ph id="ph2">`executeMD`</ph> or <ph id="ph3">`execute2D`</ph> to get a multidimensional array or a data frame back.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>olapR<ept id="p1">**</ept> requires the Analysis Services OLE DB provider.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If you do not have SQL Server Analysis Services installed on your computer, download the provider from Microsoft: <bpt id="p1">[</bpt>Data providers used for Analysis Services connections<ept id="p1">](https://docs.microsoft.com/sql/analysis-services/instances/data-providers-used-for-analysis-services-connections)</ept></source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The exact version you should install for SQL Server 2016 is <bpt id="p1">[</bpt>here<ept id="p1">](https://download.microsoft.com/download/8/7/2/872BCECA-C849-4B40-8EBE-21D48CDF1456/ENU/x64/SQL_AS_OLEDB.msi)</ept>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Function list</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Create the connection string to access the Analysis Services Database.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Construct a Query object to use on the Analysis Services Database.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Use cube, axis, columns, rows, pages, chapters, slicers to add details to the query.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Takes a Query object or an MDX string, and returns the result as a multi-dimensional array.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Takes a Query object or an MDX string, and returns the result as a 2D data frame.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Allows for exploration of cube metadata.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>MDX concepts</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>MDX is the query language for multidimensional OLAP (MOLAP) cubes containing processed and aggregated data stored in structures optimized for data analysis and exploration.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Cubes are used in business and scientific applications to draw insights about relationships in historical data.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Internally, cubes consist of mostly quantifiable numeric data, which is sliced along dimensions like date and time, geography, or other entities.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>A typical query might roll up sales for a given region and time period, sliced by product category, promotion, sales channel, and so forth.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Cube data can be accessed using various operations:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Slicing - Taking a subset of the cube by picking a value for one dimension, resulting in a cube that is one dimension smaller.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Dicing - Creating a subcube by specifying a range of values on multiple dimensions.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Drill-Down/Up - Navigate from more general to more detailed data ranges, or vice versa.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Roll-up - Summarize the data on a dimension.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Pivot - Rotate the cube.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>MDX queries are similar to SQL queries but, because of the flexibility of OLAP databases, can contain up to 128 query axes.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>The first four axes are named for convenience: Columns, Rows, Pages, and Chapters.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>It's also common to just use two (Rows and Columns), as shown in the following example:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Using an AdventureWorks OLAP cube from the <bpt id="p1">[</bpt>multidimensional cube tutorial<ept id="p1">](https://docs.microsoft.com/sql/analysis-services/multidimensional-modeling-adventure-works-tutorial)</ept>, this MDX query selects the internet sales count and sales amount and places them on the Column axis.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>On the Row axis it places all possible values of the "Product Line" dimension.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Then, using the WHERE clause (which is the slicer axis in MDX queries), it filters the query so that only the sales from Australia matter.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Without the slicer axis, we would roll up and summarize the sales from all countries.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>olapR examples</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Learn more about MDX concepts:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>OLAP Cubes: <bpt id="p1">[</bpt><ph id="ph1">https://en.wikipedia.org/wiki/OLAP_cube</ph><ept id="p1">](https://en.wikipedia.org/wiki/OLAP_cube)</ept></source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>MDX queries: <bpt id="p1">[</bpt><ph id="ph1">https://en.wikipedia.org/wiki/MultiDimensional_eXpressions</ph><ept id="p1">](https://en.wikipedia.org/wiki/MultiDimensional_eXpressions)</ept></source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Create a demo OLAP Cube (identical to examples): <bpt id="p1">[</bpt>multidimensional cube tutorial<ept id="p1">](https://docs.microsoft.com/sql/analysis-services/multidimensional-modeling-adventure-works-tutorial)</ept></source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Using data from OLAP cubes in R (SQL Server)<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/r/using-data-from-olap-cubes-in-r)</ept></source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>R Package Reference<ept id="p1">](../introducing-r-server-r-package-reference.md)</ept></source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>R Client<ept id="p1">](../../r-client/what-is-microsoft-r-client.md)</ept></source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>R Server<ept id="p1">](../../what-is-microsoft-r-server.md)</ept></source>
        </trans-unit></group></body></file></xliff>