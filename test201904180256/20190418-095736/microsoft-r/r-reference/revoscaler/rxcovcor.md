<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxcovcor.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c3088ca82427fe592afd70d19eacb581d6eb053ad.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">3088ca82427fe592afd70d19eacb581d6eb053ad</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxcovcor.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxCovCor function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Calculate the covariance, correlation, or sum of squares / cross-product matrix for a set of variables.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxCovCor, rxCov, rxCor, rxSSCP, print.rxCovCor, univar, multivariate</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxCovCor: Covariance/Correlation Matrix</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Calculate the covariance, correlation, or sum of squares / cross-product matrix for a set of variables.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>formula, as described in <bpt id="p1">[</bpt>rxFormula<ept id="p1">](rxFormula.md)</ept>, with all the terms on the right-hand side of the <ph id="ph1">`~`</ph> separated by <ph id="ph2">`+`</ph> operators.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Each term may be a single variable, a transformed variable, or the interaction of (transformed) variables separated by the <ph id="ph1">`:`</ph> operator.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>e.g. <ph id="ph1">`~ x1 + log(x2) + x3 : x4`</ph></source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>either a data source object, a character string specifying a .xdf file, or a data frame object.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Only one of <ph id="ph1">`pweights`</ph> and <ph id="ph2">`fweights`</ph> may be specified at a time.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as frequency weights for the observations.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Only one of <ph id="ph1">`pweights`</ph> and <ph id="ph2">`fweights`</ph> may be specified at a time.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>name of a logical variable in the data set (in quotes) or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rowSelection = (age &gt; 20) &amp; (age &lt; 65) &amp; (log(income) &gt; 10)`</ph> will use only observations in which the value of the <ph id="ph2">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph3">`log`</ph> of the <ph id="ph4">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations  (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function  call using the expression function.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>an expression of the form <ph id="ph1">`list(name = expression, ...)`</ph> representing the first round of variable transformations.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>) can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>a named list containing objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>variable transformation function.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>character vector defining additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and  preloaded for use in variable transformation functions, e.g., those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments or those  defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>user-defined environment to serve as a parent to  all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, all of the columns are kept in the returned matrix.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, columns (and corresponding rows in the returned matrix) that are symbolic linear combinations of other columns, see alias, are dropped.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>numeric tolerance used to identify columns in the data matrix that have near zero variance.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If the variance of a column is less than or equal to <ph id="ph1">`varTol`</ph> and <ph id="ph2">`keepAll=TRUE`</ph>, that column is dropped from the data matrix.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>character string specifying the type of matrix to return.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The supported types are:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"SSCP"`</ph>: <bpt id="p1">**</bpt>S<ept id="p1">**</ept>ums of <bpt id="p2">**</bpt>S<ept id="p2">**</ept>quares / <bpt id="p3">**</bpt>C<ept id="p3">**</ept>ross <bpt id="p4">**</bpt>P<ept id="p4">**</ept>roducts matrix.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Cov"`</ph>: covariance matrix.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Cor"`</ph>: correlation matrix.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`type`</ph> argument is case insensitive, e.g. <ph id="ph2">`"SSCP"`</ph> and <ph id="ph3">`"sscp"`</ph> are equivalent.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, additional summary information is printed.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>a valid <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`RxSpark`</ph> and <ph id="ph2">`RxHadoopMR`</ph> compute contexts distribute the computation among the nodes specified by the compute context; for other compute contexts, the computation is distributed if possible on the local computer.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Revolution Compute Engine.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>an object of class "rxCovCor".</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, header information is printed.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxCovCor`</ph>, and the appropriate convenience functions <ph id="ph2">`rxCov`</ph>, <ph id="ph3">`rxCor`</ph> and <ph id="ph4">`rxSSCP`</ph>, calculates either the covariance, Pearson's correlation, or a sums of squares/cross-product matrix, which may or may not use probability or frequency weights.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The sums of squares/cross-product matrix differs from the other two output types in that an initial column of <ph id="ph1">`1`</ph>s or square root of the weights, if specified, is added to the data matrix prior to multiplication so the first row and first column must be dropped from the output to obtain the cross-product of just the specified data matrix.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxCovCor`</ph>, an object of class "rxCovCor" with the following list elements:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>numeric matrix representing either the (weighted) covariance, correlation, or sum of squares/cross-product.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>For type = "Cor" and "Cov", numeric vector of (weighted)  standard deviations of the columns.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>For type = "SSCP", the standard deviations are not calculated and the return value is <ph id="ph1">`numeric(0)`</ph>.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>numeric vector containing the (weighted) column means.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>number of valid observations.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>number of missing observations.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>either the sum of the weights or <ph id="ph1">`NA`</ph> if no weights are specified.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>character vector containing the names of the data columns that were dropped during the calculations.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>integer vector containing the indices of the data columns that were dropped during the calculations.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>parameters sent to Microsoft R Services Compute Engine.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>the matched call.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>formula as described in <bpt id="p1">[</bpt>rxFormula<ept id="p1">](rxFormula.md)</ept>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxCov`</ph>, a covariance matrix.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxCor`</ph>, a correlation matrix.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxSSCP`</ph>, a sum of squares/cross-product matrix.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>cov, cor, <bpt id="p1">[</bpt>rxCovData<ept id="p1">](rxCovRegression.md)</ept>, <bpt id="p2">[</bpt>rxCorData<ept id="p2">](rxCovRegression.md)</ept>.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>