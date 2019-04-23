<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="what-is-r-client-r-server.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338af4fe1bc57bc91505ab7aff2d1a87e083c65e0ad7.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">f4fe1bc57bc91505ab7aff2d1a87e083c65e0ad7</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\what-is-r-client-r-server.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Microsoft R Server vs R Client: Scale</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn about Microsoft R features and components in R Server, R Client, R Open.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>R Server vs. R Client: Scale</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Microsoft R Server<ept id="p1">](what-is-microsoft-r-server.md)</ept> and <bpt id="p2">[</bpt>Microsoft R Client<ept id="p2">](r-client/what-is-microsoft-r-client.md)</ept> offer virtually identical packages, but each one targets different scenarios.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>R Client is intended for data scientists who create solutions that run locally.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>R Server is commercial software that runs on a range of platforms, at much greater scale, with infrastructure for handling major workloads, on client-server topologies that support remote access over authenticated connections.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>You can learn and develop on R Client, and then migrate your work to R Server or execute it remotely on an R Server whenever you need the scale, support, and infrastructure of an operationalized server.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>On R Server, the RevoScaleR package offers almost unbounded scale in running R workloads in parallel and distributed configurations.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Although you can call RevoScaleR functions on a system having just R Client, RevoScaleR is throttled on R Client: datasets must fit in memory, and processing is capped at a maximum of two processors on the local system.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Only R Server gives you RevoScaleR at full capacity, with support for remote compute context, data chunking, parallelization, and distributed workloads.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Given a platform that supports it, functions in RevoScaleR provide high performance, parallelized, and distributable analytics functions that scale from small data sets in memory to huge data sets stored on disk on a cluster of computers.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The analytics functions provided include summary statistics, cubes and crosstabs, linear models, logistic regression, generalized linear models, kmeans clustering, decision trees, and decision forests.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>These algorithms are parallelized and distributed automatically, and process data in chunks so that all of your data does not need to be in memory at one time; you can use the same analysis code for your giant data set as you do for a small data set in memory.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>RevoScaleR also provides traditional high performance computing (tools if you prefer to construct your own distributed computations.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>In addition, in many environments, there are full-featured tools for data cleaning and manipulation.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Functions in RevoScaleR are prefixed with ‘rx’ for analysis and data manipulation.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Additionally, use ‘rxExec’ for high performance computing.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If you are computing decision trees, also check out the included RevoTreeView package that allows you to interactively visualize your decision trees.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>What's new in R Server<ept id="p1">](whats-new-in-r-server.md)</ept><ph id="ph1">
</ph><bpt id="p2">[</bpt>What's new in R Client<ept id="p2">](r-client/whats-new-in-r-client.md)</ept></source>
        </trans-unit></group></body></file></xliff>