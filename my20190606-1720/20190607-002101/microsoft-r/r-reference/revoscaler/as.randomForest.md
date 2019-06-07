<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="as.randomForest.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c378d5703d4e9a127c6e88cbe87dfa16b653e9e5316.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8d5703d4e9a127c6e88cbe87dfa16b653e9e5316</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\as.randomForest.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>as.randomForest function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Converts objects containing decision tree results to an randomForest object.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), as.randomForest, as.randomForest.rxDForest, as.randomForest.rxDTree, as.randomForest.rpart, category, models</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>as.randomForest: Conversion of an rxDForest, rxDTree, or rpart object to an randomForest Object</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Converts objects containing decision tree results to an randomForest object.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>object of class rxDForest, rxDTree, or rpart.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>a logical value (default being <ph id="ph1">`TRUE`</ph>) specifying if the majority splitting direction  at a node should be decided based on the sum of case weights or the number of observations when the split variable at the node is a factor or ordered factor  but a certain level is not present (or not defined for the factor).</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>a character string specifying how ties are handled when deciding the majority direction,  with the default being <ph id="ph1">`"random"`</ph>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Refer to max.col for details.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to <ph id="ph1">`as.randomForest.rpart`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>These functions convert an existing object of class rxDForest, rxDTree, or rpart to an object of class <ph id="ph1">`randomForest`</ph>, respectively.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The underlying structure of the output object will be a subset of that produced by an equivalent call to <ph id="ph1">`randomForest`</ph>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Often, this method can be used to coerce an object for use with the <bpt id="p1">**</bpt>pmml<ept id="p1">**</ept> package.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> model objects that contain <ph id="ph1">`transforms`</ph> or a <ph id="ph2">`transformFunc`</ph> are not supported.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>an object of class randomForest.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxDForest<ept id="p1">](rxDForest.md)</ept>, <bpt id="p2">[</bpt>rxDTree<ept id="p2">](rxDTree.md)</ept>, rpart, randomForest, <bpt id="p3">[</bpt>as.rpart<ept id="p3">](as.rpart.md)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>