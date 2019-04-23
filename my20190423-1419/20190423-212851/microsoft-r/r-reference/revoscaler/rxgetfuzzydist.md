<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxgetfuzzydist.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a208835a20bad897c6380838c048d979a109985d6.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">208835a20bad897c6380838c048d979a109985d6</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxgetfuzzydist.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxGetFuzzyDist function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>EXPERIMENTAL: Get fuzzy distances for a character vector</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxGetFuzzyDist, manip</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxGetFuzzyDist: Fuzzy distances for a character vector</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>EXPERIMENTAL: Get fuzzy distances for a character vector</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Character vector of strings to process or name of character variable.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>or data frame or RevoScaleR data source containing the variable to process.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>or RevoScaleR data source in which to put output.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>or character vector of variables from the input 'data' to keep in the output data set.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>They will be replicated for multiple matches.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Method for matching to dictionary: 'none' for no matching, 'lv' for Levenshtein; 'j' for Jaro, 'jw' for JaroWinkler,  'exact' for exact matching</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Transformation type in creating keys to be matched: 'all' to retain all characters, 'alphanum' for alphanumeric characters only,  'alpha' for letters only", 'mphone3' for Metaphone3 phonetic transformation, 'soundex' for Soundex phonetic transformation,  'mphone3Vowels' for Metaphone3 encoding more than initial vowels, 'mphone3Exact' for Metaphone3 with more exact consonants, 'soundexNum' for Soundex with numbers only, 'soundexAll' for Soundex not truncated at 4 characters, and 'soundexAm' for the American variant of Soundex.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>A logical specifying whether or not to ignore case when comparing strings to the dictionary</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>A logical specifying whether or not to ignore spaces.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, for phonetic conversions each word in the string is processed separately and then concatenated together.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>A logical.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, numbers are converted to words before phonetic processing.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, numbers are ignored or removed</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>An optional character vector containing words to ignore when matching.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>A logical.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, if a match is not found an empty string is returned.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Only applies when dictionary is provided.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Minimum distance required for a match; applies only to distance metric algorithms (Levenshtein, Jaro, JaroWinkler).</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>One is a perfect match.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Zero is no similarity.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Character vector containing the dictionary for string comparisons.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>from strings before processing.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>A logical specifying whether to return the string and dictionary values</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>or logical specifying whether to return the string and dictionary indexes.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, it is set to <ph id="ph2">`!returnString`</ph> .</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>A logical.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> and the specified <ph id="ph2">`outFile`</ph> exists, it will be overwritten.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Four similarity distance measures are provided: Levenshtein, Jaro, Jaro-Winkler, and Bag of Words.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The Levenshtein edit-distance algorithm computes the least number of edit operations (number of insertions, deletions, and substitutions) that are necessary to modify one string to obtain another string.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The Jaro distance measure considers the number of matching characters and transpositions.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Jaro-Winkler adds a prefix-weighting, giving higher match values to strings where prefixes match.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The Bag of Words measure looks at the number of matching words in a phrase, independent of order.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>In the implementation used in <ph id="ph1">`rxGetFuzzyDist`</ph>, all measures are normalized to the same scale, where 0 is no match and 1 is a perfect match.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>For information on phonetic conversions, see <bpt id="p1">[</bpt>rxGetFuzzyKeys<ept id="p1">](rxGetFuzzyKeys.md)</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>A data frame or data source containing the distances and either string and dictionary values or indexes.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxGetFuzzyKeys<ept id="p1">](rxGetFuzzyKeys.md)</ept>, <bpt id="p2">[</bpt>rxDataStep<ept id="p2">](rxDataStep.md)</ept></source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>