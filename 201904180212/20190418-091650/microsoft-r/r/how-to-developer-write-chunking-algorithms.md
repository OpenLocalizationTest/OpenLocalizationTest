<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-developer-write-chunking-algorithms.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b456937e6a4e3ae1d972e542b51da28c3353f7e686.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">56937e6a4e3ae1d972e542b51da28c3353f7e686</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-developer-write-chunking-algorithms.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Write custom chunking algorithms in ScaleR (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn how to use rxDataStep to apply arbitrary R functions on chunked data.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Write custom chunking algorithms using rxDataStep in RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Scalability in RevoScaleR is based on chunking or external memory algorithms that can analyze chunks of data in parallel and then combine intermediate results into a single analysis.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Because of the chunking algorithms, it's possible to analyze huge datasets that vastly exceed the memory capacity of any one machine.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>All of the main analysis functions in RevoScaleR (<bpt id="p1">*</bpt>rxSummary<ept id="p1">*</ept>, <bpt id="p2">*</bpt>rxLinMod<ept id="p2">*</ept>, <bpt id="p3">*</bpt>rxLogit<ept id="p3">*</ept>, <bpt id="p4">*</bpt>rxGlm<ept id="p4">*</ept>, <bpt id="p5">*</bpt>rxCube<ept id="p5">*</ept>, <bpt id="p6">*</bpt>rxCrossTabs<ept id="p6">*</ept>, <bpt id="p7">*</bpt>rxCovCor<ept id="p7">*</ept>, <bpt id="p8">*</bpt>rxKmeans<ept id="p8">*</ept>, <bpt id="p9">*</bpt>rxDTree<ept id="p9">*</ept>, <bpt id="p10">*</bpt>rxBTrees<ept id="p10">*</ept>, <bpt id="p11">*</bpt>rxNaiveBayes<ept id="p11">*</ept>, and <bpt id="p12">*</bpt>rxDForest<ept id="p12">*</ept>) use chunking or external memory algorithms.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>However, for scenarios where specialized behaviors are needed, you can create a custom chunking algorithms using the <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept> function to automatically chunk through your data set and apply arbitrary R functions to process your data.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>In this article, you'll step through an example that teaches a simple chunking algorithm for tabulating data implemented using <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A more realistic tabulation approach is to use the <bpt id="p1">*</bpt>rxCrossTabs<ept id="p1">*</ept> or <bpt id="p2">*</bpt>rxCube<ept id="p2">*</ept> functions, but since <bpt id="p3">*</bpt>rxDataStep<ept id="p3">*</ept> is simpler, it's a better choice for instruction.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept> does not provide sufficient customization, you can build a custom parallel external memory algorithm from the ground up using functions in the <bpt id="p2">**</bpt>RevoPemaR<ept id="p2">**</ept> package.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>How to use the RevoPemaR library in Machine Learning Server<ept id="p1">](how-to-developer-pemar.md)</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Sample data for this example is the <bpt id="p1">*</bpt>AirlineDemoSmall.xdf<ept id="p1">*</ept> file with a local compute context.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>For instructions on how to import this data set, see the tutorial in <bpt id="p1">[</bpt>Practice data import and exploration<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Chunking is supported on Machine Learning Server, but not on the free R Client.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Because the dataset is small enough to reside in memory on most computers, most systems succeed in running this example locally.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>however, if the data does not fit in memory, you will need to use Machine Learning Server instead.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>About chunking algorithms</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>An updating algorithm takes a given set of values and a chunk of data, and then outputs a revised set of values cumulative for all chunks.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The simplest example is an updating sum: sum is computed for the first chunk, followed by a second chunk, which each successive chunk contributing to a revised value until reaching the cumulative sum.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Updating algorithms perform four main tasks:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Initialization: declare and initialize variables needed in the computation.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>ProcessData: for each block, perform calculations on the data in the block.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>UpdateResults: combine all of the results of the ProcessData step.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>ProcessResults: when results from all blocks have been combined, do any final computations.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>In this example, no initialization is required.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Example: rxDataStep and sample airline data</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The ProcessData step is performed within a <bpt id="p1">*</bpt>transformFunc<ept id="p1">*</ept> called by <bpt id="p2">*</bpt>rxDataStep<ept id="p2">*</ept> for each chunk of data.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>In this case we begin with a simple call to the <bpt id="p1">*</bpt>table<ept id="p1">*</ept> function after converting the chunk to a data frame.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The results are then converted back to a data frame with a single row, which will be appended to a data set on disk.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>So, the call to <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept> reads in the data chunk-by-chunk and creates a new summary data set where each row represents the “intermediate results” of a chunk.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>AggregateResults<ept id="p1">*</ept> function shown below combines the <bpt id="p2">*</bpt>UpdateResults<ept id="p2">*</ept> and <bpt id="p3">*</bpt>ProcessResults<ept id="p3">*</ept> tasks.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The summary data set is simply read into memory and the columns are summed.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>To try this out, create a new script <bpt id="p1">*</bpt>chunkTable.R<ept id="p1">*</ept> with the following contents:</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Note that the <ph id="ph1">`blocksPerRead`</ph> argument is ignored if this script runs locally using R Client.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Since Microsoft R Client can only process datasets that fit into the available memory, chunking is not supported in R Client.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>When run locally with R Client, all data must be read into memory.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>You can work around this limitation when you push the compute context to a <bpt id="p1">[</bpt>Machine Learning Server instance<ept id="p1">](../what-is-machine-learning-server.md)</ept>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>To test the function, use the sample data <bpt id="p1">*</bpt>AirlineDemoSmall.xdf<ept id="p1">*</ept> file with a local compute context.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>For more information, see the tutorial in <bpt id="p1">[</bpt>Practice data import and exploration<ept id="p1">](tutorial-revoscaler-data-import-transform.md)</ept>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>We’ll call our new <bpt id="p1">*</bpt>chunkTable<ept id="p1">*</ept> function, processing 1 block at a time so we can take a look at the intermediate results:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>You will see the following results:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>To see the intermediate results, we can read the data set into memory:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>And to delete the intermediate results file:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>This article provides an example of a simple chunking algorithm for tabulating data using <bpt id="p1">*</bpt>rxDataStep<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>In practice, you might want to use the <bpt id="p1">*</bpt>rxCrossTabs<ept id="p1">*</ept> or <bpt id="p2">*</bpt>rxCube<ept id="p2">*</ept> functions.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>rxCrossTabs<ept id="p1">](~/r-reference/revoscaler/rxcrosstabs.md)</ept> and <bpt id="p2">[</bpt>rxCube<ept id="p2">](~/r-reference/revoscaler/rxcube.md)</ept>, respectively.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How-to guides in Machine Learning Server<ept id="p1">](how-to-introduction.md)</ept></source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR Functions<ept id="p1">](~/r-reference/revoscaler/revoscaler.md)</ept></source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Analyze large data with ScaleR<ept id="p1">](tutorial-revoscaler-large-data-airline.md)</ept></source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Census data example for analyzing large data<ept id="p1">](tutorial-revoscaler-large-data-census.md)</ept></source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Loan data example for analyzing large data<ept id="p1">](tutorial-revoscaler-large-data-loan.md)</ept></source>
        </trans-unit></group></body></file></xliff>