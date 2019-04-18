<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-admin-console-permissions-with-roles.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18cee49622a89ce29c8b6ea2e58eb0cbbeb3af43e82.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">ee49622a89ce29c8b6ea2e58eb0cbbeb3af43e82</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-admin-console-permissions-with-roles.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>DeployR Administration Console Help - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Managing Roles in the DeployR Administration Console</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Managing Permissions with Roles</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Users are granted permissions to perform operations on the DeployR Web services API by the role(s) assigned to them.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Having clearly defined roles in this console simplifies the process of granting permissions to new or existing users.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>DeployR is delivered with predefined system roles you can assign to users.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>These predefined system roles determine user permissions within DeployR by granting individual users access to the console or programmatic access on the API.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>You can also create custom roles to constrain access to certain scripts.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Once you have created a custom role for that purpose, a script author can set a script’s access rights to <bpt id="p1">**</bpt>Restricted<ept id="p1">**</ept> and specify one or more new custom roles.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Then, only those users assigned to at least one of the roles specified for that script are permitted to execute the script.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>You can manage the access rights to a file in the <bpt id="p1">[</bpt>DeployR Repository Manager<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>You can view the available roles by clicking <bpt id="p1">**</bpt>Roles<ept id="p1">**</ept> in the main menu.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Clicking a role in the list reveals the list of users assigned to this role.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">_</bpt>Figure: Role List page<ept id="p1">_</ept></source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Predefined System Roles</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The following DeployR system roles are shipped with DeployR and can be assigned to user accounts.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Role Name</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Role<ph id="ph1">&amp;nbsp;</ph>Description</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The<ph id="ph1"> `ADMINISTRATOR`</ph> role identifies the user as an administrator.<bpt id="p1"> [</bpt>There is only one administrator for the console<ept id="p1">](deployr-admin-console-user-accounts.md#preconfigured-user-accounts)</ept>, and that is the user<ph id="ph2"> `admin`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Users with this role are granted permissions to access the full API and to install R packages.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Full access includes the ability to execute scripts and arbitrary blocks of R code.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Users with this role are granted permissions to access the full API with the exception of being able to execute arbitrary blocks of R code on the API.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>However, they can execute R scripts.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Users with this role are granted permissions to install R packages using the<ph id="ph1"> `install.packages()`</ph><ph id="ph2"> </ph>command.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>By default,<ph id="ph1"> `ADMINISTRATOR`</ph><ph id="ph2"> </ph>and<ph id="ph3"> `POWER_USER`</ph><ph id="ph4"> </ph>have implicit<ph id="ph5"> `PACKAGE_MANAGER`</ph><ph id="ph6"> </ph>rights, while <ph id="ph7">`BASIC_USER`</ph><ph id="ph8"> </ph>does not.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Viewing, Editing, and Assigning Roles</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>You can review, edit, and assign custom roles.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>System roles cannot be edited.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To view and edit a role:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>Roles<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Role List<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Role List<ept id="p1">**</ept> table, click the role you want to review or edit.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Role Details<ept id="p1">**</ept> page displays the role’s name and description as well as the names of any users to which the role is assigned.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The list of scripts to which a role may be assigned does not appear on this page.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">_</bpt>Figure: Role Details page<ept id="p1">_</ept></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>To edit a custom role, do the following:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Edit<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Change the name or description as needed.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If you change the name of role, it is updated throughout the console.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>You cannot edit a system role delivered with the product.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Update<ept id="p1">**</ept> to save the changes.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To assign a role to a user:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>Users<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>User List<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Click the account name you want to edit.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>User Details<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Edit<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Edit User<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Select all applicable roles.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Update<ept id="p1">**</ept> to save the changes.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Creating Custom Roles</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>While the system roles will suffice in many cases, there are times when it might be beneficial to create custom roles to constrain access to certain scripts according to a specific organizational, departmental, or functional need.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Any script author can set the access rights to his or her script to <bpt id="p1">**</bpt>Restricted<ept id="p1">**</ept> and specify one or more roles.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Then, only the users assigned to one of the specified roles are permitted to execute that script.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>For more details on defining access rights for scripts, refer the <bpt id="p1">[</bpt>DeployR Repository Manager<ept id="p1">](../what-is-operationalization.md)</ept> documentation.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To create a custom role:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>Roles<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Role List<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>From the <bpt id="p1">**</bpt>Role List<ept id="p1">**</ept> page, click <bpt id="p2">**</bpt>New Role<ept id="p2">**</ept> in the menu.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>New Role<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><bpt id="p1">_</bpt>Figure: New Role page<ept id="p1">_</ept></source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Enter a <bpt id="p1">**</bpt>Role name<ept id="p1">**</ept> and <bpt id="p2">**</bpt>Description<ept id="p2">**</ept> for the new role.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create<ept id="p1">**</ept> to save the new role.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>You can now assign this role to users or scripts in the console.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>To assign a role, edit the user or script and select the role(s).</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Deleting Custom Roles</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>While you cannot delete any of the system roles, you can delete a custom role.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>If you delete a custom role that is assigned to users, then that association between user and role is automatically removed upon deletion.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>To delete a custom role:</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>Roles<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Role List<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Click name of the custom role you want to delete.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Role Details<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Delete<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept> to confirm that you want to delete.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Exporting Roles</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>You can export roles in a CSV file.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Exporting can be useful when you want to copy the roles to another machine or to preserve them as a backup, for example.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>You can later import the contents of this file to this server or across multiple server deployments.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source><bpt id="p1">_</bpt>Figure: Export Roles page<ept id="p1">_</ept></source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To export:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>Roles<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>From the <bpt id="p1">**</bpt>Role List<ept id="p1">**</ept>, click <bpt id="p2">**</bpt>Export Roles<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Select the role(s) to be exported.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Export to File<ept id="p1">**</ept> and save the file.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Importing Roles</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Importing into the server database allows you to retrieve all of the roles from a previously exported CSV file.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Alternately, you can also import a CSV file you have created yourself using the proper format.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source><bpt id="p1">_</bpt>Figure: Import Roles page<ept id="p1">_</ept></source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>To import:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>Roles<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>From the <bpt id="p1">**</bpt>Role List<ept id="p1">**</ept>, click <bpt id="p2">**</bpt>Import Roles<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Browse<ept id="p1">**</ept> and select the file to be imported.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>By default, the file has the CSV extension.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Load<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Choose which role(s) to import.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Import<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>If a role by the same name already exists, a message appears to inform you that the incoming role was rejected.</source>
        </trans-unit></group></body></file></xliff>