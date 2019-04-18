<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="remotescript.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea9266158f1a0921db708b480b9a8873da2235252e29f.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">6158f1a0921db708b480b9a8873da2235252e29f</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\mrsdeploy\remotescript.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>remoteScript function (mrsdeploy) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>A simple wrapper function for executing a remote R script.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(mrsdeploy), remoteScript</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>remoteScript: Wrapper function for remote script execution.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>A simple wrapper function for executing a remote R script.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The R Script file to be executed.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>JSON encoded string of R objects that are loaded into the Remote R session's workspace prior to execution.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Only R objects of type: primitives, vectors and dataframes are supported via this parameter.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Alternatively the <bpt id="p1">[</bpt>putLocalObject<ept id="p1">](putLocalObject.md)</ept> can be used, prior to a call to this function, to move any R object from the local workspace into the  remote R session.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Character vector of the names of the objects to retrieve.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Only primitives, vectors and dataframes can be retrieved using this function  Use <bpt id="p1">[</bpt>getRemoteObject<ept id="p1">](getRemoteObject.md)</ept>to get any type of R object from the remote session.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, plots generate during execution are displayed in the local plot window.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>NOTE<ept id="p1">**</ept> This capability requires that the '<ph id="ph1">`png`</ph>' package is installed on the local machine</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, plots generated during execution are copied to the working directory of the local session.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, plots will be created using the '<ph id="ph2">`recordPlot`</ph>' function in R.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the remote script will be run asynchronously in a separate window.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the async R session will quit upon completion.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Only applies if <ph id="ph1">`async=TRUE`</ph></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Complete documentation: <bpt id="p1">[</bpt><ph id="ph1">`https://go.microsoft.com/fwlink/?linkid=836352`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?linkid=836352)</ept></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>A list containing the results of the execution.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>remoteExecute<ept id="p1">](remoteExecute.md)</ept></source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>