<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxgetfuzzykeys.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338ace9655edc1c18db612ccbb11d413d0550d586a04.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">ce9655edc1c18db612ccbb11d413d0550d586a04</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxgetfuzzykeys.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxGetFuzzyKeys function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>EXPERIMENTAL: Get fuzzy keys for a character vector</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxGetFuzzyKeys, manip</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxGetFuzzyKeys: Fuzzy keys for a character vector</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>EXPERIMENTAL: Get fuzzy keys for a character vector</source>
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
          <source>If <ph id="ph1">`NULL`</ph>, all variables are kept.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Ignored if data is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Method for matching to dictionary: 'none' for no matching, 'lv' for Levenshtein; 'j' for Jaro, 'jw' for JaroWinkler,  'bag' for bag of words, 'exact' for exact matching.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The default matchMethod is 'lv'.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Transformation type in creating keys: 'all' to retain all characters, 'alphanum' for alphanumeric characters only,  'alpha' for letters only", 'mphone3' for Metaphone3 phonetic transformation, 'soundex' for Soundex phonetic transformation,  'mphone3Vowels' for Metaphone3 encoding more than initial vowels, 'mphone3Exact' for Metaphone3 with more exact consonants, 'soundexNum' for Soundex with numbers only, 'soundexAll' for Soundex not truncated at 4 characters, and 'soundexAm' for the American variant of Soundex.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>A logical specifying whether or not to ignore case when comparing strings to the dictionary</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>A logical specifying whether or not to ignore spaces.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, for phonetic conversions each word in the string is processed separately and then concatenated together.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>A logical.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, numbers are converted to words before phonetic processing.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, numbers are ignored or removed.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>An optional character vector containing words to ignore when matching.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>A logical.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, if a match is not found an empty string is returned.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Only applies when dictionary is provided.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Minimum distance required for a match; applies only to distance metric algorithms (Levenshtein, Jaro, JaroWinkler).</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>One is a perfect match.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Zero is no similarity.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Character vector containing the dictionary for string comparisons.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Used for distance metric algorithms.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>from strings before processing.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>or a character string specifying the name to use for the newly created key variable.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the new variable name will be constructed using the <ph id="ph2">`stringsIn`</ph> variable name and <ph id="ph3">`.key`</ph>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Ignored if <ph id="ph1">`data`</ph> is <ph id="ph2">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>A named numeric vector with names <ph id="ph1">`insert`</ph>, <ph id="ph2">`delete`</ph>, and  <ph id="ph3">`subst`</ph> giving the respective costs for computing the Levenshtein distance.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The default uses unit cost for all three.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Ignored if Levenshtein distance not being used.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>or a character string specifying the name to use for a logical variable indicating whether word was matched to dictionary or not.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, no variable will be created.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>or a character string specifying the name to use for a numeric variable containing the distance of the match.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, no variable will be created.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>or a character string specifying the name to use for an integer variable containing the number of alternative matches were found that satisfied  <ph id="ph1">`minDistance`</ph> criterion .</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, no variable will be created.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>A logical.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> and the specified <ph id="ph2">`outFile`</ph> exists, it will be overwritten.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Two basic algorithms are provided, Soundex and Metaphone 3, with variations on both of them.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxGetFuzzyKeys`</ph> function can process a character vector of data, a character column in a data frame, or a string variable in a RevoScaleR data source.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The simplified Soundex algorithm creates a 4-letter code:  the first letter of the word as is, followed by 3 numbers representing consonants in the word, or zeros if necessary to fill out the four characters.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Non-alphabetical characters are ignored.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The Soundex method is used widely, and is available, for example, on the RootsWeb web site <bpt id="p1">[</bpt><ph id="ph1">`http://searches.rootsweb.ancestry.com/cgi-bin/Genea/soundex.sh`</ph><ept id="p1">](http://searches.rootsweb.ancestry.com/cgi-bin/Genea/soundex.sh)</ept> .</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>American Soundex differs slightly from standard simplified Soundex in its treatment of 'H' and 'W', which are treated differently when present between two other consonants.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>This is described by the U.S. National Archives <bpt id="p1">[</bpt><ph id="ph1">`http://www.archives.gov/research/census/soundex.html`</ph><ept id="p1">](http://www.archives.gov/research/census/soundex.html)</ept> .</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Another variant of Soundex is to code the first letter in the same way that all letters are coded, giving the first letter less importance.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Using <ph id="ph1">`soundexNums`</ph> as the <ph id="ph2">`keyType`</ph> provides this variant.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Another popular variant of Soundex is to continue coding all letters rather than stopping at 4.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Extra zeros are not added to fill out the code, so the result may be less than 4 characters.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>For this variant, use <ph id="ph1">`soundexAll`</ph> as the <ph id="ph2">`keyType`</ph>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Note that in this case, spaces are treated as vowels in separating consonants.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The Metaphone 3 algorithm was developed by Lawrence Philips, who designed and developed the original Metaphone algorithm in 1990 and the Double Metaphone algorithm in 2000.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Metaphone 3 is reported to increase the accuracy of phonetic encoding from the 89 against a database of the most common English words, and names and non-English words familiar in North America.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>In Metaphone3, all vowels are encoded to the same value - 'A'.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`mphone3`</ph> is used as the <ph id="ph2">`keyType`</ph>, only initial vowels will be encoded at all.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`mphone3Vowels`</ph> is used as the <ph id="ph2">`keyType`</ph>, 'A' will be encoded at all places in the word that any vowels are normally pronounced.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>'W' as well as 'Y' are treated as vowels.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`mphone3Exact`</ph> keyType is a variant of Metaphone3 that allows you to encode consonants as exactly as possible.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>This does not include 'S' vs. 'Z', since Americans will pronounce 'S' at the at the end of many words as 'Z', nor does it include 'CH' vs. 'SH'.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>It does cause a distinction to be made between 'B' and 'P', 'D' and 'T', 'G' and 'K', and 'V' and 'F'.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>In phonetic matching, all non-alphabetic characters are ignored, so that any strings containing numbers may give misleading results.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>This is typically handled by removing numbers from strings and handling them separately, but occasionally it is convenient to have the numbers converted to their phonetic equivalent.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>This is accomplished by setting the <ph id="ph1">`ignoreNumbers`</ph> parameter to FALSE.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Phonetic matching also typically treats the entire string as a single word.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Setting the <ph id="ph1">`ignoreSpaces`</ph> argument to <ph id="ph2">`TRUE`</ph> results in each word being processed separately, with the result concatenated into a single (longer) code.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>For information on similarity distance measures, see <bpt id="p1">[</bpt>rxGetFuzzyDist<ept id="p1">](rxGetFuzzyDist.md)</ept>.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>A character vector containing the fuzzy keys or a data source containing the fuzzy keys in a new variable.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxGetFuzzyDist<ept id="p1">](rxGetFuzzyDist.md)</ept>, <bpt id="p2">[</bpt>rxDataStep<ept id="p2">](rxDataStep.md)</ept></source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>