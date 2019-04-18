<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-data-source.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f99bf0d24bfeca38f6934fb79f3235f84f9b6c4bb.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">99bf0d24bfeca38f6934fb79f3235f84f9b6c4bb</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-data-source.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Data source objects in RevoScaleR (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn when and how to create data source objects in R code leveraging the RevoScaleR function libraries.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Data Sources in RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">*</bpt>data source<ept id="p1">*</ept> in RevoScaleR is an R object representing a data set.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>It is the return object of <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> for read operations and <bpt id="p2">**</bpt>rxDataStep<ept id="p2">**</ept> for write operations.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Although the data itself may be on disk, a data source is an in-memory object that allows you to treat data from disparate sources in a consistent manner within RevoScaleR.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Behind the scenes, <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> often creates data sources implicitly to facilitate data import.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>You can explicitly create data sources for more control over how data is imported, such as setting arguments to control how many rows are read into the object.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>This article explains how to create a variety of data sources and use them in an analytical context.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Data Source Constructors</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>To create data sources directly, use the constructors listed in the following table:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Source Data<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Data Source Constructor<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Text (fixed-format or delimited)</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxTextData<ept id="p1">](how-to-revoscaler-data-import.md)</ept></source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>SAS</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxSasData<ept id="p1">](../r-reference/revoscaler/rxsasdata.md)</ept></source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>SPSS</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxSpssData<ept id="p1">](../r-reference/revoscaler/rxspssdata.md)</ept></source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>ODBC Database</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxOdbcData<ept id="p1">](how-to-revoscaler-data-odbc.md)</ept></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Teradata Database</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxTeradata<ept id="p1">](../r-reference/revoscaler/rxteradata.md)</ept></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>SQL Server Database</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxSqlServerData<ept id="p1">](how-to-revoscaler-data-sql.md)</ept></source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Spark data: Hive, Parquet and ORC</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxSparkData<ept id="p1">](../r-reference/revoscaler/rxsparkdata.md)</ept> or <bpt id="p2">**</bpt>RxHiveData<ept id="p2">**</ept>, <bpt id="p3">**</bpt>RxParquetData<ept id="p3">**</ept>, <bpt id="p4">**</bpt>RxOrcData<ept id="p4">**</ept></source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>.xdf data files</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxXdfData<ept id="p1">](concept-what-is-xdf.md)</ept></source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>XDF files<ept id="p1">](concept-what-is-xdf.md)</ept> are the out files for <bpt id="p2">**</bpt>rxImport<ept id="p2">**</ept> read operations, but you also use them as a data source input when loading all or part of an .xdf into a data frame.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Using an XDF data source is recommended for repeated analysis of a single data set.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>It is almost always faster to import data into an .xdf file and run analyses on the .xdf data source than to load data from an original data source.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>When to create a data source</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>For simple data import, it's not necessary to explicitly create a data source.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>You can simply specify a file path for a file that <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> can read, and RevoScaleR will read it using the default settings.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>However, if you need to provide additional options specific to that data source type, you should create a data source using a constructor from the previous list.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>How to create a data source</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>You can create a data source the same way you create any object in R, by giving it a name and using a constructor.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The first argument of any RevoScaleR data source is the source data:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>As a coding best practice, create a file object first, and pass that to the data source:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>After the data source object is created, you can return object properties, precomputed metadata, and rows.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Use standard R methods</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>A number of standard R methods can be used with RevoScaleR data sources.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>You might be familiar with <bpt id="p1">**</bpt>names<ept id="p1">**</ept> for viewing variable names, or <bpt id="p2">**</bpt>head<ept id="p2">**</ept> for viewing the first few rows:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>By loading data into a data frame using <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept>, you can use additional functions, such as the <bpt id="p2">**</bpt>dim<ept id="p2">**</ept> function to return dimensions, and  <bpt id="p3">**</bpt>colnames<ept id="p3">**</ept> or <bpt id="p4">**</bpt>dimnames<ept id="p4">**</ept> as an alternative to <bpt id="p5">**</bpt>RxGetVarInfo<ept id="p5">**</ept> to obtain variable names.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>You can obtain the number of variables using the <bpt id="p1">**</bpt>length<ept id="p1">**</ept> function:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>View the <bpt id="p1">**</bpt>last<ept id="p1">**</ept> rows of a data source using the <bpt id="p2">**</bpt>tail<ept id="p2">**</ept> function:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>By adding <bpt id="p1">*</bpt>outFile<ept id="p1">*</ept> to <bpt id="p2">**</bpt>rxImport<ept id="p2">**</ept>, you create an XDF data source, which you can return using <bpt id="p3">**</bpt>summary<ept id="p3">**</ept>:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>For .xdf file data sources, <bpt id="p1">**</bpt>dimnames<ept id="p1">**</ept> returns only column names.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Row names are not provided because .xdf files do not contain row names:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Data source by compute context</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>In the local compute context, all of RevoScaleR’s supported data sources are available to you.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>In a distributed context, the data source object aligns to the compute context.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Thus, <bpt id="p1">**</bpt>RxInSqlServer<ept id="p1">**</ept> only supports <bpt id="p2">**</bpt>RxSqlServerData<ept id="p2">**</ept> objects.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Likewise for <bpt id="p1">**</bpt>RxInTeradata<ept id="p1">**</ept>, which supports only the <bpt id="p2">**</bpt>RxTeradata<ept id="p2">**</ept> data sources.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Compute context<ept id="p1">](concept-what-is-compute-context.md)</ept>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Compute Context</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Data Source</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>RxLocalSeq</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>RxSpark</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>RxHadoopMR</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>RxInSqlServer</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>RxInTeradata</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Delimited Text (RxTextData)</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Fixed-Format Text (RxTextData)</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>.xdf data files (RxXdfData)</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>SAS data files (RxSasData)</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>SPSS data files (RxSpssData)</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>ODBC data (RxOdbcData)</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>SQL Server database (RxSqlServerData)</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Teradata database (RxTeradata)</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Spark data <bpt id="p1">[</bpt>RxSparkData<ept id="p1">](../r-reference/revoscaler/rxsparkdata.md)</ept></source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>x</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The following examples show how to instantiate and use various data sources.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>RxSasData</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Sample data includes claims.sas7bdat, which you can load without having SAS installed.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Retrieve variables in the data by calling R's <bpt id="p1">**</bpt>names<ept id="p1">**</ept> function:</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Compute a regression, passing the data source as the data argument to <bpt id="p1">**</bpt>rxLinMod<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>RxSpssData</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Similarly, you could use the SPSS version of the claims data as follows:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>RxXdfData</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>This example shows how to create a data source from the built-in claims.xdf data set:</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Use the open method <bpt id="p1">**</bpt>rxOpen<ept id="p1">**</ept> to open the data source:</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Use the method <bpt id="p1">**</bpt>rxReadNext<ept id="p1">**</ept> to read the next block of data from the data source:</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">**</bpt>rxClose<ept id="p1">**</ept> method to close the data source:</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>XDF data sources with biglm</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Since data sources for xdf files read data in chunks, it is a good match for the CRAN package <bpt id="p1">**</bpt>biglm<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>biglm<ept id="p1">**</ept> package does a linear regression on an initial chunk of data, then updates the results with subsequent chunks.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Below is a function that loops through an xdf file object and creates and updates the <bpt id="p1">**</bpt>biglm<ept id="p1">**</ept> results.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>To use the function, we first open the data file.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>For example, we can again use the large airline data set AirOnTime87to12.xdf:</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Then we will time the computation, doing the regression for all the rows— 148,619,655 if you are using the full data set.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Note that it takes several minutes to load the data, even on a very fast machine.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>We can see the coefficients by looking at a summary of the object returned:</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>It is, of course, much faster to compute a linear model using the <bpt id="p1">**</bpt>rxLinMod<ept id="p1">**</ept> function, but the <bpt id="p2">**</bpt>biglm<ept id="p2">**</ept> package provides alternative methods of computation.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Next Steps</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Continue on to the following data import articles to learn more about XDF and other data formats:</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>XDF files<ept id="p1">](concept-what-is-xdf.md)</ept></source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Import SQL Server data<ept id="p1">](how-to-revoscaler-data-sql.md)</ept></source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Import text data<ept id="p1">](how-to-revoscaler-data-import.md)</ept></source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Import and consume data on HDFS<ept id="p1">](how-to-revoscaler-data-hdfs.md)</ept></source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR Functions<ept id="p1">](~/r-reference/revoscaler/revoscaler.md)</ept><ph id="ph1"> </ph></source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Tutorial: data import and exploration<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept> <bpt id="p2">[</bpt>Tutorial: data manipulation and statistical analysis<ept id="p2">](tutorial-revoscaler-data-model-analysis.md)</ept></source>
        </trans-unit></group></body></file></xliff>