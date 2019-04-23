<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="ngram.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338aeaf13cfb94fc78cdf749a5e94ac23683a50eb262.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eaf13cfb94fc78cdf749a5e94ac23683a50eb262</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\ngram.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>ngram function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Feature Extractors that can be used with mtText.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), ngram, ngramCount, ngramHash, transform</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>ngram: Machine Learning Feature Extractors</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Feature Extractors that can be used with mtText.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>An integer that specifies the maximum number of tokens to take when constructing an n-gram.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The default value is 1.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>An integer that specifies the maximum number of tokens to skip when constructing an n-gram.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If the value specified as skip length is <ph id="ph1">`k`</ph>, then n-grams can contain up to k skips (not necessarily consecutive).</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>For example, if <ph id="ph1">`k=2`</ph>, then the 3-grams extracted from the text "the sky is blue today" are: "the sky is", "the sky blue", "the sky today", "the is blue", "the is today" and "the blue today".</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The default  value is 0.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>An integer that specifies the maximum number of categories  to include in the dictionary.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The default value is 10000000.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>A character string that specifies the weighting criteria:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>: to use term frequency.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>: to use inverse document frequency.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>: to use both term frequency and inverse document   frequency.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Number of bits to hash into.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Must be between 1 and 30, inclusive.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Hashing seed.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>to include the position of each term in the  hash.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Otherwise, <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>An integer specifying the limit on the number of keys  that can be used to generate the slot name.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>means no invert  hashing; <ph id="ph1">`-1`</ph> means no limit.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>While a zero value gives better  performance, a non-zero value is needed to get meaningful coefficient names.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>allows defining arguments for count-based feature extraction.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>It accepts following options: <ph id="ph1">`ngramLength`</ph>, <ph id="ph2">`skipLength`</ph>, <ph id="ph3">`maxNumTerms`</ph> and <ph id="ph4">`weighting`</ph>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>allows defining arguments for hashing-based feature extraction.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>It accepts the following options: <ph id="ph1">`ngramLength`</ph>, <ph id="ph2">`skipLength`</ph>, <ph id="ph3">`hashBits`</ph>, <ph id="ph4">`seed`</ph>, <ph id="ph5">`ordered`</ph> and <ph id="ph6">`invertHash`</ph>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>A character string defining the transform.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>featurizeText<ept id="p1">](featurizeText.md)</ept>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>