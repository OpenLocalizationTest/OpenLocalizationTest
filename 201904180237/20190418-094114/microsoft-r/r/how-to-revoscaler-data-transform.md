<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-data-transform.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea9263516149b5176ce6542b153eadd2f828c706267a9.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">3516149b5176ce6542b153eadd2f828c706267a9</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-data-transform.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to transform and subset data in RevoScaleR (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to manipulate and transform data in RevoScaleR.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to transform and subset data using RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>A crucial step in many analyses is transforming the data into a form best suited for the chosen analysis.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>For example, to reduce variations in scale between variables, you might take a log or a power of the original variable before fitting the dataset to a linear model.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Additionally, transforming data minimizes passes through the data, which is more efficient.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>In RevoScaleR, you can perform data transformations in virtually all of its functions, from <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> to <bpt id="p2">**</bpt>rxDataStep<ept id="p2">**</ept>, as well as the analysis functions <bpt id="p3">**</bpt>rxSummary<ept id="p3">**</ept>, <bpt id="p4">**</bpt>rxLinMod<ept id="p4">**</ept>, <bpt id="p5">**</bpt>rxLogit<ept id="p5">**</ept>, <bpt id="p6">**</bpt>rxGlm<ept id="p6">**</ept>, <bpt id="p7">**</bpt>rxCrossTabs<ept id="p7">**</ept>, <bpt id="p8">**</bpt>rxCube<ept id="p8">**</ept>, <bpt id="p9">**</bpt>rxCovCor<ept id="p9">**</ept>, and <bpt id="p10">**</bpt>rxKmeans<ept id="p10">**</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>In all cases, the basic approach for data transforms is the same.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The heart of the RevoScaleR data step is a list of <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept>, each of which specifies an R expression to be evaluated.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The data step typically is an assignment that either creates a new variable or modifies an existing variable from the original data set.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>This article uses examples to illustrate common data manipulation tasks.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>For more background, see <bpt id="p1">[</bpt>Data Transformations<ept id="p1">](concept-what-is-data-transformations.md)</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Subset data by row or variable</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A common use of <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> is to create a new data set with a subset of rows and variables.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The following simple example uses a data frame as the input data set.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The call to <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> uses the <bpt id="p2">*</bpt>rowSelection<ept id="p2">*</ept> argument to select only the rows where the variable <bpt id="p3">*</bpt>y<ept id="p3">*</ept> is greater than .5, and the <bpt id="p4">*</bpt>varsToKeep<ept id="p4">*</ept> argument to keeps only the variables <bpt id="p5">*</bpt>y<ept id="p5">*</ept> and <bpt id="p6">*</bpt>z<ept id="p6">*</ept>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rowSelection<ept id="p1">*</ept> argument is an R expression that evaluates to <bpt id="p2">*</bpt>TRUE<ept id="p2">*</ept> if the observation should be kept.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>varsToKeep<ept id="p1">*</ept> argument contains a list of variable names to read in from the original data set.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Because no <bpt id="p1">*</bpt>outFile<ept id="p1">*</ept> is specified, a data frame is returned.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>You should see the following results:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Subsetting is particularly useful if your original data set contains millions of rows or hundreds of thousands of variables.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>As a smaller example, the CensusWorkers.xdf sample data file has six variables and 351,121 rows.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>To create a subset containing only workers who have worked less than 30 weeks in the year and five variables, we can again use <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> with the <bpt id="p2">*</bpt>rowSelection<ept id="p2">*</ept> and <bpt id="p3">*</bpt>varsToKeep<ept id="p3">*</ept> arguments.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Since the resulting data set will clearly fit in memory, we omit the <bpt id="p1">*</bpt>outFile<ept id="p1">*</ept> argument and assign the result of the data step, then use <bpt id="p2">**</bpt>rxGetInfo<ept id="p2">**</ept> to see our results as usual:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The result is a data set with 14,317 rows:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Alternatively, and in this case more easily, you can use <bpt id="p1">*</bpt>varsToDrop<ept id="p1">*</ept> to prevent variables from being read in from the original data set.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>This time we’ll specify an <bpt id="p1">*</bpt>outFile<ept id="p1">*</ept>; use the <bpt id="p2">*</bpt>overwrite<ept id="p2">*</ept> argument to allow the output file to be replaced.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>As noted above, if you omit the <bpt id="p1">*</bpt>outFile<ept id="p1">*</ept> argument to <bpt id="p2">**</bpt>rxDataStep<ept id="p2">**</ept>, then the results will be returned in a data frame in memory.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>This is true whether or not the input data is a data frame or an .xdf file (assuming the resulting data is small enough to reside in memory).</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If an <bpt id="p1">*</bpt>outFile<ept id="p1">*</ept> is specified, a data source object representing the new .xdf file is returned, which can be used in subsequent RevoScaleR function calls.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Subset and transform in one operation</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Still working with the CensusWorkers dataset, this exercise shows how to combine subsetting and transformations in one data step operation.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Suppose we want to extract the same five variables as before from the CensusWorkers data set, but also add a factor variable based on the integer variable <bpt id="p1">*</bpt>age<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>For example, to create our factor variable, we can use the following <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept> argument:</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>In doing a data step operation, RevoScaleR reads in a chunk of data read from the original data set, including only the variables indicated in <bpt id="p1">*</bpt>varsToKeep<ept id="p1">*</ept>, or omitting variables specified in <bpt id="p2">*</bpt>varsToDrop<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>It then passes the variables needed for data transformations back to R for manipulation:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rxGetInfo<ept id="p1">**</ept> function reveals the added variable:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>We can combine the <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept> argument with the <bpt id="p2">*</bpt>transformObjects<ept id="p2">*</ept> argument to create new variables from objects in your global environment (or other environments in your current search path).</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>For example, suppose you would like to estimate a linear model using wage income as the dependent variable, and want to include state-level of per capita expenditure on education as one of the independent variables.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>We can define a named vector to contain this state-level data as follows:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>We can then use <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> to add the per capita education expenditure as a new variable using the <bpt id="p2">*</bpt>transforms<ept id="p2">*</ept> argument, passing <bpt id="p3">*</bpt>educExp<ept id="p3">*</ept> to the <bpt id="p4">*</bpt>transformObjects<ept id="p4">*</ept> argument as a named list:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rxGetInfo<ept id="p1">**</ept> function reveals the added variable:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Create a variable</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Suppose we want to extract five variables from the <bpt id="p1">*</bpt>CensusWorkers<ept id="p1">*</ept> data set, but also add a factor variable based on the integer variable age.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>This example shows how to use a transform function to create new variables.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>For example, to create our factor variable, we can create the following function:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>To test the function, read an arbitrary chunk out of the data set.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>For efficiency reasons, the data passed to the transformation function is stored as a list rather than a data frame, so when reading from the .xdf file we set the <bpt id="p1">*</bpt>returnDataFrame<ept id="p1">*</ept> argument to FALSE to emulate this behavior.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Since we only use the variable <bpt id="p1">*</bpt>age<ept id="p1">*</ept> in our transformation function, we restrict the variables extracted to that.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The resulting list of data (displayed as a data frame) shows us that our transformations are working as expected:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>In doing a data step operation, RevoScaleR reads in a chunk of data read from the original data set, including only the variables indicated in <bpt id="p1">*</bpt>varsToKeep<ept id="p1">*</ept>, or omitting variables specified in <bpt id="p2">*</bpt>varsToDrop<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>It then passes the variables needed for data transformations back to R for manipulation.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>We specify the variables needed to process the transformation in the <bpt id="p1">*</bpt>transformVars<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Including extra variables does not alter the analysis, but it does reduce the efficiency of the data step.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>In this case, since <bpt id="p1">*</bpt>ageFactor<ept id="p1">*</ept> depends only on the <bpt id="p2">*</bpt>age<ept id="p2">*</ept> variable for its creation, the <bpt id="p3">*</bpt>transformVars<ept id="p3">*</ept> argument needs to specify just that:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rxGetInfo<ept id="p1">**</ept> function reveals the added and dropped variables:</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Modify variable metadata</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>To change variable information (rather than the data values themselves), use the function <bpt id="p1">**</bpt>rxSetVarInfo<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>For example, using the CensusData, we can change the names of two variables and add descriptions:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Add data to an analysis</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>It is sometimes useful to access additional information from within a transform function.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>For example, you might want to match additional data in the process of creating new variables.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Transform functions are evaluated in a “sterilized” environment which includes the parent environment of the function closure.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>To provide access to additional data within the function, you can use the <bpt id="p1">*</bpt>transformObjects<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>For example, suppose you would like to estimate a linear model using wage income as the dependent variable, and want to include state-level of per capita expenditure on education as one of the independent variables.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>We can define a named vector to contain this state-level data as follows:</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>We can then define a transform function that uses this information as follows:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>We can then use the transform function and our named vector in a call to <bpt id="p1">**</bpt>rxLinMod<ept id="p1">**</ept> as follows:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>When the transform function is evaluated, it will have access to the <bpt id="p1">*</bpt>educExp<ept id="p1">*</ept> object.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The final results show:</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Create a row selection variable</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>One common use of the <bpt id="p1">*</bpt>transformFunc<ept id="p1">*</ept> argument is to create a logical variable to use as a row selection variable.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>For example, suppose you want to create a random sample from a massive data set.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>You can use the <bpt id="p1">*</bpt>transformFunc<ept id="p1">*</ept> argument to specify a transformation that creates a random binomial variable, which can then be coerced to logical and used for row selection.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>The object name <bpt id="p1">*</bpt>.rxRowSelection<ept id="p1">*</ept> is reserved for the row selection variable; if RevoScaleR finds this object, it is used for row selection.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>If you both specify a <bpt id="p1">*</bpt>rowSelection<ept id="p1">*</ept> argument and define a <bpt id="p2">*</bpt>.rxRowSelection<ept id="p2">*</ept> variable in your transform function, the one specified in your transform function will be overwritten by the contents of the <bpt id="p3">*</bpt>rowSelection<ept id="p3">*</ept> argument, so that expression takes precedence.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The following code creates a random selection variable to create a data frame with a random 10% subset of the census workers file:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The resulting data frame, <bpt id="p1">*</bpt>df<ept id="p1">*</ept>, has approximately 35,000 rows.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>You can look at the first few rows using <bpt id="p1">*</bpt>head<ept id="p1">*</ept> as follows:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Equivalently, we could create the temporary row selection variable using the <bpt id="p1">*</bpt>rowSelection<ept id="p1">*</ept> argument with the internal <bpt id="p2">*</bpt>.rxNumRows<ept id="p2">*</ept> variable, which provides the number of rows in the current chunk of data being processed:</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Convert a data frame to XDF</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>You can use all of the functionality provided by the <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> function to create an .xdf file from a data frame for further use.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>For example, create a simple data frame:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Now create an .xdf file, using a row selection and creating a new variable.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rowsPerRead<ept id="p1">*</ept> argument will specify how many rows of the original data frame to process at a time before writing out a block of the new .xdf file.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Convert XDF to Text</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>If you need to share data with others not using .xdf data files, you can export your .xdf files to text format using the <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> function.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>For example, we can write the claims.xdf file we created earlier to text format as follows:</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>By default, the text file created is comma-delimited, but you can change this by specifying a different delimiter with the <bpt id="p1">*</bpt>delimiter<ept id="p1">*</ept> argument to the RxTextData function:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>If you have a large number of variables, you can choose to write out only a subsample by using the <bpt id="p1">*</bpt>VarsToKeep<ept id="p1">*</ept> or <bpt id="p2">*</bpt>VarsToDrop<ept id="p2">*</ept> argument.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Here we write out the claims data, omitting the <bpt id="p1">*</bpt>number<ept id="p1">*</ept> variable:</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Convert strings to factors</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Factors are variables that represent categories.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>An example is “sex”, which has the categories “Male” and “Female”.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>There are two parts to a factor variable:</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>A vector of integer indexes with values in the range of 1:K, where K is the number of categories.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>For example, “sex” has two categories with indexes 1 and 2.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>The length of the vector corresponds to the number of observations.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>A vector of K character strings that are used when the factor is displayed.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>In R, these are normally printed without quote marks, to indicate that the variable is a factor instead of a character string.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>If you have character data in an .xdf file or data frame, you can use the <bpt id="p1">**</bpt>rxFactors<ept id="p1">**</ept> function to convert it to a factor.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Let’s create a simple data frame with character data.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Note that by default, <bpt id="p1">*</bpt>data.frame<ept id="p1">*</ept> converts character data to factor data.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>That is, the <bpt id="p1">*</bpt>stringsAsFactors<ept id="p1">*</ept> argument defaults to <bpt id="p2">*</bpt>TRUE<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>In RevoScaleR’s <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> function, <bpt id="p2">*</bpt>stringsAsFactors<ept id="p2">*</ept> has a default of <bpt id="p3">*</bpt>FALSE<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Now we can use <bpt id="p1">**</bpt>rxFactors<ept id="p1">**</ept> to convert the character data to factors.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>We can just specify a vector of variable names to convert as the <bpt id="p1">*</bpt>factorInfo<ept id="p1">*</ept>:</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Note that by default, the factor levels are in the order in which they are encountered.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>If you would like to have them sorted alphabetically, specify <bpt id="p1">*</bpt>sortLevels<ept id="p1">*</ept> to be <bpt id="p2">*</bpt>TRUE<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>If you have variables that are already factors, you may want change the order of the levels, the names of the levels, or how they are grouped.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Typically recoding a factor means changing from one set of indexes to another.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>For example, if the levels of “sex” are currently arranged in the order “M”, “F” and you want to change that to “F”, “M”, you need to change the index for every observation.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>You can use the <bpt id="p1">**</bpt>rxFactors<ept id="p1">**</ept> function to recode factors in RevoScaleR.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>For example, suppose we have some test scores for a set of male and female subjects.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>We can generate such data randomly as follows:</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>If we look at just the sex variable, we see the levels M or F for each observation:</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>To recode this factor so that “Female” is the first level and “Male” the second, we can use <bpt id="p1">**</bpt>rxFactors<ept id="p1">**</ept> as follows:</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Looking at the new Gender variable, we see how the levels have changed:</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>As mentioned earlier, by default, RevoScaleR codes factor levels in the order in which they are encountered in the input file(s).</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>This could lead you to have a State variable ordered as “Maine”, “Vermont”, “New Hampshire”, “Massachusetts”, “Connecticut”, and so forth.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Usually, you would prefer to have the levels of such a variable sorted in alphabetical order.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>You can do this with <bpt id="p1">**</bpt>rxFactors<ept id="p1">**</ept> using the sortLevels flag.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>It is most useful to specify this flag as part of the <bpt id="p1">*</bpt>factorInfo<ept id="p1">*</ept> list for each variable, although if you have a large number of factors and want most of them to be sorted, you can also set the flag to TRUE globally and then specify <bpt id="p2">*</bpt>sortLevels=FALSE<ept id="p2">*</ept> for those variables you want to order in a different way.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>When using the <bpt id="p1">*</bpt>sortLevels<ept id="p1">*</ept> flag, it is useful to keep in mind that it is the <bpt id="p2">*</bpt>levels<ept id="p2">*</ept> that are being sorted, not the data itself, and that the levels are always character data.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>If you are using the individual values of a continuous variable as factor levels, you may be surprised by the sorted order of the levels: for example, the levels 1, 3, 20 are sorted as “1”, “20”, “3”.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Another common use of factor recoding is in analyzing survey data gathered using Likert items with five or seven level responses.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>For example, suppose a customer satisfaction survey offered the following seven-level responses to each of four questions:</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Completely satisfied</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Mostly satisfied</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Somewhat satisfied</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Neither satisfied nor dissatisfied</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Somewhat dissatisfied</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Mostly dissatisfied</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Completely dissatisfied</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>In analyzing this data, the survey analyst may recode the factors to focus on those who were largely satisfied (combining levels 1 and 2), largely dissatisfied (combining levels 6 and 7) and somewhere in-between (combining levels 3, 4, and 5).</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>The CustomerSurvey.xdf file in the SampleData directory contains 25 responses to each of the four survey questions.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>We can read it into a data frame as follows:</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>To recode each question as desired, we can use <bpt id="p1">**</bpt>rxFactors<ept id="p1">**</ept> as follows:</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Looking at just Q1, we see the recoded factor:</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Recode factors for compatibility</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>One important use of factor recoding in RevoScaleR is to ensure that the factor variables in two files are compatible, that is, have the same levels with the same coding.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>This use comes up in a variety of contexts, including prediction, merging, and distributed computing.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>For example, suppose you are creating a logistic regression model of whether a given airline flight will be late, and are using the first fifteen years of the airline data as a training set.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>You then want to test the model on the remaining years of the airline data.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>You need to ensure that the two files, the training set and the test set, have compatible factor variables.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>You can generally do this easily using <bpt id="p1">**</bpt>rxGetInfo<ept id="p1">**</ept> (with getVarInfo=TRUE) together with <bpt id="p2">**</bpt>rxFactors<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Use <bpt id="p1">**</bpt>rxGetInfo<ept id="p1">**</ept> to find all the levels in all the files, then use <bpt id="p2">**</bpt>rxFactors<ept id="p2">**</ept> to recode each file so that every factor variable contains all the levels found in any of the files.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rxMerge<ept id="p1">**</ept> function automatically checks for factor variable compatibility and recodes on the fly if necessary.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Impute values</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>A common use case is replace missing values with the variable mean.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>This example uses generated data in a simple data frame.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>A call to <bpt id="p1">**</bpt>rxGetInfo<ept id="p1">**</ept> returns precomputed metadata showing missing values "NA" in both variables:</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>Now use <bpt id="p1">**</bpt>rxSummary<ept id="p1">**</ept> to compute summary statistics that includes a variable mean, putting both computed means into a named vector:</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>The computed statistics are:</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Finally, pass the computed means into a <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> using the <bpt id="p2">*</bpt>transformObjects<ept id="p2">*</ept> argument:</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>The resulting data set information substitutes NA with computed means generated in the previous step:</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Use internal variables in a transformation</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>This example shows how to compute moving averages using internal variables in a transformation function.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Four additional variables providing information on the RevoScaleR processing are available for use in your transform functions:</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>.rxStartRow: The row number from the original data that was read as the first row of the current chunk.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>.rxChunkNum: The current chunk being processed.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>.rxReadFileName: The name of the .xdf file currently being read.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>.rxIsTestChunk: Whether the chunk being processed is being processed as a test sample of data.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>These are particularly useful if you need to access additional rows of data when processing a chunk.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>This is the case, for example, when you want to include lagged data in a calculation.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>The following example is a transformation function “generator” to compute a simple moving average.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>By creating this “function within a function” we are able to easily pass arguments into a transformation function.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>This one takes as arguments the number of days (or time units) for the moving average, the name of the variable that will be used to compute the moving average, and the name of the new variable to create.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>The transformation function computes the number of lagged observations to read in, then reads in that data to create a long data vector with the lags.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>The simple moving average calculations are performed and put into a new variable.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>The additional lagged rows are removed from the original data vector before returning from the function.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>We could use this function with <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> to add a variable to our data set, or on-the-fly, for example for plotting.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>Here we will use the sample data set containing daily information on the Dow Jones Industrial Average.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>We compute a 360-day moving average for the adjusted close (adjusted for dividends and stock splits) and plot it:</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Extended example showing a series of transformations</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept> argument can be a powerful way to effect a sequence of changes on a row by row basis.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept> argument is specified as a list of expressions.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>Given R expressions operate row-by-row (that is, the computed value of the new variable for an observation is only dependent on values of other variables for that observation), you can combine them into a single <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept> argument, as this example demonstrates.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Start with a simple data frame containing a small sample of transaction data:</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>Apply a series of data transformations:</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>Compute the total expenditures for each store visit</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>Compute the average category expenditure for each store visit</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>Set the variable <bpt id="p1">*</bpt>Age<ept id="p1">*</ept> to missing if the value is 99</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>Create a new logical variable <bpt id="p1">*</bpt>UnderAge<ept id="p1">*</ept> if the purchaser is under 21</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>Find the day of week the purchase was made using R’s <bpt id="p1">*</bpt>as.POSIXlt<ept id="p1">*</ept> function, then convert it to a factor.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>[Note that when creating factors in a transform, you must specify the levels or you may get unpredictable results.</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>Alternatively use <bpt id="p1">**</bpt>rxFactors<ept id="p1">**</ept>.]</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>Create a factor variable for categories of expenditure levels</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>Create a logical variable for expenditures of $50 or more on either Food or Wine</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>Remove the variable BuyDate from the data set</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>The following call to <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> will accomplish all of the above, returning a new data frame with the transformed variables:</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>The new data frame shows all of the transformed data:</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>If we had a large data set containing expenditure data in an .xdf file, we could use exactly the same transformation code; the only changes in the call to <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> would be the <bpt id="p2">*</bpt>inData<ept id="p2">*</ept> and the addition of an <bpt id="p3">*</bpt>outFile<ept id="p3">*</ept> for the newly created data set.</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>Next Steps</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>Continue on to the following data-related articles to learn more about XDF, data source objects, and other data formats:</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Data transformations (introduction)<ept id="p1">](concept-what-is-data-transformations.md)</ept></source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>XDF files<ept id="p1">](concept-what-is-xdf.md)</ept></source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Data Sources<ept id="p1">](how-to-revoscaler-data-source.md)</ept></source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Import text data<ept id="p1">](how-to-revoscaler-data-import.md)</ept></source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Import ODBC data<ept id="p1">](how-to-revoscaler-data-odbc.md)</ept></source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Import and consume data on HDFS<ept id="p1">](how-to-revoscaler-data-hdfs.md)</ept></source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR Functions<ept id="p1">](~/r-reference/revoscaler/revoscaler.md)</ept><ph id="ph1"> </ph></source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Tutorial: data import and exploration<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept> <bpt id="p2">[</bpt>Tutorial: data visualization and analysis<ept id="p2">](tutorial-revoscaler-data-model-analysis.md)</ept></source>
        </trans-unit></group></body></file></xliff>