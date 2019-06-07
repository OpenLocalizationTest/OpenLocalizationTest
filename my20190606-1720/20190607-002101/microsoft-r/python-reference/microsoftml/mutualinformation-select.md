<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="mutualinformation-select.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37451ebe9e77bafbf6d3ef5dd100993e5a41353208.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">451ebe9e77bafbf6d3ef5dd100993e5a41353208</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\mutualinformation-select.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>mutualinformation_select: Machine Learning Mutual Information Mode Feature Selection Transform</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Selects the top k features across all specified columns ordered by their mutual information with the label column.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>feature, selection, mutual, information</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.mutualinformation_select<ept id="p1">*</ept>: Feature selection based on mutual information</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Selects the top k features across all specified columns ordered by their mutual information with the label column.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The mutual information of two random variables <ph id="ph1">`X`</ph> and <ph id="ph2">`Y`</ph> is a measure of the mutual dependence between the variables.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Formally, the mutual information can be written as:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>where the expectation is taken over the joint distribution of <ph id="ph1">`X`</ph> and <ph id="ph2">`Y`</ph>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Here <ph id="ph1">`p(x,y)`</ph> is the joint probability density function of <ph id="ph2">`X`</ph> and <ph id="ph3">`Y`</ph>, <ph id="ph4">`p(x)`</ph> and <ph id="ph5">`p(y)`</ph> are the marginal probability density functions of <ph id="ph6">`X`</ph> and <ph id="ph7">`Y`</ph> respectively.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>In general, a higher mutual information between the dependent variable (or label) and an independent variable (or feature) means that the label has higher mutual dependence over that feature.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The mutual information feature selection mode selects the features based on the mutual information.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>It keeps the top <ph id="ph1">`num_features_to_keep`</ph> features with the largest mutual information with the label.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>cols</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Specifies character string or list of the names of the variables to select.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>label</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Specifies the name of the label.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>num_features_to_keep</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If the number of features to keep is specified to be <ph id="ph1">`n`</ph>, the transform picks the <ph id="ph2">`n`</ph> features that have the highest mutual information with the dependent variable.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The default value is 1000.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>num_bins</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Maximum number of bins for numerical values.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Powers of 2 are recommended.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The default value is 256.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>kargs</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Additional arguments sent to compute engine.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>An object defining the transform.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Wikipedia: Mutual Information</source>
        </trans-unit></group></body></file></xliff>