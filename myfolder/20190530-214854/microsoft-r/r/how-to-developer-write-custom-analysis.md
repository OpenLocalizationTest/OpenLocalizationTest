<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-developer-write-custom-analysis.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e4c66657673656924289028178926f6f2354e0037.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">4c66657673656924289028178926f6f2354e0037</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-developer-write-custom-analysis.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Writing custom analyses for large data sets using RevoScaleR (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Get started with custom analysis of big data using RevoScaleR functions in Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Writing custom analyses for large data sets in RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>This article explains how to use RevoScaleR to get data one chunk at a time, and then perform a custom analysis.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>There are four basic steps in the analysis:</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Initialize results</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Process data, a chunk at a time</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Update results, after processing each chunk</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Final processing of results</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Sample data is the airline flight delay dataset.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>For information on how to obtain this data, see <bpt id="p1">[</bpt>Sample data for RevoScaleR and revoscalepy<ept id="p1">](sample-built-in-data.md)</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Tutorial walkthrough: Custom chunk operations</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>For illustrative purposes, suppose that we want to compute the average arrival delay for flights that leave in the morning, afternoon, and evening.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>For each chunk of data, we need to compute the sum of arrival delay for each of the three time intervals, as well as the counts for each interval.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>We will accumulate these results in a list of “transformObjects” containing the six values.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>At the end after processing all the data, we will divide the accumulated totals by the accumulated counts to compute the averages.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Most of the work takes place within a transformation function, which processes the data and updates the results for each chunk of data that is read in.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>We use the .rxGet and .rxSet functions to store information from one pass of the data to the next.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Because we are processing data and not creating newly transformed variables, we return NULL from the function:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Our transformation object values are initialized in a list passed into rxDataStep.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>We also use the argument <bpt id="p1">*</bpt>returnTransformObjects<ept id="p1">*</ept> to indicate that we want updated values of the <bpt id="p2">*</bpt>transformObjects<ept id="p2">*</ept> returned rather than a transformed data set:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The rxDataStep function will automatically chunk through the data for us.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>All we need to do is process the final results:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The calculated results are:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>In this case we can check our results by using the <bpt id="p1">*</bpt>rowSelection<ept id="p1">*</ept> argument in <bpt id="p2">*</bpt>rxSummary<ept id="p2">*</ept>:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Machine Learning Server</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>How-to guides in Machine Learning Server</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>RevoScaleR Functions</source>
        </trans-unit></group></body></file></xliff>