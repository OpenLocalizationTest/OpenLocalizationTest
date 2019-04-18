<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="concat.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907fdb484d9de470e81dbd3762b51bf61223d99f0ad6.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">db484d9de470e81dbd3762b51bf61223d99f0ad6</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\concat.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>concat function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Combines several columns into a single vector-valued column.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), concat, transform</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>concat: Machine Learning Concat Transform</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Combines several columns into a single vector-valued column.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A named list of character vectors of input variable names and the name of the output variable.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Note that all the input variables must be of the same type.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>It is possible to produce multiple output columns  with the concatenation transform.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>In this case, you need to use a list of  vectors to define a one-to-one mapping between input and output variables.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>For example, to concatenate columns InNameA and InNameB into column OutName1 and also columns InNameC and InNameD into column OutName2, use the list:  (list(OutName1 = c(InNameA, InNameB), outName2 = c(InNameC, InNameD)))</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Additional arguments sent to the compute engine</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`concat`</ph> creates a single vector-valued column from multiple</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>columns.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>It can be performed on data before training a model.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The concatenation</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>can significantly speed up the processing of data when the number of columns is as large as hundreds to thousands.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>A <ph id="ph1">`maml`</ph> object defining the concatenation transform.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>featurizeText<ept id="p1">](featurizeText.md)</ept>, <bpt id="p2">[</bpt>categorical<ept id="p2">](categorical.md)</ept>, <bpt id="p3">[</bpt>categoricalHash<ept id="p3">](categoricalHash.md)</ept>, <bpt id="p4">[</bpt>rxFastTrees<ept id="p4">](rxFastTrees.md)</ept>, <bpt id="p5">[</bpt>rxFastForest<ept id="p5">](rxFastForest.md)</ept>, <bpt id="p6">[</bpt>rxNeuralNet<ept id="p6">](rxNeuralNet.md)</ept>, <bpt id="p7">[</bpt>rxOneClassSvm<ept id="p7">](rxOneClassSvm.md)</ept>, <bpt id="p8">[</bpt>rxLogisticRegression<ept id="p8">](rxLogisticRegression.md)</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>