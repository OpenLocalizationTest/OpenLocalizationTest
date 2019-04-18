<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-authenticate-in-python.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b45c30dff67e2278a08c9e99ec503db7399e76ba2d.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5c30dff67e2278a08c9e99ec503db7399e76ba2d</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\python\how-to-authenticate-in-python.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Connect to Machine Learning Server in Python using azureml-model-management-sdk</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Publish and consume Python web services with Microsoft R Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Authenticate with Machine Learning Server in Python with azureml-model-management-sdk</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: Machine Learning Server<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>azureml-model-management-sdk<ept id="p1">](../../python-reference/azureml-model-management-sdk/azureml-model-management-sdk.md)</ept> package, delivered with Machine Learning Server, provides functions for publishing and managing a Python web service that is backed by the Python code block or script you provided.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This section describes how to authenticate with Machine Learning Server on-premises or in the cloud using azureml-model-management-sdk.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Every API call between the client and the Web node must be authenticated.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The azureml-model-management-sdk functions, which place API calls on your behalf, are no different.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>If the user does not provide a valid login, an <ph id="ph1">`Unauthorized`</ph> HTTP <ph id="ph2">`401`</ph> status code is returned.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Overview</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>azureml-model-management-sdk provides the client that supports several ways of authenticating against the Machine Learning Server.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Authentication of user identity is handled via Active Directory.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Machine Learning Server never stores or manages any usernames and passwords.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Ask your administrator for <bpt id="p1">[</bpt>authentication type configured<ept id="p1">](../configure-authentication.md)</ept> for Machine Learning Server and the connection details.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>By default, all web services operations are available to authenticated users.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Tasks, such as deleting or updating a web service, are available only to the user who initially created the service.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>However, your administrator can also <bpt id="p1">[</bpt>assign role-based authorization controls<ept id="p1">](../configure-roles.md)</ept> to further restrict the permissions around web services.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>On premises authentication</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Use this approach if you are:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>authenticating using Active Directory server on your network</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>using the <bpt id="p1">[</bpt>default administrator account<ept id="p1">](../configure-authentication.md#local)</ept></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Pass the username and password as a Python tuple for on premises authentication.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If you do not know your connection settings, contact your administrator.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>This code calls the <ph id="ph1">`/user/login`</ph> API.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Argument</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>host endpoint</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Required.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The Machine Learning Server HTTP/HTTPS endpoint, including the port number.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>username</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Required.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Enter your AD username or 'admin' if <bpt id="p1">[</bpt>default administrator account<ept id="p1">](../configure-authentication.md#local)</ept> defined.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>password</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Required.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Enter the password.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Cloud authentication (AAD)</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Use this approach if you are authenticating using Azure Active Directory in the cloud.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Pass the credentials as a Python dictionary <ph id="ph1">{}</ph> for AAD authentication.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If you do not know your tenant ID, clientid, or other details, contact your administrator.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Or, if you have access to the Azure portal for the relevant Azure subscription, you can find <bpt id="p1">[</bpt>these authentication details<ept id="p1">](../configure-authentication.md#azure-active-directory)</ept>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Argument</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>host endpoint</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Required.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The Machine Learning Server HTTP/HTTPS endpoint, including the port number.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>This endpoint is the SIGN-ON URL value from the web application</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>authuri</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Required.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The URI of the authentication service for Azure Active Directory.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>tenant</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Required.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The tenant ID of the Azure Active Directory account being used to authenticate is the domain of AAD account.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>clientid</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Required.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>The numeric CLIENT ID of the AAD "native" application for the Azure Active Directory account.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>resource</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Required.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The numeric CLIENT ID from the AAD "Web" application for the Azure Active Directory account, also known by the <ph id="ph1">`Audience`</ph> in the configuration file.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>username</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Optional.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>If NULL, user is prompted.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>See following section.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>password</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Optional.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>If NULL, user is prompted.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>See following section.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Alternatives to putting the username and password in the script<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>If you omit the username and password from the dictionary for the AAD context, then you can either:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Get a device code to complete authentication and token creation via Azure Active Directory Authentication Libraries (ADAL).</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Enter that code at <ph id="ph1">https://aka.ms/devicelogin</ph> to complete the authentication.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Programmatically authenticate using a call back, such as:</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>A note about access tokens</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Keep in mind that all APIs require authentication; therefore, all users must authenticate when making an API call using the <ph id="ph1">`POST /login`</ph> API or through Azure Active Directory.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>To simplify this process, bearer access tokens are issued so that users need not provide their credentials for every single call.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>This bearer token is a lightweight security token that grants the “bearer” access to a protected resource, in this case, Machine Learning Server's APIs.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>After authentication, the user does not need to provide credentials again as long as the token is still valid, and a header is submitted with every request.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The application must validate the user’s bearer token to ensure that authentication was successful for the intended parties.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more about managing these tokens.<ept id="p1">](../how-to-manage-access-tokens.md)</ept></source>
        </trans-unit></group></body></file></xliff>