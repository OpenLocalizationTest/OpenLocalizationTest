<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-security-account-locking.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e171e2d9808ead303087eeb80f158d32b393650bd.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">171e2d9808ead303087eeb80f158d32b393650bd</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-security-account-locking.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Security - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Security in DeployR: Authentication, HTTPS, SSL, and access controls for server, Project file and Repository File, and more.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Account Locking Policies</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>To protect against brute force techniques that can be used to try and "guess" passwords on <bpt id="p1">*</bpt>basic authentication<ept id="p1">*</ept> and <bpt id="p2">*</bpt>PAM authenticated<ept id="p2">*</ept> user accounts, DeployR enforces automatic account locking when repeated authentication attempts fail within a given period of time for a given user account:</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>By default, automatic account locking is enabled and activates following 10 failed attempts at authentication on a given user account.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>To disable this feature, set the following configuration property to <ph id="ph1">`false`</ph>:</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>When enabled, a count of failed authentication attempts is maintained by DeployR for each user account.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The count is compared to the value specified on the following configuration property:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>If the count exceeds the <ph id="ph1">`failures.limit`</ph> value, then the user account is locked and any further attempts to authentication on that account will be rejected with an error indicating that the account has been temporarily locked.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>To manage locked user accounts, the administrator has two choices.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The chosen behavior is determined by the value assigned to the following configuration property:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`lock.timeout`</ph> value is set to 0, then locked user accounts must be manually unlocked by the administrator in the <bpt id="p1">[</bpt>Users tab<ept id="p1">](deployr-admin-console-user-accounts.md#viewing-and-editing-user-accounts)</ept> of the Administration Console.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`lock.timeout`</ph> value (measured in seconds), is set to any non-zero, positive value then a locked user account will be automatically <bpt id="p1">*</bpt>unlocked<ept id="p1">*</ept> by DeployR once the <ph id="ph2">`lock.timeout`</ph> period of time has elapsed without further activity on the account.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>By default, automatic account <bpt id="p1">*</bpt>unlocking<ept id="p1">*</ept> is enabled and occurs 30 minutes after the last failed attempt at authentication on an account.</source>
        </trans-unit></group></body></file></xliff>