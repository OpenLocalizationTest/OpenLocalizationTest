<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-security-project-access.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e41442cdb57bc44547b9262dbc65122fd9fc19736.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">41442cdb57bc44547b9262dbc65122fd9fc19736</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-security-project-access.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Security - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Security in DeployR: Authentication, HTTPS, SSL, and access controls for server, Project file and Repository File, and more.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Project and Repository File Access Controls</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>DeployR enforces a consistent security model across projects and repository-managed files.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>This model is based on two simple precepts: ownership and access levels.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Project Access Controls</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>When a project is created, it is privately owned by default, meaning it is visible only to its owner.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Such user-based privacy is a central aspect of the DeployR security model.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The owner of a temporary or persistent project has, by default, full read-write access to that project and use of the full set of project-related APIs.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>DeployR introduced a type of secure, temporary project called a <bpt id="p1">*</bpt>blackbox project<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Blackbox projects restrict access to the underlying R session.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>In this case, the project owner can use only a small subset of the project-related APIs, collectively known as the “Blackbox API Controls”.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If the owner of a project wants to grant read-only access to that project to other authenticated users, then the owner can set the access level for the project to <ph id="ph1">`Shared`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>You can change the access level on a project using the <ph id="ph1">`/r/project/about/update`</ph> API call.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Anonymous users are not permitted access to projects.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>For more information, refer to the <bpt id="p1">[</bpt>API Reference Help<ept id="p1">](deployr-api-reference.md)</ept>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Repository File Access Controls</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>When a repository-managed file is created, it is privately owned by default, meaning it is visible only to its owner.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Such user-based privacy is a central aspect of the DeployR security model.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The owner of a repository-managed file has full read-write access to that file and use of the full set of repository-related APIs.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If the owner of a repository-managed file wants to grant read-only access to that file to other users, then the owner can set the file’s access level to one of the following values:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>- the default access level, the file is visible to its author(s) only.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>- the file is visible to authenticated users that have been granted one or more of the roles indicated on the restricted property of the file.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>- the file is visible to all authenticated users when the shared property is true.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>- the file is visible to all authenticated and all anonymous users when the published property is true.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>You can change the access level on a repository-managed file using the <ph id="ph1">`/r/repository/file/update`</ph> <bpt id="p1">[</bpt>API call<ept id="p1">](deployr-api-reference.md#repository-on-the-api)</ept> or using the <bpt id="p2">[</bpt>Repository Manager<ept id="p2">](deployr-repository-manager-files.md#about-file-properties)</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Repository File Download Controls</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The repository file download controls provide fine-grain control over who can download repository file data.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>It is important to tailor the configuration of these controls in your DeployR external configuration file in order to enforce your preferred download policy for repository-managed files.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Repository Scripts Access Controls</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Repository-managed R scripts can be exposed as an executable on the API.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Since repository-managed R scripts are a type of repository-managed file, all information in the <bpt id="p1">[</bpt>previous section<ept id="p1">](#repository-file-access-controls)</ept> also applies to repository-managed scripts.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>However, repository-managed R scripts deserve special mention since scripts can be managed through the Administration Console interface.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Additionally, when you work with the R scripts in the Administration Console, you will likely also use and work with roles so as to impose restricted access to your R scripts.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For information on how to use roles as a means to restrict access to individual R scripts, refer to the <bpt id="p1">[</bpt>Administration Console Help<ept id="p1">](deployr-admin-managing-server-policies.md#server-policy-properties)</ept>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Repository Script Download Controls</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The repository script download controls provide fine-grain control over who can download repository script data.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>It is important to tailor the configuration of these controls in your DeployR external configuration file in order to enforce your preferred download policy for repository-managed scripts.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>File Type Black List Controls</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The file type black-list controls provide fine-grain control over the types of files that can be:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Uploaded, transferred and written into the repository or</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Uploaded, transferred, written and loaded into the working directory of a project (R session).</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>These controls are particularly useful if an administrator wants to ensure malicious executable files or shell scripts are not uploaded and executed on the DeployR server.</source>
        </trans-unit></group></body></file></xliff>