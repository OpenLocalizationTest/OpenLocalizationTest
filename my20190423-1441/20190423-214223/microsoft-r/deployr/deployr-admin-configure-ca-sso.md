<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-admin-configure-ca-sso.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca864f92257578c5aa2213e76ad39627af721523385d.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">4f92257578c5aa2213e76ad39627af721523385d</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-admin-configure-ca-sso.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Configuring CA Single Sign-On - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to configure CA Single Sign-On for DeployR</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Configuring CA Single Sign-On for DeployR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept> (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Introduction</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This document is written as a guide for CA Single Sign-On (formerly known as SiteMinder) administrators interested in configuring CA Single Sign-On policies for use with DeployR.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>It is not meant to be a complete step-by-step manual, but rather offer enough instruction to permit experienced administrators to perform the necessary steps to configure for DeployR.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Please consult the <bpt id="p1">[</bpt>CA website<ept id="p1">](https://support.ca.com/)</ept> for the complete CA Single Sign-On documentation.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Create the Agent</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The first step to configuring CA Single Sign-On for DeployR is to create an agent.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>To create an agent:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>In the Administrative interface for CA Single Sign-On, click on the <bpt id="p1">**</bpt>Infrastructure<ept id="p1">**</ept> tab.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Agent<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Agents<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create a new object of type Agent<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Create Agent</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Name<ept id="p1">**</ept> field, enter the name <ph id="ph1">`deployr`</ph>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Submit<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Create the Agent Group</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The second step is to create an Agent Group.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>To create an agent group:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>In the Administrative interface for CA Single Sign-On, click on the <bpt id="p1">**</bpt>Infrastructure<ept id="p1">**</ept> tab.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Agent<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Agent Groups<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create Agent Group<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create a new object of type Agent Group<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Create Agent Group</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Name<ept id="p1">**</ept> field, enter the name <ph id="ph1">`deployrGroup`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Add/Remove<ept id="p1">**</ept> button.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Create Agent Group</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Select the <ph id="ph1">`deployr`</ph> agent from the list of available members and move it to <bpt id="p1">**</bpt>Selected Members<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Submit<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Create Agent Configuration Object</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>To create agent configuration objects:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Infrastructure, Agent Configuration Objects, Create Agent Group<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create Agent Configuration<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Create Agent Configuration</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Create a copy of an object of type Agent Configuration<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Select <ph id="ph1">`ApacheDefaultsSettings`</ph>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Modify Agent Configuration</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Name<ept id="p1">**</ept> field, enter the name <ph id="ph1">`deployrApacheSettings`</ph>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Click on <bpt id="p1">**</bpt>Submit<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Configure Agent Configuration Object</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>To configure new agent configuration objects:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Click on the pencil icon next to the <ph id="ph1">`deployrApacheSettings`</ph> object to enter the configuration page.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Configuration page</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>In the table, click on the pencil icon next to <ph id="ph1">`DefaultAgentName`</ph>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Enter the agent name that was created above.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Remove the preceding <ph id="ph1">\#</ph>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Modify Agent Configuration</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>In the table, click on the pencil icon to the left of <ph id="ph1">`BadUrlChars`</ph>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Update the <bpt id="p1">**</bpt>Value<ept id="p1">**</ept> to the following characters:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Modify Agent Configuration</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Click on the pencil icon next to <ph id="ph1">`LogoffUri`</ph>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Change the <bpt id="p1">**</bpt>Value<ept id="p1">**</ept> to:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Remove preceding <ph id="ph1">`#`</ph> character in the <bpt id="p1">**</bpt>Name<ept id="p1">**</ept> field.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Submit<ept id="p1">**</ept> to save all changes.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Create the Domain</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>A domain is a logical grouping of resources associated with one or more user directories.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To create a new domain<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>In the Administrative interface for CA Single Sign-On, click on the <bpt id="p1">**</bpt>Policies<ept id="p1">**</ept> tab.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Domain -<ph id="ph1">&amp;gt;</ph> Domains<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create Domain<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>General<ept id="p1">**</ept> tab, enter <ph id="ph1">`deployrDomain`</ph> in the <bpt id="p2">**</bpt>Name<ept id="p2">**</ept> field.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Create New Domain</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>User Directory<ept id="p1">**</ept> window, click <bpt id="p2">**</bpt>Create<ept id="p2">**</ept> and fill in the following info:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Create User Directory</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Submit<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Create the Realm &amp; Sub-Realms</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>A realm defines a group of resources with the same security or personalization requirements.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Each realm can only be associated with one agent/agent group and with one authorization scheme.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Conceptually, a realm is the door that protects the resources.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To create a realm<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Click the <bpt id="p1">**</bpt>Realms<ept id="p1">**</ept> tab.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create Realm<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Enter the following information in the form.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Create User Directory</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Rules<ept id="p1">**</ept> section, click <bpt id="p2">**</bpt>Create<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Enter the following information in the form.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Create User Directory</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Create the following sub-realms for your configuration using the values in the following table.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>There are no rules associated with the sub-realms.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Create Realm</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Name</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>ResourceFilter</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Create Responses</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>A response returns information to the web agent or redirects the user to another site and must be paired with a rule.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>It can be a static response or a value from Active Directory.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Responses are only available to protected resources.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To create responses<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Click on <bpt id="p1">**</bpt>Policies<ept id="p1">**</ept><ph id="ph1"> -</ph><ph id="ph2">&amp;gt;</ph> <bpt id="p2">**</bpt>Domain<ept id="p2">**</ept><ph id="ph3"> -</ph><ph id="ph4">&amp;gt;</ph> <bpt id="p3">**</bpt>Create Responses<ept id="p3">**</ept>.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Enter the following information in the form.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Create Response</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create Response Attribute<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Create Response Attribute<ept id="p1">**</ept> window appears.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Fill in the information as shown in the image below.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Create Response Attribute</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Submit<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Create Response Groups</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Policies<ept id="p1">**</ept><ph id="ph1"> -</ph><ph id="ph2">&amp;gt;</ph> <bpt id="p2">**</bpt>Domain<ept id="p2">**</ept><ph id="ph3"> -</ph><ph id="ph4">&amp;gt;</ph> <bpt id="p3">**</bpt>Response Groups<ept id="p3">**</ept>.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create Response Group<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Enter the following information in the form.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Create Response</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Add/Remove<ept id="p1">**</ept> and add <ph id="ph1">`deployrGroupResponse`</ph>.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Create Response</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Move <ph id="ph1">`deployrGroupResponse`</ph> from <bpt id="p1">**</bpt>Available Members<ept id="p1">**</ept> to <bpt id="p2">**</bpt>Selected Members<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Submit<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Create the Policy</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Policies define how users can interact with resources.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>When a user creates policies in the <bpt id="p1">**</bpt>Policy Server User Interface<ept id="p1">**</ept>, he or she links together (binds) objects that identify users, resources, and actions associated with the resources.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Policies<ept id="p1">**</ept><ph id="ph1"> -</ph><ph id="ph2">&amp;gt;</ph> <bpt id="p2">**</bpt>Domain<ept id="p2">**</ept><ph id="ph3"> -</ph><ph id="ph4">&amp;gt;</ph> <bpt id="p3">**</bpt>Domain Policies<ept id="p3">**</ept>.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create Policy<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Fill in the following information in the form.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Create Policy</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Click the <bpt id="p1">**</bpt>Users<ept id="p1">**</ept> tab.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Add Members</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Add Members<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Add Members</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Select <ph id="ph1">`CN=scriptGroup,OU=engineering,DC=revolution,DC=com`</ph>.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Add Members</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Add Rule<ept id="p1">**</ept> and select <ph id="ph1">`GeneralRuleDeployr`</ph>.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Submit<ept id="p1">**</ept>.</source>
        </trans-unit></group></body></file></xliff>