<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-cluster.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3ec71105293da7dc8e70a2c93ec2a7dd8502fd2a66.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">c71105293da7dc8e70a2c93ec2a7dd8502fd2a66</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-cluster.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Cluster classification using RevoScaleR (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>k-means clustering with RevoScaleR.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Cluster classification in RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Clustering<ept id="p1">*</ept> is the general name for any of a large number of classification techniques that involve assigning observations to membership in one of two or more clusters on the basis of some distance metric.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>K-means Clustering</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>K-means clustering is a classification technique that groups observations of numeric data using one of several <bpt id="p1">*</bpt>iterative relocation<ept id="p1">*</ept> algorithms.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Starting from some initial classification, which may be random, points are moved from cluster to another so as to minimize sums of squares.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>In RevoScaleR, the algorithm used is that of Lloyd.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>To perform k-means clustering with RevoScaleR, use the <bpt id="p1">*</bpt>rxKmeans<ept id="p1">*</ept> function.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Clustering the Airline Data</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>As a first example of k-means clustering, we will cluster the arrival delay and scheduled departure time in the airline data 7% subsample.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>To start, we extract variables of interest into a new working data set to which we are writing additional information:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>We specify the variables to cluster as a formula, and specify the number of clusters we’d like.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Initial centers for these clusters are then chosen at random.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>This produces the following output (because the initial centers are chosen at random, your output will probably look different):</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The value returned by <bpt id="p1">*</bpt>rxKmeans<ept id="p1">*</ept> is a list similar to the list returned by the standard R kmeans function.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The printed output shows a subset of this information, including the number of valid and missing observations, the cluster sizes, the cluster centers, and the within-cluster sums of squares.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The cluster membership component is returned if the input is a data frame, but if the input is a .xdf file, cluster membership is returned only if <bpt id="p1">*</bpt>outFile<ept id="p1">*</ept> is specified, in which case it is returned not as part of the return object, but as a column in the specified file.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>In our example, we specified an <bpt id="p1">*</bpt>outFile<ept id="p1">*</ept>, and we see the cluster membership variable when we look at the file with <bpt id="p2">*</bpt>rxGetInfo<ept id="p2">*</ept>:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Using the Cluster Membership Information</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>A common follow-up to clustering is to use the cluster membership information to see whether a given model varies appreciably from cluster to cluster.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Since we can use the <bpt id="p1">*</bpt>rowSelection<ept id="p1">*</ept> argument to extract a single cluster on the fly, there is no need to sort the data first.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>As an example, we fit our original linear model of ArrDelay by DayOfWeek for two of the clusters:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Looking at the summary for <bpt id="p1">*</bpt>clust1Lm<ept id="p1">*</ept> shows the following:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Similarly, the summary for clust5Lm shows the following:</source>
        </trans-unit></group></body></file></xliff>