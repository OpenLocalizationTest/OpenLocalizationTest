<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-data-sort.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc775054bc56365345002ef407e446f332f1c61b0ce716.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">54bc56365345002ef407e446f332f1c61b0ce716</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-data-sort.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Sort data in RevoScaleR using rxSort (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to sort data in a data frame or XDF file with the RevoScaleR rxSort function.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to sort data using rxSort in RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Many analysis and plotting algorithms require as a first step that the data be sorted.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Sorting a massive data set is both memory-intensive and time-consuming, but the <bpt id="p1">**</bpt>rxSort<ept id="p1">**</ept> function provides an efficient solution.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rxSort<ept id="p1">**</ept> function allows you to sort by one or many keys.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">*</bpt>stable<ept id="p1">*</ept> sorting routine is used, so that, in the case of ties, remaining columns are left in the same order as they were in the original data set.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>As a simple example, we can sort the census worker data by <bpt id="p1">*</bpt>age<ept id="p1">*</ept> and <bpt id="p2">*</bpt>incwage<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>We will sort first by <bpt id="p1">*</bpt>age<ept id="p1">*</ept>, using the default increasing sort, and then by <bpt id="p2">*</bpt>incwage<ept id="p2">*</ept>, which we will sort in decreasing order:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The first few lines of the sorted file can be viewed as follows:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If the sort keys contain missing values, you can use the <bpt id="p1">*</bpt>missingsLow<ept id="p1">*</ept> flag to specify whether they are sorted as low values (<bpt id="p2">*</bpt>missingsLow=TRUE<ept id="p2">*</ept>, the default) or high values (<bpt id="p3">*</bpt>missingsLow=FALSE<ept id="p3">*</ept>).</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Remove duplicates during sort</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>In many situations, you are sorting a large data set by a particular key, for example, userID, but are looking for a sorted list of unique userIDs.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>removeDupKeys<ept id="p1">*</ept> argument to <bpt id="p2">**</bpt>rxSort<ept id="p2">**</ept> allows you to remove the duplicate entries from a sorted list.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>This argument is supported only for <bpt id="p1">*</bpt>type="auto"<ept id="p1">*</ept> and <bpt id="p2">*</bpt>type="mergeSort"<ept id="p2">*</ept>; it is ignored for <bpt id="p3">*</bpt>type="varByVar"<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>When you use <bpt id="p1">*</bpt>removeDupKeys=TRUE<ept id="p1">*</ept>, the first record containing a unique combination of the <bpt id="p2">*</bpt>sortByVars<ept id="p2">*</ept> is retained; subsequent matching records are omitted from the sorted results, but, if desired, a count of the matching records is maintained in a new <bpt id="p3">*</bpt>dupFreqVar<ept id="p3">*</ept> output column.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>For example, the following artificial data set simulates a small amount of transaction data, with a user name, a state, and a transaction amount.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>When we sort by the variables <bpt id="p1">*</bpt>users<ept id="p1">*</ept> and <bpt id="p2">*</bpt>state<ept id="p2">*</ept> and specify <bpt id="p3">*</bpt>removeDupKeys=TRUE<ept id="p3">*</ept>, the <bpt id="p4">*</bpt>transAmt<ept id="p4">*</ept> shown for duplicate entries is the transaction amount for the <bpt id="p5">*</bpt>first<ept id="p5">*</ept> transaction encountered:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Removing duplicates can be a useful way to reduce the size of a data set without losing information of interest.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>For example, consider an analysis of using data from the sample <bpt id="p1">*</bpt>AirlineDemoSmall<ept id="p1">*</ept> xdf file.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>It has 600,000 observations and contains the variables <bpt id="p1">*</bpt>DayOfWeek<ept id="p1">*</ept>, <bpt id="p2">*</bpt>CRSDepTime<ept id="p2">*</ept>, and <bpt id="p3">*</bpt>ArrDelay<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>We can create a smaller data set reducing the number of observations, and adding a variable that contains the frequency of the duplicated observation.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The new data file contains about 1/3 of the observations and one additional variable:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>By using the frequency weights argument, we can use many of the RevoScaleR analysis functions on this smaller data set and get same results as we would using the full data set.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>For example, a linear model for Arrival Delay can be specified as follows, using the <bpt id="p1">*</bpt>fweights<ept id="p1">*</ept> argument:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Using the full data set, we get the following results:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The rxQuantile Function and the Five-Number Summary</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Sorting data is, in the general case, a prerequisite to finding exact quantiles, including medians.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>However, it is possible to compute approximate quantiles by counting binned data then computing a linear interpolation of the empirical cdf.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If the data are integers, or can be converted to integers by exact multiplication, and integral bins are used, the computation is exact.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The RevoScaleR function rxQuantile does this computation, and by default returns an approximate five-number summary:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept> <bpt id="p2">[</bpt>Install Machine Learning Server on Windows<ept id="p2">](../install/machine-learning-server-windows-install.md)</ept></source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server on Linux</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server on Hadoop</source>
        </trans-unit></group></body></file></xliff>