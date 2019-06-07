<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-admin-console-user-accounts.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37c37f386b02cc59152f5eb26b618a7026afd0956c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">c37f386b02cc59152f5eb26b618a7026afd0956c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-admin-console-user-accounts.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>DeployR Administration Console Help - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Managing Users in the DeployR Administration Console</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Creating &amp; Managing User Accounts</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>User accounts, which are <bpt id="p1">[</bpt>created<ept id="p1">](../deployr/deployr-admin-console-permissions-with-roles.md#creating-custom-roles)</ept> and <bpt id="p2">[</bpt>managed<ept id="p2">](../deployr/deployr-admin-console-permissions-with-roles.md#viewing-editing-and-assigning-roles)</ept> in this Administration Console, provide authenticated access to the DeployR Web Services API, the API Explorer tool, and the Administration Console.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>  Aside from the <ph id="ph1">`admin`</ph> account, user accounts represent script authors, client application developers, or client application end-users.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Each user has an account with <bpt id="p1">[</bpt>properties<ept id="p1">](deployr-admin-console-user-accounts.md#user-account-properties)</ept> such as their username, password, permissions, and so on.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>A user can represent an individual or an entity such as a dedicated DeployR client application.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The role(s) assigned to users determine their rights to access the console, their rights to access all or some of the API, and in some cases, their rights to access certain scripts.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>When you click <bpt id="p1">**</bpt>Users<ept id="p1">**</ept> in the main menu, you can review the list of DeployR user accounts.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The user list includes the username, display name, account status (enabled or disabled), and the date the account was last modified.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If there are more than 20 accounts, click <bpt id="p1">**</bpt>Next<ept id="p1">**</ept> to proceed to the remaining accounts.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>As an alternative, you can choose another form of <bpt id="p1">[</bpt>authentication for DeployR<ept id="p1">](../operationalize/configure-authentication.md)</ept>, such as Active Directory, LDAP, or PAM.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Figure: User List page</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>You cannot log in to DeployR from multiple accounts using a single brand of browser program.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>To use two or more accounts concurrently, you must log in to each one in a separate brand of browser.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Preconfigured User Accounts</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The following table presents the preconfigured DeployR user accounts and their default passwords.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Name</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Description and Recommendations</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>A default system administrator account for immediate access to the console.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>  This account cannot be renamed, disabled, or deleted.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>A default test account for client developers.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>We strongly recommend that you disable this account in production deployments.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>This account comes locked and you’ll need to set a password in order to use it.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>User Account Properties</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>For each user, there are a number of properties that can be defined.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The properties of a new account are described in the following table.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Property</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>When<bpt id="p1"> **</bpt>Enabled<ept id="p1">**</ept><ph id="ph1"> </ph>is selected, the user account is active, thereby allowing this user to access DeployR services on the API.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>If you uncheck this box, the account is disabled and the user will not have access to the console or the API calls.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Enter a unique name consisting of at least three alphanumeric characters, but no spaces or symbols.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Enter a display name of any combination of up to 50 alphanumeric characters or spaces.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>When the user logs into the Administration Console, this name appears in the upper right.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Enter the new password and re-enter it a second time to confirm.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Whenever this checkbox is selected, the user will be redirected to the DeployR Account Password Reset page the next time the user attempts to login so that they can define a new password.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>This applies only to basic authentication.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>When this checkbox is selected, the user account is locked.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The user will not be permitted to log into the console.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>This applies only to basic authentication.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Optionally, assign a<bpt id="p1"> [</bpt>boundary<ept id="p1">](../deployr/deployr-admin-managing-r-boundaries.md)</ept><ph id="ph1"> </ph>to the user.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Boundaries impose a set of runtime constraints on the user when he or she executes code or scripts on the API.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Note<ept id="p1">**</ept>: Grid node boundaries take precedence over user boundaries, and user boundaries take precedence over the server-wide default boundary.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Assign<bpt id="p1"> [</bpt>roles<ept id="p1">](../deployr/deployr-admin-managing-server-policies.md)</ept><ph id="ph1"> </ph>in order to grant the user permissions to execute API calls, access the Administration Console, access some or all of the event streams, and access certain scripts.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>If you do not specify any roles, then the<ph id="ph1"> `BASIC_USER` </ph>is automatically assigned.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Viewing and Editing User Accounts</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>To view and edit a user account:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>Users<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>User List<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>User List<ept id="p1">**</ept> table, click the name of the user whose account you want to review or edit.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>User Details<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Figure: User Details page</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>To edit the account, click <bpt id="p1">**</bpt>Edit<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Edit User<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Make your changes to the <bpt id="p1">[</bpt>user properties<ept id="p1">](deployr-admin-console-user-accounts.md#user-account-properties)</ept>.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Update<ept id="p1">**</ept> to save the changes.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Creating New User Accounts</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>To create a new user:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>Users<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>User List<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>New User<ept id="p1">**</ept> in the menu bar.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The New User page appears.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Figure: New User page</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>New User<ept id="p1">**</ept> page, enter all required <bpt id="p2">[</bpt>properties<ept id="p2">](deployr-admin-console-user-accounts.md#user-account-properties)</ept> for the user account as well as any optional details.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create<ept id="p1">**</ept> to save the new user.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Deleting User Accounts</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>To delete a user account:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>Users<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>User List<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>User List<ept id="p1">**</ept> table, click the name of the user whose account you want to delete.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>User Details<ept id="p1">**</ept> page appears and displays the account.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Delete<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept> to confirm that you want to delete the user account.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Exporting User Accounts</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>You can export user accounts into a CSV file.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Exporting can be used to copy the accounts to another machine or to preserve them as a backup.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>When an account is exported, the assigned boundaries or roles are <bpt id="p1">**</bpt>not included<ept id="p1">**</ept> in the export.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>If you import the account later, the <ph id="ph1">`BASIC_USER`</ph> role is automatically assigned unless you choose to assign the <ph id="ph2">`POWER_USER`</ph> role to all accounts being imported.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Keep in mind that you can manually <bpt id="p1">[</bpt>assign roles<ept id="p1">](../deployr/deployr-admin-console-permissions-with-roles.md)</ept> individually later.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Figure: Export User Accounts page</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>To export:</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>Users<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>User List<ept id="p1">**</ept> appears.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Export User Accounts<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Select the account(s) to be exported.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Export to File<ept id="p1">**</ept> and download the file.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Importing User Accounts</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Importing allows you to retrieve all of the accounts from a previously exported CSV file.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Alternately, you can also import a CSV file you have created yourself using the proper format.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Since role and boundary assignments cannot be exported, all imported user accounts are automatically assigned the <ph id="ph1">`BASIC_USER`</ph> role at import time unless you choose to assign the <ph id="ph2">`POWER_USER`</ph> role.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>You can, of course, manually add roles to users later after importing.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>For security reasons, user passwords are not exported.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>You can add a plain text password manually in the password field in the exported CSV file <bpt id="p1">**</bpt>prior to import<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>To import:</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>Users<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>From the <bpt id="p1">**</bpt>User List<ept id="p1">**</ept>, click <bpt id="p2">**</bpt>Import User Accounts<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Browse<ept id="p1">**</ept> and select the CSV file to be imported.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Load<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><bpt id="p1">_</bpt>Figure: Import User Accounts page<ept id="p1">_</ept> <ph id="ph1">![](media/deployr-admin-console-user-accounts/0300000C_624x252.png)</ph></source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>To disable user accounts so that they do not have access to the server until you are ready, select the <bpt id="p1">**</bpt>Disable user account<ept id="p1">**</ept> option.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>You can always enable or disable user accounts individually later.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>If desired, select the option to <bpt id="p1">**</bpt>Automatically grant POWER_USER permissions to user accounts on this import<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>It is not always prudent to assign this role to all users so weigh this option carefully.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Note that all imported users are automatically assigned to the BASIC_USER role.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`ADMINISTRATOR`</ph> and <ph id="ph2">`POWER_USER`</ph> roles have implicit permissions to install R packages.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`BASIC_USER`</ph> role does not have permissions to manage R packages.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>To allow a user that was assigned only to the <ph id="ph1">`BASIC_USER`</ph> role the rights to install an R package, you must edit the user account after importing and assign the <ph id="ph2">`PACKAGE_MANAGER`</ph> role.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Choose the account(s) to import.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Import<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>If a user account by the same name already exists, a message appears to inform you that the incoming account was rejected.</source>
        </trans-unit></group></body></file></xliff>