<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="extractpixels.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc77502fa26c0ae8f0340834b0ad7b025a4d1406b6a715.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">2fa26c0ae8f0340834b0ad7b025a4d1406b6a715</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\extractpixels.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>extractPixels function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Extracts the pixel values from an image.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), extractPixels, image, transform</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>extractPixels: Machine Learning Extract Pixel Data Transform</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Extracts the pixel values from an image.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A named list of character vectors of input variable names and the name of the output variable.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Note that the input variables must be of the same type.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>For one-to-one mappings between input and output variables, a named character vector can be used.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Specifies whether to use alpha channel.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Specifies whether to use red channel.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Specifies whether to use green channel.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Specifies whether to use blue channel.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Whether to separate each channel or interleave in ARGB order.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>This might be important, for example, if you are training a convolutional neural network, since this would affect the shape of the kernel, stride etc.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Whether to convert to floating point.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Specifies the offset (pre-scale).</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>This requires <ph id="ph1">`convert = TRUE`</ph>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Specifies the scale factor.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>This requires <ph id="ph1">`convert = TRUE`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>extracts the pixel values from an image.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The input variables are images of the same size, typically the output of a <ph id="ph1">`resizeImage`</ph> transform.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The output is pixel data in vector form that are typically used as features for a learner.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>A <ph id="ph1">`maml`</ph> object defining the transform.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>