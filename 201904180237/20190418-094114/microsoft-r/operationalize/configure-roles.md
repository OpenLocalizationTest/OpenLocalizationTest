<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="configure-roles.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea9269b50f893c052aff89e9ca0c1687039d042841e99.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9b50f893c052aff89e9ca0c1687039d042841e99</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\configure-roles.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Control web services permissions with roles RBAC - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Role based access control in Machine Learning Server using roles like owner, contributor, reader</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Roles and permissions (RBAC)</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Machine Learning Server, Microsoft R Server 9.1<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server (and R Server), Role-Based Access Control (RBAC) enables fine-grained access management for the operationalization APIs.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Using RBAC, you can grant only the level of access that users need to perform their jobs.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>This article helps you get up and running with RBAC.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>By default, all authenticated users can publish/deploy, list, and get any web services as well as call all APIs.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Additionally, users can also update and delete the web services they have deployed.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Use the roles defined in this article to restrict who can call the APIs and publish, update, and delete web services.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>How users are assigned to roles depends on the authentication method configured for Machine Learning Server.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>For more on configuring authentication, read the article, <bpt id="p1">[</bpt>"Authentication options."<ept id="p1">](configure-authentication.md)</ept></source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>These roles are not the same as RBAC in Azure Active Directory.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>While the default roles described here-in bear the same names as the roles you can define in Azure, it is not possible to inherit the Azure roles.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If you want role-based access control over web services and APIs, you must set up roles again in Machine learning server.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>What do I need?</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>To assign groups of users in your Active Directory to Machine Learning Server roles, you must have:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>An instance of Machine Learning Server that is <bpt id="p1">[</bpt>configured to operationalize analytics<ept id="p1">](configure-start-for-administrators.md#configure-server-for-operationalization)</ept></source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Authentication for this instance must be via Active Directory/LDAP (AD/LADP) or Azure Active Directory (AAD) and <bpt id="p1">[</bpt>already configured<ept id="p1">](configure-authentication.md)</ept></source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The names of the groups that contain the users to whom you want to give special permissions</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Security groups versus Machine Learning Server roles</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>In AD/LDAP and AAD, security groups are used to collect user accounts, computer accounts, and other groups into manageable units.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Working with groups instead of with individual users helps simplify network maintenance and administration.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Your organization might have groups like 'Admin', 'Engineering', 'Level3', and so on.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>And, users might belong to more than one group.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>You can use the AD groups you have already defined in your organization to assign a collection of users to roles for web services.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Security group names must be unique across your LDAP/AAD configuration in order to be assigned to a Machine Learning Server role.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If a group in LDAP or AAD bears the same name as another group in that LDAP or AAD directory, then it cannot be assigned to a role in Machine Learning Server or R Server.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server, the administrator can assign one or more Active Directory groups to one or more of the following roles: 'Owner', 'Contributor', and 'Reader'.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Roles give specific permissions related to deploying and interacting with web services and other APIs.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>- Owner (highest permissions)</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><ph id="ph1">-</ph><ph id="ph2">&amp;nbsp;</ph>Contributor<ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph><ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph><ph id="ph7">&amp;nbsp;</ph><ph id="ph8">&amp;nbsp;</ph><ph id="ph9">&amp;nbsp;</ph><ph id="ph10">&amp;nbsp;</ph><ph id="ph11">&amp;nbsp;</ph><ph id="ph12">&amp;nbsp;</ph><ph id="ph13">&amp;nbsp;</ph><ph id="ph14">&amp;nbsp;</ph><ph id="ph15">&amp;nbsp;</ph><ph id="ph16">&amp;nbsp;</ph></source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>- Reader</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Checkbox</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Roles and their permissions</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>When roles are declared in the configuration file, the administrator has the choices of putting groups (of users) into these roles.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Role</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Permitted</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Prohibited</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Owner</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>These users can manage any service and call any API, including centralized configuration APIs.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Web service APIs:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; Publish <bpt id="p1">**</bpt>any<ept id="p1">**</ept> service</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; Update <bpt id="p1">**</bpt>any<ept id="p1">**</ept> service</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; Delete <bpt id="p1">**</bpt>any<ept id="p1">**</ept> service</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; List <bpt id="p1">**</bpt>any<ept id="p1">**</ept> service</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; Consume <bpt id="p1">**</bpt>any<ept id="p1">**</ept> service</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Other APIs:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; Call <bpt id="p1">**</bpt>any<ept id="p1">**</ept> other API</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>No API restrictions</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Contributor</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>These users can publish/deploy services and manage the services they publish.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>They can also call most other APIs.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Web service APIs:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; Publish <bpt id="p1">**</bpt>any<ept id="p1">**</ept> service</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; Update their services</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; Delete their services</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; List <bpt id="p1">**</bpt>any<ept id="p1">**</ept> service</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; Consume <bpt id="p1">**</bpt>any<ept id="p1">**</ept> service</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Other APIs:</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; Call almost any other API</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2716; Update service published by another</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2716; Delete service published by another</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2716; Centralized node configuration (v9.2+)</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Reader</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server 9.2+, these users can list and consume any service and call most other APIs.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>In R Server 9.1, this catchall role is implicitly given to any authenticated user  not assigned a role.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Users can list and consume services.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Never explicitly declared.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Web service APIs:</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; List <bpt id="p1">**</bpt>any<ept id="p1">**</ept> service</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; Consume <bpt id="p1">**</bpt>any<ept id="p1">**</ept> service</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Other APIs:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2714; Call almost any other APIs</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2716; Publish <bpt id="p1">**</bpt>any<ept id="p1">**</ept> service</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2716; Update <bpt id="p1">**</bpt>any<ept id="p1">**</ept> service</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2716; Delete <bpt id="p1">**</bpt>any<ept id="p1">**</ept> service</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><ph id="ph1">&amp;nbsp;</ph>&amp;#x2716; Centralized node configuration (v9.2+)</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>How are roles assigned</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>When a user calls a Machine Learning Server API, the server checks to see whether any roles were declared.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>When roles are declared, Machine Learning Server checks to see to which group the user belongs.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>If the user belongs to an AD/LDAP or AAD group assigned to a role, then that user is  given permissions according to their role.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>If a user belongs to groups that are assigned to multiple roles, then the user is assigned to the role with the highest permissions.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Here is an example of different LDAP group configurations and the resulting roles assigned to the persona.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Example User</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>/ Persona</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>User's</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>LDAP Groups</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Machine<ph id="ph1">&amp;nbsp;</ph>Learning<ph id="ph2">&amp;nbsp;</ph>Server</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>RBAC Configuration</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>User's</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Role</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Checkbox</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Administrator</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>admins<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>engineering</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>FTE-north</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>"Owner":<ph id="ph1">&amp;nbsp;</ph>["<bpt id="p1">**</bpt>admins<ept id="p1">**</ept>",<ph id="ph2">&amp;nbsp;</ph>"managers"],<ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph><ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph><ph id="ph7">&amp;nbsp;</ph><ph id="ph8">&amp;nbsp;</ph><ph id="ph9">&amp;nbsp;</ph><ph id="ph10">=</ph></source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>"Contributor": ["stats"]</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Owner<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Checkbox</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Lead data scientist</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>managers<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>stats<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>FTE-north</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>"Owner": ["admins", "<bpt id="p1">**</bpt>managers<ept id="p1">**</ept>"],<ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph><ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph><ph id="ph7">&amp;nbsp;</ph><ph id="ph8">=</ph></source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>"Contributor": ["<bpt id="p1">**</bpt>stats<ept id="p1">**</ept>"],</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>"Reader": ["app-devs"]</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Owner<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Checkbox</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>R programmer</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>stats<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>FTE-north</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>"Owner": ["admins", "managers"],<ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph><ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph><ph id="ph7">&amp;nbsp;</ph><ph id="ph8">=</ph></source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>"Contributor": ["<bpt id="p1">**</bpt>stats<ept id="p1">**</ept>"],</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>"Reader": ["app-devs"]</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Contributor<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Checkbox</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Python developer</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>stats</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>FTE-north</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>"Owner": ["admins", "managers"]<ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph><ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph><ph id="ph7">&amp;nbsp;</ph><ph id="ph8">=</ph></source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Contributor<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Checkbox</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Application<ph id="ph1">&amp;nbsp;</ph>Developer</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>app-devs<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>FTE-north</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>"Owner": ["admins", "managers"],<ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph><ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph><ph id="ph7">&amp;nbsp;</ph><ph id="ph8">=</ph></source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>"Contributor": ["stats"],</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>"Reader": ["<bpt id="p1">**</bpt>app-devs<ept id="p1">**</ept>"]</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Reader<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Checkbox</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>System Integrator</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>vendor2</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>"Owner": ["admins", "managers"],<ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph><ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph><ph id="ph7">&amp;nbsp;</ph><ph id="ph8">=</ph></source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>"Contributor": ["stats"]</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Reader<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Checkbox</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Sales</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>sales</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>"Owner": ["admins", "managers"],<ph id="ph1">&amp;nbsp;</ph><ph id="ph2">&amp;nbsp;</ph><ph id="ph3">&amp;nbsp;</ph><ph id="ph4">&amp;nbsp;</ph><ph id="ph5">&amp;nbsp;</ph><ph id="ph6">&amp;nbsp;</ph><ph id="ph7">&amp;nbsp;</ph><ph id="ph8">=</ph></source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>"Contributor": ["stats"]</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>"Reader": ["app-devs"]</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>no role or permissions</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Role configuration states</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>The permissions assigned to users are influenced not only by the roles you define, but also by the roles you <bpt id="p1">**</bpt>do not<ept id="p1">**</ept> define.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>When one or more roles is not defined, then certain permissions are implicitly assumed.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>By default, no roles are declared.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>The table shows which permissions are granted to those authenticated users who are not explicitly assigned to any role.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Possible configurations</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Users without a role are implicitly assigned to</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>- No roles: RBAC not configured</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Contributor</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>- Owner only</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>Contributor</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>- Contributor + Owner <ph id="ph1">&amp;nbsp;</ph><bpt id="p1">_</bpt>-or-<ept id="p1">_</ept></source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>- Contributor only</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Reader</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>- Reader + Contributor + Owner <ph id="ph1">&amp;nbsp;</ph><bpt id="p1">_</bpt>-or-<ept id="p1">_</ept></source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>- Reader + Owner <ph id="ph1">&amp;nbsp;</ph><bpt id="p1">_</bpt>-or-<ept id="p1">_</ept></source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>- Reader only</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>v9.2+:  all API access denied</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>v9.1: not applicable since Reader is never declared</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>How to declare roles</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>If you configure Machine Learning Server (or R Server) to <bpt id="p1">[</bpt>use Active Directory/LDAP or Azure Active Directory authentication<ept id="p1">](configure-authentication.md)</ept>, then you can assign roles using Active Directory groups as described here.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>If only the default local administrator account is defined for Machine Learning Server (or R Server), then roles are not needed.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>In this case, the 'admin' user is implicitly assigned to the Owner role (can call any API).</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>Step 1.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Define desired roles</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>On each web node, edit the appsettings.json configuration file in order to declare the roles and the groups that belong to them.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>Open the configuration file, <bpt id="p1">[</bpt><ph id="ph1">\&lt;</ph>web-node-install-path&gt;<ept id="p1">](../operationalize/configure-find-admin-configuration-file.md)</ept>/appsettings.json.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>Search for the following section: <ph id="ph1">`"Authorization": {`</ph></source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>In that section, add only the roles you need.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Then, map the security groups to each role you want to define such as:</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>The 'CacheLifeTimeInMinutes' attribute was added in Machine Learning Server 9.2.1.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>It indicates the length of time that Machine Learning Server caches the information received from LDAP or AAD regarding user group membership.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>After the cache lifetime elapses, the roles and users are checked again.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>The changes you make to the groups in your LDAP or AAD configuration are not reflected in  Machine Learning Server until the cache lifetime expires and the configuration is checked again.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>Defining a Reader role might affect web service consumption latency as roles are being validated on each call to the web service.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>For AD/LDAP authentications:</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>Be careful not to use the 'CN=' portion of the distinguished names.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>For example, if the distinguished name appears as 'CN=Administrators', enter only 'Administrators' here.</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>Ensure that the username returned for the value of 'UniqueUserIdentifierAttributeName' matches the username returned by 'SearchFilter'.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>For example, if <ph id="ph1">`"SearchFilter": "cn={0}"`</ph> and <ph id="ph2">`"UniqueUserIdentifierAttributeName": "userPrincipalName"`</ph>, then the values for <ph id="ph3">`cn`</ph> and <ph id="ph4">`userPrincipalName`</ph> must match.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>For R Server 9.1 users: If you specify LDAP Root as the SearchBase in web node's appsettings.json, a search of the roles returns <bpt id="p1">[</bpt>LDAP referrals<ept id="p1">](https://technet.microsoft.com/en-us/library/cc978014.aspx)</ept> and throws a 'LDAPReferralException'.</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>A workaround is to change the LDAP port in web node's appsettings.json from 389 to Global Catalog Port 3268.</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>Or, for LDAPS, change Port to 3269 instead of 636.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>Global Catalogs do not return LDAP referrals in LDAP Search Results.</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>Step 2.</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>Validate groups against AD/LDAP or AAD</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>Return to <bpt id="p1">[</bpt>the appsetting.json file<ept id="p1">](configure-find-admin-configuration-file.md)</ept> on each web node and make these updates:</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>For Azure Active Directory:<ept id="p1">**</ept> In appsettings.json, find the "AzureActiveDirectory" section.</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>Make sure the alphanumeric client key you created in the portal <bpt id="p1">**</bpt>for the web app<ept id="p1">**</ept> is used for "Key": property.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>This key allows Machine Learning Server to verify that the groups you've declared are valid in AAD.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>See following example.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>Learn more about <bpt id="p1">[</bpt>configuring Machine Learning Server to authenticate with Azure Active Directory<ept id="p1">](configure-authentication.md#aad)</ept>.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>For more security, we recommend you <bpt id="p1">[</bpt>encrypt the key<ept id="p1">](configure-admin-cli-encrypt-credentials.md)</ept> before adding the information to appsettings.json.</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>If a user belongs to more groups than allowed in AAD, AAD provides an overage claim in the token it returns.</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>This claim along with the key you provide here allows Machine Learning Server to retrieve the group memberships for the user.</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>For Active Directory/LDAP:<ept id="p1">**</ept> In appsettings.json, find the "LDAP" section.</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>The server verifies that the groups you have declared are valid in AD/LDAP using the QueryUserDn and QueryUserPassword values in the "LDAP" section.</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>See the following example: These settings allow Machine Learning Server to verify that each declared group is, in fact, a valid, existing group in AD.</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>Learn more about <bpt id="p1">[</bpt>configuring Machine Learning Server  to authenticate with Active Directory/LDAP<ept id="p1">](configure-authentication.md#ldap)</ept>.</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>With AD/LDAP, you can <bpt id="p1">**</bpt>restrict which users can log in and call APIs<ept id="p1">**</ept> by declaring the groups with permissions in the <bpt id="p2">[</bpt>'SearchFilter' LDAP property<ept id="p2">](configure-admin-cli-encrypt-credentials.md)</ept>.</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>Then, users in other groups are not able to call any APIs.</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>In this example, only members of the 'mrsreaders', 'mrsowners', and 'mrscontributors' groups can call APIs after logging in.</source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>Step 3.</source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>Apply the changes to Machine Learning Server / R Server</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Restart the web node<ept id="p1">](configure-admin-cli-stop-start.md)</ept> for the changes to take effect.</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>Log in  using <bpt id="p1">[</bpt>the local 'admin' account<ept id="p1">](configure-authentication.md#local)</ept> in the administration tool/CLI.</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>Repeat these changes in every web node you have configured.</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>The configuration must be the same across all web nodes.</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>Here is an example of roles declared for AD/LDAP in appsettings.json on the web node:</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>Web service permissions after role change</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source>Over time, a user role can change if they are no longer part of a security group in AD/LDAP or AAD, or if a security group is no longer mapped to a role in Machine Learning Server.</source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>Whenever a user's role changes, that user may not longer be able to perform the same tasks on their web services.</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source>If you publish a web service while assigned to the "Owner" role, you can continue to manage and interact with that web service version as long as you are assigned this role.</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>However, if you are reassigned to "Contributor", then you can still interact with that web service version as before, but you cannot update or delete the services published by others.</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source>Or, if roles are defined and you are no longer assigned to any roles, then you are implicitly assigned to the "Reader" role if it exists (<bpt id="p1">[</bpt>see here<ept id="p1">](#configroles)</ept>.</source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source>Consequently, you can no longer manage any services, including those services that you published previously when you were assigned to a role.</source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="324" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to publish and manage web services in R<ept id="p1">](how-to-deploy-web-service-publish-manage-in-r.md)</ept></source>
        </trans-unit><trans-unit id="325" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to interact with and consume web services in R<ept id="p1">](how-to-consume-web-service-interact-in-r.md)</ept></source>
        </trans-unit><trans-unit id="326" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Authentication options for Machine Learning Server when operationalizing analytics<ept id="p1">](configure-authentication.md)</ept></source>
        </trans-unit><trans-unit id="327" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Blog article: Role Based Access Control With MRS 9.1.0<ept id="p1">](https://blogs.msdn.microsoft.com/rserver/2017/04/10/role-based-access-control-with-mrs-9-1-0/)</ept></source>
        </trans-unit></group></body></file></xliff>