<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="service-response.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b313c8325f8c7bae35966298d7ab4a867067231d8f.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">13c8325f8c7bae35966298d7ab4a867067231d8f</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\azureml-model-management-sdk\service-response.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>ServiceResponse class: from azureml-model-management-sdk Python module in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve">
          <source>Class ServiceResponse</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>ServiceResponse</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Represents the response from a service invocation.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The response will contain any outputs and file artifacts produced in addition to any console output or errors messages.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>api</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Gets the api endpoint.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>artifact</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A convenience function to look up a file artifact by name and optionally base64 decode it.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>artifact_name</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The name of the file artifact.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>decode</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Whether to decode the Base64 encoded artifact string.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The default is <ph id="ph1">`True`</ph>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>encoding</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The encoding scheme to be used.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The default is to apply no encoding.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>For a list of all encoding schemes please visit <bpt id="p1">*</bpt>Standard Encodings:<ept id="p1">*</ept><ph id="ph1">
</ph><bpt id="p2">[</bpt><ph id="ph2">https://docs.python.org/3/library/codecs.html#standard-encodings</ph><ept id="p2">](https://docs.python.org/3/library/codecs.html#standard-encodings)</ept></source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The file artifact as a Base64 encoded string if <ph id="ph1">`decode=False`</ph> otherwise the decoded string.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>artifacts</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Gets the non-decoded response file artifacts if present.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>:returns: A <ph id="ph1">`list`</ph> of non-decoded response file artifacts if present.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>console_output</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Gets the console output if present.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>error</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Gets the error if present.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>output</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>output</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The name of the output.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The service output’s value.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>outputs</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Gets the response outputs if present.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>raw_outputs</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Gets the raw response outputs if present.</source>
        </trans-unit></group></body></file></xliff>