<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-security.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f37f76ff980ada0e41014d58a0d61bf94886dd58a.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">37f76ff980ada0e41014d58a0d61bf94886dd58a</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-security.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Security in DeployR - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Security in DeployR: Authentication, HTTPS, SSL, and access controls for server, Project file and Repository File, and more.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Overview of DeployR Security</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>DeployR is a server framework that exposes the R platform as a service to allow the integration of R statistics, analytics, and visualizations inside Web, desktop, and mobile applications.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>In addition to providing a simple yet powerful Web services API, the framework also supports a highly flexible, enterprise security model.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>By default, DeployR supports basic authentication.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Users simply provide plain text username and password credentials, which are then matched against user account data stored in the DeployR database.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>User accounts are created and managed by an administrator using the DeployR Administration Console.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Given these credentials are passed from client to server as plain text, we strongly recommend, in your production environments, that you <bpt id="p1">[</bpt>enable and use HTTPS connections<ept id="p1">](../operationalize/configure-https.md)</ept> every time your application attempts to authenticate with DeployR.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>While basic authentication provides a simple and reliable authentication solution, the ability to deliver a seamless integration with existing enterprise security solutions is often paramount.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The DeployR enterprise security model can easily be configured to "plug" into a number of widely adopted enterprise security solutions.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Get More DeployR Power:<ept id="p1">**</ept> Basic Authentication is available for all DeployR configurations and editions.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Get DeployR Enterprise today to take advantage of great DeployR features like enterprise security and <bpt id="p1">[</bpt>a scalable grid framework<ept id="p1">](deployr-admin-managing-the-grid.md)</ept>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Note that DeployR Enterprise is part of Microsoft R Server.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The DeployR security model is sufficiently flexible that it can work with multiple enterprise security solutions at the same time.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>As such, DeployR Enterprise ships with a number of security providers that together represent a provider-chain upon which user credentials are evaluated.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Authentication and Authorization<ept id="p1">](../operationalize/configure-authentication.md)</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Every aspect of the DeployR security model is controlled by the configuration properties found in the DeployR external configuration file.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>This file can be found at <ph id="ph1">`$DEPLOYR_HOME/deployr/deployr.groovy`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The following security topics detail how to work with these configuration properties to achieve your preferred security implementation.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Authorization and Authentication<ept id="p1">](../operationalize/configure-authentication.md)</ept></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>HTTPS and SSL Support<ept id="p1">](../operationalize/configure-https.md)</ept></source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Server Access Policies<ept id="p1">](deployr-security-server-access.md)</ept></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Project and Repository File Access Controls<ept id="p1">](deployr-security-project-access.md)</ept></source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Password Policies<ept id="p1">](deployr-security-passwords.md)</ept></source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Account Locking Policies<ept id="p1">](deployr-security-account-locking.md)</ept></source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RServe Execution Context<ept id="p1">](deployr-security-rserve-execution-context.md)</ept></source>
        </trans-unit></group></body></file></xliff>