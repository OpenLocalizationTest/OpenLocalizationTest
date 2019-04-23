<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="resize-image.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338abe74ff0adee2d8f4486b273200d2ea26643e09a0.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be74ff0adee2d8f4486b273200d2ea26643e09a0</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\resize-image.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>resize_image: Machine Learning Resize Image Transform</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Resizes an image to a specified dimension using a specified resizing method.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>transform, image</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>microsoftml.resize_image<ept id="p1">*</ept>: Resizes an Image</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Resizes an image to a specified dimension using a specified resizing method.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>resizes an image to the specified height and width using a specified resizing method.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The input variables to this transform must be images, typically the result of the <ph id="ph1">`load_image`</ph> transform.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>cols</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>A character string or list of variable names to transform.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`dict`</ph>, the keys represent the names of new variables to be created.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>width</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Specifies the width of the scaled image in pixels.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The default value is 224.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>height</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Specifies the height of the scaled image in pixels.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The default value is 224.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>resizing_option</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Specified the resizing method to use.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Note that all methods are using bilinear interpolation.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The options are:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>: The image is resized such that the aspect ratio is preserved.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If needed, the image is padded with black to fit the new width or height.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>: The image is resized such that the aspect ratio is preserved.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If needed, the image is cropped to fit the new width or height.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>: The image is stretched to the new width and height, without preserving the aspect ratio.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`"IsoPad"`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>kargs</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Additional arguments sent to compute engine.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>An object defining the transform.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`load_image`</ph><ept id="p1">](load-image.md)</ept>, <bpt id="p2">[</bpt><ph id="ph2">`extract_pixels`</ph><ept id="p2">](extract-pixels.md)</ept>, <bpt id="p3">[</bpt><ph id="ph3">`featurize_image`</ph><ept id="p3">](featurize-image.md)</ept>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Output:</source>
        </trans-unit></group></body></file></xliff>