<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-data-summaries.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e7674f411f3e0390faa31490c488eefcff7f22395.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">7674f411f3e0390faa31490c488eefcff7f22395</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-data-summaries.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Data Summaries using RevoScaleR (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Summarizing data in RevoScaleR using rxGetVarInfo, rxSummary, and rxLorenz functions.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to summarize data using RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Summary statistics can help you understand the characteristics and shape of an unfamiliar data set.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>RevoScaleR<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept>, you can use the <bpt id="p2">[</bpt>rxGetVarInfo<ept id="p2">](../r-reference/revoscaler/rxgetvarinfo.md)</ept> function to learn more about variables in the data set, and <bpt id="p3">[</bpt>rxSummary<ept id="p3">](../r-reference/revoscaler/rxsummary.md)</ept> for statistical measures.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>The rxSummary function also provides a count of observations, and the number of missing values (if any).</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>This article teaches by example, using built-in sample data sets so that you can practice each skill.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>It covers the following tasks:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>List variable metadata including name, description, type, labels, Low/High values</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Compute summary statistics: mean, standard deviation, minimum, maximum values</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Compute summary statistics for factor variables</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Create temporary factor variables used in computations</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Compute summary statistics on a row subset</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Execute in-flight data transformations</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Compute and plot a Lorenz curve</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Tips for wide data sets</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>List variable information</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>rxGetVarInfo<ept id="p1">](../r-reference/revoscaler/rxgetvarinfo.md)</ept> function returns information about the variables in a data frame or .xdf file, including variable names, descriptions, type, and high and low values.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The following examples, based on the built-in sample Census data set, demonstrate function usage.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>names function<ept id="p1">](https://www.rdocumentation.org/packages/base/versions/3.4.3/topics/names)</ept> is a base R function, which is called on the object to return the following variable names:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Once you have a variable name, you can drill down further to examine its metadata.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This is the output for age:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Numeric variables include Low/High values.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The Low/High values do not necessarily indicate the minimum and maximum of a numeric or integer variable.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Rather, they indicate the values RevoScaleR uses to establish the lowest and highest <bpt id="p1">*</bpt>factor levels<ept id="p1">*</ept> when treating the variable as a factor.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>For practical purposes, this is more helpful for data visualization than a true minimum or maximum on the variable.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>For example, suppose you want to create histograms or hexbin plots, treating the numerical data as categorical, with levels corresponding to the plotting bins. In this scenario, it is often convenient to cut off the highest and lowest data points, and the Low/High values provide this information.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>This example demonstrates getting the High value from the age variable:</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Similarly, the Low value is obtained as follows:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Suppose you are interested in workers between the ages of 30 and 50.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>You could create a copy of the data file in the working directory, set the High/Low fields as follows and then treat age as a factor in subsequent analysis:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Results (restricted to the 35 to 50 age range)<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>To reset the low and high values, repeat the previous steps with the original values:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Compute summary statistics</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>rxSummary<ept id="p1">](../r-reference/revoscaler/rxsummary.md)</ept> function provides descriptive statistics using a <bpt id="p2">*</bpt>formula<ept id="p2">*</ept> argument similar to that used in R’s modeling functions.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The formula specifies the independent variables to summarize.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The basic structure of a formula is a <bpt id="p1">[</bpt>tilde<ept id="p1">](https://www.rdocumentation.org/packages/base/versions/3.4.3/topics/tilde)</ept> symbol "~" with one or more independent or right-hand variables, separated by "+".</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>To include all of the variables, you can append a dot (.) to the tilde as "~.".</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The rxSummary function also takes a data object as the source of the variables.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>For example, returning to the CensusWorkers sample, run the following script to obtain a data summary of that file:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>For each term in the formula, the mean, standard deviation, minimum, maximum, and number of valid observations is shown.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>If rxSummary includes <ph id="ph1">`byTerm=FALSE`</ph>, the observations (rows) containing missing values for any of the specified variables are omitted in calculating the summary.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Cell counts for categorical variables are included.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Results</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Compute median values</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>You might have noticed that rxSummary does not compute a median value for each variable.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>This is because rxSummary only produces statistics that can be computed in chunks, and a median computation is not a chunkable calculation.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Median calculations are predicated on a sort operation, which is expensive on large data sets, and thus excluded from rxSummary.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Assuming your data set fits in memory, you could get the median value of a given variable using the base R <bpt id="p1">[</bpt>median<ept id="p1">](https://www.rdocumentation.org/packages/stats/versions/3.4.3/topics/median)</ept> function:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Results</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>For larger disk-bound datasets, you should use visualization techniques to uncover skewness in the underlying data.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Compute summary statistics on factor variables</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>You can obtain summary statistics on numeric data that are specific to levels within a variable, such as days of the week, months in a year, age or income levels constructed from column values, and so forth.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>To do this, specify an interaction between a numeric variable and a factor variable.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>For example, using the sample data set AirlineDemoSmall.xdf, use the following command to request a summary of arrival delay by day of week:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Results</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>The request produces summary statistics for a factor variable, with output for each level.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Interactions provide the one exception to the “responseless” formula mentioned preceding.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>If you want to obtain the interaction of a continuous variable with one or more factors, you can use a formula of the form <ph id="ph1">`y ~ x:z`</ph>, where y is the continuous variable and x and z are factors.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>This has precisely the same effect as specifying the formula as <ph id="ph1">`~y:x:z`</ph>, but is more suggestive of the result: specifically, summary statistics for y at every combination of levels of x and z.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Create a temporary factor variable</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>You can force RevoScaleR to treat a variable as a factor (with a level for each integer value from the low to high value) by wrapping it with the function call syntax <ph id="ph1">`F()`</ph>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Returning to the CensusWorkers.xdf file, in the following example a factor level is temporarily created for each age from 20 through 65:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Results</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The results provide not only summary statistics for wage income in the overall data set, but summary statistics on wage income for each age:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>If you include an interaction between two factors, the summary provides cell counts for all combinations of levels of the factors.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Since the census data has probability weights, you can use the <ph id="ph1">`pweights`</ph> argument to get weighted counts:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Results</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Compute summary statistics on a row subset</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The following example shows how to restrict the analysis to specific rows (in this case, people aged 30 to 39).</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>You can use the <ph id="ph1">`low`</ph> and <ph id="ph2">`high`</ph> arguments of the <ph id="ph3">`F()`</ph> function to restrict the creation of on-the-fly factor levels to the same range:</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Results</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>The fourth argument in the function, <ph id="ph1">`exclude`</ph>, defaults to TRUE.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>This is reflected in the T that appears in the output variable name.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Write summary statistics to XDF</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>By-group statistics are often computed for further analysis or plotting.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>It can be convenient to store these results in a .xdf file, especially when there are a large number of groups.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>In this example, compute the mean and standard deviation of wage income and number of weeks work for each year of age for both men and women using the CensusWorkers.xdf file with data from three states:</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Results</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>You can take a quick look at the first five rows in the data set to see that the first variables are the two factor variables determining the groups: F<ph id="ph1">\_</ph>age and sex.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>The remaining variables are the computed by-group statistics.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Results</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>You can plot directly from the .xdf file to visualize the results:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Transform data in-flight</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>You can use the <ph id="ph1">`transforms`</ph> argument to modify your data set before computing a summary.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>When used in this way, the original data is unmodified and no permanent copy of the modified data is written to disk.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>The data summaries returned, however, reflect the modified data.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>You can also transform data in the formula itself, by specifying simple functions of the original variables.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>For example, you can get a summary based on the natural logarithm of a variable as follows:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Results</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Compute and plot Lorenz curves</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>The Lorenz curves were originally developed to illustrate income inequality.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>For example, it can show us what percentage of total income is attributed to the lowest earning 10% of the population.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>rxLorenz<ept id="p1">](../r-reference/revoscaler/rxlorenz.md)</ept> function from RevoScaleR provides a "big data" version, using approximate quantiles to quickly compute the cumulative distribution by quantile in a single pass through the data.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>The rxLorenz function requires an <ph id="ph1">`orderVarName`</ph>, the name of the variable used to compute the quantiles.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>A separate <ph id="ph1">`valueVarName`</ph> can also be specified.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>This is the name of the variable used to compute the mean values by quantile.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>By default, the same variable is used for both.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>We can continue to use the Census Workers data set as an example, computing a Lorenz curve for the distribution of income:</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>The returned object contains the cumulative values and the percentages.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Using the plot method for rxLorenz, we can get a visual representation of the income distribution and compare it with the horizontal line representing perfect equality:</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>The Gini coefficient is often used as a summary statistic for Lorenz curves.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>It is computed by estimating the ratio of the area between the line of equality and the Lorenz curve to the total area under the line of equality (using trapezoidal integration).</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>The Gini coefficient can range from 0 to 1, with 0 representing perfect equality.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>We can compute it from using the output from rxLorenz:</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Tips for wide data sets</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Building a better understanding of the distribution of each variable and the relationships between variables improves decision making during the modeling phase.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>This is especially true for wide data sets containing hundreds if not thousands of variables.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>For wide data sets, the main goal of data exploration should be to find any outliers or influential data points, identify redundant variables or correlated variables and transform or combine any variables that seem appropriate.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>The functions rxGetVarInfo and rxSummary provide useful information can help in this effort, but these two functions may need to be used differently when the data contain many variables.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>As a first step, import the data to an .xdf so that you can execute functions providing metadata and summary statistics.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Recall that rxGetVarInfo returns metadata about the data object.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>After loading data into an XDF data source, the data type information can easily be accessed using the rxGetVarInfo function.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Because wide data has so many variables, printed output can be hard to read.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>As an alternative, save the variable information to an object that can serve as in informal data dictionary.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>We demonstrate this using the Claims data from the sample data directory:</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>We can then obtain the information for an individual variable as follows:</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>The rxSummary function is a great way to look at the distribution of individual variables and identify outliers.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>With wide data, you want to store the results of this function into an object.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>This object contains a data frame with the results of the numeric variables, “sDataFrame”, and a list of data frames with the counts for each categorical variable,”categorical”:</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Printing the rxSummary results to the console wouldn’t be useful with so many variables.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Saving the results in an object allows us to not only access the summary results programmatically, but also to view the results separately for numeric and categorical variables.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>We access the sDataFrame (printed to show structure) as follows:</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>To view the categorical variables, we access the categorical component:</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Another key piece of data exploration for wide data is looking at the relationships between variables to find variables that are measuring the same information or variables that are correlated.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>With variables that are measuring the same information, perhaps one stands out as being representative of the group.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>During data exploration, you must rely on your domain knowledge to group variables into related sets or prioritize variables that are important based on the field or industry.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Paring the data set down to related sets allow you to look more closely at redundancy and relatedness within each set.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>When looking for correlation between variables the function <bpt id="p1">[</bpt>rxCrosstabs<ept id="p1">](../r-reference/revoscaler/rxcrosstabs.md)</ept> is useful.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>Crosstabs<ept id="p1">](how-to-revoscaler-crosstabs.md)</ept>, you see how to use rxCrosstabs and <bpt id="p2">[</bpt>rxLinePlot<ept id="p2">](../r-reference/revoscaler/rxlineplot.md)</ept> to graph the relationship between two variables.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Graphs allow for a quick view of the relationship between two variables, which comes in handy when you have many variables to consider.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Visualizing Huge Data Sets: An Example from the U.S. Census<ept id="p1">](how-to-revoscaler-visualize-huge-data-sets.md)</ept>.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Tutorial: Data import and exploration using RevoScaleR</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Tutorial: Transform and subset data using RevoScaleR</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Sample data for RevoScaleR and revoscalepy</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Importing text data in Machine Learning Server</source>
        </trans-unit></group></body></file></xliff>