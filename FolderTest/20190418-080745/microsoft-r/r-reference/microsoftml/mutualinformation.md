<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="mutualinformation.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef0690673358752b842dd573571a0ba5eef8b1b45a5cb2abfd4.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8752b842dd573571a0ba5eef8b1b45a5cb2abfd4</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\mutualinformation.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>mutualInformation function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Mutual information mode of feature selection used in the feature selection transform <bpt id="p1">[</bpt>selectFeatures<ept id="p1">](selectFeatures.md)</ept>.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), mutualInformation, feature, information, mutual, selection</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>mutualInformation: Feature Selection Mutual Information Mode</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Mutual information mode of feature selection used in the feature selection transform <bpt id="p1">[</bpt>selectFeatures<ept id="p1">](selectFeatures.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>If the number of features to keep is specified to be <ph id="ph1">`n`</ph>, the transform picks the <ph id="ph2">`n`</ph> features that have the highest mutual information with the dependent variable.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The default value is 1000.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Maximum number of bins for numerical values.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Powers of 2 are recommended.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The default value is 256.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed directly to the Microsoft Compute Engine.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The mutual information of two random variables <ph id="ph1">`X`</ph> and <ph id="ph2">`Y`</ph> is a measure of the mutual dependence between the variables.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Formally, the mutual information can be written as:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>where the expectation is taken over the joint distribution of <ph id="ph1">`X`</ph> and <ph id="ph2">`Y`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Here <ph id="ph1">`p(x,y)`</ph> is the joint probability density function of <ph id="ph2">`X`</ph> and <ph id="ph3">`Y`</ph>, <ph id="ph4">`p(x)`</ph> and <ph id="ph5">`p(y)`</ph> are the marginal probability density functions of <ph id="ph6">`X`</ph> and <ph id="ph7">`Y`</ph> respectively.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>In general, a higher mutual information between the dependent variable (or label) and an independent varialbe (or feature) means that the label has higher mutual dependence over that feature.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The mutual information feature selection mode selects the features based on the mutual information.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>It keeps the top <ph id="ph1">`numFeaturesToKeep`</ph> features with the largest mutual information with the label.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>a character string defining the mode.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>minCount<ept id="p1">](minCount.md)</ept> <bpt id="p2">[</bpt>selectFeatures<ept id="p2">](selectFeatures.md)</ept></source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>