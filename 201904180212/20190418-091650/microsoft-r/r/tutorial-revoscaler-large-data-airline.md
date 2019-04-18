<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="tutorial-revoscaler-large-data-airline.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b42b8771fdc895bf0c77170a46d485f080eceea8d5.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">2b8771fdc895bf0c77170a46d485f080eceea8d5</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\tutorial-revoscaler-large-data-airline.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Tutorial: Load and analyze a large airline data set with RevoScaleR in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn how to work with big data using a sample airline dataset in this RevoScaleR tutorial walkthrough.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Tutorial: Load and analyze a large airline data set with RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>This tutorial builds on what you learned in the <bpt id="p1">[</bpt>first RevoScaleR tutorial<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept> by exploring the functions, techniques, and issues arising when working with larger data sets.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>As before, you'll work with sample data to complete the steps, except this time you will use a much larger data set.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Download the airline dataset</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>To really get a feel for RevoScaleR, you should work with functions using a larger data set.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Larger data sets are available for download <bpt id="p1">[</bpt>from this web page<ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698896&amp;clcid=0x409)</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>You can use a smaller or larger data set with this tutorial.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Datasets for this tutorial include the following:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>AirOnTime87to12<ept id="p1">*</ept>: An .xdf file containing information on flight arrival and departure details for all commercial flights within the USA, from October 1987 to December 2012.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>This is a large dataset: there are nearly 150 million records in total.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>It is just under 4 GB unpacked.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>AirOnTime7Pct<ept id="p1">*</ept>: A 7% subsample of AirOnTimeData87to12.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>This is an .xdf file containing just the variables used in the examples in this tutorial.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>It can be used as an alternative.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>This subsample contains a little over 10 million rows of data.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>It is about 100 MB unpacked.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>When downloading these files, put them in a directory where you can easily access them.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>For example, create a directory "C:\MRS\BigData" and unpack the files there.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>When running examples using these files, you will want to specify this location as your <bpt id="p1">*</bpt>bigDataDir<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Origin of the sample datasets</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Airline on-time performance data for the years 1987 through 2008 was used in the American Statistical Association Data Expo in 2009 (<bpt id="p1">[</bpt><ph id="ph1">http://stat-computing.org/dataexpo/2009/</ph><ept id="p1">](http://stat-computing.org/dataexpo/2009/)</ept>).</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>ASA describes the data set as follows:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The data consists of flight arrival and departure details for all commercial flights within the USA, from October 1987 to April 2008.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>This is a large dataset: there are nearly 120 million records in total, and takes up 1.6 gigabytes of space compressed and 12 gigabytes when uncompressed.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Data by month can be downloaded as comma-delimited text files from the Research and Innovative Technology Administration (RITA) of the Bureau of Transportation Statistics web site (<bpt id="p1">[</bpt><ph id="ph1">http://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=236</ph><ept id="p1">](http://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=236)</ept>).</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Data from 1987 through 2012 has been imported into an .xdf file named <bpt id="p1">*</bpt>AirOnTime87to12.xdf<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>A much smaller subset containing 7% of the observations for the variables used in this example is also available as <bpt id="p1">*</bpt>AirOnTime7Pct.xdf<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>This subsample contains a little over 10 million rows of data, so has about 60 times the rows of the smaller subsample used in the previous example.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>More information on this data set can be found in the help file: <ph id="ph1">`?AirOnTime87to12`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>To view the help file, enter the file name at the <ph id="ph1">`&gt;`</ph> prompt in the R interactive window.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Explore the data</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Assuming you specified a location of your downloaded data as the <bpt id="p1">*</bpt>bigDataDir<ept id="p1">*</ept> variable, create an object for the dataset as <bpt id="p2">*</bpt>airDataName<ept id="p2">*</ept>:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>or</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Create an in-memory <bpt id="p1">*</bpt>RxXdfObject<ept id="p1">*</ept> data source object to represent the .xdf data file:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">*</bpt>rxGetInfo<ept id="p1">*</ept> function to get summary information on the active data set.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The full data set has 46 variables and almost 150 million observations.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Reading a Chunk of Data</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Data stored in the xdf file format can be read into a data frame, allowing the user to choose the rows and columns.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>For example, read  1000 rows beginning at the 100,000th row for the variables <bpt id="p1">*</bpt>ArrDelay<ept id="p1">*</ept>, <bpt id="p2">*</bpt>DepDelay<ept id="p2">*</ept>, and <bpt id="p3">*</bpt>DayOfWeek<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>You should see the following information if <bpt id="p1">*</bpt>bigAirDS<ept id="p1">*</ept> is the full data set, <bpt id="p2">*</bpt>AirlineData87to08.xdf<ept id="p2">*</ept>:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>And we can easily run a regression using the <bpt id="p1">*</bpt>lm<ept id="p1">*</ept> function in R using this small data set:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>It yields the following:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>But this is only 1/148,619 of the rows contained in the full data set.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If we try to read all the rows of these columns, we will likely run into memory problems.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>For example, on most systems with 8GB or less of RAM, running the commented code below will fail on the full data set with a "cannot allocate vector" error.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>In the next section you will see how you can analyze a data set that is too big to fit into memory by using <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Estimating a Linear Model with a Huge Data Set</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The RevoScaleR compute engine is designed to work very efficiently with .xdf files, particularly with factor data.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>When working with larger data sets, the <bpt id="p1">*</bpt>blocksPerRead<ept id="p1">*</ept> argument is important in controlling how much data is processed in memory at one time.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If too many blocks are read in at one time, you may run out of memory.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>If too few blocks are read in at one time, you may experience slower total processing time.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>You can experiment with <bpt id="p1">*</bpt>blocksPerRead<ept id="p1">*</ept> on your system and  time the estimation of a linear model as follows:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more...<ept id="p1">](tutorial-revoscaler-data-import-transform.md#chunking)</ept></source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The linear model you get will not vary as you change <bpt id="p1">*</bpt>blocksPerRead<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>To see a summary of your results:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>You should see the following results for the full data set:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>DayOfWeek=Sun  6.062001   0.006993   866.8 2.22e-16 ***</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>20308838</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Notice that because we specified <bpt id="p1">*</bpt>cube = TRUE<ept id="p1">*</ept>, we have an estimated coefficient for each day of the week (and not the intercept).</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Because the computation is so fast, we can easily expand our analysis.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>For example, we can compare Arrival Delays with Departure Delays.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>First, we rerun the linear model, this time using Departure Delay as the dependent variable.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Next, combine the information from regression output in a data frame for plotting.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Then use the following code to plot the results, comparing the Arrival and Departure Delays by the Day of Week</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>You should see the following plot for the full data set:</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>DayOfWeek Plot</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Turning Off Progress Reports</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>By default, <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> reports on the progress of the model fitting so that you can see that the computation is proceeding normally.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>You can specify an integer value from 0 through 3 to specify the level of reporting done; the default is 2.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>(See help on rxOptions to change the default.) For large model fits, this is usually reassuring.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>However, if you would like to turn off the progress reports, just use the argument <bpt id="p1">*</bpt>reportProgress=0<ept id="p1">*</ept>, which turns off reporting.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>For example, to suppress the progress reports in the estimation of the delayDep rxLinMod object, repeat the call as follows:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more...<ept id="p1">](tutorial-revoscaler-data-import-transform.md#chunking)</ept></source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Handling Larger Linear Models</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The data set contains a variable <bpt id="p1">*</bpt>UniqueCarrier<ept id="p1">*</ept> which contains airline codes for 29 carriers.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Because the RevoScaleR Compute Engine handles factor variables so efficiently, we can do a linear regression looking at the Arrival Delay by Carrier.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>This will take a little longer, of course, than the previous analysis, because we are estimating 29 instead of 7 factor levels.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more...<ept id="p1">](tutorial-revoscaler-data-import-transform.md#chunking)</ept></source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Next, sort the coefficient vector so that the we can see the airlines with the highest and lowest values.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Next, use the <bpt id="p1">*</bpt>head<ept id="p1">*</ept> function to show the top 10 with the lowest arrival delays:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>In the full data set the result is:</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Then use the <bpt id="p1">*</bpt>tail<ept id="p1">*</ept> function to show the bottom 10 with the highest arrival delays:</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>With all of the data, you should see:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Notice that Hawaiian Airlines comes in as the best in on-time arrivals, while United is closer to the bottom of the list.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>We can see the difference by subtracting the coefficients:</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>which results in:</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Estimating Linear Models with Many Independent Variables</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>One ambitious question we could ask is to what extent the difference in delays is due to the differences in origins and destinations of the flights.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>To control for Origin and Destination we would need to add over 700 dummy variables in the full data set to represent the factor levels of <bpt id="p1">*</bpt>Origin<ept id="p1">*</ept> and <bpt id="p2">*</bpt>Dest<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>The RevoScaleR Compute Engine is particularly efficient at handling this type of problem, so we can in fact run the regression:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more...<ept id="p1">](tutorial-revoscaler-data-import-transform.md#chunking)</ept></source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Accounting for origin and destination reduces the airline-specific difference in average delay:</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>We can continue in this process, next adding variables to take account of the hour of day that the flight departed.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Using the <bpt id="p1">*</bpt>F<ept id="p1">*</ept> function around the <bpt id="p2">*</bpt>CRSDepTime<ept id="p2">*</ept> will break the variable into factor categories, with one level for each hour of the day.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Now we can summarize all of our results:</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>For the full data set, the results look like:</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Predicting Airline Delay</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Using the estimated regression coefficients, write a function to estimate the predicted delay given the carrier, the airport of origin, the destination airport, and the departure time (0 – 24 hours):</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>We can use this function to compare, for example, the expected delay for trips going from Seattle to New York, or Newark, or Honolulu:</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>The three expected delays are calculated (using the full data set) as:</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Computing a Large Scale Regression Using a Compute Cluster</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Up to now, all of our examples have assumed you are running your computations on a single computer, which might have multiple computational cores.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Many users with large data to analyze, however, have access to compute clusters that work together to provide greater computing power.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>With RevoScaleR, you can easily connect to a Hadoop cluster and distribute your computation among the various nodes of the cluster.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Here we will show a quick example of using a Spark (Hadoop) cluster consisting of a name node and one or more data nodes.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>To connect to a high availability cluster using default values, you only need to provide the cluster nameNode and port.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>nameNode<ept id="p1">*</ept> manages the namespace of the cluster.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>You can then make the cluster connection object active by using <bpt id="p1">*</bpt>rxSetComputContext<ept id="p1">*</ept>:</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>With your compute context set to the cluster, all of the RevoScaleR data analysis functions (i.e., rxSummary, rxCube, rxCrossTabs, rxLinMod, rxLogit, rxGlm, rxCovCor (and related functions), rxDTree, rxDForest, rxBTrees, rxNaiveBayes, and rxKmeans) automatically distribute computations across the nodes of the cluster.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>It is assumed that copies of the data are in the same path on each node.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>(Other options are discussed in the <bpt id="p1">[</bpt>RevoScaleR Distributed Computing Guide<ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698560&amp;clcid=0x409)</ept>.)</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Now you can re-run the large scale regression, this time just specifying the name of the data file without the path:</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more...<ept id="p1">](tutorial-revoscaler-data-import-transform.md#chunking)</ept></source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>The computations are automatically distributed over all the nodes of the cluster.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>To reset the compute context to your local machine, use:</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>If you missed the first tutorial, see <bpt id="p1">[</bpt>Practice data import and exploration<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept> for an overview.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>For more advanced lessons, see <bpt id="p1">[</bpt>Write custom chunking algorithms<ept id="p1">](how-to-developer-write-chunking-algorithms.md)</ept>.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How-to guides in Machine Learning Server<ept id="p1">](how-to-introduction.md)</ept></source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR Functions<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept></source>
        </trans-unit></group></body></file></xliff>