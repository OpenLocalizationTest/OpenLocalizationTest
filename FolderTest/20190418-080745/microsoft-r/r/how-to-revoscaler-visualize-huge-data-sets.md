<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-visualize-huge-data-sets.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335bfbd00034f55811cf22bc4eb2c143b0349d32ed8.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">bfbd00034f55811cf22bc4eb2c143b0349d32ed8</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-visualize-huge-data-sets.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Visualizing Huge Data Sets using RevoScaleR (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Visualizing huge data sets with an example from the U.S. Census.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Visualizing Huge Data Sets: An Example from the U.S. Census</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>By combining the power and flexibility of the open-source R language with the fast computations and rapid access to huge datasets provided by RevoScaleR, it is easy and efficient to not only do fine-grained calculations “on the fly” for plotting, but to visually drill down into these patterns.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>This example focuses on a basic demographic pattern: in general, more boys than girls are born and the death rate is higher for males at every age.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>So, typically we observe a decline in the ratio of males to females as age increases.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Important!<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Since Microsoft R Client can only process datasets that fit into the available memory,  chunking is not supported.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>When run locally with R Client, the <ph id="ph1">`blocksPerRead`</ph> argument is ignored and all data must be read into memory.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>When working with Big Data, this may result in memory exhaustion.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>You can work around this limitation when you push the compute context to a Machine Learning Server instance.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Examining the Data</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>We can examine this pattern in the United States using the 5% Public Use Microdata Sample (PUMS) of the 2000 United States Census, stored in an .xdf file of about 12 gigabytes.[1] Using the rxGetInfo function, we can get a quick summary of the data set:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>It contains over 14 million rows, has 264 variables, and has been stored in 98 data blocks in the .xdf file.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>First let’s use the rxCube function to count the number of males and females for each age, using the weighting variable provided by the census bureau.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>We’ll read in the data in chunks of 15 blocks, or about 2 million rows at a time.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more...<ept id="p1">](#chunking)</ept></source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>In the computation, we’re treating age as a categorical variable so we’ll get counts for each age.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Since we’ll be converting this factor data back to integers on a regular basis, we’ll write a function to do the conversion:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>We can now write a simple function in R to take the counts information returned from rxCube and do the arithmetic to compute the sex ratio for each age.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>It returns a data frame with the counts for Males and Females, the SexRatio, and age for all groups in which there are positive counts for both Males and Females.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Ages over 90 are also excluded.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Let’s use that function and then plot the results:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The graph shows the expected downward trend at the younger ages.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>But look at what happens at the age of 65!</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>At the age of 65, there are suddenly about 12 men for every 10 women.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>We can quickly drill down, and do the same computation for each region:</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>We see the unlikely “spike” at age 65 in all regions:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Let’s try looking at ethnicity, comparing whites with non-whites.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>There are interesting differences between the two groups, but again there is the familiar spike at age 65 in both cases.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>How about comparing married people with those not living with a spouse?</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>We can create a temporary variable using the transform argument to do this computation:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>First, notice that the spike at age 65 is absent for unmarried people.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>But also look at the very different trends.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>For married 20 year-olds, there are about 5 men for every 10 women, but for married 60 year-olds, there would be about 11 men for every 10 women.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>This may at first seem counter-intuitive, but it’s consistent with the notion that men tend to marry younger women.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Let’s explore that next.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Extending the Analysis</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>We’d like to compare the ages of men with ages of their wives.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>This is more complicated than the earlier computations because the spouse’s age is stored in a different record in the data file.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>To handle this, we’ll create a new data set using RevoScaleR’s data step functionality with a transformation function.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>This transformation function makes use of RevoScaleR’s ability to go back and read additional rows from an .xdf file as it is reading through it in chunks.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>It also uses internal variables that are provided inside a transformation function: <bpt id="p1">*</bpt>.rxStartRow<ept id="p1">*</ept>, which is the row number from the original data set for the first row of the chunk of data being processed; <bpt id="p2">*</bpt>.rxReadFileName<ept id="p2">*</ept> gives the name of the file being read.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>It first checks the spouse location for the relative position of the spouse in the data set.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>It then determines which of the observations have spouses in the previous, current, or next chunk of data.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Then, in each of the three cases, it looks up the spouse information and adds it to the original observation.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>We can test the transform function by reading in a small number of rows of data.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>First we will read in a chunk that has a spouse in the previous block and a spouse in the next block, and call the transform function.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>We will repeat this, expanding the chunk of data to include both spouses, and double check to make sure the results are the same for the equivalent rows:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>To create the new data set, we’ll use the transformation function with <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Observations for males living with female spouses will be written to a new data .xdf file named <bpt id="p1">*</bpt>spouseCensus2000.xdf<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>It will include information about the age of their spouse.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more...<ept id="p1">](#chunking)</ept></source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Now for each husband age we can compute the distribution of spouse age.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Then, after converting age back to an integer, we can plot the age difference by age of husband:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Beginning at ages in the early 20’s, men tend to be married to younger women.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>The age difference increases as men get older.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>But beginning at age 65, our smooth trend stops and we see more erratic behavior, suggesting that our data has misinformation about ages of spouses within households at age 65 and above.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>With our new data set we can also calculate the counts for each combination of husband’s age and wife’s age:</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>A level plot is a good way to visualize the results, where the color indicates the count of each category of combination of husband’s and wife’s age.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>In the level plot, there is a very clear pattern with the mode of the relative age of wife dropping gradually as the age of husband increases.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Now, repeat with husbands aged 60 to 80.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>This shows a different story.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Notice that there are very few men in the 60 to 80 age range married to 65 year-old women, and in particular, there are very few 65-year-old men married to 65-year-old women.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>To examine this further, we can look at line plots of the distributions of wife’s ages for men ages 62 to 67:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The blue lines show husbands ages 62 through 64.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The mode of the wife’s age is a couple of years younger than the husband, and we have a reasonable looking distribution in both tails.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>But starting at age 65, with the red lines, we have a very different pattern.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>It appears that when husbands reach the age of 65 they begin to leave (or lose) their 65-year-old wives in droves – and marry older women.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>This certainly makes one suspicious of the data.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>In fact, it turns out the aberration in the data was introduced by disclosure avoidance techniques applied to the data by the census bureau.</source>
        </trans-unit></group></body></file></xliff>