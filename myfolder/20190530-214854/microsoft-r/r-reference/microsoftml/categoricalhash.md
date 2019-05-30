<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="categoricalhash.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e1af80923fa909b621dceab1ab41caefd5ca4b019.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1af80923fa909b621dceab1ab41caefd5ca4b019</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\categoricalhash.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>categoricalHash function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Categorical hash transform that can be performed on data before  training a model.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), categoricalHash, transform</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>categoricalHash: Machine Learning Categorical HashData Transform</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Categorical hash transform that can be performed on data before training a model.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A character vector or list of variable names to transform.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If named, the names represent the names of new variables to be created.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>An integer specifying the number of bits to hash into.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Must be between 1 and 30, inclusive.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The default value is 16.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>An integer specifying the hashing seed.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The default value is 314489979.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>to include the position of each term in the  hash.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Otherwise, <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>An integer specifying the limit on the number of keys  that can be used to generate the slot name.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>means no invert  hashing; <ph id="ph1">`-1`</ph> means no limit.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>While a zero value gives better  performance, a non-zero value is needed to get meaningful coefficient names.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`0`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>A character string that specifies the kind of output kind.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>: Outputs an indicator vector.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The input column is a vector   of categories, and the output contains one indicator vector per slot in   the input column.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>: Outputs a multi-set vector.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If the input column is a  vector of categories, the output contains one vector, where the value in   each slot is the number of occurrences of the category in the input  vector.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If the input column contains a single category, the indicator  vector and the bag vector are equivalent</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>: Outputs an index.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The output is an integer ID (between 1 and the number of categories in the dictionary) of the category.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`"Bag"`</ph>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Additional arguments sent to the compute engine.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>converts a categorical value into an indicator array by hashing the value and using the hash as an index in the bag.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If the input column is a vector, a single indicator bag is returned for it.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>does not currently support handling factor data.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>a <ph id="ph1">`maml`</ph> object defining the transform.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxFastTrees<ept id="p1">](rxFastTrees.md)</ept>, <bpt id="p2">[</bpt>rxFastForest<ept id="p2">](rxFastForest.md)</ept>, <bpt id="p3">[</bpt>rxNeuralNet<ept id="p3">](rxNeuralNet.md)</ept>, <bpt id="p4">[</bpt>rxOneClassSvm<ept id="p4">](rxOneClassSvm.md)</ept>, <bpt id="p5">[</bpt>rxLogisticRegression<ept id="p5">](rxLogisticRegression.md)</ept>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>