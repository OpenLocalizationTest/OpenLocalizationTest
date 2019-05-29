<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="ensembleControl.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b36858207d14b0ecd52c8774f2a73bf8d39dde3347.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">6858207d14b0ecd52c8774f2a73bf8d39dde3347</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\ensembleControl.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>ensembleControl function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Control the parameters used to create an ensemble.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), ensembleControl</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>ensembleControl: ensembleControl</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Control the parameters used to create an ensemble.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Specifies the random seed.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Specifies the number of models to train.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`1`</ph>, meaning no ensembling occurs.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>A logical value specifying if the sampling of observations should be done with  or without replacement.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>a scalar of positive value specifying the percentage of observations to sample for  each trainer.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The default is 1.0 for sampling with replacement (i.e., replace=TRUE) and 0.632  for sampling without replacement (i.e., replace=FALSE).</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>A logical value that specifies whether or not to train the base models  on non-overlapping partitions.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The default is <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>It is available only for <ph id="ph1">`RxSpark`</ph> compute context and is ignored for others.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Specifies the method used to combine the models:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>to compute the median of the individual model outputs,</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>to compute the average of the individual model outputs and</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>to compute (pos-neg) / the total number of models, where 'pos' is the number of positive outputs  and 'neg' is the number of negative outputs.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`median`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Not used currently.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>A list of ensemble parameters.</source>
        </trans-unit></group></body></file></xliff>