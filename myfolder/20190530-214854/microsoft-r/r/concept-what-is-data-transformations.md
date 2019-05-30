<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="concept-what-is-data-transformations.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e132ab5fc022f6ed064d7cffe690d33ea8ac940f3.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">132ab5fc022f6ed064d7cffe690d33ea8ac940f3</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\concept-what-is-data-transformations.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Data transformations in RevoScaleR - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RevoScaleR transform functions.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Data transformations using RevoScaleR functions (Machine Learning Server)</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Loading an initial dataset is typically just the first step in a continuum of data manipulation tasks that persist until your project is completed.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Common examples of data manipulation include isolating a subset, slicing a dataset by variables or rows, and converting or merging variables into new forms, often resulting in new data structures along the way.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>There are two main approaches to data transformation using the RevoScaleR library:</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Define an external based R <bpt id="p1">*</bpt>function<ept id="p1">*</ept> and reference it.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Define an embedded transformation as an input to a <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept> argument on another RevoScaleR function.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Embedded transformations are supported in <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept>, <bpt id="p2">**</bpt>rxDataStep<ept id="p2">**</ept>, and in analysis functions like <bpt id="p3">**</bpt>rxLinMod<ept id="p3">**</ept> and <bpt id="p4">**</bpt>rxCube<ept id="p4">**</ept>, to name a few.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Embedded transformations are easier to work with, but external functions allow for a greater degree of complexity and reuse.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The following section provides an illustration of both techniques.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Compare approaches</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Embedded transformations provide instructions within a formula, through arguments on a function.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Using just arguments, you can manipulate data using <bpt id="p1">*</bpt>transformations<ept id="p1">*</ept>, or select a rowset with the <bpt id="p2">*</bpt>rowSelection<ept id="p2">*</ept> argument.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Externally defined functions provide data manipulation instructions in an outer <bpt id="p1">*</bpt>function<ept id="p1">*</ept>, which is then referenced by a RevoScaleR function.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>An external transformation function is one that takes as input a list of variables and returns a list of (possibly different) variables.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Due to the external definition, the object can assume a complex structure and be repurposed across multiple functions supporting transformation.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>For more examples of both approaches, see <bpt id="p1">[</bpt>How to transform and subset data<ept id="p1">](how-to-revoscaler-data-transform.md)</ept>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Arguments used in transformations</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>To specify an external function, use the <bpt id="p1">*</bpt>transformFunc<ept id="p1">*</ept> argument to most RevoScaleR functions.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>To pass a list of variables to the function, use the <bpt id="p1">*</bpt>transformVars<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The following table numerates the arguments used in data manipulation tasks.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Argument</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>transforms</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>A formula for manipulating or transforming data, passed as an argument to a RevoScaleR function like <bpt id="p1">**</bpt>rxImport<ept id="p1">**</ept> or <bpt id="p2">**</bpt>rxDataStep<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>This expression can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>rowSelection</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Criteria for selecting a subset of rows in the current data frame.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>function</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>A base R class used to create functions in R script.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>transformFunc</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Assigns a function to a RevoScaleR function supporting data manipulation and transformations.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If this argument is specified, it is evaluated before any other transformations specified in the <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept>, <bpt id="p2">*</bpt>rowSelection<ept id="p2">*</ept>, or <bpt id="p3">*</bpt>formula<ept id="p3">*</ept> arguments.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The list of variables to be passed to the transform function is specified as the <bpt id="p1">*</bpt>transformVars<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>transformVars</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>A list of variables to pass to your external transform function.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>transformObjects</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>A named list of  objects that can be referenced by <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept>, <bpt id="p2">*</bpt>transformFunc<ept id="p2">*</ept>, or <bpt id="p3">*</bpt>rowSelection<ept id="p3">*</ept> arguments.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>transformPackages</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>A list of packages, in addition to those specified in <bpt id="p1">**</bpt>rxGetOption("transformPackages")<ept id="p1">**</ept>, to be preloaded, that provide libraries and functions used in <bpt id="p2">*</bpt>transforms<ept id="p2">*</ept>, <bpt id="p3">*</bpt>transformFunc<ept id="p3">*</ept>, or <bpt id="p4">*</bpt>rowSelection<ept id="p4">*</ept> arguments.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>transformEnvir</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>A user-defined environment to serve as a parent to all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Functions supporting transformations</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The following functions support embedded transformations or reference an external transformation function.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Use case</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>rxDataStep</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Create a subset rows or variables, or create new variables by transforming existing variables.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Also used for easy conversion between data in data frames and .xdf files.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>rxImport</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Invoke a transformation while loading data into a data frame or .xdf file.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>rxSummary</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Transform data inline, while computing summary statistics.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>rxLinMod</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Create or transform variables used in the data set of a linear regression.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>rxLogit</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Create or transform variables used in the data set of a logistic regression.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>rxCube</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Create new variables or transform an existing variable used to create the list of variables in <bpt id="p1">**</bpt>rxCube<ept id="p1">**</ept> output.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Other functions don't accept transformation logic, but are used for data manipulation operations:</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>rxSetVarInfo<ept id="p1">**</ept> Change variable information, such as the name or description, in an .xdf file or data frame.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>rxSetInfo<ept id="p1">**</ept>  Add or change a data set description.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>rxFactors<ept id="p1">**</ept> Add or change a factor levels</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>rxMerge<ept id="p1">**</ept> Combines two or more datasets.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>rxSort<ept id="p1">**</ept> Orders a dataset based on some criteria</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>How transforms are evaluated</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>User-defined transforms and transform functions are evaluated in essentially the same way.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>User-defined transforms are combined into an implicit transform function for evaluation purposes.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>At evaluation time, the process is the same whether the function is predefined or user-defined.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>An evaluation environment is constructed from the base environment together with the utils, stats, methods packages, any packages specified with the <bpt id="p1">*</bpt>transformPackages<ept id="p1">*</ept> argument, and any specified <bpt id="p2">*</bpt>transformObjects<ept id="p2">*</ept>, and the closure of the transform function.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Functions are then evaluated in the context of this environment.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Functions that are in packages but not part of the evaluation environment can be used if fully qualified (specifically, prefixed by the package name and two or three colons, depending on whether the function is exported).</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>If you are using methods packages, you can modify the basic list by setting the <bpt id="p1">**</bpt>rxOption<ept id="p1">**</ept> <bpt id="p2">*</bpt>transformPackages<ept id="p2">*</ept> argument.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Transformations to avoid</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Transform functions are very powerful, but there are four types of transformation that should be avoided:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Transformations that change the length of a variable.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>This includes, naturally, most model-fitting functions.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Transformations that depend upon all observations simultaneously.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Because RevoScaleR works on chunks of data, such transformations will not have access to all the data at once.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Examples of such transformations are matrix operations such as poly or solve.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Transformations that have the possibility of creating different mappings of factor codes to factor labels.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Transformations that involve sampling with replacement.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Again, this is because RevoScaleR works on chunks of data, and sampling with replacement chunk by chunk is not equivalent to sampling with replacement from the full data set.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>If you change the length of one variable, you will get errors from subsequent analysis functions that not all variables are the same length.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>If you try to change the length of all variables (essentially, performing some sort of row selection), you need to pass all of your data through the transform function, and this can be very inefficient.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>To avoid this problem, use row selection to work on data one slice at a time.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>If you create a factor within a transformation function, you may get unexpected results because all of the data is not in memory at one time.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>When creating a factor within a transformation function, you should always explicitly set the values and labels.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Next Steps</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Continue on to the following data-related articles to learn more about XDF, data source objects, and other data formats:</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>How to transform and subset data</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>XDF files</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Data Sources</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Import text data</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Import ODBC data</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Import and consume data on HDFS</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>RevoScaleR Functions</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Tutorial: data import and exploration<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept> <bpt id="p2">[</bpt>Tutorial: data visualization and analysis<ept id="p2">](tutorial-revoscaler-data-model-analysis.md)</ept></source>
        </trans-unit></group></body></file></xliff>