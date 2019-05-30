<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxkmeans.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3ea1796e98776fc6561998d82aa6d4bcc4f3a19465.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a1796e98776fc6561998d82aa6d4bcc4f3a19465</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxkmeans.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxKmeans function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Perform k-means clustering on small or large data.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxKmeans, print.rxKmeans, cluster, multivariate, clustering</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxKmeans: K-Means Clustering</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Perform k-means clustering on small or large data.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>formula as described in <bpt id="p1">[</bpt>rxFormula<ept id="p1">](rxFormula.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>a data source object, a character string specifying a .xdf file, or a data frame object.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>either an RxXdfData data source object or a character string specifying the .xdf file for storing the resulting cluster indexes.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, then no cluster indexes are stored to disk.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Note that in the case that the input data is a data frame, the cluster indexes are returned automatically.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Note also that, if <ph id="ph1">`rowSelection`</ph> is specified and not <ph id="ph2">`NULL`</ph>, then <ph id="ph3">`outFile`</ph> cannot be the same as the <ph id="ph4">`data`</ph> since the resulting set of cluster indexes will generally not have the same number of rows as the original data source.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>character string to be used as a column name for the resulting  cluster indexes if <ph id="ph1">`outFile`</ph> is not <ph id="ph2">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Note that make.names is used on <ph id="ph1">`outColName`</ph> to ensure that the column name is valid.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`outFile`</ph> is an <ph id="ph2">`RxOdbcData`</ph> source, dots are first converted to underscores.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Thus, the default <ph id="ph1">`outColName`</ph> becomes <ph id="ph2">`"X_rxCluster"`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, and the output file is different from the input file, variables in the model will be written to the output file in addition to the cluster numbers.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If variables from the input data set are transformed in the model, the transformed variables will also be written out.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>or character vector of additional variables names from the input data to include in the <ph id="ph1">`outFile`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`writeModelVars`</ph> is <ph id="ph2">`TRUE`</ph>, model variables will be included as well.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outFile`</ph> with an existing column named <ph id="ph3">`outColName`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>number of clusters <ph id="ph1">`k`</ph> to create.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, then the <ph id="ph2">`centers`</ph>argument must be specified.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>a <ph id="ph1">`k x p`</ph> numeric matrix containing a set of initial (distinct) cluster centers.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, then the <ph id="ph2">`numClusters`</ph> argument must be specified.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>character string defining algorithm to use in defining the clusters.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Currently supported algorithms are <ph id="ph1">`"Lloyd"`</ph>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>This argument is case insensitive.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>integer specifying the size of the sample used to choose initial centers.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If 0, (the default), the size is chosen as the minimum of the number of observations or 10 times the number of clusters.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>maximum number of iterations allowed.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>if <ph id="ph1">`centers`</ph> is <ph id="ph2">`NULL`</ph>, <ph id="ph3">`k`</ph> rows are randomly selected from the data source  for use as initial starting points.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`numStarts`</ph> argument defines the number of these random sets that are  to be chosen and evaluated, and the best result is returned.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`numStarts`</ph> is 0, the first <ph id="ph2">`k`</ph> rows in the data set are used.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Random selection of rows is only supported for .xdf data sources using the native file system and data frames.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>If the .xdf file is compressed, the random sample is taken from a maximum of the first 5000 rows of data.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>name of a logical variable in the data set (in quotes) or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>will use only observations in which the value of the <ph id="ph1">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph2">`log`</ph> of the <ph id="ph3">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations  (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function  call using the expression function.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>an expression of the form <ph id="ph1">`list(name = expression, ...)`</ph> representing the first round of variable transformations.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>)  can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>a named list containing objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>variable transformation function.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>character vector defining additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and  preloaded for use in variable transformation functions, e.g., those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments or those  defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>user-defined environment to serve as a parent to  all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent  <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, additional summary information is printed.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>a valid <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`RxSpark`</ph> and <ph id="ph2">`RxHadoopMR`</ph> compute  contexts distribute the computation among the nodes specified by the  compute context; for other compute contexts, the  computation is distributed if possible on the local computer.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>integer in the range of -1 to 9 indicating the compression  level for the output data if written to an <ph id="ph1">`.xdf`</ph> file.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the  amount of compression - resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>If  <ph id="ph1">`xdfCompressionLevel`</ph> is set to 0, there will be no compression and files will be compatible  with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression  will be used.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Revolution Compute Engine.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>object of class rxKmeans.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, header information is printed.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Performs scalable k-means clustering using the classical Lloyd algorithm.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>For reproducibility when using random starting values, you can pass a random seed by specifying <ph id="ph1">`seed=`</ph><bpt id="p1">*</bpt>value<ept id="p1">*</ept> as part of your call.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>See the Examples.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>An object of class "rxKmeans" which is a list with components:</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>A vector of integers indicating the cluster to which each point is allocated.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>This information is always returned if the data source is a data frame.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>If the data source is not a data frame and <ph id="ph1">`outFile`</ph> is specified.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>i.e., not <ph id="ph1">`NULL`</ph>, the cluster indexes are written/appended to the specified file with a column name as defined by <ph id="ph2">`outColName`</ph>.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>matrix of cluster centers.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>within-cluster sum of squares (relative to the center) for each cluster.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>total within-cluster sum of squares.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>sum of the <ph id="ph1">`withinss`</ph> vector.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>between-cluster sum of squares.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>number of points in each cluster.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>number of valid observations.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>number of missing observations.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>number iterations performed.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>parameters sent to Microsoft R Services Compute Engine.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>formula as described in <bpt id="p1">[</bpt>rxFormula<ept id="p1">](rxFormula.md)</ept>.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>the matched call.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Lloyd, S. P.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>(1957, 1982) Least squares quantization in PCM.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Technical Note, Bell Laboratories.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Published in 1982 in <bpt id="p1">*</bpt>IEEE Transactions on Information Theory<ept id="p1">*</ept> 28, 128-137.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>kmeans.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>