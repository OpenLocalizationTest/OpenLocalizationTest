<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="sqlrutils.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3a9d576b764fd5926581055a216f1cb9054d4de5c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a9d576b764fd5926581055a216f1cb9054d4de5c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\sqlrutils\sqlrutils.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>sqlrutils Functions R Package for Machine Learning Server and R Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>A package used for executing stored procedures on SQL Server from R script.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>sqlrutils package reference</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>sqlrutils package</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>sqlrutils<ept id="p1">**</ept> package provides a mechanism for R users to put their R scripts into a T-SQL stored procedure, register that stored procedure with a database, and run the stored procedure from an R development environment.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Package details</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Current version:</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>1.0.0</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Built on:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>R 3.4.3</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Package distribution:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>SQL Server 2017 Machine Learning Services (Windows only) and SQL Server 2016 R Services</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>R Client (Windows and Linux)</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>How to use sqlrutils</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>sqlrutils<ept id="p1">**</ept> library is installed as part of SQL Server Machine Learning when you add R to your installation.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>You get the full collection of proprietary packages plus an R distribution with its base packages and interpreters.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>You can use any R IDE to write R script calling functions in <bpt id="p1">**</bpt>sqlrutils<ept id="p1">**</ept>, but the script must run on a computer having SQL Server Machine Learning with R.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The workflow for using this package includes the following steps:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Define stored procedure parameters (inputs, outputs, or both)</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Generate and register the stored procedure</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Execute the stored procedure</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>In an R session, load <bpt id="p1">**</bpt>sqlrutils<ept id="p1">**</ept> from the command line by typing <ph id="ph1">`library(sqlrutils)`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>You can load this library on computer that does not have SQL Server (for example, on an R Client instance) if you change the compute context to SQL Server and execute the code in that compute context.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Function list</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Class</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>executeStoredProcedure</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Execute a SQL stored procedure.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>getInputParameters</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Get a list of input parameters to the stored procedure.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>InputData</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Input data for the stored procedure.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>InputParameter</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Input parameters for the stored procedure.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>OutputData</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Output from the stored procedure.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>OutputParameter</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Output parameters from the stored procedure.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>registerStoredProcedure</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Register the stored procedure with a database.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>setInputDataQuery</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Assign a query to an input data parameter of the stored procedure.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>setInputParameterValue</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Assign a value to the an input parameter of the stored procedure.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>StoredProcedure</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>A stored procedure object.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Add R packages to your computer by running setup for R Server or R Client:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>R Client</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>R Server</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Next, review the steps in a typical sqlrutils workflow:</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Generating an R Stored Procedure for R Code using the sqlrutils Package</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Package Reference</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>R tutorials for SQL Server</source>
        </trans-unit></group></body></file></xliff>