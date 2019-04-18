<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxrealtimescoring.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907ff1f5ea42bca81bb37ca1030041fec5b033fa22e6.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">f1f5ea42bca81bb37ca1030041fec5b033fa22e6</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxrealtimescoring.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxRealTimeScoring function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Real-time scoring brings the rxPredict functionality available in <bpt id="p1">**</bpt>RevoScaleR/revoscalepy<ept id="p1">**</ept> and <bpt id="p2">**</bpt>MicrosoftML<ept id="p2">**</ept> packages to  Microsoft ML Server and SQL Server platforms with near real-time performance.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This functionality is available on SQL Server 2017+.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>On SQL Server 2016, you can take advantage of this functionality by upgrading your in-database R Services to the latest Microsoft ML Server using the information in the following <bpt id="p1">[</bpt>link<ept id="p1">](https://docs.microsoft.com/en-us/sql/advanced-analytics/r-services/use-sqlbindr-exe-to-upgrade-an-instance-of-r-services)</ept> .</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source><bpt id="p1">**</bpt>NOTE:<ept id="p1">**</ept> This document contains information regarding <bpt id="p2">**</bpt>Real-time scoring in SQL Server ML Services<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>For information regarding <bpt id="p1">**</bpt>Real-time scoring in ML Server<ept id="p1">**</ept>, please refer to the <bpt id="p2">[</bpt>publishService<ept id="p2">](https://msdn.microsoft.com/en-us/microsoft-r/operationalize/data-scientist-manage-services#publishservice)</ept>  documentation.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxRealTimeScoring, rxRTS, realtime, realtimescoring, rts, rxPredict</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>rxRealTimeScoring: Real-time scoring in SQL Server ML Services</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Real-time scoring brings the <ph id="ph1">`rxPredict`</ph> functionality available in <bpt id="p1">**</bpt>RevoScaleR/revoscalepy<ept id="p1">**</ept> and <bpt id="p2">**</bpt>MicrosoftML<ept id="p2">**</ept> packages to  Microsoft ML Server and SQL Server platforms with near real-time performance.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>This functionality is available on SQL Server 2017+.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>On SQL Server 2016, you can take advantage of this functionality by upgrading your in-database R Services to the latest Microsoft ML Server using the information in the following <bpt id="p1">[</bpt><ph id="ph1">`link`</ph><ept id="p1">](https://docs.microsoft.com/en-us/sql/advanced-analytics/r-services/use-sqlbindr-exe-to-upgrade-an-instance-of-r-services)</ept> .</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>NOTE:<ept id="p1">**</ept> This document contains information regarding <bpt id="p2">**</bpt>Real-time scoring in SQL Server ML Services<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>For information regarding <bpt id="p1">**</bpt>Real-time scoring in ML Server<ept id="p1">**</ept>, please refer to the <bpt id="p2">[</bpt><ph id="ph1">`publishService`</ph><ept id="p2">](https://msdn.microsoft.com/en-us/microsoft-r/operationalize/data-scientist-manage-services#publishservice)</ept> documentation.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>With Microsoft R Server 9.1 version, we are introducing this feature which allows models trained using <bpt id="p1">**</bpt>RevoScaleR(revoscalepy)<ept id="p1">**</ept> and <bpt id="p2">**</bpt>MicrosoftML<ept id="p2">**</ept> packages to be used for high performance scoring in SQL Server.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>These models can be published and scored without using R interpreter, which reduces the overhead of multiple process interactions.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Hence it allows for faster prediction performance.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The following is the list of models that are currently supported in real-time scoring:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>rxLogit</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>rxLinMod</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>rxBTrees</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>rxDTree</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>rxDForest</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>MicrosoftML<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>rxFastTrees</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>rxFastForest</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>rxLogisticRegression</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>rxOneClassSvm</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>rxNeuralNet</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>rxFastLinear</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Workflow for Real-time scoring in SQL Server<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The high-level workflow for real-time scoring in SQL Server is as follows:</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>1 Serialize model for real-time scoring</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>1 Publish model to SQL Server</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>1 Enable real-time scoring functionality in SQL Server ML Services using RegisterRExt tool</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>1 Call real-time scoring stored procedure using T-SQL</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The following sections describe each of these steps in details.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>These steps are illustrated with a sample in the Example section below.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>1. Serialize model for Real-time scoring<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>To enable this functionality in SQL Server, we are adding support for serializing the model trained in R in a specific <ph id="ph1">`raw`</ph> format that allows the model to be scored in an efficient manner.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The serialized model can then be stored in a SQL Server database table for doing real-time scoring.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The following new APIs are introduced to allow this serialization functionality</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxSerializeModel<ept id="p1">](rxSerializeModel.md)</ept>() - Serialize a <bpt id="p2">**</bpt>RevoScaleR<ept id="p2">**</ept><ph id="ph1">/</ph><bpt id="p3">**</bpt>MicrosoftML<ept id="p3">**</ept> model in <ph id="ph2">`raw`</ph> format to enable saving the model to a database.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>This enables the model to be loaded into SQL Server for real-time scoring.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxUnserializeModel<ept id="p1">](rxSerializeModel.md)</ept>() - Retrieve the original R model object from the serialized raw model.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>2. Publish model to SQL Server<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The serialized models can be published to the target SQL Server Database table in <ph id="ph1">`VARBINARY`</ph> format for real-time scoring.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>You can use the existing <ph id="ph1">`rxWriteObject`</ph> API to publish the model to SQL Server.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Alternatively, you can also save the <ph id="ph1">`raw`</ph> type to a file and load into SQL Server.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxWriteObject<ept id="p1">](rxWriteObject.md)</ept>() - Store/retrieve R objects to/from ODBC data sources like SQL Server.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The API is modeled after a simple key value store.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>NOTE:<ept id="p1">**</ept> Since the model is already serialized via <ph id="ph1">`rxSerializeModel`</ph> there is no need to additionally serialize in <ph id="ph2">`rxWriteObject`</ph>, so the <ph id="ph3">`serialize`</ph> flag need to set to <ph id="ph4">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>3. Enable Real-time scoring functionality in SQL Server ML Services<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>By default, real-time scoring functionality is disabled on SQL Server ML Services and it needs to be enabled for the instance and particular SQL database.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>To use this functionality, the server administrator needs use the RegisterRExt.exe tool.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt><ph id="ph1">`RegisterRExt.exe`</ph><ept id="p1">**</ept> is the command line utility which ships with RevoScaleR package and allows administrators to enable real-time scoring feature in the SQL server instance and database.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>You can find RegisterRExt.exe at either of the following locations:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>R Services<ept id="p1">**</ept><ph id="ph1"> - </ph><ph id="ph2">`&lt;SQLInstancePath&gt;\R_SERVICES\library\RevoScaleR\rxLibs\x64\RegisterRExt.exe`</ph>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Python Services<ept id="p1">**</ept><ph id="ph1"> - </ph><ph id="ph2">`&lt;SQLInstancePath&gt;\PYTHON_SERVICES\Lib\site-packages\RevoScalepy\rxLibs\RegisterRext.exe`</ph>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>3a. Enable real-time scoring for SQL Server instance<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Open an elevated command prompt and run the following command:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>To disable real-time scoring for SQL Server instance, open an elevated command prompt and run the following command:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>3b. Enable real-time scoring for a particular database<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Open an elevated command prompt and run the following command:</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>To disable real-time scoring for a particular database, open an elevated command prompt and run the following command:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The /instance flag is optional if the database is part of the default SQL Server instance.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>This command will create assemblies and stored procedure on the SQL Server database to allow real-time scoring.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Additionally, it creates a database role <ph id="ph1">`rxpredict_users`</ph> to help database admins to grant permission to use the real-time scoring functionality.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>/python flag is required only if using PYTHON SERVICES version of registerrext.exe</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>NOTE:<ept id="p1">**</ept> In SQL Server 2016, RegisterRExt will enable  SQL CLR functionality in the instance and the specific database will be marked as <ph id="ph1">`TRUSTWORTHY`</ph>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Please carefully consider additional security implications of doing this.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>In SQL Server 2017 and higher, SQL CLR will be enabled and specific CLR assemblies are trusted using sp_addtrustedassembly.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>4. Call real-time scoring stored procedure using T-SQL<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The functionality once installed, will be available in the particular SQL Server database via a stored procedure called <ph id="ph1">`sp_rxPredict`</ph>.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Here is the syntax of the <ph id="ph1">`sp_rxPredict`</ph> stored procedure</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Syntax<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`@model [VARBINARY](max)`</ph>,</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>where</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`@model`</ph> - Real-time model to be used for scoring in <ph id="ph2">`VARBINARY`</ph> format</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`@inputData`</ph> - SQL query to be used to get the input data for scoring</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Limitations<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>1 Real-time scoring does not use an R/python interpreter for scoring hence any functionality requiring R interpreter is not supported.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Here are a few unsupported scenarios:</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Models of <ph id="ph1">`rxGlm`</ph> and <ph id="ph2">`rxNaiveBayes`</ph> algorithms are not currently supported</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> Models with R transform function or transform based formula (e.g <ph id="ph1">`"A ~ log(B)"`</ph>) are not supported in real-time scoring.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Such transforms to input data may need to be handled before calling real-time scoring.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>1 Arguments other than <ph id="ph1">`modelObject`</ph><ph id="ph2">/</ph><ph id="ph3">`data`</ph> available in <ph id="ph4">`rxPredict`</ph> are not supported in real-time scoring</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Known Issues<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>1 <ph id="ph1">`sp_rxPredict`</ph> with <ph id="ph2">`RevoScaleR`</ph> model only supports only following .NET column types are double, float, short, ushort, long, ulong and string.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>You may need to filter out unsupported types in your input data before using it for real-time scoring.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>For corresponding SQL type information refer <bpt id="p1">[</bpt><ph id="ph1">`SQL-CLR Type Mapping`</ph><ept id="p1">](https://msdn.microsoft.com/en-us/library/bb386947(v=vs.110).aspx)</ept></source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>1 <ph id="ph1">`sp_rxPredict`</ph> is optimized for fast predictions on smaller data (from a few rows to a few 1000 rows), the performance may start degrading on larger data sets.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>1 <ph id="ph1">`sp_rxPredict`</ph> returns inaccurate error message when NULL value is passed as model</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`System.Data.SqlTypes.SqlNullValueException:`</ph><bpt id="p1">**</bpt>Data in Null<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxSerializeModel<ept id="p1">](rxSerializeModel.md)</ept>, <bpt id="p2">[</bpt>rxWriteObject<ept id="p2">](rxWriteObject.md)</ept>, publishService, <bpt id="p3">[</bpt>rxPredict<ept id="p3">](rxPredict.md)</ept></source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>