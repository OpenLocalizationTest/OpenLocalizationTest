<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="featurize-text.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37b8a647f48cd1224113309be6b5f64726a01f7b23.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">b8a647f48cd1224113309be6b5f64726a01f7b23</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\featurize-text.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>featurize_text: Machine Learning Text Transform</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Text transforms that can be performed on data before training a model.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>transform, featurizer, text</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.featurize_text<ept id="p1">*</ept>: Converts text columns into numerical features</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Text transforms that can be performed on data before training a model.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`featurize_text`</ph> transform produces a bag of counts of sequences of consecutive words, called n-grams, from a given corpus of text.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>There are two ways it can do this:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>build a dictionary of n-grams and use the ID in the dictionary as the index in the bag;</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>hash each n-gram and use the hash value as the index in the bag.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The purpose of hashing is to convert variable-length text documents into equal-length numeric feature vectors, to support dimensionality reduction and to make the lookup of feature weights faster.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The text transform is applied to text input columns.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>It offers language detection, tokenization, stopwords removing, text normalization and feature generation.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>It supports the following languages by default: English, French, German, Dutch, Italian, Spanish and Japanese.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The n-grams are represented as count vectors, with vector slots corresponding either to n-grams (created using <ph id="ph1">`n_gram`</ph>) or to their hashes (created using <ph id="ph2">`n_gram_hash`</ph>).</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Embedding ngrams in a vector space allows their contents to be compared in an efficient manner.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The slot values in the vector can be weighted by the following factors:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>term frequency<ept id="p1">*</ept> - The number of occurrences of the slot in the text</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>inverse document frequency<ept id="p1">*</ept> - A ratio (the logarithm of inverse relative slot frequency) that measures the information a slot provides by determining how common or rare it is across the entire text.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>term frequency-inverse document frequency<ept id="p1">*</ept> - the product term frequency and the inverse document frequency.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>cols</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>A character string or list of variable names to transform.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`dict`</ph>, the keys represent the names of new variables to be created.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>language</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Specifies the language used in the data set.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The following values are supported:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>: for automatic language detection.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>stopwords_remover</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Specifies the stopwords remover to use.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>There are three options supported:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>None<ept id="p1">*</ept>: No stopwords remover is used.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>: A precompiled language-specific list of stop words is used that includes the most common words from Microsoft Office.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>: A user-defined list of stopwords.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>It accepts the following option: <ph id="ph1">`stopword`</ph>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>case</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Text casing using the rules of the invariant culture.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Takes the following values:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`"Lower"`</ph>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>keep_diacritics</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>to remove diacritical marks; <ph id="ph1">`True`</ph> to retain diacritical marks.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`False`</ph>.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>keep_punctuations</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>to remove punctuation; <ph id="ph1">`True`</ph> to retain punctuation.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`True`</ph>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>keep_numbers</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>to remove numbers; <ph id="ph1">`True`</ph> to retain numbers.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`True`</ph>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>dictionary</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>A dictionary of whitelisted terms which accepts the following options:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>: An optional character vector of terms or categories.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>: Drop items.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>: Specifies how to order items when vectorized.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Two orderings are</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>: items appear in the order encountered.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>: items are sorted according to their default comparison.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>For example, text sorting will be case sensitive (e.g., ‘A’ then ‘Z’ then ‘a’).</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Note that the stopwords list takes precedence over the dictionary whitelist as the stopwords are removed before the dictionary terms are whitelisted.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>word_feature_extractor</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Specifies the word feature extraction arguments.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>There are two different feature extraction mechanisms:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>: Count-based feature extraction (equivalent to WordBag).</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>It accepts the following options: <ph id="ph1">`max_num_terms`</ph> and <ph id="ph2">`weighting`</ph>.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>: Hashing-based feature extraction (equivalent to WordHashBag).</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>It accepts the following options: <ph id="ph1">`hash_bits`</ph>, <ph id="ph2">`seed`</ph>, <ph id="ph3">`ordered`</ph> and <ph id="ph4">`invert_hash`</ph>.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`n_gram`</ph>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>char_feature_extractor</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Specifies the char feature extraction arguments.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>There are two different feature extraction mechanisms:</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>: Count-based feature extraction (equivalent to WordBag).</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>It accepts the following options: <ph id="ph1">`max_num_terms`</ph> and <ph id="ph2">`weighting`</ph>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>: Hashing-based feature extraction (equivalent to WordHashBag).</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>It accepts the following options: <ph id="ph1">`hash_bits`</ph>, <ph id="ph2">`seed`</ph>, <ph id="ph3">`ordered`</ph> and <ph id="ph4">`invert_hash`</ph>.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>vector_normalizer</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Normalize vectors (rows) individually by rescaling them to unit norm.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Takes one of the following values:</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`"L2"`</ph>.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>kargs</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Additional arguments sent to compute engine.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>An object defining the transform.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`n_gram`</ph><ept id="p1">](n-gram.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`n_gram_hash`</ph><ept id="p2">](n-gram-hash.md)</ept>, <bpt id="p3">[</bpt><ph id="ph3">`n_gram`</ph><ept id="p3">](custom.md)</ept>, <bpt id="p4">[</bpt><ph id="ph4">`n_gram_hash`</ph><ept id="p4">](predefined.md)</ept>, <bpt id="p5">[</bpt><ph id="ph5">`get_sentiment`</ph><ept id="p5">](get-sentiment.md)</ept>.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>N-grams extractors</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.n_gram<ept id="p1">*</ept>: Converts text into features using n-grams</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.n_gram_hash<ept id="p1">*</ept>: Converts text into features using hashed n-grams</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Stopwords removers</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.custom<ept id="p1">*</ept>: Removes custom stopwords</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.predefined<ept id="p1">*</ept>: Removes predefined stopwords</source>
        </trans-unit></group></body></file></xliff>