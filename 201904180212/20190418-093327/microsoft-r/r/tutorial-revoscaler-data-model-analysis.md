<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="tutorial-revoscaler-data-model-analysis.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4b9b6387f1022774ea4ef8ef0ab968833c03f0308.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">b9b6387f1022774ea4ef8ef0ab968833c03f0308</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\tutorial-revoscaler-data-model-analysis.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Tutorial: Visualize and analyze data using RevoScaleR (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn how to visualize and analyze data using the RevoScaleR functions in Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Tutorial: Visualize and analyze data using RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: Microsoft R Client, Machine Learning Server<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>This tutorial builds on what you learned in the previous <bpt id="p1">[</bpt>data import and exploration tutorial<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept> by adding more steps and functions that broaden your experience with RevoScaleR functions.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>As before, you'll work with airline sample data to complete the steps.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>This tutorial focuses on analysis and predictions.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>R Client and Machine Learning Server are interchangeable in terms of RevoScaleR as long as <bpt id="p1">[</bpt>data fits into memory and processing is single-threaded<ept id="p1">](tutorial-revoscaler-data-import-transform.md#chunking)</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>If datasets exceed memory, we recommend pushing the <bpt id="p1">[</bpt>compute context<ept id="p1">](concept-what-is-compute-context.md)</ept> to Machine Learning Server.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>What you will learn</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>How to fit a linear model</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Compute crosstabs</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Fit a logistic regression model</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Compute predicted values</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>To complete this tutorial as written, use an R console application.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>On Windows, go to \Program Files\Microsoft\R Client\R_SERVER\bin\x64 and double-click <bpt id="p1">**</bpt>Rgui.exe<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>On Linux, at the command prompt, type <bpt id="p1">**</bpt>Revo64<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>You must also have data to work with.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The previous tutorial, <bpt id="p1">[</bpt>Data import and exploration<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept>, explains functions and usage scenarios.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Run the following script to reload data from the previous tutorial:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>How to fit a model</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>This section of the tutorial demonstrates several approaches for fitting a model to the sample data.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Fit a linear model</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">**</bpt>rxLinMod<ept id="p1">**</ept> function to fit a linear model using airXdfData from the previous tutorial.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Use a single dependent variable, the factor <bpt id="p1">*</bpt>DayOfWeek<ept id="p1">*</ept>:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The resulting output is:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Using the cube argument and plotting results</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If you are using categorical data in your regression, you can use the <bpt id="p1">*</bpt>cube<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>cube<ept id="p1">*</ept> is set to TRUE and the first term of the regression is categorical (a factor or an interaction of factors), the regression is done using a partitioned inverse, which may be faster and use less memory than standard regression computation.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Averages/counts of the category "bins" can be computed in addition to standard regression results.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The intercept will also be automatically dropped so that each category level will now have an estimated coefficient.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>cube<ept id="p1">*</ept> is set to TRUE and the first term is not categorical, you get an error message.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Re-estimate the linear model, this time setting cube to TRUE.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Print a summary of the results:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>You should see the following output:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The coefficient estimates are the mean arrival delay for each day of the week.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>When the cube argument is set to TRUE and the model has only one term as an independent variable, the "countDF" component of the results object also contains category means.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>This data frame can be extracted using the <bpt id="p1">*</bpt>rxResultsDF<ept id="p1">*</ept> function, and is particularly convenient for plotting.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>You should see the following output:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Now plot the average arrival delay for each day of the week:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The following plot is generated, showing the lowest average arrival delay on Thursdays:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>DayOfWeek Plot</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Linear model with multiple independent variables</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>We can run a more complex model examining the dependency of arrival delay on both day of week and the departure time.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>We’ll estimate the model using the <bpt id="p1">*</bpt>F<ept id="p1">*</ept> expression to have the <bpt id="p2">*</bpt>CRSDepTime<ept id="p2">*</ept> variable interpreted as a categorical or factor variable.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>F()<ept id="p1">*</ept> is not an R function, although it looks like one when used inside RevoScaleR formulas.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>An <bpt id="p1">*</bpt>F<ept id="p1">*</ept> expression tells RevoScaleR to create a factor by creating one level for each integer in the range <bpt id="p2">*</bpt>(floor(min(x)), floor(max(x)))<ept id="p2">*</ept> and binning all the observations into the resulting set of levels.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>You can look up the <bpt id="p1">[</bpt><bpt id="p2">**</bpt>rxFormula<ept id="p2">**</ept><ept id="p1">](../r-reference/revoscaler/rxformula.md)</ept> for more information.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>By interacting <bpt id="p1">*</bpt>DayOfWeek<ept id="p1">*</ept> with <bpt id="p2">*</bpt>F(CRSDepTime)<ept id="p2">*</ept> we are creating a dummy variable for every combination of departure hour and day of the week.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The output shows the first fifteen rows of the counts data frame.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The variable <bpt id="p1">*</bpt>CRSDepTime<ept id="p1">*</ept> gives the hour of the departure time and <bpt id="p2">*</bpt>ArrDelay<ept id="p2">*</ept> shows the average departure delay for that hour for that day of week.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Counts gives the number of observations that contain that combination of day of week and departure hour.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Now plot the results:</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>You should see the following plot:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>CRSDepTime Plot</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Subset the data and compute a crosstab</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Create a new data set containing a subset of rows and variables.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>This is convenient if you intend to do lots of analysis on a subset of a large data set.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>To do this, we use the <bpt id="p1">**</bpt>rxDataStep<ept id="p1">**</ept> function with the following arguments:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>outFile:<ept id="p1">*</ept> the name of the new data set</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>inData:<ept id="p1">*</ept>  the name of an .xdf file or an RxXdfData object representing the original data set you are subsetting</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>varsToDrop:<ept id="p1">*</ept> a character vector of variables to drop from the new data set, here CRSDepTime</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>rowSelection:<ept id="p1">*</ept> keep only the rows where the flight was more than 15 minutes late</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The resulting call is as follows:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>You will see that the new data set has only two variables and has dropped from 600,000 to 148,526 observations.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Compute a crosstab showing the mean arrival delay by day of week.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The results show that in this data set “late” flights are on average over 10 minutes later on Tuesdays than on Sundays:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Run a logistic regression on the new data</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The function <bpt id="p1">**</bpt>rxLogit<ept id="p1">**</ept> takes a binary dependent variable.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Here we will use the variable <bpt id="p1">*</bpt>Late<ept id="p1">*</ept>, which is <bpt id="p2">*</bpt>TRUE<ept id="p2">*</ept> (or <bpt id="p3">*</bpt>1<ept id="p3">*</ept>) if the plane was more than 15 minutes late arriving.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>For dependent variables we will use the <bpt id="p1">*</bpt>DepHour<ept id="p1">*</ept>, the departure hour, and <bpt id="p2">*</bpt>Night<ept id="p2">*</ept>, indicating whether or not the flight departed at night.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>You should see the following results:</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Using the same function, let's estimate whether or not a flight is “very late” depending on the day of week:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>The results show that in this sample, a flight on Tuesday is most likely to be very late or canceled, followed by flights departing on Friday.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>In this model, Sunday is the control group, so that coefficient estimates for other days of the week are relative to Sunday.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The intercept shown is the same as the coefficient you would get for Sunday if you omitted the intercept term:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Computing predicted values</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>You can use the object returned from the call to <bpt id="p1">**</bpt>rxLogit<ept id="p1">**</ept> in the previous section to compute predicted values.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>In addition to the model object, we specify the data set on which to compute the predicted values and the data set in which to put the newly computed predicted values.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>In the call below, we use the same dataset for both.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>In general, the data set on which to compute the predicted values must be similar to the original data set used to estimate the model in the following ways; it should have the same variable names and types, and factor variables must have the same levels in the same order.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>You should see the following information:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>This tutorial demonstrated how to use several important functions, but on a small data set.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Next up are additional tutorials that explore RevoScaleR with bigger data sets, and customization approaches if built-in functions are not quite enough.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Analyze large data with RevoScaleR and airline flight delay data<ept id="p1">](tutorial-revoscaler-large-data-airline.md)</ept></source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Example: Analyzing loan data with RevoScaleR<ept id="p1">](tutorial-revoscaler-large-data-loan.md)</ept></source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Example: Analyzing census data with RevoScaleR<ept id="p1">](tutorial-revoscaler-large-data-census.md)</ept></source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Write custom chunking algorithms<ept id="p1">](how-to-developer-write-chunking-algorithms.md)</ept></source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Try demo scripts</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Another way to learn about ScaleR is through demo scripts.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Scripts provided in your Machine Learning Server installation contain code that's very similar to what you see in this tutorial.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>You can highlight portions of the script, right-click <bpt id="p1">**</bpt>Execute in Interactive<ept id="p1">**</ept> to run the script in RTVS.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Demo scripts are located in the <bpt id="p1">*</bpt>demoScripts<ept id="p1">*</ept> subdirectory of your Machine Learning Server installation.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>On Windows, this is typically:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR Getting Started with Hadoop<ept id="p1">](how-to-revoscaler-hadoop.md)</ept></source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR Getting Started with SQL server<ept id="p1">](how-to-revoscaler-sql-server.md)</ept></source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept><ph id="ph1"> </ph></source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How-to guides in Machine Learning Server<ept id="p1">](how-to-introduction.md)</ept> <bpt id="p2">[</bpt>RevoScaleR Functions<ept id="p2">](../r-reference/revoscaler/revoscaler.md)</ept></source>
        </trans-unit></group></body></file></xliff>