<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="featurizetext.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18cfa8cb68d07ec43f36fe40aa706b665127ef763db.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">fa8cb68d07ec43f36fe40aa706b665127ef763db</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\featurizetext.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>stopwordsDefault function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Text transforms that can be performed on data before training  a model.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), stopwordsDefault, featurizeText, stopwordsCustom, termDictionary, transform</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>stopwordsDefault: Machine Learning Text Transform</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Text transforms that can be performed on data before training a model.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>character: <ph id="ph1">&lt;string&gt;</ph>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Data file containing the terms (short form data).</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>An optional character vector of terms or categories.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Specifies how to order items when vectorized.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Two orderings are supported:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"occurrence"`</ph>: items appear in the order encountered.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"value"`</ph>: items are sorted according to their default comparison.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>For example, text sorting will be case sensitive (e.g., 'A' then 'Z'   then 'a').</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>A named list of character vectors of input variable names and the name of the output variable.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Note that the input variables must be of the same type.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>For one-to-one mappings between input and output variables, a named character vector can be used.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Specifies the language used in the data set.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The following  values are supported:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"AutoDetect"`</ph>: for automatic language detection.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"English"`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"French"`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"German"`</ph>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Dutch"`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Italian"`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Spanish"`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"Japanese"`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Specifies the stopwords remover to use.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>There are three options supported:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> No stopwords remover is used.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`stopwordsDefault`</ph>: A precompiled language-specific list of stop words is used that includes the most common words from Microsoft Office.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`stopwordsCustom`</ph>: A user-defined list of stopwords.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>It accepts   the following option: <ph id="ph1">`dataFile`</ph>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Text casing using the rules of the invariant culture.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Takes the following values:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"lower"`</ph>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"upper"`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"none"`</ph>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`"lower"`</ph>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`FALSE`</ph> to remove diacritical marks; <ph id="ph2">`TRUE`</ph> to  retain diacritical marks.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`FALSE`</ph> to remove punctuation; <ph id="ph2">`TRUE`</ph> to  retain punctuation.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`FALSE`</ph> to remove numbers; <ph id="ph2">`TRUE`</ph> to retain numbers.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>A <ph id="ph1">`termDictionary`</ph> of whitelisted terms which accepts the following options:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`terms`</ph>,</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`dataFile`</ph>, and</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`sort`</ph>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Note that the stopwords list takes precedence over the dictionary whitelist as the stopwords are removed before the dictionary terms are whitelisted.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Specifies the word feature extraction arguments.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>There  are two different feature extraction mechanisms:</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>ngramCount<ept id="p1">](ngram.md)</ept>: Count-based feature extraction (equivalent   to WordBag).</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>It accepts the following options: <ph id="ph1">`maxNumTerms`</ph> and <ph id="ph2">`weighting`</ph>.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>ngramHash<ept id="p1">](ngram.md)</ept>: Hashing-based feature extraction (equivalent  to WordHashBag).</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>It accepts the following options: <ph id="ph1">`hashBits`</ph>,  <ph id="ph2">`seed`</ph>, <ph id="ph3">`ordered`</ph> and <ph id="ph4">`invertHash`</ph>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`ngramCount`</ph>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Specifies the char feature extraction arguments.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>There  are two different feature extraction mechanisms:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>ngramCount<ept id="p1">](ngram.md)</ept>: Count-based feature extraction (equivalent   to WordBag).</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>It accepts the following options: <ph id="ph1">`maxNumTerms`</ph> and <ph id="ph2">`weighting`</ph>.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>ngramHash<ept id="p1">](ngram.md)</ept>: Hashing-based feature extraction (equivalent  to WordHashBag).</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>It accepts the following options: <ph id="ph1">`hashBits`</ph>,  <ph id="ph2">`seed`</ph>, <ph id="ph3">`ordered`</ph> and <ph id="ph4">`invertHash`</ph>.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Normalize vectors (rows) individually by rescaling them to unit norm.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Takes one of the following values:</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"none"`</ph>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"l2"`</ph>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"l1"`</ph>.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`"linf"`</ph>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`"l2"`</ph>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Additional arguments sent to the compute engine.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`featurizeText`</ph> transform produces a bag of counts of</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>sequences of consecutive words, called n-grams, from a given corpus of text.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>There are two ways it can do this:</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>build a dictionary of n-grams and use the ID in the dictionary as the index in the bag;</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>hash each n-gram and use the hash value as the index in the bag.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>The purpose of hashing is to convert variable-length text documents into equal-length numeric feature vectors, to support dimensionality reduction and to make the lookup of feature weights faster.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>The text transform is applied to text input columns.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>It offers language detection, tokenization, stopwords removing, text normalization and feature generation.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>It supports the following languages by default: English, French, German, Dutch, Italian, Spanish and Japanese.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>The n-grams are represented as count vectors, with vector slots corresponding either to n-grams (created using <ph id="ph1">`ngramCount`</ph>) or to their hashes (created using <ph id="ph2">`ngramHash`</ph>).</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Embedding ngrams in a vector space allows their contents to be compared in an efficient manner.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>The slot values in the vector can be weighted by the following factors:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>term frequency - The number of occurrences of the slot in the text</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>inverse document frequency - A ratio (the logarithm of inverse relative slot frequency) that measures the information a slot provides by determining how common or rare it is across the entire text.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>term frequency-inverse document frequency - the product term frequency and the inverse document frequency.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>A <ph id="ph1">`maml`</ph> object defining the transform.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>ngramCount<ept id="p1">](ngram.md)</ept>, <bpt id="p2">[</bpt>ngramHash<ept id="p2">](ngram.md)</ept>, <bpt id="p3">[</bpt>rxFastTrees<ept id="p3">](rxFastTrees.md)</ept>, <bpt id="p4">[</bpt>rxFastForest<ept id="p4">](rxFastForest.md)</ept>, <bpt id="p5">[</bpt>rxNeuralNet<ept id="p5">](rxNeuralNet.md)</ept>, <bpt id="p6">[</bpt>rxOneClassSvm<ept id="p6">](rxOneClassSvm.md)</ept>, <bpt id="p7">[</bpt>rxLogisticRegression<ept id="p7">](rxLogisticRegression.md)</ept>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>