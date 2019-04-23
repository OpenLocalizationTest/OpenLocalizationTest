<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="tutorial-revoscaler-large-data-census.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a0bfa0f223ec2e892b944c4ecc65e2fa27780dd1c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">0bfa0f223ec2e892b944c4ecc65e2fa27780dd1c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\tutorial-revoscaler-large-data-census.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Tutorial: Analyzing census data using RevoScaleR in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn how to work with big datasets using sample census data in this RevoScaleR tutorial walkthrough.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Tutorial: Analyzing US census data with RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>This example builds on what you learned in an <bpt id="p1">[</bpt>earlier tutorial<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept> by exploring the import and statistical RevoScaleR functions typically used with larger data sets.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>As before, you'll work with sample data to complete the steps.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Download the census dataset</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The data set used in this tutorial is <bpt id="p1">*</bpt>CensusUS5Pct2000.xdf<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>You can download the .xdf file or zipped files <bpt id="p1">[</bpt>from this web site<ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698896&amp;clcid=0x409)</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>When downloading these files, put them in a directory where you can easily access them.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>For example, create a directory "C:\MRS\BigData" and unpack the files there.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>When running examples using these files, you will want to specify this location as your <bpt id="p1">*</bpt>bigDataDir<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Explore the data</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The built-in data set <bpt id="p1">*</bpt>CensusWorkers.xdf<ept id="p1">*</ept> provides a subsample of the 2000 5% IPUMS U.S. Census data.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>It contains information on individuals from 20 to 65 years old in the states of Connecticut, Indiana, and Washington who worked during 2000.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>First, let’s learn a little about the sample data set:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The results show that the data set has 6 variables and a little over 300,000 observations.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Plotting the Weighted Counts of Males and Females by Age</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Use <bpt id="p1">*</bpt>rxCube<ept id="p1">*</ept> to compute and plot the Age/Sex distribution by year of age for the data set.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>This data set has probability weights associated with each observation in the variable <bpt id="p1">*</bpt>perwt<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>We will use those weights in our calculations.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>As seen above, <bpt id="p1">*</bpt>age<ept id="p1">*</ept> is an integer variable.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>We would like to have it treated as a categorical or factor variable in the calculation, so we will use the <bpt id="p1">*</bpt>F()<ept id="p1">*</ept> function when using <bpt id="p2">*</bpt>age<ept id="p2">*</ept> in the formula:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>To extract a data frame containing the counts for every combination of age and sex, use <bpt id="p1">*</bpt>rxResultsDF<ept id="p1">*</ept>:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Now plot the number of males and females by age.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The resulting graph is shown below:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Age Graph</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The graph shows us that for the population in the data set, there are more men than women at every age.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Looking at Wage Income by Age and Sex</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Next, run a regression looking at the relationship between age, sex, and wage income and plot the results:</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The resulting graph shows that, in this data set, wage income is higher for males than females at every age:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Wage Income by Age and Sex</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Looking at Weeks Worked by Age and Sex</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>We can further explore the data by looking at the relationship between weeks worked and age and sex, following a similar process.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>This resulting graph shows that it is also the case that on average females work fewer weeks per year at every age during the working years:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Weeks Worked by Age and Sex</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Looking at Wage Income by Age, Sex, and State</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Last, we can drill down by state.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>For example, let’s look at the distribution of wage income by sex for each of the three states.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>First, do the computations as in the earlier examples:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Now draw the plot:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Wage Income by Age and Sex</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Subsetting an .xdf File into a Data Frame</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>One advantage of storing data in .xdf file is that it is very fast to access a subsample of rows and columns.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>If not too large, the subset of data can be easily read into a data frame and analyzed using any of the numerous functions available for data frames in R.  For example, suppose that we want to perform further analysis on workers in Connecticut who are 50 years old or under:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The resulting data frame has only 60,755 observations, so can be used quite easily in R for analysis.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>For example, use the standard R summary function to compute descriptive statistics:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>This should give the result:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>If you missed the first tutorial, see <bpt id="p1">[</bpt>Practice data import and exploration<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept> for an overview.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>For more advanced lessons, see <bpt id="p1">[</bpt>Write custom chunking algorithms<ept id="p1">](how-to-developer-write-chunking-algorithms.md)</ept>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Machine Learning Server</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>How-to guides in Machine Learning Server</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>RevoScaleR Functions</source>
        </trans-unit></group></body></file></xliff>