<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="updateservice.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338aff02571b41bafb069c913bd7ee37ebf41383f515.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">ff02571b41bafb069c913bd7ee37ebf41383f515</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\mrsdeploy\updateservice.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>updateService function (mrsdeploy) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Updates an existing web service on an R Server instance.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(mrsdeploy), updateService</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>updateService: Updates an existing web service.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Updates an existing web service on an R Server instance.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A string representing the web service name.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Use quotes such as  "MyService".</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The version of the web service you want to update.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>(optional) For standard web services, the R code to publish if you are  updating the code.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If you use a path, the base path is your local current working directory.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>can take the form of:</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>A function handle such as</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>A block of arbitrary R code as a character string such as</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>A filepath to a local <ph id="ph1">`.R`</ph> file containing R code such as <ph id="ph2">`code = "/path/to/R/script.R"`</ph> If serviceType is 'Realtime', code has to be NULL.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>(optional) For standard web services, an <ph id="ph1">`object`</ph> or a filepath to an external representation of R objects to be loaded and used  with <ph id="ph2">`code`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The specified file can be:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Filepath to a local <ph id="ph1">`.RData`</ph> file holding R objects to be loaded.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>For example,</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Filepath to a local <ph id="ph1">`.R`</ph> file that is evaluated into an environment and loaded.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>For example,</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>An object.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>For example,  <ph id="ph1">`model = "model = am.glm"`</ph> For real-time web services (serviceType = 'Realtime'), only an R model  object is accepted.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>For example,</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>(optional) Identifier of the session snapshot to load.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Can replace the model argument or be merged with it.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If serviceType is 'Realtime', snapshot has to be NULL.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>(optional) Defines the web service input schema.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>If empty, the service will not accept inputs.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>are defined as a named list  <ph id="ph1">`list(x = "logical")`</ph> which describes the input parameter  names and their corresponding <bpt id="p1">**</bpt>data types<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If serviceType is 'Realtime', inputs has to be NULL.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Once published,  service inputs automatically default to  list(inputData = 'data.frame').</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>(optional) Defines the web service output schema.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If empty, the service will not return a response value.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>are defined as a  named list <ph id="ph1">`list(x = "logical")`</ph> that describes the output parameter  names and their corresponding <bpt id="p1">**</bpt>data types<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Note: If <ph id="ph1">`code`</ph> is defined as a <ph id="ph2">`function`</ph>, then only one output value can be claimed.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If serviceType is 'Realtime', outputs has to be NULL.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Once published,  service outputs automatically default to  list(inputData = 'data.frame').</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>(optional) A character vector of filenames defining which file artifacts should be returned during service consumption.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>File content is encoded as a <ph id="ph1">`Base64 String`</ph>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>(optional) An alias name of the prediction remote procedure call (RPC) function used to consume the service.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>If code is a function,  then it will use that function name by default.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>(optional) The codegen output directory location.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>(optional) The description of the web service.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>(optional) The type of the web service.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Valid values are  'Script' and 'Realtime'.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Defaults to 'Script', which is for a standard web  service, contains arbitrary R code, R scripts and/or models.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>'Realtime' contains only a supported model object (see 'model' argument above).</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Complete documentation: <bpt id="p1">[</bpt><ph id="ph1">`https://go.microsoft.com/fwlink/?linkid=836352`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?linkid=836352)</ept></source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Updates an existing service by <ph id="ph1">`name`</ph> and version <ph id="ph2">`v`</ph>.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Other service methods: <bpt id="p1">[</bpt>deleteService<ept id="p1">](deleteService.md)</ept>, <bpt id="p2">[</bpt>getService<ept id="p2">](getService.md)</ept>, <bpt id="p3">[</bpt>listServices<ept id="p3">](listServices.md)</ept>, <bpt id="p4">[</bpt>print.serviceDetails<ept id="p4">](print.serviceDetails.md)</ept>, <bpt id="p5">[</bpt>publishService<ept id="p5">](publishService.md)</ept>, <bpt id="p6">[</bpt>serviceOption<ept id="p6">](serviceOption.md)</ept>, <bpt id="p7">[</bpt>summary.serviceDetails<ept id="p7">](summary.serviceDetails.md)</ept></source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>