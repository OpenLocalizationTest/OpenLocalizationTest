<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="tutorial-rxexecby.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f8e4fe607266b6ba1b2d67ebe12e768bbd6293baf.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8e4fe607266b6ba1b2d67ebe12e768bbd6293baf</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\tutorial-rxexecby.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxExecBy example: parallel processing on partitioned data in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Parallel processing of partitioned data with the RevoScaleR function rxExecBy</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>RevoScaleR rxExecBy parallel processing example</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Many of our enterprise customers don’t have a "big data, big model" problem.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>They have a "small data, many models" problem, where there is a need to train separate models such as ARIMA (for time-series forecasting) or boosted trees over a large number of small data sets.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>The trained models could be used for time-series predictions, or to score fresh data for each small data partition.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Typical examples include time-series forecasting of smart meters for households, revenue forecasting for product lines, or loan approvals for bank branches.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The new <ph id="ph1">`rxExecBy`</ph> function in <bpt id="p1">[</bpt>RevoScaleR<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept> is designed for use cases calling for high-volume parallel processing over a large number of small data sets.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Given this data profile, you can use <ph id="ph1">`rxExecBy`</ph> to read in the data, partition the data, and then call a function to iterate over each partition in parallel.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>How to use rxExecBy</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxExecBy`</ph> takes four inputs and produces an output for each partition, in whatever product the user-defined function computes.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The function can be almost any user-defined or analytical or statistical function from the collection of Machine Learning Server packages, able to <bpt id="p1">[</bpt>execute jobs in parallel<ept id="p1">](how-to-revoscaler-distributed-computing-parallel-jobs.md)</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The data sets can be .csv files loaded via <ph id="ph1">`RxTextData`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The parallel processing occurs when you run the <ph id="ph1">`rxExecby`</ph> script on a platform offering distributed computing.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>In this case, either Spark or SQL Server Machine Learning Services.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Input criteria</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Method</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Data sources</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>RxTextData, RxXdfData, RxHiveData, RxParquetData, RxOrcData, rxSparkDataOps</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Keys</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Choose one or more fields used to group data, such as an ID.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Compute context</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>rxSpark, rxInSQLServer</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>User-defined functions</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>rxLinMod, rxLogit, rxPredict, rxGlm, rxCovCor, rxDtree, and others</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Sample code using Airline data set</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>To demonstrate <ph id="ph1">`rxExecBy`</ph>, we will use the airline dataset with flight delay data values for multiple airports, over multiple years.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>In just the small dataset alone, there are over #### data points.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>In our demonstration, our objective is to understand the flight delays by day of the week; in other words, the average delay for Mondays, Tuesdays, and so forth.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The script in this tutorial shows you how to accomplish this task using  <ph id="ph1">`rxExecBy`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept></source>
        </trans-unit></group></body></file></xliff>