<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="configure-authentication.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926fdca4ca85e7a8e97fb42e11f4e68450eb7a02c53.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">fdca4ca85e7a8e97fb42e11f4e68450eb7a02c53</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\configure-authentication.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>LDAP AD and Azure Active Directory authentication for Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Authenticate Machine Learning Server users against LDAP AD or Azure Active Directory</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Machine Learning Server LDAP-S, LDAP, AD, Azure Active Directory, AAD, Azure AD, Authentication, Microsoft R Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Authenticate Machine Learning Server users against LDAP AD or Azure Active Directory</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Machine Learning Server, Microsoft R Server 9.x<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Machine Learning Server's offers seamless integration with authentication solutions when configured to operationalize analytics.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Security</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>To secure connections and communications, you have several options:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Authentication Method</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>When to Use</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Local 'admin' account<ept id="p1">](#local)</ept></source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">[</bpt>one-box<ept id="p1">](configure-machine-learning-server-one-box.md)</ept> configurations</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Active Directory / LDAP<ept id="p1">](#ldap)</ept></source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">[</bpt>enterprise<ept id="p1">](configure-machine-learning-server-enterprise.md)</ept> on-premises configurations</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Active Directory / LDAP-S<ept id="p1">](#ldap)</ept></source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">[</bpt>enterprise<ept id="p1">](configure-machine-learning-server-enterprise.md)</ept> on-premises configurations with SSL/TLS enabled</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Azure Active Directory<ept id="p1">](#aad)</ept></source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">[</bpt>enterprise<ept id="p1">](configure-machine-learning-server-enterprise.md)</ept> cloud configurations</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Local Administrator Account Authentication</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>During configuration, a default administrator account, 'admin', is created to manage the web and compute nodes for In Machine Learning Server (and R Server).</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>This account allows you to use the <bpt id="p1">[</bpt>CLI or administration utility<ept id="p1">](configure-admin-cli-launch.md)</ept> to configure this feature, edit ports, restart nodes, and so on.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This account might be sufficient when trying to operationalize with a <bpt id="p1">[</bpt>one-box configuration<ept id="p1">](configure-machine-learning-server-one-box.md)</ept> since everything is running within the trust boundary.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>However, it is insufficient for <bpt id="p1">[</bpt>enterprise configurations<ept id="p1">](configure-machine-learning-server-enterprise.md)</ept>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>To set or change the password for the local administrator account after the configuration script has been run, <bpt id="p1">[</bpt>follow these steps<ept id="p1">](configure-admin-cli-local-password.md)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>To log in to Machine Learning Server with this user for remote execution or web service functionalities, use remoteLogin() as described in the article "<bpt id="p1">[</bpt>Connecting to Machine Learning Server with mrsdeploy<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept>."</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If you enable Azure Active Directory or Active Directory/LDAP authentication, this 'admin' account can no longer be used to authenticate with Machine Learning Server.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Active Directory and LDAP/LDAP-S</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Active Directory (AD) and LDAP are a great authentication option for on-premises configurations to ensure that domain users have access to the APIs.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>LDAP is the standard protocol for reading data from and writing data to Active Directory (AD) domain controllers.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>AD LDAP traffic is unsecured by default, which makes it possible to use network-monitoring software to view the LDAP traffic between clients and domain controllers.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>By default, the LDAP security provider is not configured.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>To enable LDAP authentication support, update the relevant properties in your configuration file.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The values you assign to these properties must match the configuration of your LDAP Directory Information Tree (DIT).</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>You can make LDAP traffic confidential and secure using Secure Sockets Layer (SSL) / Transport Layer Security (TLS) technology.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>This combination is referred to as LDAP over SSL (or LDAP-S).</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>To ensure that no one else can read the traffic, SSL/TLS establishes an encrypted tunnel between an LDAP client and a domain controller.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more about enabling SSL/TLS.<ept id="p1">](configure-https.md)</ept></source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Reasons for enabling LDAP-S include:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Organizational security policies typically require that all client/server communication is encrypted.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Applications use simple BIND to transport credentials and authenticate against a Domain Controller.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>As simple BIND exposes the users’ credentials in clear text, using SSL/TLS to encrypt the authentication session is recommended.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Use of proxy binding or password change over LDAP, which requires LDAP-S.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Bind to an AD LDS instance Through a Proxy Object</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Applications that integrate with LDAP servers (such as Active Directory or Active Directory Domain Controllers) might require encrypted LDAP communications.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>You cannot have both Azure Active Directory and Active Directory/LDAP enabled at the same time.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If one is set to <ph id="ph1">`"Enabled": true`</ph>, then the other must be set to <ph id="ph2">`"Enabled": false`</ph>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On each web node:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Enable LDAP/LDAP-S in the external JSON configuration file, appsettings.json:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Open the configuration file, <bpt id="p1">[</bpt><ph id="ph1">\&lt;</ph>web-node-install-path&gt;<ept id="p1">](../operationalize/configure-find-admin-configuration-file.md)</ept>/appsettings.json.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Search for the section starting with <ph id="ph1">`"LDAP": {`</ph></source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;a name="encrypt"&gt;</bpt><ept id="p1">&lt;/a&gt;</ept>Enable this section and update the properties so that they match the values in your Active Directory Service Interfaces Editor.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>For better security, we recommend you <bpt id="p1">[</bpt>encrypt the password<ept id="p1">](configure-admin-cli-encrypt-credentials.md)</ept> before adding the information to appsettings.json.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>LDAP Properties</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Definition</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Host</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Address of the Active Directory server</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Port</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>(version 9.1+) Used to override the default LDAP port.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>By default, the LDAP port is 389 and the LDAP-S port is 636.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>UseLDAPS</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Set 'true' for LDAP-S or 'false' for LDAP</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Note:<ept id="p1">**</ept> If LDAP-S is configured, an installed LDAP service certificate is assumed so that the tokens produced by Active Directory/LDAP can be signed and accepted by Machine Learning Server.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>BindFilter</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>(version 9.0.1 only) The template used to do the Bind operation.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>For example, "CN=<ph id="ph1">{0}</ph>,CN=DeployR,DC=TEST,DC=COM".</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source><ph id="ph1">{0}</ph> is the user's DN.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>QueryUserDn</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Distinguished name of user with read-only query capabilities with which to authenticate</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>QueryUserPassword</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Password for that user with which to authenticate (value must be encrypted).</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>We highly recommend that you <bpt id="p1">[</bpt>encrypt LDAP login credentials<ept id="p1">](configure-admin-cli-encrypt-credentials.md)</ept> before adding the information to this file.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>QueryUserPasswordEncrypted</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>True/False.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>If 'True', it means the value of QueryUserPassword is an encrypted string.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>SearchBase</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Context name to search in, relative to the base of the configured ContextSource, for example, 'ou=users,dc=example,dc=com'.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>SearchFilter</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The pattern to be used for the user search.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>"SearchFilter": "cn=<ph id="ph1">{0}</ph>" is for each user's DN.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>In legacy systems, some use "SearchFilter": "sAMAccountName=<ph id="ph1">{0}</ph>"</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>UniqueUserIdentifierAttributeName</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>(Version 9.1) The attribute name that stores the unique user ID for each user.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>If you are configuring roles, you must ensure that the username returned for this value matches the username returned by SearchFilter.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>For example, if "SearchFilter": "cn=<ph id="ph1">{0}</ph>" and "UniqueUserIdentifierAttributeName": "userPrincipalName", then the values for cn and userPrincipalName must match.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>DisplayNameAttributeName</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>(Version 9.1) The attribute name that stores the display name for each user.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>EmailAttributeName</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>(Version 9.1) The attribute name that stores the email address for each user.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>The entities created by the users, specifically web services and <bpt id="p1">[</bpt>session snapshots<ept id="p1">](../r/how-to-execute-code-remotely.md#snapshot)</ept>, are tied to their usernames.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>For this reason, you must be careful to prevent changes to the user identifier over time.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Otherwise, pre-existing web services and snapshots cannot be mapped to the users who created them.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>For this reason, we strongly recommend that you DO NOT change the unique LDAP identifier in appsettings.json once users start publishing service or creating snapshots.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Similarly, if your organization changes its usernames, those users can no longer access the web services and snapshots they created unless they are <bpt id="p1">[</bpt>assigned to the <ph id="ph1">`Owner`</ph> role<ept id="p1">](configure-roles.md)</ept>.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>For 9.0.1 Users!</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>The unique identifier is always set to the <ph id="ph1">`userPrincipalName`</ph> in version 9.0.1.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Therefore, make sure that a value is defined for the <ph id="ph1">`userPrincipalName`</ph> in the Active Directory Service Interfaces Editor or the authentication may fail.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>In the Explorer, connect to the domain controller, find the user to authorize, and then make sure that the value for the  UserPrincipalName (UPN) property is not null.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>For example, with R Server 9.1:</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Need help figuring out your Active Directory/LDAP settings?</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Check out your LDAP settings using the <ph id="ph1">`ldp.exe`</ph> tool and compare them to what you’ve declared in appsettings.json.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>You can also consult with any Active Directory experts in your organization to identify the correct parameters.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>To set different levels of permissions for users interacting with web services, <bpt id="p1">[</bpt>assign them roles<ept id="p1">](configure-roles.md)</ept>.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>If using a certificate for access token signing, you must:</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>You must use a certificate for access token signing whenever you have multiple web nodes so the tokens are signed consistently by every web node in your configuration.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>In production environments, we recommend that you use a certificate with a private key to sign the user access tokens between the web node and the LDAP server.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Tokens are useful to the application developers who use them to identify and authenticate users who are sending API calls within their application.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more...<ept id="p1">](how-to-manage-access-tokens.md)</ept></source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Every web node must have the same values<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>On each machine hosting the Web node, install the trusted, signed <bpt id="p1">**</bpt>access token signing certificate<ept id="p1">**</ept> with a private key in the certificate store.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Take note of the <ph id="ph1">`Subject`</ph> name of the certificate as you need this information later.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Read <bpt id="p1">[</bpt>this blog post<ept id="p1">](https://blogs.msdn.microsoft.com/rserver/2017/05/19/using-certificates-in-r-server-operationalization-for-linux/)</ept> to learn how to use a self-signed certificate in Linux for access token signing.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Self-signed certificates are NOT recommended for production usage.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>In the appsettings.json file, search for the section starting with <ph id="ph1">`"JWTSigningCertificate": {`</ph></source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Enable this section and update the properties so that they match the values for your token signing certificate:</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`"Thumbprint"`</ph> to ensure that the correct certificate is loaded if there are multiple certificates on the same system with same name used for different purposes such as IPsec, TLS Web Server Authentication, Client Authentication, Server Authentication, and so on.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>If you do not have multiple certificates with same name, you can leave the Thumbprint field empty.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Save changes to appsettings.json.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Restart the web node<ept id="p1">](configure-admin-cli-stop-start.md)</ept> using the administration utility so that the changes can take effect.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Run the <bpt id="p1">[</bpt>diagnostic tests<ept id="p1">](configure-run-diagnostics.md)</ept> to ensure all tests are passing in the configuration.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>If you run into connection issues when configuring for Active Directory/LDAP, try the ldp.exe tool to search the LDAP settings and compare them to what you declared in appsettings.json.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>To identify the correct parameters, consult with any Active Directory experts in your organization.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Repeat these steps on each machine hosting the web node.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Share the connection details with any users who authenticate with Machine Learning Server either to make <bpt id="p1">[</bpt>API calls<ept id="p1">](concept-api.md)</ept> directly or indirectly in R <bpt id="p2">[</bpt>using remoteLogin() function in the mrsdeploy package<ept id="p2">](how-to-connect-log-in-with-mrsdeploy.md)</ept>.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Azure Active Directory</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Azure Active Directory (AAD)<ept id="p1">](https://www.microsoft.com/cloud-platform/azure-active-directory)</ept> can be used to securely authenticate  in the cloud when the client application and Web node have access to the internet.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Step 1: Log in to the Azure portal<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Sign in to the <bpt id="p1">[</bpt>Azure portal<ept id="p1">](http://portal.azure.com)</ept>.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Select the upper-right hand corner and select the Active Directory account from the list.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>If the Azure Active Directory has not been set up yet, contact your system administrator.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>In our example, that directory is <ph id="ph1">`MyMLServer`</ph>.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Azure Active Directory<ept id="p1">**</ept> from the left-hand side.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Azure Active Directory icon</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>App registrations<ept id="p1">**</ept> tab at the top.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>The application list appears.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>You may not have any applications yet.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>App registrations</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Step 2: Create a web application<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Now, create a web app that is tied to the Azure Active Directory as follows:</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>New application registration<ept id="p1">**</ept> at the top.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source><ph id="ph1">![</ph>New app registrations<ph id="ph2">](./media/configure-authentication/aad-new-app-registration.png)</ph></source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Enter a <bpt id="p1">**</bpt>Name<ept id="p1">**</ept> for your application, such as <ph id="ph1">`Machine Learning Server Web app`</ph>.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source><ph id="ph1">![</ph>New app registrations<ph id="ph2">](./media/configure-authentication/aad-create-web-app-name.png)</ph></source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>For the <bpt id="p1">**</bpt>Application type<ept id="p1">**</ept>, select the <bpt id="p2">**</bpt>Web app / API<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Sign-on URL<ept id="p1">**</ept> box, enter <ph id="ph1">http://localhost:12800</ph>.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>This is the port that R Client and R Server listen on.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Create<ept id="p1">**</ept> to create the new web application.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>New app registrations</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>The application is created and its details appear onscreen.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Copy the <bpt id="p1">**</bpt>Application ID<ept id="p1">**</ept> for the web application.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>You use this later when you configure your Native application and Machine Learning Server using this ID.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Newly created web app</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Settings<ept id="p1">**</ept> <ph id="ph1">![</ph>Azure Active Directory icon<ph id="ph2">](./media/configure-authentication/aad-settings.png)</ph>.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Settings<ept id="p1">**</ept> pane appears on the right.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Keys<ept id="p1">**</ept> from the <bpt id="p2">**</bpt>Settings<ept id="p2">**</ept> pane.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Keys<ept id="p1">**</ept> pane appears.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>Keys</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Password<ept id="p1">**</ept> area, add a client key.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Provide a description of your choosing and select a key duration.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Keys</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Save<ept id="p1">**</ept> to save the key.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Be sure to copy the key.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Keys</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Take note of this key as it is needed to configure <bpt id="p1">[</bpt>roles to give web services permissions to certain users<ept id="p1">](configure-roles.md)</ept>.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Also, take note of the application's tenant ID.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>The tenant ID is the domain of the Azure Active Directory account, for example,  <ph id="ph1">`myMLServer.contoso.com`</ph>.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Step 3: Create a native application<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Now, let's create a native application.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>This application links the web application to the Machine Learning Server web node.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>In the Azure portal, select <bpt id="p1">**</bpt>Azure Active Directory<ept id="p1">**</ept> from the left-hand side.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>App registrations<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>App registrations</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>New application registration<ept id="p1">**</ept> at the top.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>New app registrations</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>Enter a <bpt id="p1">**</bpt>Name<ept id="p1">**</ept> for your application, such as <ph id="ph1">`Machine Learning Server native app`</ph>.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>New app registrations</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>For the <bpt id="p1">**</bpt>Application type<ept id="p1">**</ept>, select the <bpt id="p2">**</bpt>Native<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>New app registrations</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Redirect URI<ept id="p1">**</ept> field, enter:</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Create<ept id="p1">**</ept> to create the new native application.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>The application is created and its details appear onscreen.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>Copy the <bpt id="p1">**</bpt>Application ID<ept id="p1">**</ept> for the web application.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>You use this ID later to enable AAD in Machine Learning Server.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>Newly created web app</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Settings<ept id="p1">**</ept> <ph id="ph1">![</ph>Azure Active Directory icon<ph id="ph2">](./media/configure-authentication/aad-settings.png)</ph>.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Settings<ept id="p1">**</ept> pane appears on the right.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Required permissions<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>Required permissions</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Add<ept id="p1">**</ept> at the top.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source><ph id="ph1">![</ph>Required permissions<ph id="ph2">](./media/configure-authentication/aad-settings-perms-add.png)</ph></source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Select an API<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>Required permissions</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>In the search field at the top, type the name of the web application you created.</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>In our example, we use the name <ph id="ph1">`Machine Learning Server Web app`</ph>.</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>Required permissions</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>Select the web application name.</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>Select the <bpt id="p1">**</bpt>Select<ept id="p1">**</ept> button.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Select permissions &gt; Enable Access<ept id="p1">**</ept> fields appear.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>Select the checkmark next to the name of the web application.</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>Required permissions</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>Select the <bpt id="p1">**</bpt>Select<ept id="p1">**</ept> button.</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>The pane closes.</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Done<ept id="p1">**</ept> at the bottom to finish adding the permissions.</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Step 4: Enable Azure AD on each web node<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>Open the configuration file, <bpt id="p1">[</bpt><ph id="ph1">\&lt;</ph>web-node-install-path&gt;<ept id="p1">](../operationalize/configure-find-admin-configuration-file.md)</ept>/appsettings.json.</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>Search for the section starting with:</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>You cannot have both Azure Active Directory and Active Directory/LDAP enabled at the same time.</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>If one is set to <ph id="ph1">`"Enabled": true`</ph>, then the other must be set to <ph id="ph2">`"Enabled": false`</ph>.</source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>Enable Azure Active Directory as the authentication method:  <ph id="ph1">`"Enabled": true,`</ph></source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>Update the other properties in that section so that they match the values in the Azure portal.</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source>Properties include:</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>Azure AD Properties</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>Definition</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>Enabled</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>To use AAD for authentication, set to 'true'.</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>Else, set to 'false'.</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>Authority</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source>Use '<ph id="ph1">https://login.windows.net/\&lt;URL</ph> to AAD login&gt;' where <ph id="ph2">\&lt;</ph>URL to AAD login&gt; is the URL to the AAD login.</source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>For example, if the AAD account domain is myMLServer.contoso.com, then the Authority would be '<ph id="ph1">&lt;https://login.windows.net/myMLServer.contoso.com&gt;</ph>'</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source>Audience</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>Use the Application ID value for the WEB app you created in the Azure portal.</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source>ClientId</source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source>Use the Application ID value for the NATIVE app you created in the Azure portal.</source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source>Key</source>
        </trans-unit><trans-unit id="324" translate="yes" xml:space="preserve">
          <source>This is the key for the WEB application you took note of before.</source>
        </trans-unit><trans-unit id="325" translate="yes" xml:space="preserve">
          <source>KeyEncrypted</source>
        </trans-unit><trans-unit id="326" translate="yes" xml:space="preserve">
          <source>We highly recommend that you <bpt id="p1">[</bpt>encrypt login credentials<ept id="p1">](configure-admin-cli-encrypt-credentials.md)</ept> before adding the information to this file.</source>
        </trans-unit><trans-unit id="327" translate="yes" xml:space="preserve">
          <source>Set KeyEncrypted to 'true' if using encrypted information.</source>
        </trans-unit><trans-unit id="328" translate="yes" xml:space="preserve">
          <source>For plain text, set to 'false'.</source>
        </trans-unit><trans-unit id="329" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="330" translate="yes" xml:space="preserve">
          <source>To set different levels of permissions for users interacting with web services, <bpt id="p1">[</bpt>assign them roles<ept id="p1">](configure-roles.md)</ept>.</source>
        </trans-unit><trans-unit id="331" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Restart the web node<ept id="p1">](configure-admin-cli-stop-start.md)</ept> for the changes to take effect.</source>
        </trans-unit><trans-unit id="332" translate="yes" xml:space="preserve">
          <source>Authorize this machine for Azure Active Directory Test by running a <bpt id="p1">[</bpt>diagnostic test<ept id="p1">](configure-run-diagnostics.md)</ept> of the configuration.</source>
        </trans-unit><trans-unit id="333" translate="yes" xml:space="preserve">
          <source>You must run the diagnostic tests once on each web node to authorize this device for Azure Active Directory.</source>
        </trans-unit><trans-unit id="334" translate="yes" xml:space="preserve">
          <source>You will not be able to log in using AAD until this has been done.</source>
        </trans-unit><trans-unit id="335" translate="yes" xml:space="preserve">
          <source>Repeat these steps on each machine hosting a web node.</source>
        </trans-unit><trans-unit id="336" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Step 5: Share the required AAD connection details with your users<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="337" translate="yes" xml:space="preserve">
          <source>Share the connection details, such as the Authority and Audience, with any users who need to authenticate with Machine Learning Server to make <bpt id="p1">[</bpt>API calls<ept id="p1">](concept-api.md)</ept> directly or indirectly in R <bpt id="p2">[</bpt>using remoteLoginAAD() function in the mrsdeploy package<ept id="p2">](how-to-connect-log-in-with-mrsdeploy.md#aad-arguments)</ept>.</source>
        </trans-unit><trans-unit id="338" translate="yes" xml:space="preserve">
          <source>If you do not specify a username and password as arguments to the login call or R functions, you are prompted for your AAD username (<ph id="ph1">&lt;username&gt;</ph>@&lt;AAD-account-domain&gt;) and password.</source>
        </trans-unit><trans-unit id="339" translate="yes" xml:space="preserve">
          <source>Learn how to authenticate with AAD using the remoteLoginAAD() function in the mrsdeploy R package as described in this article: "<bpt id="p1">[</bpt>Connecting to Machine Learning Server with mrsdeploy<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept>."</source>
        </trans-unit><trans-unit id="340" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="341" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Blog article: Step-by-step setup for LDAPS on Windows Server<ept id="p1">](https://blogs.msdn.microsoft.com/rserver/2017/04/10/step-by-step-guide-to-setup-ldaps-on-windows-server/)</ept></source>
        </trans-unit></group></body></file></xliff>