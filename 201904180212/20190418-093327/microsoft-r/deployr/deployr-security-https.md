<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-security-https.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b45d5c0b18eb1975ff4499b2ef8033492f5d216673.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5d5c0b18eb1975ff4499b2ef8033492f5d216673</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-security-https.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Security - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Security in DeployR: Authentication, HTTPS, SSL, and access controls for server, Project file and Repository File, and more.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Configure SSL/TLS for DeployR (HTTPS)</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Both <bpt id="p1">**</bpt>Transport Layer Security<ept id="p1">**</ept> (TLS) protocol version 1.2 and its predecessor <bpt id="p2">**</bpt>Secure Sockets Layer (SSL)<ept id="p2">**</ept> are commonly-used cryptographic protocols for managing the security of message transmissions on the Internet.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>DeployR allows for HTTPS within a connection encrypted by TLS and/or SSL.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>In DeployR Enterprise for Microsoft R Server 8.0.5, the DeployR Web server as well as all APIs calls and utilities support TLS 1.2 and SSL.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>However, HTTPS is disabled by default.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>In DeployR 8.0.0, only SSL is supported.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Enabling TLS/SSL Support</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Once enabled, your client applications can make API calls that connect over HTTPS.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>For security reasons, we strongly recommend that TLS/SSL be enabled in <bpt id="p1">**</bpt>all production environments.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Since we cannot ship TLS/SSL certificates for you, TLS/SSL protocols on DeployR are disabled by default.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Enabling for DeployR for Microsoft R Server 8.0.5</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Securing connections between the DeployR Web server and client</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>In your firewall, be sure to open the Tomcat HTTPS port (8051) to the outside on the DeployR server machine.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If you are using the IPTABLES firewall or equivalent service for your server, use the <ph id="ph1">`iptables`</ph> command (or equivalent command/tool) to open the port.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If you are provisioning your server on a cloud service such as <bpt id="p1">[</bpt>Azure or an AWS EC2 instance<ept id="p1">](deployr-admin-install-in-cloud.md)</ept>, then you must also add endpoints for port 8051.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Enable HTTPS in the DeployR administrator utility:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Launch the utility with administrator privileges to enable HTTPS:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>For Linux</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>For Windows:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>From the main menu, choose option <bpt id="p1">**</bpt>Web Context and Security<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>From the sub-menu, choose option <bpt id="p1">**</bpt>Configure Server SSL/HTTPS<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>When prompted, answer <ph id="ph1">`Y`</ph> to the question <bpt id="p1">**</bpt>Enable SSL?<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>When prompted to provide the full file path to the trusted SSL certificate file, type the full path to the file.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If you do not have a trusted SSL certificate from a registered authority, you'll need a temporary keystore for testing purposes.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn how to create a temporary keystore<ept id="p1">](#temporary-keystore)</ept>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>We recommend that you use a trusted SSL certificate from a registered authority <bpt id="p1">**</bpt>as soon as possible<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>When prompted whether the certificate file is self-signed, answer <ph id="ph1">`N`</ph> if you are using a trusted SSL certificate from a registered authority -or- <ph id="ph2">`Y`</ph> if self-signed.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Return to the main menu and choose the option <bpt id="p1">**</bpt>Start/Stop Server<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>You must restart DeployR so that the changes can take effect.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>When prompted whether you want to stop (S) or restart (R) the DeployR server, enter <ph id="ph1">`R`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>It may take some time for the Tomcat process to terminate and restart.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Exit the utility.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Test these changes by logging into the landing page and visiting DeployR Administration Console using the new HTTPS URL at <ph id="ph1">`https://&lt;DEPLOYR_SERVER_IP&gt;:8051/deployr/landing`</ph>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`&lt;DEPLOYR_SERVER_IP&gt;`</ph> is the IP address of the DeployR main server machine.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If you are using an untrusted, self-signed certificate, and you or your users are having difficulty reaching DeployR in your browser, see this <bpt id="p1">[</bpt>Alert<ept id="p1">](#alertusers)</ept>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Securing connections between DeployR Web server and the database</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If your corporate policies require that you secure the communications between the Web server and the DeployR database, then you should configure DeployR to use either a <bpt id="p1">[</bpt>SQL Server database<ept id="p1">](deployr-install-on-windows.md#sqlserver)</ept> or a <bpt id="p2">[</bpt>PostgreSQL database<ept id="p2">](deployr-install-on-linux.md#postgresql)</ept> rather than the default H2 database.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>After configuring DeployR to use one of those databases, you must also properly secure the database connections and force encryption.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>For SQL Server 2016, you should:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Read these articles for information on how to enable TLS for SQL Server:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>In the <ph id="ph1">`$DEPLOYR_HOME/deployr/deployr.groovy`</ph> external configuration file, add <ph id="ph2">`encrypt=true;trustServerCertificate=true`</ph> to the connection string.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>For PostgreSQL, you should:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Review the documentation here: <ph id="ph1">https://www.postgresql.org/docs/9.1/static/ssl-tcp.html</ph></source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>In the <ph id="ph1">`$DEPLOYR_HOME\deployr\deployr.groovy`</ph> external configuration file, add <ph id="ph2">`ssl=true`</ph> to the <ph id="ph3">`properties`</ph> section of the <ph id="ph4">`dataSource`</ph> property block.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Enabling for DeployR 8.0.0</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Provide an SSL certificate.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>If you have a trusted SSL certificate from a registered authority, then copy it to the Tomcat directory so it can be deployed at startup.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>(If you do not have one, skip to the next bullet to define a temporary certificate.)</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Be sure to specify the correct Tomcat path for the <ph id="ph1">`-keystore`</ph> argument.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>For Linux / OS X:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>This example is written for user <ph id="ph1">`deployr-user`</ph>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>For another user, use the appropriate filepath to the <ph id="ph1">`.keystore`</ph>.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Go to the directory in which the keystore is stored.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Copy the certificate keystore to the Tomcat directory.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>At the prompt, type:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>For Windows:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Go to the directory in which the keystore is stored.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Launch a command window as administrator and type the following at the prompt:</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>If you do not yet have a trusted SSL certificate from a registered authority, then create a temporary keystore for testing purposes.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>This temporary keystore will contain a “self-signed” certificate for Tomcat SSL on the server machine.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn how to create a temporary keystore<ept id="p1">](#temporary-keystore)</ept>.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Next, enable SSL support for Tomcat.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>For Linux / OS X:</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>This example is written for <ph id="ph1">`deployr-user`</ph>.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>For another user, use the appropriate filepath to <ph id="ph1">`server.xml`</ph> and <ph id="ph2">`web.xml`</ph> as well as the <ph id="ph3">`keystoreFile`</ph> property on the Connector.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Enable the HTTPS connector on Tomcat by <bpt id="p1">**</bpt>removing the comments<ept id="p1">**</ept> around the following code in the file <ph id="ph1">`$DEPLOYR_HOME/tomcat/tomcat7/conf/server.xml`</ph>.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Force Tomcat to upgrade all HTTP connections to HTTPS connections by <bpt id="p1">**</bpt>removing the comments<ept id="p1">**</ept> around the following code in the file <ph id="ph1">`$DEPLOYR_HOME/tomcat/tomcat7/conf/web.xml`</ph>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Be sure to open the Tomcat HTTPS port (8001) to the outside on the DeployR server machine.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>If you are using the IPTABLES firewall or equivalent service for your server, use the iptables command (or equivalent command/tool) to open the port.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>If you are provisioning your server on a cloud service such as <bpt id="p1">[</bpt>Azure or AWS EC2<ept id="p1">](deployr-admin-install-in-cloud.md)</ept>, then you must also add endpoints for port 8001.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>For Windows:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Enable the HTTPS connector/channel on Tomcat by <bpt id="p1">**</bpt>removing the comments<ept id="p1">**</ept> around the following code in the file <ph id="ph1">`C:\Program Files\Microsoft\DeployR-8.0\Apache_Tomcat\conf\server.xml`</ph>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Force Tomcat to upgrade all HTTP connections to HTTPS connections by <bpt id="p1">**</bpt>removing the comments<ept id="p1">**</ept> around the following code in the file <ph id="ph1">`C:\Program Files\Microsoft\DeployR-8.0\Apache_Tomcat\conf\web.xml`</ph>.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Be sure to open the Tomcat HTTPS port (8001) to the outside on the DeployR server machine.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>If you are using the IPTABLES firewall or equivalent service for your server, use the iptables command (or equivalent command/tool) to open the port.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>If you are provisioning your server on a cloud service such as <bpt id="p1">[</bpt>Azure or AWS EC2<ept id="p1">](deployr-admin-install-in-cloud.md)</ept>, then you must also add endpoints for port 8001.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Then, enable SSL support for DeployR.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>For Linux / OS X:</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Enable SSL support on the Administration Console by changing <ph id="ph1">`false`</ph> to <ph id="ph2">`true`</ph> in the following line of the DeployR external configuration file, <ph id="ph3">`$DEPLOYR_HOME/deployr/deployr.groovy`</ph>:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Enable HTTPS in the server policies so that any non-HTTPS connections to the server are automatically rejected.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Run the <ph id="ph1">`setWebContext.sh`</ph> script and specify the value of <ph id="ph2">`true`</ph> for the <ph id="ph3">`https`</ph> argument:</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>For Windows:</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Enable SSL support on the Administration Console by changing <ph id="ph1">`false`</ph> to <ph id="ph2">`true`</ph> in the following line of the DeployR external configuration file, <ph id="ph3">`C:\Program Files\Microsoft\DeployR-8.0\deployr/deployr.groovy`</ph>:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Enable HTTPS in the server policies so that any non-HTTPS connections to the server are automatically rejected.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Run the <ph id="ph1">`setWebContext.bat`</ph> script and specify the value of <ph id="ph2">`true`</ph> for the <ph id="ph3">`https`</ph> argument:</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Upon completion of this script with <ph id="ph1">`-https true`</ph>, the following changes will have been made to the <bpt id="p1">[</bpt>server policies<ept id="p1">](deployr-admin-managing-server-policies.md#server-policy-properties)</ept> in the Administration Console:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The server web context now resembles <ph id="ph1">`https://xx.xx.xx.xx:8001/deployr`</ph> instead of <ph id="ph2">`http://xx.xx.xx.xx:8000/deployr`</ph>.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`Enable HTTPS`</ph> properties for each of operation policies (authenticated, anonymous, and asynchronous) are all checked.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Restart DeployR<ept id="p1">**</ept> by <bpt id="p2">[</bpt>stopping and starting all its services<ept id="p2">](deployr-common-administration-tasks.md#startstop)</ept> so the changes can take effect.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Between stopping and starting, be sure to pause long enough for the Tomcat process to terminate.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Test<ept id="p1">**</ept> these changes by logging into the landing page and visiting DeployR Administration Console using the new HTTPS URL at <ph id="ph1">`https://&lt;DEPLOYR_SERVER_IP&gt;:8001/deployr/landing`</ph>.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`&lt;DEPLOYR_SERVER_IP&gt;`</ph> is the IP address of the DeployR main server machine.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>If you are using an untrusted, self-signed certificate, and you or your users are having difficulty reaching DeployR in your browser, see the <bpt id="p1">[</bpt>Alert<ept id="p1">](#alertusers)</ept> at the end of step 1.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Generating a Temporary Keystore</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>If you do not have a trusted SSL certificate from a registered authority, you'll need a temporary keystore for testing purposes.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>This temporary keystore will contain a “self-signed” certificate for Tomcat SSL on the server machine.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Be sure to specify the correct Tomcat path for the <ph id="ph1">`-keystore`</ph> argument.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>For Windows:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Launch a command window <bpt id="p1">**</bpt>as administrator<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Run the <ph id="ph1">`keytool`</ph> to generate a temporary keystore file.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>At the prompt, type:</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>where <ph id="ph1">`&lt;JAVA_HOME&gt;`</ph> is the path to the supported version of JAVA and <ph id="ph2">`&lt;PATH-TO-KEYSTORE&gt;`</ph> is the full file path to the temporary keystore file.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Provide the information when prompted by the script as described below in this topic.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>For Linux:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Run the <ph id="ph1">`keytool`</ph> to generate a temporary keystore file.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>At a terminal prompt, type:</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>where <ph id="ph1">`&lt;PATH-TO-KEYSTORE&gt;`</ph> is the full file path to the temporary keystore file.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Provide the information when prompted by the script as described below in this topic.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>For Mac OS X:<ept id="p1">**</ept> (DeployR 8.0.0 Open only)</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Run the <ph id="ph1">`keytool`</ph> to generate a temporary keystore file.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>At a terminal prompt, type:</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>where <ph id="ph1">`&lt;PATH-TO-KEYSTORE&gt;`</ph> is the full file path to the temporary keystore file.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Provide the information when prompted by the script as described below in this topic.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>When prompted by the script, provide the following information when prompted by the script:</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>For the keystore password, enter <ph id="ph1">`changeit`</ph> and confirm this password.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>For your name, organization, and location, either provide the information or press the Return key to skip to the next question.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>When presented with the summary of your responses, enter <ph id="ph1">`yes`</ph> to accept these entries.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>For a key password for Tomcat, press the Return key to use <ph id="ph1">`changeit`</ph>.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Alert Your Users!<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>If using a self-signed certificates, then alert your users.When they attempt to open the DeployR landing page, Administration Console, or Repository Manager in their Web browser, they will be prompted to acknowledge and accept your self-signed certificate as a security precaution.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Each browser prompts in a different way, such as requiring users to acknowledge "I Understand the Risks” (Firefox), or to click “Advanced” (Chrome) or click “Continue” (Safari).</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>We strongly recommend that you use a trusted SSL certificate from a registered authority in your production environments.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Disabling SSL Support</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Disabling for DeployR for Microsoft R Server 8.0.5</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Secure Sockets Layer (SSL)<ept id="p1">**</ept> is a commonly-used protocol for managing the security of message transmissions on the Internet.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>By default, SSL on DeployR is disabled.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>If you have enabled SSL at some time and you now wish to disable SSL, follow the steps in this section.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>We strongly recommended that SSL/HTTPS be enabled in <bpt id="p1">**</bpt>all production environments.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>In the firewall, be sure to close the Tomcat HTTPS port (8051) to the outside on the DeployR server machine.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>If you are using the IPTABLES firewall or equivalent service for your server, use the <ph id="ph1">`iptables`</ph> command (or equivalent command/tool) to close the port.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>If you are provisioning your server on a cloud service such as <bpt id="p1">[</bpt>Azure or an AWS EC2 instance<ept id="p1">](deployr-admin-install-in-cloud.md)</ept>, then you must also remove endpoints for port 8051.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Launch the DeployR administrator utility script with administrator privileges to disable HTTPS:</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>For Linux</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>For Windows:</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>From the main menu, choose option <bpt id="p1">**</bpt>Web Context and Security<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>From the sub-menu, choose option <bpt id="p1">**</bpt>Configure Server SSL/HTTPS<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>When prompted, answer <ph id="ph1">`Y`</ph> to the question <bpt id="p1">**</bpt>Disable SSL?<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Return to the main menu and choose option <bpt id="p1">**</bpt>Start/Stop Server<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>You must restart DeployR so that the change can take effect.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Enter <ph id="ph1">`R`</ph> to restart the server.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>It may take some time for the Tomcat process to terminate and restart.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Test these changes by logging into the landing page and visiting DeployR Administration Console using the new HTTP URL at <ph id="ph1">`https://&lt;DEPLOYR_SERVER_IP&gt;:8050/deployr/landing`</ph>.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`&lt;DEPLOYR_SERVER_IP&gt;`</ph> is the IP address of the DeployR main server machine.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Disabling for DeployR 8.0.0</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Disable SSL support for Tomcat.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>For Linux / OS X:</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>This example is written for <ph id="ph1">`deployr-user`</ph>.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>For another user, use the appropriate filepath to <ph id="ph1">`server.xml`</ph> as well as the <ph id="ph2">`keystoreFile`</ph> property on the Connector.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>For another user,also use the appropriate filepath to <ph id="ph1">`web.xml`</ph>.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>Disable the HTTPS connector on Tomcat by <bpt id="p1">**</bpt>commenting out<ept id="p1">**</ept> the following code in the file <ph id="ph1">`$DEPLOYR_HOME/tomcat/tomcat7/conf/server.xml`</ph>.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Be sure to close the Tomcat HTTPS port (8001) to the outside on the DeployR server machine.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>If you are using the IPTABLES firewall or equivalent service for your server, use the <ph id="ph1">`iptables`</ph> command (or equivalent command/tool) to close the port.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>If you are provisioning your server on a cloud service such as <bpt id="p1">[</bpt>Azure or AWS EC2<ept id="p1">](deployr-admin-install-in-cloud.md)</ept>, then you must also remove endpoints for port 8001.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Disable the upgrade of all HTTP connections to HTTPS connections by <bpt id="p1">**</bpt>commenting out<ept id="p1">**</ept> the following code in the file <ph id="ph1">`$DEPLOYR_HOME/tomcat/tomcat7/conf/web.xml`</ph>.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>For Windows:</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>This example is written for <ph id="ph1">`deployr-user`</ph>.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>For another user, use the appropriate filepath to <ph id="ph1">`server.xml`</ph> as well as the <ph id="ph2">`keystoreFile`</ph> property on the Connector.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>For another user,also use the appropriate filepath to <ph id="ph1">`web.xml`</ph>.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Disable the HTTPS connector/channel on Tomcat by <bpt id="p1">**</bpt>commenting out<ept id="p1">**</ept> the following code in the file <ph id="ph1">`C:\Program Files\Microsoft\DeployR-8.0\Apache_Tomcat\conf\server.xml`</ph>.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Be sure to close the Tomcat HTTPS port (8001) to the outside on the DeployR server machine.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>If you are using the IPTABLES firewall or equivalent service for your server, use the <ph id="ph1">`iptables`</ph> command (or equivalent command/tool) to close the port.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>If you are provisioning your server on a cloud service such as <bpt id="p1">[</bpt>Azure or AWS EC2<ept id="p1">](deployr-admin-install-in-cloud.md)</ept>, then you must also remove endpoints for port 8001.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>Disable the upgrade of all HTTP connections to HTTPS connections by <bpt id="p1">**</bpt>commenting out<ept id="p1">**</ept> the following code in the file <ph id="ph1">`C:\Program Files\Microsoft\DeployR-8.0\Apache_Tomcat\conf\web.xml`</ph>.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Next, disable SSL support for DeployR.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>For Linux / OS X:</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>Disable SSL support on the Administration Console by changing <ph id="ph1">`true`</ph> to <ph id="ph2">`false`</ph> in the following line of the DeployR external configuration file, <ph id="ph3">`$DEPLOYR_HOME/deployr/deployr.groovy`</ph>:</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Disable HTTPS in the server policies.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>Run the <ph id="ph1">`setWebContext.sh`</ph> script and specify the value of <ph id="ph2">`false`</ph> for the <ph id="ph3">`https`</ph> argument:</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>For Windows:</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>Enable SSL support on the Administration Console by changing <ph id="ph1">`false`</ph> to <ph id="ph2">`true`</ph> in the following line of the DeployR external configuration file, <ph id="ph3">`C:\Program Files\Microsoft\DeployR-8.0\deployr/deployr.groovy`</ph>:</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>Run the <ph id="ph1">`setWebContext.bat`</ph> script and specify the value of <ph id="ph2">`false`</ph> for the <ph id="ph3">`https`</ph> argument:</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Upon completion of the <ph id="ph1">`setWebContext`</ph> script with <ph id="ph2">`-https false`</ph>, the following changes will have been made to the <bpt id="p1">[</bpt>server policies<ept id="p1">](deployr-admin-managing-server-policies.md#server-policy-properties)</ept> in the Administration Console:</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>The server web context now resembles <ph id="ph1">`http://xx.xx.xx.xx:8000/deployr`</ph>.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`Enable HTTPS`</ph> properties for each of operation policies (authenticated, anonymous, and asynchronous) are disabled.</source>
        </trans-unit></group></body></file></xliff>