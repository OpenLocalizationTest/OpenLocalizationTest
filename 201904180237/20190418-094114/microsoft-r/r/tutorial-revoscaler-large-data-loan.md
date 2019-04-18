<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="tutorial-revoscaler-large-data-loan.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926bbedb336db3ef149e6c1e6ef3436f5ad894eeea4.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">bbedb336db3ef149e6c1e6ef3436f5ad894eeea4</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\tutorial-revoscaler-large-data-loan.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Tutorial: Analyzing loan data using RevoScaleR in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn how to work with big datasets using sample loan data in this RevoScaleR tutorial walkthrough.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Tutorial: Analyzing loan data with RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>This example builds on what you learned in an <bpt id="p1">[</bpt>earlier tutorial<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept> by showing you how to import .csv files to create an .xdf file, and use statistical RevoScaleR functions to summarize the data.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>As before, you'll work with sample data to complete the steps.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Get the mortgage default data set</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Data import and exploration are covered further on, but to complete those steps you will need a collection of .csv files providing the sample data.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The sample data used in this tutorial consists of simulated data on mortgage defaults.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A small version of the data set is pre-installed with the <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> package that ships with R Client and Machine Learning Server.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>It provides 100,000 observations.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Alternatively, you can download a larger version of the data set providing 10 million observations.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Use the pre-installed .csv files<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Small versions of the data sets can be found in the sample data directory:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Each file contains 10,000 rows, for a total of 100,000 observations.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Download the larger data set<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>To work with a larger dataset, you can download <bpt id="p1">*</bpt>mortDefault<ept id="p1">*</ept>, a set of ten comma-separated files, each of which contains one million observations of simulated data on mortgage defaults.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>You can download zipped <bpt id="p1">[</bpt>from this web site<ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698896&amp;clcid=0x409)</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Windows users should download the zip version, mortDefault.zip.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Linux users should download mortDefault.tar.gz.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>File size is approximately 220 MB unpacked.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>When downloading these files, put them in a directory where you can easily access them.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>For example, create a directory "C:\MRS\BigData" and unpack the files there.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>When running examples using these files, you will want to specify this location as your <bpt id="p1">*</bpt>bigDataDir<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Each download contains ten files, each of which contains one million observations for a total of 10 million:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>About the data</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>This example uses simulated data at the individual level to analyze loan defaults.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Data has been collected every year for 10 years on mortgage holders, stored in a comma delimited data set for each year.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The data contains 5 variables:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>default<ept id="p1">*</ept> – a 0/1 binary variable indicating whether or not the mortgage holder defaulted on the loan</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>creditScore<ept id="p1">*</ept> – a credit rating</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>yearsEmploy<ept id="p1">*</ept> – the number of years the mortgage holder has been employed at their current job</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>ccDebt<ept id="p1">*</ept> – the amount of credit card debt</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>houseAge<ept id="p1">*</ept> – the age (in years) of the house</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>year<ept id="p1">*</ept> – the year the data was collected</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>As in previous tutorials, you can use package help to get more information by typing<ph id="ph1">`?mortDefaultSmall`</ph> at the <ph id="ph2">`&gt;`</ph> prompt in the R interactive window.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Specify the input files and output XDF file</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The first step is to import the data into an XDF file format for analysis.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>First, specify the source files you will be using.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>For the smaller data sets that exist in the sample data directory, enter:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>For the large files, enter the location of your downloaded data:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Notice that the file path uses a forward slash / character.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>This is the correct syntax, even for file paths on Windows operating systems that would otherwise use the back slash character.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Next, specify the name of the .xdf file you will create in your working directory (use "<bpt id="p1">*</bpt>mortDefault<ept id="p1">*</ept>" instead of "<bpt id="p2">*</bpt>mortDefaultSmall<ept id="p2">*</ept>" if you are using the large data sets):</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>or</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Import a set of files in a loop using append</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">*</bpt>rxImport<ept id="p1">*</ept> function to import the data.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>When the first data file is read, a new XDF file is created using the <bpt id="p1">*</bpt>dataFileName<ept id="p1">*</ept> specified above.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Subsequent data files are appended to that XDF file.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Within the loop, the name of the imported data file is created.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Output will be a series of Rows Read notifications, one for each file.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If you have previously imported the data and created the .xdf data source, you can create an .xdf data source representing the file us RxXdfData:</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>To get a basic summary of the data set and show the first 5 rows enter:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Output for the small data files should be as follows:</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Output for large data files:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Computing Summary Statistics</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">*</bpt>rxSummary<ept id="p1">*</ept> function to compute summary statistics for the variables in the data set, setting the <bpt id="p2">*</bpt>blocksPerRead<ept id="p2">*</ept> to <bpt id="p3">*</bpt>2<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if the script runs locally on R Client.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>The following output is returned (for the large data set):</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Computing a Logistic Regression</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Using the binary <bpt id="p1">*</bpt>default<ept id="p1">*</ept> variable as the dependent variable, estimate a logistic regression using <bpt id="p2">*</bpt>year<ept id="p2">*</ept>, <bpt id="p3">*</bpt>creditScore<ept id="p3">*</ept>, <bpt id="p4">*</bpt>yearsEmploy<ept id="p4">*</ept>, and <bpt id="p5">*</bpt>ccDebt<ept id="p5">*</ept> as independent variables.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Year is an integer value; if we include it as-is in the regression, we would get an estimate of a single coefficient for it indicating the trend in mortgage defaults.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Alternatively, we can treat year as a categorical or factor variable by using the F function.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>The benefit is that we get a separate coefficient estimated for each year (except the last), telling us which years have higher default rates, while controlling for the other variables in the regression.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The logistic regression is specified as follows:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more...<ept id="p1">](tutorial-revoscaler-data-import-transform.md#chunking)</ept></source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>You will see timings for each iteration and the final results printed.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The results for the large data set are:</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Computing a Logistic Regression with Many Parameters</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>If you are using the large <bpt id="p1">*</bpt>mortDefault<ept id="p1">*</ept> data set, you can continue and estimate a logistic regression with many parameters.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>One of the variables in the data set is <bpt id="p1">*</bpt>houseAge<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>As with <bpt id="p1">*</bpt>year<ept id="p1">*</ept>, we have no reason to believe that the logistic expression is linear with respect to the age of the house.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>We can look at how the age of the house is related to the default rate by including <bpt id="p1">*</bpt>houseAge<ept id="p1">*</ept> in the formula as a categorical variable, again using the <bpt id="p2">*</bpt>F<ept id="p2">*</ept> function.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>A coefficient will be estimated for 40 of the 41 values of <bpt id="p1">*</bpt>houseAge<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The results of the estimation are:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>We can extract the coefficients from logitObj for the houseAge variables and plot them:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The resulting plot shows that the age of the house is associated with a higher default rate in the middle of the range than for younger and older houses.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>HouseAge Plot</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Compute the Probability of Default</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Using the <bpt id="p1">*</bpt>rxPredict<ept id="p1">*</ept> function, we can compute the probability of default for given characteristics using our estimated logistic regression model as input.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>First create some vectors containing values of interest for each of the independent variables:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Now create a data frame with combinations of those values:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Using the <bpt id="p1">*</bpt>rxPredict<ept id="p1">*</ept> function, we can compute the predicted probability of default for each of the variable combinations.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>The predicted values will be added to the <bpt id="p1">*</bpt>outData<ept id="p1">*</ept> data set, if it already exists:</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>The results should be printed to your console, with the highest default rate at the top:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>If you missed the first tutorial, see <bpt id="p1">[</bpt>Practice data import and exploration<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept> for an overview.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>For more advanced lessons, see <bpt id="p1">[</bpt>Write custom chunking algorithms<ept id="p1">](how-to-developer-write-chunking-algorithms.md)</ept>.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How-to guides in Machine Learning Server<ept id="p1">](how-to-introduction.md)</ept></source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR Functions<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept></source>
        </trans-unit></group></body></file></xliff>