<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxserializemodel.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c49a487143f30ad2e263e59f625a9a17f8c2f0ebe.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">49a487143f30ad2e263e59f625a9a17f8c2f0ebe</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxserializemodel.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxSerializeModel function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Serialize a <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept><ph id="ph1">/</ph><bpt id="p2">**</bpt>MicrosoftML<ept id="p2">**</ept> model in raw format to enable saving the model.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This allows model to be loaded into SQL Server for real-time scoring.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxSerializeModel, rxUnserializeModel</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>rxSerializeModel:  RevoScaleR Model Serialization and Unserialization</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Serialize a <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept><ph id="ph1">/</ph><bpt id="p2">**</bpt>MicrosoftML<ept id="p2">**</ept> model in raw format to enable saving the model.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This allows model to be loaded into SQL Server for real-time scoring.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`RevoScaleR`</ph><ph id="ph2">/</ph><ph id="ph3">`MicrosoftML`</ph> model to be serialized</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Arbitrary metadata of <ph id="ph1">`raw`</ph> type to be stored with the serialized model.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Metadata will be returned when unserialized.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Drops fields not required for real-time scoring.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>NOTE: Setting this flag could reduce the model size but <ph id="ph1">`rxUnserializeModel`</ph> can no longer retrieve the RevoScaleR model</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Serialized model to be unserialized</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxSerializeModel`</ph> converts models into <ph id="ph2">`raw`</ph> bytes to allow them to be saved and used for real-time scoring.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The following is the list of models that are currently supported in real-time scoring:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>rxLogit</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>rxLinMod</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>rxBTrees</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>rxDTree</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>rxDForest</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>MicrosoftML<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>rxFastTrees</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>rxFastForest</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>rxLogisticRegression</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>rxOneClassSvm</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>rxNeuralNet</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>rxFastLinear</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> models containing R transformations or transform based formula (e.g <ph id="ph1">`"A ~ log(B)"`</ph>) are not supported in real-time scoring.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Such transforms to input data may need to be handled before calling real-time scoring.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxUnserializeModel`</ph> method is used to retrieve the original R model object and metadata from the serialized raw model.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxSerializeModel`</ph> returns a serialized model.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxUnserializeModel`</ph> returns original R model object.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If metadata is also present returns a list containing the original model object and metadata.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>