<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="categorical.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef0690673350b7613dc8448142abed3adbb9223b8eae8553081.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">0b7613dc8448142abed3adbb9223b8eae8553081</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\categorical.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>categorical: Machine Learning Categorical Data Transform</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Categorical transform that can be performed on data before training a model.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>transform, category</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.categorical<ept id="p1">*</ept>: Converts a text column into categories</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Categorical transform that can be performed on data before training a model.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`categorical`</ph> transform passes through a data set, operating on text columns, to build a dictionary of categories.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>For each row, the entire text string appearing in the input column is defined as a category.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The output of the categorical transform is an indicator vector.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Each slot in this vector corresponds to a category in the dictionary, so its length is the size of the built dictionary.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The categorical transform can be applied to one or more columns, in which case it builds a separate dictionary for each column that it is applied to.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`categorical`</ph> is not currently supported to handle factor data.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>cols</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>A character string or list of variable names to transform.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`dict`</ph>, the keys represent the names of new variables to be created.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>output_kind</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>A character string that specifies the kind of output kind.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Bag"`</ph>: Outputs a multi-set vector.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If the input column is a vector of categories, the output contains one vector, where the value in each slot is the number of occurrences of the category in the input vector.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If the input column contains a single category, the indicator vector and the bag vector are equivalent</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Ind"`</ph>: Outputs an indicator vector.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The input column is a vector of categories, and the output contains one indicator vector per slot in the input column.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Key"`</ph>: Outputs an index.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The output is an integer ID (between 1 and the number of categories in the dictionary) of the category.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Bin"`</ph>: Outputs a vector which is the binary representation of the category.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`"Ind"`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>max_num_terms</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>An integer that specifies the maximum number of categories to include in the dictionary.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The default value is 1000000.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>terms</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Optional character vector of terms or categories.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>sort</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>A character string that specifies the sorting criteria.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Occurrence"`</ph>: Sort categories by occurrences.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Most frequent is first.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Value"`</ph>: Sort categories by values.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>text_key_values</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Whether key value metadata should be text, regardless of the actual input type.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>kargs</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Additional arguments sent to compute engine.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>An object defining the transform.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit></group></body></file></xliff>