<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-data-split.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750679c94333cef092aa735139002722720a2f03964.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">679c94333cef092aa735139002722720a2f03964</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-data-split.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Split data into multiple files using rxSplit (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Split data to train and test a model, or subdivide a large dataset into smaller files.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to split datasets for model training and testing</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>This article explains how to split a dataset in two for training and testing a model, but the same technique applies for any use case where subdividing data is required.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>For example, to manually partition data across multiple nodes in a cluster, you could use the functions and workflow described in this article for that purpose.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Functions for splitting datasets</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>R developers, use <bpt id="p1">[</bpt>rxSplit (RevoScaleR)<ept id="p1">](../r-reference/revoscaler/rxsplitxdf.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The following example is from <bpt id="p1">[</bpt>Run R code in R Client and Machine Learning Server<ept id="p1">](quickstart-run-r-code.md)</ept> quickstart.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Python developers, we recommend <bpt id="p1">[</bpt>sci-kit<ept id="p1">](http://scikit-learn.org/stable/)</ept> methods for splitting data, as demonstrated in the <bpt id="p2">[</bpt>Example of binary classification with the microsoftml Python package<ept id="p2">](../python/quickstart-binary-classification-with-microsoftml.md)</ept> quickstart.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Create a distributed dataset on HDFS with rxSplit</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>In HDFS, the data is distributed automatically, typically to a subset of the nodes, and the computations are also distributed to the nodes containing the required data.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>To work with data on HDFS, we recommend <bpt id="p1">*</bpt>composite<ept id="p1">*</ept> .xdf files, which are specialized files designed to be managed by HDFS.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Import HDFS &gt; Write a composite XDF<ept id="p1">](how-to-revoscaler-data-hdfs.md#write-a-composite-xdf)</ept>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>For some computations, such as those involving distributed prediction, it is most efficient to perform the computations on a distributed data set, one in which each node sees only the data it is supposed to work on.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>You can split an .xdf file into portions suitable for distribution using the function <bpt id="p1">*</bpt>rxSplit<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>For example, to split the large airline data into five files for distribution on a five node cluster, you could use <bpt id="p1">*</bpt>rxSplit<ept id="p1">*</ept> as follows:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>By default, <bpt id="p1">*</bpt>rxSplit<ept id="p1">*</ept> simply appends a number in the sequence from 1 to <bpt id="p2">*</bpt>numOutFiles<ept id="p2">*</ept> to the base file name to create the new file names, and in this case the resulting file names, for example, “AirlineData87to081.xdf”, are a bit confusing.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>You can exercise greater control over the output file names by using the <bpt id="p1">*</bpt>outFilesBase<ept id="p1">*</ept> and <bpt id="p2">*</bpt>outFilesSuffixes<ept id="p2">*</ept> arguments.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>With <bpt id="p1">*</bpt>outFilesBase<ept id="p1">*</ept>, you can specify either a single character string to be used for all files or a character vector the same length as the desired number of files.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The latter option is useful, for example, if you would like to create four files with the same file name, but different paths:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>This creates the four directories C:/compute10, etc., and creates a file named “DistAirlineData.xdf” in each directory.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>You will want to do something like this when using distributed data with the standard <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> analysis functions such as rxLinMod and rxLogit.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>You can supply the <bpt id="p1">*</bpt>outFilesSuffixes<ept id="p1">*</ept> arguments to exercise greater control over what is appended to the end of each file.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Returning to our first example, we can add a hyphen between our base file name and the sequence 1 to 5 using <bpt id="p1">*</bpt>outFilesSuffixes<ept id="p1">*</ept> as follows:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The splitBy argument specifies whether to split your data file row-by-row or block-by-block.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The default is <bpt id="p1">*</bpt>splitBy="rows"<ept id="p1">*</ept>, to split by blocks instead, specify <bpt id="p2">*</bpt>splitBy="blocks"<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>splitBy<ept id="p1">*</ept> argument is ignored if you also specify the <bpt id="p2">*</bpt>splitByFactor<ept id="p2">*</ept> argument as a character string representing a valid factor variable.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>In this case, one file is created per level of the factor variable.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxSplit<ept id="p1">*</ept> function works in the local compute context only; once you’ve split the file you need to distribute the resulting files to the individual nodes using the techniques of the previous sections.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>You should then specify a compute context with the flag <bpt id="p1">*</bpt>dataDistType<ept id="p1">*</ept> set to <bpt id="p2">*</bpt>"split"<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Once you have done this, HPA functions such as <bpt id="p1">*</bpt>rxLinMod<ept id="p1">*</ept> will know to split their computations according to the data on each node.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Data Analysis with Split Data on HDFS</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>To use split data in your distributed data analysis, the first step is generally to split the data using rxSplit, which as we have seen is a local operation.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>So the next step is then to copy the split data to your cluster nodes.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Create an XDF source object:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Connect to the cluster:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Set the compute context to your cluster:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>We are now ready to fit a simple linear model:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>When we print the object, we see that we obtain the same model as when computed with the full data on all nodes:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>With data in the .xdf format, you have your choice of using the full data set or a split data set on each node.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>For other data sources, you must have the data split across the nodes.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>For example, the airline data’s original form is a set of .csv files, one for each year from 1987 to 2008.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>(Additional years are now available, but have not been included in our big airline data.) If we copy the year 2000 data to compute10, the year 2001 data to compute11, the year 2002 data to compute12, and the year 2003 data to compute13 with the file name SplitAirline.csv, we can analyze the data as follows:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>We can then perform an rxLogit model to classify flights as “Late” as follows:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Distributed Predictions on HDFS</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>You can predict (or score) from a fitted model in a distributed context, but in this case, your data <bpt id="p1">*</bpt>must<ept id="p1">*</ept> be split.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>For example, if we fit our distributed linear model with <bpt id="p1">*</bpt>covCoef=TRUE<ept id="p1">*</ept> (and <bpt id="p2">*</bpt>cube=FALSE<ept id="p2">*</ept>), we can compute standard errors for the predicted values:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if script runs locally using R Client.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The output data is also split, in this case holding fitted values, residuals, and standard errors for the predicted values.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Split Training and Test Datasets on HDFS</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>One common technique for validating models is to break the data to be analyzed into training and test subsamples, then fit the model using the training data and score it by predicting on the test data.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Once you have split your original data set onto your cluster nodes, you can split the data on the individual nodes by calling rxSplit again within a call to rxExec.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If you specify the RNGseed argument to rxExec (see <bpt id="p1">[</bpt>Parallel Random Number Generation<ept id="p1">](how-to-revoscaler-distributed-computing-parallel-jobs.md#parallel-random-number-generation)</ept>), the split becomes reproducible:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The result is two new data files, airlineData.testSplitVar.Train.xdf and airlineData.testSplitVar.Test.xdf, on each of your nodes.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>We can fit the model to the training data and predict with the test data as follows:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if script runs locally using R Client.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Perform Data Operations on Each Node</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>To create or modify data on each node, use the data manipulation functions within rxExec.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>For example, suppose that after looking at the airline data we decide to create a “cleaner” version of it by keeping only the flights where: there is information on the arrival delay,  the flight did not depart more than one hour early, and the actual and scheduled flight time is positive.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>We can put a call to <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept> (and any other code we want processed) into a function to be processed on each node via <bpt id="p2">*</bpt>rxExec<ept id="p2">*</ept>:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept> <bpt id="p2">[</bpt>Install Machine Learning Server on Hadoop<ept id="p2">](../install/machine-learning-server-hadoop-install.md)</ept></source>
        </trans-unit></group></body></file></xliff>