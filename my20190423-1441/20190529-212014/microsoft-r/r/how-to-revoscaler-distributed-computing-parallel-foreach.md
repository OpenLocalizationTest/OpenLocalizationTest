<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-distributed-computing-parallel-foreach.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b326716be8ffbd7e7258ea4b94633749771eb8bc57.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">26716be8ffbd7e7258ea4b94633749771eb8bc57</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-distributed-computing-parallel-foreach.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Parallel execution using foreach and doRSR for script containing RevoScaleR and foreach constructs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Parallel execution using the doRSR package for script containing RevoScaleR and foreach constructs.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Parallel execution using doRSR for script containing RevoScaleR and foreach constructs</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Machine Learning Server includes the open-source <bpt id="p1">[</bpt>foreach package<ept id="p1">](https://CRAN.R-project.org/package=foreach)</ept> in case you need to substitute the built-in parallel execution methodology of RevoScaleR with a custom implementation.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>To execute code that leverages foreach, you will need a parallel backend engine, similar to <bpt id="p1">**</bpt>NetWorkSpaces<ept id="p1">**</ept>, <bpt id="p2">**</bpt>snow<ept id="p2">**</ept>, and <bpt id="p3">**</bpt>rmpi<ept id="p3">**</ept>.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>For integration with script leveraging RevoScaleR, you can use the <bpt id="p1">**</bpt>doRSR<ept id="p1">**</ept> package.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>doRSR<ept id="p1">**</ept> package is a parallel backend for RevoScaleR, built on top of <bpt id="p2">[</bpt>rxExec<ept id="p2">](../r-reference/revoscaler/rxexec.md)</ept>, and included with all RevoScaleR distributions.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Example script using doRSR</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>To get started with doRSR, load the package and register the backend:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The doRSR package uses your current compute context to determine how to run your job.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>In most cases, the job is run via rxExec, sequentially in the local compute context and in parallel in a distributed compute context.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>In the special case where you are in the local compute context and have set <ph id="ph1">`rxOptions(useDoParallel=TRUE)`</ph>, doRSR will pass your foreach jobs to the <bpt id="p1">**</bpt>doParallel<ept id="p1">**</ept> package for execution in parallel using multiple cores on your machine.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>A simple example is this one from the foreach help file:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This returns, as expected, a list containing the square roots of 1, 2, and 3:</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Another example is what the help file reports as a “simple (and inefficient) parallel matrix multiply”:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>This returns the multiplied matrix:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Use case: simulation</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>Running jobs in parallel<ept id="p1">](how-to-revoscaler-distributed-computing-parallel-jobs.md)</ept>, we introduced the simulation function <ph id="ph1">`playDice`</ph> to simulate a single game of dice rolling, using <bpt id="p2">[</bpt>rxExec<ept id="p2">](../r-reference/revoscaler/rxexec.md)</ept> to play 10000 games.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>You can do the same thing with foreach:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Although outcomes are equivalent in both approaches, the rxExec approach is several times faster because you can call it directly.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Use case: naïve parallelization of the standard R kmeans function</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Also in the <bpt id="p1">[</bpt>previous article<ept id="p1">](how-to-revoscaler-distributed-computing-parallel-jobs.md)</ept>, we created a function kmeansRSR to perform a naïve parallelization of the standard R kmeans function.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>We can do the same thing with foreach directly as follows:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Recall that the idea was to run a specified number of kmeans fits, then find the best set of results, where “best” is the result with the lowest within-group sum of squares.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>We can run this function as follows:</source>
        </trans-unit></group></body></file></xliff>