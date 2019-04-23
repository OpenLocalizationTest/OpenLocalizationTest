<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="operationalization.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86c8a8f5db3340e52516a9d889e787a513ae94c276.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">c8a8f5db3340e52516a9d889e787a513ae94c276</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\azureml-model-management-sdk\operationalization.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Operationalization class: from azureml-model-management-sdk Python module in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve">
          <source>Class Operationalization</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Operationalization</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Operationalization<ept id="p1">*</ept> is designed to be a low-level abstract foundation class from which other service operationalization attribute classes in the <bpt id="p2">*</bpt>mldeploy<ept id="p2">*</ept> package can be derived.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>It provides a standard template for creating attribute-based operationalization lifecycle phases providing a consistent  <bpt id="p1">*</bpt><bpt id="p2">__</bpt>init()<ept id="p2">__</ept><ept id="p1">*</ept>, <bpt id="p3">*</bpt><bpt id="p4">__</bpt>del()<ept id="p4">__</ept><ept id="p3">*</ept> sequence that chains initialization (initializer), authentication (authentication), and destruction (destructor) methods for the class hierarchy.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>authentication</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Authentication lifecycle method.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Invokes the authentication entry-point for the class hierarchy.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>An optional <bpt id="p1">_</bpt>noonp<ept id="p1">_</ept> method where subclass implementers MAY provide this method definition by overriding.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Sub-class should override and implement.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>context</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The optional authentication context as defined in the implementing sub-class.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>delete_service</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Sub-class should override and implement.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>deploy_realtime</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Sub-class should override and implement.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>deploy_service</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Sub-class should override and implement.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>destructor</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Destroy lifecycle method.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Invokes destructors for the class hierarchy.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>An optional <bpt id="p1">_</bpt>noonp<ept id="p1">_</ept> method where subclass implementers MAY provide this method definition by overriding.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Sub-class should override and implement.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>get_service</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Retrieve service meta-data from the name source and return a new service instance.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Sub-class should override and implement.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>initializer</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Init lifecycle method, invoked during construction.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Sets up attributes and invokes initializers for the class hierarchy.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>An optional <bpt id="p1">_</bpt>noonp<ept id="p1">_</ept> method where subclass implementers MAY provide this method definition by overriding.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Sub-class should override and implement.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>list_services</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Sub-class should override and implement.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>realtime_service</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Begin fluent API chaining of properties for defining a <bpt id="p1">*</bpt>real-time<ept id="p1">*</ept> web service.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The web service name.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt><ph id="ph1">`RealtimeDefinition`</ph><ept id="p1">](realtime-definition.md)</ept> instance for fluent API chaining.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Sub-class should override and implement.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>redeploy_service</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Sub-class should override and implement.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>service</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Begin fluent API chaining of properties for defining a <bpt id="p1">*</bpt>standard<ept id="p1">*</ept> web service.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Example:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>name</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The web service name.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">[</bpt><ph id="ph1">`ServiceDefinition`</ph><ept id="p1">](service-definition.md)</ept> instance for fluent API chaining.</source>
        </trans-unit></group></body></file></xliff>