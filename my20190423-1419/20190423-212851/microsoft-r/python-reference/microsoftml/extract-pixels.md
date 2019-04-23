<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="extract-pixels.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338add48bea546a14f589bbf1e237af5f25a4fc3300d.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">dd48bea546a14f589bbf1e237af5f25a4fc3300d</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\extract-pixels.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>extract_pixels: Machine Learning Extract Pixel Data Transform</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Extracts the pixel values from an image.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>transform, image</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.extract_pixels<ept id="p1">*</ept>: Extracts pixels from an image</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Extracts the pixel values from an image.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>extracts the pixel values from an image.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The input variables are images of the same size, typically the output of a <ph id="ph1">`resizeImage`</ph> transform.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The output is pixel data in vector form that are typically used as features for a learner.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>cols</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A character string or list of variable names to transform.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`dict`</ph>, the keys represent the names of new variables to be created.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>use_alpha</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Specifies whether to use alpha channel.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`False`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>use_red</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Specifies whether to use red channel.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`True`</ph>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>use_green</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Specifies whether to use green channel.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`True`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>use_blue</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Specifies whether to use blue channel.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`True`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>interleave_argb</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Whether to separate each channel or interleave in ARGB order.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>This might be important, for example, if you are training a convolutional neural network, since this would affect the shape of the kernel, stride etc.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>convert</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Whether to convert to floating point.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`False`</ph>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>offset</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Specifies the offset (pre-scale).</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>This requires <ph id="ph1">`convert = True`</ph>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>scale</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Specifies the scale factor.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>This requires <ph id="ph1">`convert = True`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The default value is <bpt id="p1">*</bpt>None<ept id="p1">*</ept>.</source>
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
          <source><bpt id="p1">[</bpt><ph id="ph1">`load_image`</ph><ept id="p1">](load-image.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`resize_image`</ph><ept id="p2">](resize-image.md)</ept>, <bpt id="p3">[</bpt><ph id="ph3">`featurize_image`</ph><ept id="p3">](featurize-image.md)</ept>.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit></group></body></file></xliff>