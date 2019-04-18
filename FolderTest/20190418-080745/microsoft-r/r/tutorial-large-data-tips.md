<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="tutorial-large-data-tips.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef0690673353135767c73715c397a41efb60f0f665b6502db5b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">3135767c73715c397a41efb60f0f665b6502db5b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\tutorial-large-data-tips.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Tips on Computing with Big Data in R (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Tips on Computing with Big Data in R on Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Tips on Computing with Big Data in R</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Working with very large data sets yields richer insights.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>You can relax assumptions required with smaller data sets and let the data speak for itself.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>But big data also presents problems, especially when it overwhelms hardware resources.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> package that is included with Machine Learning Server provides functions that process in parallel.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Analysis functions are threaded to use multiple cores, and computations can be distributed across multiple computers (nodes) on a cluster or in the cloud.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>In this article, we review some tips for handling big data with R.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Upgrade hardware</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>It is always best to start with the easiest things first, and in some cases getting a better computer, or improving the one you have, can help a great deal.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Usually the most important consideration is memory.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If you are analyzing data that just about fits in R on your current system, getting more memory will not only let you finish your analysis, it is also likely to speed up things by a lot.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This is because your operating system starts to “thrash” when it gets low on memory, removing some things from memory to let others continue to run.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>This can slow your system to a crawl.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Getting more cores can also help, but only up to a point.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>R itself can generally only use one core at a time internally.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>In addition, for many data analysis problems the bottlenecks are disk I/O and the speed of RAM, so efficiently using more than 4 or 8 cores on commodity hardware can be difficult.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Minimize copies of data</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>When working with small data sets, an extra copy is not a problem.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>With big data it can slow the analysis, or even bring it to a screeching halt.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Be aware of the ‘automatic’ copying that occurs in R. For example, if a data frame is passed into a function, a copy is only made if the data frame is modified.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>But if a data frame is put into a list, a copy is automatically made.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>In many of the basic analysis algorithms, such as <bpt id="p1">*</bpt>lm<ept id="p1">*</ept> and <bpt id="p2">*</bpt>glm<ept id="p2">*</ept>, multiple copies of the data set are made as the computations progress, resulting in serious limitations in processing big data sets.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The RevoScaleR analysis functions (for instance, <bpt id="p1">*</bpt>rxSummary<ept id="p1">*</ept>, <bpt id="p2">*</bpt>rxCube<ept id="p2">*</ept>, <bpt id="p3">*</bpt>rxLinMod<ept id="p3">*</ept>, <bpt id="p4">*</bpt>rxLogit,<ept id="p4">*</ept> <bpt id="p5">*</bpt>rxGlm<ept id="p5">*</ept>, <bpt id="p6">*</bpt>rxKmeans<ept id="p6">*</ept>) are all implemented with a focus on efficient use of memory; data is not copied unless absolutely necessary.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The plot below shows an example of how reducing copies of data and tuning algorithms can dramatically increase speed and capacity.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Process data in chunks</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Processing your data a chunk at a time is the key to being able to scale your computations without increasing memory requirements.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>External memory (or “out-of-core”) algorithms don’t require that all of your data be in RAM at one time.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Data is processed a chunk at time, with intermediate results updated for each chunk.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>When all of the data is processed, final results are computed.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The core functions provided with <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> all process data in chunks.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>So, if the number of rows of your data set doubles, you can still perform the same data analyses—it will just take longer, typically scaling linearly with the number of rows.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Your analysis is not bound by memory constraints.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The plot following shows how data chunking allows unlimited rows in limited RAM.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>biglm<ept id="p1">*</ept> package, available on CRAN, also estimates linear and generalized linear models using external memory algorithms, although they are not parallelized.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Compute in parallel</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Using more cores and more computers (nodes) is the key to scaling computations to really big data.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Since data analysis algorithms tend to be I/O bound when data cannot fit into memory, the use of multiple hard drives can be even more important than the use of multiple cores.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> analysis functions are written to automatically compute in parallel on available cores, and can also be used to automatically distribute computations across the nodes of a cluster.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>These functions combine the advantages of external memory algorithms (see <bpt id="p1">[</bpt>Process Data in Chunks<ept id="p1">](#process-data-in-chunks)</ept> preceding) with the advantages of High-Performance Computing.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>That is, these are Parallel External Memory Algorithm’s (PEMAs)—external memory algorithms that have been parallelized.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Such algorithms process data a chunk at a time in parallel, storing intermediate results from each chunk and combining them at the end.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Iterative algorithms repeat this process until convergence is determined.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Any external memory algorithm that is not “inherently sequential” can be parallelized; results for one chunk of data cannot depend upon prior results.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Dependence on data from a prior chunk is OK, but must be handled specially.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The plot following shows an example of how using multiple computers can dramatically increase speed, in this case taking advantage of memory caching on the nodes to achieve super-linear speedups.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Microsofts’ <bpt id="p1">*</bpt>foreach<ept id="p1">*</ept> package, which is open source and available on CRAN, provides easy-to-use tools for executing R functions in parallel, both on a single computer and on multiple computers.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>This is useful for “embarrassingly parallel” types of computations such as simulations, which do not involve lots of data and do not involve communication among the parallel tasks.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Leverage integers</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>In R the two choices for continuous data are <bpt id="p1">*</bpt>numeric<ept id="p1">*</ept>, which is an 8 byte (double) floating point number and <bpt id="p2">*</bpt>integer<ept id="p2">*</ept>, which is a 4-byte integer.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If your data can be stored and processed as an integer, it's more efficient to do so.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>First, it only takes half of the memory.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Second, in some cases integers can be processed much faster than doubles.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>For example, if you have a variable whose values are integral numbers in the range from 1 to 1000 and you want to find the median, it is much faster to count all the occurrences of the integers than it is to sort the variable.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>A tabulation of all the integers, in fact, can be thought of as a way to compress the data with no loss of information.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>The resulting tabulation can be converted into an exact empirical distribution of the data by dividing the counts by the sum of the counts, and all of the empirical quantiles including the median can be obtained from this.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The R function <bpt id="p1">*</bpt>tabulate<ept id="p1">*</ept> can be used for this, and is very fast.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>The following code illustrates this:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>A vector of 100 million doubles is created, with randomized integral values in the range from 1 to 1,000.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Sorting this vector takes about 15 times longer than converting to integers and tabulating, and 25 times longer if the conversion to integers is not included in the timing (this is relevant if you convert to integers once and then operate multiple times on the resulting vector).</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Sometimes decimal numbers can be converted to integers without losing information.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>An example is temperature measurements of the weather, such as 32.7, which can be multiplied by 10 to convert them into integers.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> provides several tools for the fast handling of integral values.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>For instance, in formulas for linear and generalized linear models and other analysis functions, the “F()” function can be used to virtually convert numeric variables into factors, with the levels represented by integers.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxCube<ept id="p1">*</ept> function allows rapid tabulations of factors and their interactions (for example, age by state by income) for arbitrarily large data sets.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Use efficient file formats and data types</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>If your data doesn’t easily fit into memory, you want to store it as a .xdf for fast access from disk.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>If you use appropriate data types, you can save on storage space and access time.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Take advantage of integers, and store data in 32-bit floats not 64-bit doubles.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>A 32-bit float can represent seven decimal digits of precision, which is more than enough for most data, and it takes up half the space of doubles.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>(Save the 64-bit doubles for computations).</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Recognize that relational databases are not always optimal for storing data for analysis.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Even with the best indexing they are typically not designed to provide fast sequential reads of blocks of rows for specified columns, which is the key to fast access to data on disk.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> provides an efficient .xdf file format that provides storage of a wide variety of data types, and is designed for fast sequential reads of blocks of data.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>There are tools for rapidly accessing data in .xdf files from R and for importing data into this format from SAS, SPSS, and text files and SQL Server, Teradata, and ODBC connections.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Load only data you need</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Even though a data set may have many thousands of variables, typically not all of them are being analyzed at one time.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>The .xdf file format is designed for easy access to column-based variables.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>By just reading from disk the actual variables and observations needed for analysis, you can speed up the analysis considerably.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>For example, when estimating a model, only the variables used in the model are read from the .xdf file.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Minimize loops</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>It is well-known that processing data in loops in R can be very slow compared with vector operations.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>For example, if you compare the timings of adding two vectors, one with a loop and the other with a simple vector operation, you find the vector operation to be orders of magnitude faster:</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>On a good laptop, the loop over the data was timed at about 430 seconds, while the vectorized add is barely timetable.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>In R the core operations on vectors are typically written in C, C++ or FORTRAN, and these compiled languages can provide much greater speed for this type of code than can the R interpreter.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Use compiled languages</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>One of the best features of R is its ability to integrate easily with other languages, including C, C++, and FORTRAN.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>You can pass R data objects to other languages, do some computations, and return the results in R data objects.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>It is typically the case that only small portions of an R program can benefit from the speedups that compiled languages like C, C++, and FORTRAN can provide.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Indeed, much of the code in the base and recommended packages in R is written in this way—the bulk of the code is in R but a few core pieces of functionality are written in C, C++, or FORTRAN.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>The type of code that benefits the most from this involves loops over data vectors.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>The package <bpt id="p1">*</bpt>Rcpp,<ept id="p1">*</ept> which is available on CRAN, provides tools that make it very easy to convert R code into C++ and to integrate C and C++ code into R. Before writing code in another language, it pays to do some research to see if the type of functionality you want is already available in R, either in the base and recommended packages or in a 3<bpt id="p2">&lt;sup&gt;</bpt>rd<ept id="p2">&lt;/sup&gt;</ept> party package.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>For example, all of the core algorithms for the <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> package are written in optimized C++ code.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>It also pays to do some research to see if there is publically available code in one of these compiled languages that does what you want.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Use batch processing</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>When working with small data sets, it is common to perform data transformations one at a time.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>For instance, one line of code might create a new variable, and the next line might multiply that variable by 10.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Each of these lines of code processes all rows of the data.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>With a big data set that cannot fit into memory, there can be substantial overhead to making a pass through the data.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>With <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept>’s <bpt id="p2">*</bpt>rxDataStep<ept id="p2">*</ept> function, you can specify multiple data transformations that can be performed in just one pass through the data, processing the data a chunk at a time.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>A little planning ahead can save a lot of time.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Use row-oriented data transforms</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>When data is processed in chunks, basic data transformations for a single row of data should in general not be dependent on values in other rows of data.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>The key is that your transformation expression should give the same result even if only some of the rows of data are in memory at one time.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Data manipulations using lags can be done but require special handling.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Use factor variables with caution</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Categorical or factor variables are extremely useful in visualizing and analyzing big data, but they need to be handled efficiently with big data because they are typically expanded when used in modeling.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>For example, if you use a factor variable with 100 categories as an independent variable in a linear model with <bpt id="p1">*</bpt>lm<ept id="p1">*</ept>, behind the scenes 100 dummy variables are created when estimating the model.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>The analysis modeling functions in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> use special handling of categorical data to minimize the use of memory when processing them; they do not generally need to explicitly create dummy variable to represent factors.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Creating factor variables also often takes more careful handling with big data sets.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>This is because not all of the factor levels may be represented in a single chunk of data.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>For example, if you want to use the <bpt id="p1">*</bpt>factor<ept id="p1">*</ept> function in a data transformation used on chunks of data, you must explicitly specify the levels or you might end up with incompatible factor levels from chunk to chunk.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxImport<ept id="p1">*</ept> and <bpt id="p2">*</bpt>rxFactors<ept id="p2">*</ept> functions in <bpt id="p3">**</bpt>RevoScaleR<ept id="p3">**</ept> provide functionality for creating factor variables in big data sets.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Watch for same-size inputs and outputs</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Most analysis functions return a relatively small object of results that can easily be handled in memory.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>But occasionally, output has the same number of rows as your data, for example, when computing predictions and residuals from a model.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>In order for this to scale, you want the output written out to a file rather than kept in memory.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>For this reason, the <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> modeling functions such as <bpt id="p2">*</bpt>rxLinMod<ept id="p2">*</ept>, <bpt id="p3">*</bpt>rxLogit<ept id="p3">*</ept>, and <bpt id="p4">*</bpt>rxGlm<ept id="p4">*</ept> do not automatically compute predictions and residuals.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxPredict<ept id="p1">*</ept> function provides this functionality and can add predicted values to an existing .xdf file.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Sort with caution</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>When working with small data sets, it is common to sort data at various stages of the analysis process.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Although <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept>’s <bpt id="p2">*</bpt>rxSort<ept id="p2">*</ept> function is very efficient for .xdf files and can handle data sets far too large to fit into memory, sorting is by nature a time-intensive operation, especially on big data.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>One of the major reasons for sorting is to compute medians and other quantiles.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>As noted above in the section on taking advantage of integers, when the data consists of integral values, a tabulation of those values is generally much faster than sorting and gives exact values for all empirical quantiles.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Even when the data is not integral, scaling the data and converting to integers can give very fast and accurate quantiles.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>As an example, if the data consists of floating point values in the range from 0 to 1,000, converting to integers and tabulating will bound the median or any other quantile to within two adjacent integers.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Interpolation within those values can get you closer, as can a small number of additional iterations.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>If the original data falls into some other range (for example, 0 to 1), scaling to a larger range (for example, 0 to 1,000) can accomplish the same thing.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxQuantile<ept id="p1">*</ept> function uses this approach to rapidly compute approximate quantiles for arbitrarily large data.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Another major reason for sorting is to make it easier to compute aggregate statistics by groups.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>If the data are sorted by groups, then contiguous observations can be aggregated.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>However, it is often possible, and much faster, to make a single pass through the original data and to accumulate the desired statistics by group.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>aggregate<ept id="p1">*</ept> function can do this for data that fits into memory, and <bpt id="p2">**</bpt>RevoScaleR<ept id="p2">**</ept>’s <bpt id="p3">*</bpt>rxSummary<ept id="p3">*</ept>, <bpt id="p4">*</bpt>rxCube<ept id="p4">*</ept>, and <bpt id="p5">*</bpt>rxCrossTabs<ept id="p5">*</ept> provide extremely fast ways to do this on large data.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions <bpt id="p2">*</bpt>rxRoc<ept id="p2">*</ept>, and <bpt id="p3">*</bpt>rxLorenz<ept id="p3">*</ept> are other examples of ‘big data’ alternatives to functions that traditionally rely on sorting.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>In summary, by using the tips and tools outlined above you can have the best of both worlds: the ability to rapidly extract information from big data sets using R and the flexibility and power of the R language to manipulate and graph this information.</source>
        </trans-unit></group></body></file></xliff>