<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-security-authentication.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca8668e308020fc1d8e0b32ca1fb8f85a55b971d206c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">68e308020fc1d8e0b32ca1fb8f85a55b971d206c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-security-authentication.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Authentication and Authorization - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Security in DeployR: Authentication, HTTPS, SSL, and access controls for server, Project file and Repository File, and more.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Authentication and Authorization</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>DeployR ships with security providers for the following enterprise security solutions:</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Basic Authentication</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>LDAP / LDAP-S Authentication</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Active Directory Services</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>PAM Authentication Services</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>CA Single Sign-On</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>R Session Process Controls</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The DeployR security model is sufficiently flexible that it can work with multiple enterprise security solutions at the same time.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If two or more enterprise security solutions are active, then user credentials are evaluated by each of the DeployR security providers in the order indicated in preceding list.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If a security provider, at any depth in the provider-chain, establishes that the credentials are valid, then the login call succeeds.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If the user credentials are not validated by any of the security providers in the provider-chain, then the login call fails.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>When DeployR processes a user login, there are two key steps involved:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Credentials must be authenticated</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Access privileges must be determined</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>DeployR access privileges are determined by the roles assigned to a user.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>In the case of basic authentication, an administrator simply assigns roles to a user within the DeployR Administration Console.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Learn More!</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>For information on how to manage user accounts as well as how to use roles as a means to assign access privileges to a user or to restrict access to individual R scripts, refer to the <bpt id="p1">[</bpt>Administration Console Help<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>When you integrate with an external enterprise security solution, you want access privileges to be inherited from the external system.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>This is achieved with simple mappings in the DeployR configuration properties, which link external groups to internal roles.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Basic Authentication</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>By default, the Basic Authentication security provider is enabled.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The Basic Authentication provider is enabled by default and there are no additional security configuration properties for this provider.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If you enable <bpt id="p1">[</bpt>Active Directory Services<ept id="p1">](#active-directory-authentication)</ept> or <bpt id="p2">[</bpt>CA Single Sign-On (SiteMinder)<ept id="p2">](#ca-single-sign-on-siteminder-pre-authentication)</ept>, Basic Authentication is automatically disabled and you will no longer be able to login with the default users <ph id="ph1">`admin`</ph> and <ph id="ph2">`testuser`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">[</bpt>PAM Authentication Services<ept id="p1">](#pam-authentication)</ept> and <bpt id="p2">[</bpt>LDAP<ept id="p2">](#ldap)</ept> scenarios, basic authentication remains enabled even with PAM or LDAP enabled.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>LDAP / LDAP-S Authentication</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>By default, the <bpt id="p1">**</bpt>LDAP<ept id="p1">**</ept> security provider is disabled.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>To enable LDAP authentication support, you must update the relevant properties in your DeployR external configuration file.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The values you assign to these properties should match the configuration of your LDAP Directory Information Tree (DIT).</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The standard protocol for reading data from and writing data to Active Directory (AD) domain controllers (DCs) is LDAP.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>AD LDAP traffic is unsecured by default, which makes it possible to use network-monitoring software to view the LDAP traffic between clients and DCs.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>You can make LDAP traffic confidential and secure using Secure Sockets Layer (SSL) / Transport Layer Security (TLS) technology.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>This combination is referred to as LDAP over SSL (or LDAP-S).</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>To ensure that no one else can read the traffic, SSL/TLS establishes an encrypted tunnel between an LDAP client and a DC.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Learn more about enabling SSL/TLS for DeployR.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Reasons for enabling LDAP-S include:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Organizational security policies typically require that all client/server communication is encrypted.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Applications use simple BIND to transport credentials and authenticate against a DC.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>As simple BIND exposes the users’ credentials in clear text, using SSL/TLS to encrypt the authentication session is strongly recommended.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Use of proxy binding or password change over LDAP, which requires LDAP-S.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Bind to an AD LDS instance Through a Proxy Object</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Applications that integrate with LDAP servers (such as Active Directory or Active Directory Domain Controllers) might require encrypted LDAP communications.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Basic authentication remains enabled even with LDAP enabled.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>To enable LDAP or LDAP-S:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The LDAP and Active Directory security providers are one and the same, but their <bpt id="p1">[</bpt>configuration properties<ept id="p1">](#ldap-active-directory-configuration-properties)</ept> differ.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>As such, you may enable the LDAP provider or the Active Directory provider, but not both at the same time.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Accordingly, to enable do the following:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Set</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Uncomment only the LDAP properties</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Make sure the Active Directory section is commented out <bpt id="p1">**</bpt>except<ept id="p1">**</ept> for this line which should be <bpt id="p2">**</bpt>set to false<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>For each property, use the value matching your configuration.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>For more information, see the complete list of LDAP <bpt id="p1">[</bpt>configuration properties<ept id="p1">](#ldap-active-directory-configuration-properties)</ept>.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>For LDAP, set <ph id="ph1">`grails.plugin.springsecurity.ldap.context.server`</ph> to the LDAP server URL, such as <ph id="ph2">`'ldap://localhost:389/'`</ph>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>For LDAPS, set <ph id="ph1">`grails.plugin.springsecurity.ldap.context.server`</ph> to the LDAP-S server URL, such as <ph id="ph2">`'ldaps://localhost:636/'`</ph>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>If you have enabled PAM authentication as part of the required steps for enabling R Session Process Controls, then please continue with your configuration using <bpt id="p1">[</bpt>these steps<ept id="p1">](#r-session-process-controls)</ept>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Active Directory Authentication</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>By default, the Active Directory security provider is disabled.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>To enable Active Directory authentication support you must update the relevant properties in your DeployR external configuration file.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>The values you assign to these properties should match the configuration of your Active Directory Directory Information Tree (DIT).</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>To enable Active Directory:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The LDAP and Active Directory security providers are one and the same, but their <bpt id="p1">[</bpt>configuration properties<ept id="p1">](#ldap-active-directory-configuration-properties)</ept> differ.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>As such, you may enable the LDAP provider or the Active Directory provider, but not both at the same time.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Accordingly, to enable do the following:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Set</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Uncomment only the Active Directory properties</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Make sure the LDAP section is commented out <bpt id="p1">**</bpt>except<ept id="p1">**</ept> for this line which should be <bpt id="p2">**</bpt>set to false<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>For each property, use the value matching your configuration.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>For DeployR for Microsoft R Server 8.0.5:</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>For DeployR 8.0.0</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>For more information, see the complete list of <bpt id="p1">[</bpt>configuration properties<ept id="p1">](#ldap-active-directory-configuration-properties)</ept>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>LDAP &amp; Active Directory Configuration Properties</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The following table presents the complete list of LDAP and Active Directory configuration properties.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>To use one of these configuration properties in the <ph id="ph1">`deployr.groovy`</ph> external configuration file, you must prefix the property name with <ph id="ph2">`grails.plugin.springsecurity`</ph>.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>For example, to use the <ph id="ph1">`ldap.context.server='ldap://localhost:389'`</ph> property in <ph id="ph2">`deployr.groovy`</ph>, you must write the property as such:</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;sup&gt;</bpt><ph id="ph1">\*</ph><ept id="p1">&lt;/sup&gt;</ept> These properties are for Active Directory.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Context Properties</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Property</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Default Value</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>providerNames<bpt id="p1">&lt;sup&gt;</bpt><ph id="ph1">\*</ph><ept id="p1">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>'ldapAuthProvider1'</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Do not change or omit.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Used for password management.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>ldap.server<bpt id="p1">&lt;sup&gt;</bpt><ph id="ph1">\*</ph><ept id="p1">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>'ldap://localhost:389'</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Address of the Active Directory server.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>ldap.context.server</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>'ldap://localhost:389'</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>'ldaps://localhost:636'</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Address of the LDAP server.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Address of the LDAP-S server.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>ldap.context.managerDn</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>"'cn=admin,dc=example,dc=com'"</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>DN to authenticate with.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>ldap.context.managerPassword</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>secret'</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Manager password to authenticate with.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>ldap.context.baseEnvironmentProperties</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>None</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Extra context properties.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>ldap.context.cacheEnvironmentProperties</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>TRUE</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Whether environment properties should be cached between requests.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>ldap.context.anonymousReadOnly</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>FALSE</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Whether an anonymous environment should be used for read-only operations.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>ldap.context.referral</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>null ('ignore')</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>The method to handle referrals.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Can be 'ignore' or 'follow' to enable referrals to be automatically followed.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Search Properties</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Property</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Default Value</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>ldap.search.base</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>"'ou=users,dc=example,dc=com'"</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>"Context name to search in, relative to the base of the configured ContextSource, e.g. 'ou=users,dc=example,dc=com'."</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>ldap.search.searchSubtree</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>TRUE</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>"If true then searches the entire subtree as identified by context, if false (the default) then only searches the level identified by the context."</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>ldap.search.derefLink</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>FALSE</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Enables/disables link dereferencing during the search.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>ldap.search.timeLimit</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>0 (unlimited)</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>The time to wait before the search fails.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>ldap.search.attributesToReturn</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>null (all)</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>The attributes to return as part of the search.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>ldap.authenticator.dnPatterns</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>null (none)</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>"Optional pattern(s) used to create DN search patterns, e.g. <ph id="ph1">\[</ph>""cn=<ph id="ph2">{0}</ph>,ou=people""<ph id="ph3">\]</ph>."</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>ldap.authenticator.attributesToReturn</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>null (all)</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Names of attribute IDs to return; use null to return all and an empty list to return none.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Authorities Properties</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Property</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Default Value</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>ldap.authorities.retrieveGroupRoles<bpt id="p1">&lt;sup&gt;</bpt><ph id="ph1">\*</ph><ept id="p1">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>TRUE</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Whether to infer roles based on group membership.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>ldap.authorities.retrieveDatabaseRoles</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>FALSE</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Whether to retrieve additional roles from the database using the User/Role many-to-many.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>ldap.authorities.groupRoleAttribute</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>'cn'</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>The ID of the attribute which contains the role name for a group.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>ldap.authorities.groupSearchFilter<bpt id="p1">&lt;sup&gt;</bpt><ph id="ph1">\*</ph><ept id="p1">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>'uniquemember=<ph id="ph1">{0}</ph>'</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>The pattern to be used for the user search.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source><ph id="ph1">{0}</ph> is the user's DN.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>ldap.authorities.searchSubtree<bpt id="p1">&lt;sup&gt;</bpt><ph id="ph1">\*</ph><ept id="p1">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>TRUE</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>"If true a subtree scope search will be performed, otherwise a single-level search is used."</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>ldap.authorities.groupSearchBase<bpt id="p1">&lt;sup&gt;</bpt><ph id="ph1">\*</ph><ept id="p1">&lt;/sup&gt;</ept></source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>"'ou=groups,dc=example,dc=com'"</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>The base DN from which the search for group membership should be performed.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>ldap.authorities.defaultRole</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>None</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>An optional default role to be assigned to all users.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>ldap.mapper.roleAttributes</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Null</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Optional names of role attributes.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>ldap.mapper.convertToUpperCase</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>TRUE</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>"Whether to uppercase retrieved role names (will also be prefixed with ""ROLE<ph id="ph1">\_</ph>"")"</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>PAM Authentication</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>By default, the <bpt id="p1">**</bpt>PAM<ept id="p1">**</ept> security provider is disabled.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>To enable PAM authentication support, you must:</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Update the relevant properties in your DeployR external configuration file, <ph id="ph1">`deployr.groovy`</ph>.</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>Follow the DeployR server system files configuration changes outlined below.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>PAM is the Linux Pluggable Authentication Modules provided to support dynamic authorization for applications and services in a Linux system.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>If DeployR is installed on a Linux system, then the PAM security provider allows users to authenticate with DeployR using their existing Linux system username and password.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Basic authentication remains enabled even with PAM enabled.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>Step 1: Update the DeployR external configuration file</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>Update the following properties in your DeployR external configuration file, <ph id="ph1">`deployr.groovy`</ph>:</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>Relevant snippet from <ph id="ph1">`deployr.groovy`</ph> file shown here:</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>Step 2: Apply Configuration Changes to DeployR Server System Files</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>Before making any configuration changes to the server system files, <bpt id="p1">[</bpt>stop the DeployR server<ept id="p1">](deployr-common-administration-tasks.md#startstop)</ept>.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>Grant <ph id="ph1">`root`</ph> permissions to launch the Tomcat server.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>This is required so the DeployR server can avail of PAM authentication services.</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>Log in as <ph id="ph1">`root`</ph> on your DeployR server.</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>Using your preferred editor, edit the file <ph id="ph1">`/opt/deployr/8.0.5/tomcat/tomcat7.sh`</ph>,</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>Find the following section:</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>On Redhat/CentOS platforms:</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>On SLES platforms:</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>Change <ph id="ph1">`"tomcat2"`</ph> to <ph id="ph2">`"root"`</ph> as follows:</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>On Redhat/CentOS platforms:</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>On SLES platforms:</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>Save this change and close the file in your editor.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Restart the server<ept id="p1">](deployr-common-administration-tasks.md#startstop)</ept>.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>If you have enabled PAM authentication as part of the required steps for enabling R Session Process Controls, then please continue with your configuration using <bpt id="p1">[</bpt>these steps<ept id="p1">](#r-session-process-controls)</ept>.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>CA Single Sign-On (SiteMinder) Pre-Authentication</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>By default, the <bpt id="p1">**</bpt>CA Single Sign-On<ept id="p1">**</ept> (formerly known as SiteMinder) security provider is disabled.</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>To enable CA Single Sign-On support, you must first update CA Single Sign-On Policy Server configuration.</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>Then, you must update the relevant properties in your DeployR external configuration file.</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>To enable CA Single Sign-On support:</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>Define or update your CA Single Sign-On Policy Server configuration.</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>For details on how to do this, <bpt id="p1">[</bpt>read here<ept id="p1">](deployr-admin-configure-ca-sso.md)</ept>.</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>Update the relevant properties in your DeployR external configuration file.</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>This step assumes that:</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>Your CA Single Sign-On Policy Server is properly configured and running</source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>You understand which header files are being used by your policy server</source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>R Session Process Controls</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source>By default, R sessions executing on the DeployR grid are not authorized to access files or directories outside of the R working directory.</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>To enable broader file system access for a given R session to files or directories based on specific authenticated user ID and group ID credentials, you must first do ONE of the following:</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>Enable <bpt id="p1">[</bpt>PAM authentication<ept id="p1">](#pam-authentication)</ept>, or</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>Enable <bpt id="p1">[</bpt>LDAP authentication<ept id="p1">](#ldap)</ept>, or</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>Enable <bpt id="p1">[</bpt>Active Directory authentication<ept id="p1">](#active-directory-authentication)</ept></source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>Once you have enabled PAM, LDAP, or AD authentication, you must (Step 1) update the relevant process controls properties on the server <bpt id="p1">**</bpt>and then<ept id="p1">**</ept> (Step 2) apply system-level configuration changes to every single node on your DeployR grid, as follows:</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>Step 1: Update Process Control Properties</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source>After you've enabled either PAM, LDAP, or Active Directory authentication, you can update the relevant process control properties in your DeployR server external configuration file, <ph id="ph1">`deployr.groovy`</ph>, on the main DeployR server:</source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>deployr.security.r.session.process.controls.enabled</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source>deployr.security.r.session.process.default.uid</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>deployr.security.r.session.process.default.gid</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source>Relevant snippet from <ph id="ph1">`deployr.groovy`</ph> file shown here:</source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source>Step 2: Make System-Level Configuration Changes to Every Node</source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source>Before You Begin!</source>
        </trans-unit><trans-unit id="324" translate="yes" xml:space="preserve">
          <source>Make sure you've enabled the appropriate process control properties before beginning this step.</source>
        </trans-unit><trans-unit id="325" translate="yes" xml:space="preserve">
          <source>For Non-Root Installs</source>
        </trans-unit><trans-unit id="326" translate="yes" xml:space="preserve">
          <source>Apply the following configuration changes on <bpt id="p1">**</bpt>each and every node<ept id="p1">**</ept> on your DeployR grid, including the default grid node.</source>
        </trans-unit><trans-unit id="327" translate="yes" xml:space="preserve">
          <source>On each machine hosting a grid node:</source>
        </trans-unit><trans-unit id="328" translate="yes" xml:space="preserve">
          <source>Before making any configuration changes to system files, you must stop Rserve and any other DeployR-related services:</source>
        </trans-unit><trans-unit id="329" translate="yes" xml:space="preserve">
          <source>Grant <ph id="ph1">`deployr-user`</ph> permission to execute a command as a <ph id="ph2">`sudo`</ph> user so that the RServe process can be launched.</source>
        </trans-unit><trans-unit id="330" translate="yes" xml:space="preserve">
          <source>This is required so that the DeployR server can enforce R session process controls.</source>
        </trans-unit><trans-unit id="331" translate="yes" xml:space="preserve">
          <source>A.</source>
        </trans-unit><trans-unit id="332" translate="yes" xml:space="preserve">
          <source>Log in as <ph id="ph1">`root`</ph>.</source>
        </trans-unit><trans-unit id="333" translate="yes" xml:space="preserve">
          <source>B.</source>
        </trans-unit><trans-unit id="334" translate="yes" xml:space="preserve">
          <source>Using your preferred editor, edit the file:</source>
        </trans-unit><trans-unit id="335" translate="yes" xml:space="preserve">
          <source>C.</source>
        </trans-unit><trans-unit id="336" translate="yes" xml:space="preserve">
          <source>Find the following section:</source>
        </trans-unit><trans-unit id="337" translate="yes" xml:space="preserve">
          <source>D.</source>
        </trans-unit><trans-unit id="338" translate="yes" xml:space="preserve">
          <source>Add the following line to this section:</source>
        </trans-unit><trans-unit id="339" translate="yes" xml:space="preserve">
          <source>E.</source>
        </trans-unit><trans-unit id="340" translate="yes" xml:space="preserve">
          <source>Find the following section:</source>
        </trans-unit><trans-unit id="341" translate="yes" xml:space="preserve">
          <source>F.</source>
        </trans-unit><trans-unit id="342" translate="yes" xml:space="preserve">
          <source>Add or append <ph id="ph1">`DEPLOYRRSERVE`</ph> for <ph id="ph2">`%deployr-user`</ph> to this section:</source>
        </trans-unit><trans-unit id="343" translate="yes" xml:space="preserve">
          <source>G.</source>
        </trans-unit><trans-unit id="344" translate="yes" xml:space="preserve">
          <source>Save these changes and close the file in your editor.</source>
        </trans-unit><trans-unit id="345" translate="yes" xml:space="preserve">
          <source>H.</source>
        </trans-unit><trans-unit id="346" translate="yes" xml:space="preserve">
          <source>Log out <ph id="ph1">`root`</ph>.</source>
        </trans-unit><trans-unit id="347" translate="yes" xml:space="preserve">
          <source>Update the DeployR <ph id="ph1">`startAll.sh`</ph> shell script to take advantage of the <ph id="ph2">`sudo`</ph> command configured above.</source>
        </trans-unit><trans-unit id="348" translate="yes" xml:space="preserve">
          <source>A.</source>
        </trans-unit><trans-unit id="349" translate="yes" xml:space="preserve">
          <source>Log in as <ph id="ph1">`deployr-user`</ph>.</source>
        </trans-unit><trans-unit id="350" translate="yes" xml:space="preserve">
          <source>B.</source>
        </trans-unit><trans-unit id="351" translate="yes" xml:space="preserve">
          <source>Using your preferred editor, edit the file:</source>
        </trans-unit><trans-unit id="352" translate="yes" xml:space="preserve">
          <source>C.</source>
        </trans-unit><trans-unit id="353" translate="yes" xml:space="preserve">
          <source>Find the following line:</source>
        </trans-unit><trans-unit id="354" translate="yes" xml:space="preserve">
          <source>D.</source>
        </trans-unit><trans-unit id="355" translate="yes" xml:space="preserve">
          <source>Change it to the following:</source>
        </trans-unit><trans-unit id="356" translate="yes" xml:space="preserve">
          <source>E.</source>
        </trans-unit><trans-unit id="357" translate="yes" xml:space="preserve">
          <source>Save this change and close the file in your editor.</source>
        </trans-unit><trans-unit id="358" translate="yes" xml:space="preserve">
          <source>Update the DeployR <ph id="ph1">`stopAll.sh`</ph> shell script to take advantage of the <ph id="ph2">`sudo`</ph> command configured above.</source>
        </trans-unit><trans-unit id="359" translate="yes" xml:space="preserve">
          <source>A.</source>
        </trans-unit><trans-unit id="360" translate="yes" xml:space="preserve">
          <source>Using your preferred editor, edit the file:</source>
        </trans-unit><trans-unit id="361" translate="yes" xml:space="preserve">
          <source>B.</source>
        </trans-unit><trans-unit id="362" translate="yes" xml:space="preserve">
          <source>Find the following line:</source>
        </trans-unit><trans-unit id="363" translate="yes" xml:space="preserve">
          <source>C.</source>
        </trans-unit><trans-unit id="364" translate="yes" xml:space="preserve">
          <source>Change it to the following:</source>
        </trans-unit><trans-unit id="365" translate="yes" xml:space="preserve">
          <source>D.</source>
        </trans-unit><trans-unit id="366" translate="yes" xml:space="preserve">
          <source>Save this change and close the file in your editor.</source>
        </trans-unit><trans-unit id="367" translate="yes" xml:space="preserve">
          <source>Set group privileges on the user directory containing the DeployR grid node install directory.</source>
        </trans-unit><trans-unit id="368" translate="yes" xml:space="preserve">
          <source>A.</source>
        </trans-unit><trans-unit id="369" translate="yes" xml:space="preserve">
          <source>Log in as <ph id="ph1">`root`</ph>.</source>
        </trans-unit><trans-unit id="370" translate="yes" xml:space="preserve">
          <source>B.</source>
        </trans-unit><trans-unit id="371" translate="yes" xml:space="preserve">
          <source>Set group privileges.</source>
        </trans-unit><trans-unit id="372" translate="yes" xml:space="preserve">
          <source>Add each user that will authenticate with the server to the <ph id="ph1">`deployr-user`</ph> group.</source>
        </trans-unit><trans-unit id="373" translate="yes" xml:space="preserve">
          <source>A.</source>
        </trans-unit><trans-unit id="374" translate="yes" xml:space="preserve">
          <source>Log in as <ph id="ph1">`root`</ph>.</source>
        </trans-unit><trans-unit id="375" translate="yes" xml:space="preserve">
          <source>B.</source>
        </trans-unit><trans-unit id="376" translate="yes" xml:space="preserve">
          <source>Execute the following command to add each user to the <ph id="ph1">`deployr-user`</ph> group.</source>
        </trans-unit><trans-unit id="377" translate="yes" xml:space="preserve">
          <source>C.</source>
        </trans-unit><trans-unit id="378" translate="yes" xml:space="preserve">
          <source>Repeat step <bpt id="p1">**</bpt>B.<ept id="p1">**</ept> for each user that will authenticate with the server.</source>
        </trans-unit><trans-unit id="379" translate="yes" xml:space="preserve">
          <source>D.</source>
        </trans-unit><trans-unit id="380" translate="yes" xml:space="preserve">
          <source>Log out <ph id="ph1">`root`</ph>.</source>
        </trans-unit><trans-unit id="381" translate="yes" xml:space="preserve">
          <source>Restart Rserve and any other DeployR-related services on the machine hosting the DeployR grid node:</source>
        </trans-unit><trans-unit id="382" translate="yes" xml:space="preserve">
          <source>A.</source>
        </trans-unit><trans-unit id="383" translate="yes" xml:space="preserve">
          <source>Log in as <ph id="ph1">`deployr-user`</ph>.</source>
        </trans-unit><trans-unit id="384" translate="yes" xml:space="preserve">
          <source>B.</source>
        </trans-unit><trans-unit id="385" translate="yes" xml:space="preserve">
          <source>Start Rserve and any other DeployR-related services:</source>
        </trans-unit><trans-unit id="386" translate="yes" xml:space="preserve">
          <source>Repeat these steps for each grid node.</source>
        </trans-unit><trans-unit id="387" translate="yes" xml:space="preserve">
          <source>For Root Installs</source>
        </trans-unit><trans-unit id="388" translate="yes" xml:space="preserve">
          <source>Apply the following configuration changes on <bpt id="p1">**</bpt>each and every node<ept id="p1">**</ept> on your DeployR grid, including the default grid node.</source>
        </trans-unit><trans-unit id="389" translate="yes" xml:space="preserve">
          <source>On each machine hosting a grid node:</source>
        </trans-unit><trans-unit id="390" translate="yes" xml:space="preserve">
          <source>Log in as <ph id="ph1">`root`</ph>.</source>
        </trans-unit><trans-unit id="391" translate="yes" xml:space="preserve">
          <source>Before making any configuration changes to system files, stop Rserve and any other DeployR-related services:</source>
        </trans-unit><trans-unit id="392" translate="yes" xml:space="preserve">
          <source>Grant <ph id="ph1">`root`</ph> permission to launch the RServe process.</source>
        </trans-unit><trans-unit id="393" translate="yes" xml:space="preserve">
          <source>This is required so that each DeployR grid node can enforce R session process controls.</source>
        </trans-unit><trans-unit id="394" translate="yes" xml:space="preserve">
          <source>A.</source>
        </trans-unit><trans-unit id="395" translate="yes" xml:space="preserve">
          <source>Using your preferred editor, edit the file <ph id="ph1">`/opt/deployr/8.0.5/rserve/rserve.sh`</ph> as follows:</source>
        </trans-unit><trans-unit id="396" translate="yes" xml:space="preserve">
          <source>On Redhat/CentOS platforms, find the following section:</source>
        </trans-unit><trans-unit id="397" translate="yes" xml:space="preserve">
          <source>and, change <ph id="ph1">`apache`</ph> to <ph id="ph2">`root`</ph> as follows:</source>
        </trans-unit><trans-unit id="398" translate="yes" xml:space="preserve">
          <source>On SLES platforms, find the following section:</source>
        </trans-unit><trans-unit id="399" translate="yes" xml:space="preserve">
          <source>and, change <ph id="ph1">`apache`</ph> to <ph id="ph2">`root`</ph> as follows:</source>
        </trans-unit><trans-unit id="400" translate="yes" xml:space="preserve">
          <source>B.</source>
        </trans-unit><trans-unit id="401" translate="yes" xml:space="preserve">
          <source>Save this change and close the file in your editor.</source>
        </trans-unit><trans-unit id="402" translate="yes" xml:space="preserve">
          <source>Set group privileges on the DeployR install directory.</source>
        </trans-unit><trans-unit id="403" translate="yes" xml:space="preserve">
          <source>Execute the following command to add each user to the <ph id="ph1">`apache`</ph> group.</source>
        </trans-unit><trans-unit id="404" translate="yes" xml:space="preserve">
          <source>Repeat for each user that will authenticate with the server.</source>
        </trans-unit><trans-unit id="405" translate="yes" xml:space="preserve">
          <source>Restart Rserve and any other DeployR-related services:</source>
        </trans-unit><trans-unit id="406" translate="yes" xml:space="preserve">
          <source>Repeat these steps for each grid node.</source>
        </trans-unit></group></body></file></xliff>