<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="revoscaler-hadoop-functions.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea9264ab8531e701125298615616c5464b40eed800399.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">4ab8531e701125298615616c5464b40eed800399</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\revoscaler-hadoop-functions.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Spark and Hadoop RevoScaleR functions (Machine Learning Server and Microsoft R)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Microsoft R RevoScaleR Functions for Apache Hadoop Spark and Hadoop MapReduce.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RevoScaleR, RevoScaleR, Microsoft R, Hadoop, Spark</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RevoScaleR Functions for Spark on Hadoop</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>RevoScaleR package<ept id="p1">](revoscaler.md)</ept> provides a set of portable, scalable, distributable data analysis functions.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This page presents a curated list of functions that might be particularly interesting to Hadoop users.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>These functions can be called directly from the command line.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The RevoScaleR package supports two Hadoop compute contexts:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>RxSpark (recommended), a distributed compute context in which computations are parallelized and distributed across the nodes of a Hadoop cluster via Apache Spark.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>This provides up to a 7x performance boost compared to <ph id="ph1">`RxHadoopMR`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>For guidance, see <bpt id="p1">[</bpt>How to use RevoScaleR on Spark<ept id="p1">](~/r/how-to-revoscaler-spark.md)</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>RxHadoopMR (deprecated), a distributed compute context on a Hadoop cluster.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>This compute context can be used on a node (including an edge node) of a Cloudera or Hortonworks cluster with a RHEL operating system, or a client with an SSH connection to such a cluster.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>For guidance, see <bpt id="p1">[</bpt>How to use RevoScaleR on Hadoop MapReduce<ept id="p1">](~/r/how-to-revoscaler-hadoop.md)</ept>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>On Hadoop Distributed File System (HDFS), the XDF file format stores data in a composite set of files rather than a single file.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Data Analysis Functions</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Import and Export Functions</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Function Name</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt>Help<ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Transform and subset data.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Creates an .xdf file, a comma-delimited text file, or data frame in memory (assuming you have sufficient memory to hold the output data) from an .xdf file or a data frame.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
            &lt;center&gt;</ph><ph id="ph2">&lt;small&gt;</ph><bpt id="p1">&lt;a href="rxdatastep.md" data-raw-source="[**View**](rxdatastep.md)"&gt;</bpt><bpt id="p2">&lt;strong&gt;</bpt>View<ept id="p2">&lt;/strong&gt;</ept><ept id="p1">&lt;/a&gt;</ept><ph id="ph3">&lt;center&gt;</ph><ph id="ph4">&lt;/small&gt;</ph></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Creates an efficient XDF data source object.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
            &lt;center&gt;</ph><ph id="ph2">&lt;small&gt;</ph><bpt id="p1">&lt;a href="rxxdfdata.md" data-raw-source="[**View**](rxxdfdata.md)"&gt;</bpt><bpt id="p2">&lt;strong&gt;</bpt>View<ept id="p2">&lt;/strong&gt;</ept><ept id="p1">&lt;/a&gt;</ept><ph id="ph3">&lt;center&gt;</ph><ph id="ph4">&lt;/small&gt;</ph></source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Creates a comma delimited text data source object.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
            &lt;center&gt;</ph><ph id="ph2">&lt;small&gt;</ph><bpt id="p1">&lt;a href="rxtextdata.md" data-raw-source="[**View**](rxtextdata.md)"&gt;</bpt><bpt id="p2">&lt;strong&gt;</bpt>View<ept id="p2">&lt;/strong&gt;</ept><ept id="p1">&lt;/a&gt;</ept><ph id="ph3">&lt;center&gt;</ph><ph id="ph4">&lt;/small&gt;</ph></source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Retrieves summary information from a data source or data frame.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
            &lt;center&gt;</ph><ph id="ph2">&lt;small&gt;</ph><bpt id="p1">&lt;a href="rxgetinfoxdf.md" data-raw-source="[**View**](rxgetinfoxdf.md)"&gt;</bpt><bpt id="p2">&lt;strong&gt;</bpt>View<ept id="p2">&lt;/strong&gt;</ept><ept id="p1">&lt;/a&gt;</ept><ph id="ph3">&lt;center&gt;</ph><ph id="ph4">&lt;/small&gt;</ph></source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Retrieves variable information from a data source or data frame.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
            &lt;center&gt;</ph><ph id="ph2">&lt;small&gt;</ph><bpt id="p1">&lt;a href="rxgetvarinfo.md" data-raw-source="[**View**](rxgetvarinfo.md)"&gt;</bpt><bpt id="p2">&lt;strong&gt;</bpt>View<ept id="p2">&lt;/strong&gt;</ept><ept id="p1">&lt;/a&gt;</ept><ph id="ph3">&lt;center&gt;</ph><ph id="ph4">&lt;/small&gt;</ph></source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Retrieves variable names from a data source or data frame.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
            &lt;center&gt;</ph><ph id="ph2">&lt;small&gt;</ph><bpt id="p1">&lt;a href="rxgetvarnames.md" data-raw-source="[**View**](rxgetvarnames.md)"&gt;</bpt><bpt id="p2">&lt;strong&gt;</bpt>View<ept id="p2">&lt;/strong&gt;</ept><ept id="p1">&lt;/a&gt;</ept><ph id="ph3">&lt;center&gt;</ph><ph id="ph4">&lt;/small&gt;</ph></source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Creates an HDFS file system object.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
            &lt;center&gt;</ph><ph id="ph2">&lt;small&gt;</ph><bpt id="p1">&lt;a href="rxhdfsfilesystem.md" data-raw-source="[**View**](rxhdfsfilesystem.md)"&gt;</bpt><bpt id="p2">&lt;strong&gt;</bpt>View<ept id="p2">&lt;/strong&gt;</ept><ept id="p1">&lt;/a&gt;</ept><ph id="ph3">&lt;center&gt;</ph><ph id="ph4">&lt;/small&gt;</ph></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
####</ph> Manipulation, Cleansing, and Transformation Functions</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Function Name</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt>Help<ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Transform and subset data.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Creates an .xdf file, a comma-delimited text file, or data frame in memory (assuming you have sufficient memory to hold the output) from an .xdf file or a data frame.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxdatastep.md" data-raw-source="[**View**](rxdatastep.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Create or recode factor variables in a composite XDF file in HDFS.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>A new file must be written out.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxfactors.md" data-raw-source="[**View**](rxfactors.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
####</ph> Analysis Functions for Descriptive Statistics and Cross-Tabulations</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Function Name</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt>Help<ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Computes approximate quantiles for .xdf files and data frames without sorting.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxquantile.md" data-raw-source="[**View**](rxquantile.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Basic summary statistics of data, including computations by group.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Writing by group computations to .xdf file not supported.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxsummary.md" data-raw-source="[**View**](rxsummary.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Formula-based cross-tabulation of data.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxcrosstabs.md" data-raw-source="[**View**](rxcrosstabs.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Alternative formula-based cross-tabulation designed for efficient representation returning ‘cube’ results.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Writing output to .xdf file not supported.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxcube.md" data-raw-source="[**View**](rxcube.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
####</ph> Analysis, Learning, and Prediction Functions for Statistical Modeling</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Function Name</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt>Help<ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Fits a linear model to data.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxlinmod.md" data-raw-source="[**View**](rxlinmod.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Fits a logistic regression model to data.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxlogit.md" data-raw-source="[**View**](rxlogit.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Fits a generalized linear model to data.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxglm.md" data-raw-source="[**View**](rxglm.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Calculate the covariance, correlation, or sum of squares / cross-product matrix for a set of variables.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxcovcor.md" data-raw-source="[**View**](rxcovcor.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Fits a classification or regression tree to data.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxdtree.md" data-raw-source="[**View**](rxdtree.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Fits a classification or regression decision forest to data using a stochastic gradient boosting algorithm.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxbtrees.md" data-raw-source="[**View**](rxbtrees.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Fits a classification or regression decision forest to data.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxdforest.md" data-raw-source="[**View**](rxdforest.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Calculates predictions for fitted models.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Output must be an XDF data source.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="../microsoftml/rxpredict.md" data-raw-source="[**View**](../microsoftml/rxpredict.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Performs k-means clustering.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxkmeans.md" data-raw-source="[**View**](rxkmeans.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Fit Naive Bayes Classifiers on an .xdf file or data frame for small or large data using parallel external memory algorithm.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxnaivebayes.md" data-raw-source="[**View**](rxnaivebayes.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Compute Context Functions</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Function Name</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt>Help<ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Creates an in-data, file-based Hadoop compute context.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxhadoopmr.md" data-raw-source="[**View**](rxhadoopmr.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Creates an in-data, file-based Spark compute context.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Computations are parallelized and distributed across the nodes of a Hadoop cluster via Apache Spark.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxspark.md" data-raw-source="[**View**](rxspark.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Creates a persistent Spark compute context.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
        &lt;center&gt;</ph><ph id="ph2">&lt;small&gt;</ph><bpt id="p1">&lt;a href="rxspark.md" data-raw-source="[**View**](rxspark.md)"&gt;</bpt><bpt id="p2">&lt;strong&gt;</bpt>View<ept id="p2">&lt;/strong&gt;</ept><ept id="p1">&lt;/a&gt;</ept><ph id="ph3">&lt;center&gt;</ph><ph id="ph4">&lt;/small&gt;</ph></source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Disconnects a Spark session and return to a local compute context.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
        &lt;center&gt;</ph><ph id="ph2">&lt;small&gt;</ph><bpt id="p1">&lt;a href="rxspark.md" data-raw-source="[**View**](rxspark.md)"&gt;</bpt><bpt id="p2">&lt;strong&gt;</bpt>View<ept id="p2">&lt;/strong&gt;</ept><ept id="p1">&lt;/a&gt;</ept><ph id="ph3">&lt;center&gt;</ph><ph id="ph4">&lt;/small&gt;</ph></source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Returns the list of installed packages for a compute context.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxinstalledpackages.md" data-raw-source="[**View**](rxinstalledpackages.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Returns the path to one or more packages for a compute context.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxfindpackage.md" data-raw-source="[**View**](rxfindpackage.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Data Source Functions</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Of course, not all data source types are available on all compute contexts.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>For the Hadoop compute contexts, two types of data sources can be used.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Function Name</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt>Help<ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Creates an efficient XDF data source object.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxxdfdata.md" data-raw-source="[**View**](rxxdfdata.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Creates a comma delimited text data source object.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxtextdata.md" data-raw-source="[**View**](rxtextdata.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Generates a Hive Data Source object.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
            &lt;center&gt;</ph><ph id="ph2">&lt;small&gt;</ph><bpt id="p1">&lt;a href="rxsparkdata.md" data-raw-source="[**View**](rxsparkdata.md)"&gt;</bpt><bpt id="p2">&lt;strong&gt;</bpt>View<ept id="p2">&lt;/strong&gt;</ept><ept id="p1">&lt;/a&gt;</ept><ph id="ph3">&lt;center&gt;</ph><ph id="ph4">&lt;/small&gt;</ph></source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Generates a Parquet Data Source object.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
            &lt;center&gt;</ph><ph id="ph2">&lt;small&gt;</ph><bpt id="p1">&lt;a href="rxsparkdata.md" data-raw-source="[**View**](rxsparkdata.md)"&gt;</bpt><bpt id="p2">&lt;strong&gt;</bpt>View<ept id="p2">&lt;/strong&gt;</ept><ept id="p1">&lt;/a&gt;</ept><ph id="ph3">&lt;center&gt;</ph><ph id="ph4">&lt;/small&gt;</ph></source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Lists cached <ph id="ph1">&lt;code&gt;RxParquetData&lt;/code&gt;</ph> or <ph id="ph2">&lt;code&gt;RxHiveData&lt;/code&gt;</ph> data source objects.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
            &lt;center&gt;</ph><ph id="ph2">&lt;small&gt;</ph><bpt id="p1">&lt;a href="rxsparkdataops.md" data-raw-source="[**View**](rxsparkdataops.md)"&gt;</bpt><bpt id="p2">&lt;strong&gt;</bpt>View<ept id="p2">&lt;/strong&gt;</ept><ept id="p1">&lt;/a&gt;</ept><ph id="ph3">&lt;center&gt;</ph><ph id="ph4">&lt;/small&gt;</ph></source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Removes cached <ph id="ph1">&lt;code&gt;RxParquetData&lt;/code&gt;</ph> or <ph id="ph2">&lt;code&gt;RxHiveData&lt;/code&gt;</ph> data source objects.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
            &lt;center&gt;</ph><ph id="ph2">&lt;small&gt;</ph><bpt id="p1">&lt;a href="rxsparkdataops.md" data-raw-source="[**View**](rxsparkdataops.md)"&gt;</bpt><bpt id="p2">&lt;strong&gt;</bpt>View<ept id="p2">&lt;/strong&gt;</ept><ept id="p1">&lt;/a&gt;</ept><ph id="ph3">&lt;center&gt;</ph><ph id="ph4">&lt;/small&gt;</ph></source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
##</ph> High Performance Computing and Distributed Computing Functions</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>The Hadoop compute context has a number of helpful functions used for high performance computing and distributed computing.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Learn more about the entire set of functions in the <bpt id="p1">[</bpt>Distributed Computing guide<ept id="p1">](../../r/how-to-revoscaler-distributed-computing.md)</ept>.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Function Name</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt>Help<ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Run an arbitrary R function on nodes or cores of a cluster.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxexec.md" data-raw-source="[**View**](rxexec.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Get the status of a non-waiting distributed computing job.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxgetjobresults.md" data-raw-source="[**View**](rxgetjobresults.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Get the return object(s) of a non-waiting distributed computing job.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxgetjobresults.md" data-raw-source="[**View**](rxgetjobresults.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Get the console output from a non-waiting distributed computing job.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxgetjoboutput.md" data-raw-source="[**View**](rxgetjoboutput.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Get the available distributed computing job information objects.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
                &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxgetjobs.md" data-raw-source="[**View**](rxgetjobs.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source><ph id="ph1">
##</ph> Hadoop Convenience Functions</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>RevoScaleR also provides some wrapper functions for accessing Hadoop/HDFS functionality via R. These functions require access to Hadoop, either locally or remotely via the RxHadoopMR or RxSpark compute contexts.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Function Name</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt>Help<ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Execute an arbitrary Hadoop command.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Allows you to run basic Hadoop commands.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxhadoopcommand.md" data-raw-source="[**View**](rxhadoopcommand.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Return the current Hadoop version.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxhadoopcommand.md" data-raw-source="[**View**](rxhadoopcommand.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Copy a file from a remote client to the Hadoop cluster&amp;#39;s local file system, and then to HDFS.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxhadoopcommand.md" data-raw-source="[**View**](rxhadoopcommand.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Copy a file from the native file system to HDFS.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Wraps the Hadoop <ph id="ph1">&lt;code&gt;fs -copyFromLocal&lt;/code&gt;</ph> command.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
            &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxhadoopcommand.md" data-raw-source="[**View**](rxhadoopcommand.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Copy a file in the Hadoop Distributed File System (HDFS).</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Wraps the Hadoop <ph id="ph1">&lt;code&gt;fs -cp&lt;/code&gt;</ph> command.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
                &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxhadoopcommand.md" data-raw-source="[**View**](rxhadoopcommand.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Remove a file in HDFS.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Wraps the Hadoop <ph id="ph1">&lt;code&gt;fs -rm&lt;/code&gt;</ph> command.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
                &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxhadoopcommand.md" data-raw-source="[**View**](rxhadoopcommand.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>List files in an HDFS directory.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Wraps the Hadoop <ph id="ph1">&lt;code&gt;fs -ls&lt;/code&gt;</ph> or <ph id="ph2">&lt;code&gt;fs -lsr&lt;/code&gt;</ph> command.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
                &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxhadoopcommand.md" data-raw-source="[**View**](rxhadoopcommand.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Make a directory in HDFS.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Wraps the Hadoop <ph id="ph1">&lt;code&gt;fs -mkdir&lt;/code&gt;</ph> command.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
                &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxhadoopcommand.md" data-raw-source="[**View**](rxhadoopcommand.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Move a file in HDFS.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Wraps the Hadoop <ph id="ph1">&lt;code&gt;fs -mv&lt;/code&gt;</ph> command.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
                &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxhadoopcommand.md" data-raw-source="[**View**](rxhadoopcommand.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>Remove a directory in HDFS.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Wraps the Hadoop <ph id="ph1">&lt;code&gt;fs -rmr&lt;/code&gt;</ph> command.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source><bpt id="p1">
                &lt;center&gt;</bpt><bpt id="p2">&lt;small&gt;</bpt><bpt id="p3">&lt;a href="rxhadoopcommand.md" data-raw-source="[**View**](rxhadoopcommand.md)"&gt;</bpt><bpt id="p4">&lt;strong&gt;</bpt>View<ept id="p4">&lt;/strong&gt;</ept><ept id="p3">&lt;/a&gt;</ept><ept id="p2">&lt;/small&gt;</ept><ept id="p1">&lt;/center&gt;</ept><ph id="ph1">
        </ph></source>
        </trans-unit></group></body></file></xliff>