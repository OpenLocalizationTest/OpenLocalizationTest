<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-create-manage-session-pools.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4ce5881c69300e42b7f13b59848ec39e008683ec0.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">ce5881c69300e42b7f13b59848ec39e008683ec0</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\how-to-create-manage-session-pools.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Create and manage session pools for fast web service connections in R (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Allocate resources for pre-loading web service connections and dependencies in R solutions (Machine Learning Server ).</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to create and manage session pools for fast web service connections in R</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: Machine Learning Server 9.3 (R)<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Fast connections to a web service are possible when you create sessions and load dependencies in advance.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Sessions are available in a pool dedicated to a specific web service, where each session includes an instance of the R interpreter and a copy of dependencies required by the web service.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>For example, if you create ten sessions in advance for a web service that uses Matplotlib, dplyr, cluster, RevoScaleR, MicrosoftML, and mrsdeploy, each session would have its own instance of the R interpreter plus a copy of each library loaded in memory.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>A web service having a dedicated session pool never requests connections from the <bpt id="p1">[</bpt>generic session pool<ept id="p1">](configure-evaluate-capacity.md#pool)</ept> shared resource, not even when maximum sessions are reached.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The generic session pool services only those web services that do not have dedicated resources.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>For R script, the <bpt id="p1">[</bpt>mrsdeploy<ept id="p1">](../r-reference/mrsdeploy/mrsdeploy-package.md)</ept> function library provides three functions for creating and managing sessions:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>configureServicePool<ept id="p1">](../r-reference/mrsdeploy/configureServicePool.md)</ept></source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>getPoolStatus<ept id="p1">](../r-reference/mrsdeploy/getPoolStatus.md)</ept></source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>deleteServicePool<ept id="p1">](../r-reference/mrsdeploy/deleteServicePool.md)</ept></source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Create or modify a dedicated session pool</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Given an existing connection to a Machine Learning Server with <bpt id="p1">[</bpt>operationalization<ept id="p1">](../r-reference/mrsdeploy/configureServicePool.md)</ept> enabled, you can use <bpt id="p2">[</bpt>mrsdeploy<ept id="p2">](../r-reference/mrsdeploy/mrsdeploy-package.md)</ept> functions and an R console application such as Rgui.exe to run the following commands:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Currently, there are no commands or functions that return actual session pool usage.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The log file is your best resource for analyzing connection and service activity.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Trace user actions<ept id="p1">](configure-run-diagnostics.md#trace-user-actions)</ept>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Delete a session pool</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>At the R console, on the compute node, run the following command to delete the session pool for a given service.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>This feature is still under development.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>In rare cases, the <bpt id="p1">[</bpt>deleteServicePool<ept id="p1">](../r-reference/mrsdeploy/deleteServicePool.md)</ept> command may fail to actually delete the pool on the computeNode.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If you encounter this situation, issue a new <bpt id="p1">[</bpt>deleteServicePool<ept id="p1">](../r-reference/mrsdeploy/deleteServicePool.md)</ept> request.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">[</bpt>getPoolStatus<ept id="p1">](../r-reference/mrsdeploy/getPoolStatus.md)</ept> command to monitor the status of dedicated pools on the computeNode.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>What are web services in Machine Learning Server?<ept id="p1">](concept-what-are-web-services.md)</ept></source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Evaluate web service capacity: generic session pools<ept id="p1">](configure-evaluate-capacity.md#pool)</ept></source>
        </trans-unit></group></body></file></xliff>