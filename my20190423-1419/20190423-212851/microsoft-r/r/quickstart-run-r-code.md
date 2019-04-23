<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="quickstart-run-r-code.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a9ce7e60deb8d856bc9eb6ae1d5e2ce5bf43c215e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9ce7e60deb8d856bc9eb6ae1d5e2ce5bf43c215e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\quickstart-run-r-code.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Quick Start for Microsoft R Client &amp; Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Microsoft R Client quickstart</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Client, quickstart, Microsoft R Client, Introduction, Get Started with R Client</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Quickstart: Run R code in R Client and Machine Learning Server</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Applies to: R Client 3.x, R Server 9.x, Machine Learning Server 9.x</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Learn how to predict flight delays in R locally using R Client or Machine Learning Server.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The example in this article uses historical on-time performance and weather data to predict whether the arrival of a scheduled passenger flight is delayed by more than 15 minutes.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>We approach this problem as a classification problem, predicting two classes -- whether the flight is delayed or on-time.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>In machine learning and statistics, classification is the task of identifying the class or category to which an observation belongs based on a training dataset containing observations with known categories.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Classification is generally a supervised learning problem.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>This quick start is a binary classification task with two classes.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>In this example, you train a model using many examples from historic flight data, along with an outcome measure that indicates the appropriate category or class for each example.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The two classes are '0' for on-time flights and '1' for flights delayed longer than 15 minutes.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Time estimate</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If you have completed the prerequisites, this task takes approximately 10 minutes to complete.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>This quickstart assumes that you have:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>An installed instance of Microsoft R Client or Machine Learning Server</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>R running on the command line or in an R integrated development environment (IDE).</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Read the article <bpt id="p1">[</bpt>Get Started with Microsoft R Client<ept id="p1">](../r-client-get-started.md)</ept> for more information.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>An internet connection to get <bpt id="p1">[</bpt>sample data in the RTVS GitHub repository<ept id="p1">](https://github.com/Microsoft/RTVS-docs/tree/master/examples/MRS_and_Machine_Learning/Datasets)</ept>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Example code</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>This article walks through some R code you can use to predict whether a flight will be delayed.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Here is the entire R code for the example that we walk through in the sections.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Step 1.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Prepare and import data</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Initialize some variables to specify the data sets.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Create a temporary directory to store the intermediate XDF files.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The External Data Frame (XDF) file format is a high-performance, binary file format for storing big data sets for use with RevoScaleR.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>This file format has an R interface and optimizes rows and columns for faster processing and analysis.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Learn more</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Import the flight data.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Review the first six rows of flight data.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Summarize the flight data.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Import the weather data.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Review the variable information for the weather data.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Step 2.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Pre-process data</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Rename some column names in the weather data to prepare it for merging.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Concatenate/Merge flight records and weather data.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Join flight records and weather data at origin of the flight <ph id="ph1">`OriginAirportID`</ph>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Join flight records and weather data using the destination of the flight <ph id="ph1">`DestAirportID`</ph>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Call the rxFactors() function to convert <ph id="ph1">`OriginAirportID`</ph> and <ph id="ph2">`DestAirportID`</ph> as categorical.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Step 3.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Prepare training and test datasets</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Randomly split data (80% for training, 20% for testing).</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Point to the XDF files for each set.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Step 4.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Predict using logistic regression</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Choose and apply the Logistic Regression learning algorithm.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Predict using new data.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Step 5.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Predict using decision tree</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Choose and apply the Decision Tree learning algorithm.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Predict using new data.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Now that you've tried this example, you can start developing your own solutions using the <bpt id="p1">[</bpt><ph id="ph1">`RevoScaleR` </ph>R package functions<ept id="p1">](~/r-reference/revoscaler/revoscaler.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`MicrosoftML`</ph> R package functions<ept id="p2">](../r-reference/microsoftml/microsoftml-package.md)</ept>, and APIs.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>When ready, you can run that R code using R Client or even send those R commands to a <bpt id="p1">[</bpt>remote R Server<ept id="p1">](how-to-execute-code-remotely.md)</ept> for execution.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Learn More</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>You can learn more with these guides:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Overview of Machine Learning Server</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Overview of Microsoft R Client</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>How-to guides in Machine Learning Server</source>
        </trans-unit></group></body></file></xliff>