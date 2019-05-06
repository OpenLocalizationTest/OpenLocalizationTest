<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="configure-https.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750f9649a18c8e6f35f62200e57c6a52fc951ca6e74.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">f9649a18c8e6f35f62200e57c6a52fc951ca6e74</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\configure-https.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>HTTPS SSL / TLS 1.2 for Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn how to add enterprise-grade security (HTTPS SSL / TLS 1.2) for Machine Learning Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Enable SSL or TLS for Connection Security in Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies to: Machine Learning Server, Microsoft R Server 9.x</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>For security reasons, we strongly recommend that SSL/TLS 1.2 be enabled in <bpt id="p1">**</bpt>all production environments.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Since we cannot ship certificates for you, these protocols are disabled by default.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>You can use HTTPS within a connection encrypted by SSL/TLS 1.2.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>To enable SSL/TLS, you need some or all of these certificates.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>HTTPS Certificates</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Web Node</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Compute Node</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>API certificate</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Secures communication between client applications and web node.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>This certificate works for both one-box and enterprise setups.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Yes, with private key</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>No</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Compute node certificate</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Encrypts the traffic between the web node and compute node.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>You can use a unique certificate for each compute node, or you can use one common Multi-Domain (SAN) certificate for all compute nodes.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Note: If a compute node is inside the web node's trust boundary, then this certificate is not needed.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This certificate works for enterprise setups.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>No</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Yes, with private key</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Authentication certificate</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Authenticates the web node with the compute node so that only the web node can communicate with the compute node.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Note: If a compute node is inside the web node's trust boundary, then this certificate is not needed.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>This certificate works for enterprise setups.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Yes, with private and a public key</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>No</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Encrypt the Traffic between Client Applications and Machine Learning Server/R Server</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>We strongly recommend that SSL/TLS 1.2 be enabled in <bpt id="p1">**</bpt>all production environments.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>This section walks you through the steps for securing the connections between the client application and the web node.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Doing so encrypts the communication between client and web node to prevent traffic from being modified or read.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Windows: Using Your Default ASP .NET Core Web Server to Encrypt Traffic</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>On each machine hosting the web node, install and configure the certificate in the certificate store.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>For example, if you launch "Manage Computer Certificates" from your Windows Start menu, you can:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Install the trusted, signed <bpt id="p1">**</bpt>API HTTPS certificate<ept id="p1">**</ept> with a private key in the certificate store.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Make sure the name of the certificate matches the domain name of the web node URL.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Set the private key permissions.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Right click on the certificate and choose Manage private certificate from the menu.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Add a group called NETWORK SERVICE and give that group <ph id="ph1">`Read`</ph> access.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Network service</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Take note of the <ph id="ph1">`Subject`</ph> name of the certificate as you need this info later.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Open the configuration file, <bpt id="p1">[</bpt><ph id="ph1">\&lt;</ph>web-node-install-path&gt;<ept id="p1">](../operationalize/configure-find-admin-configuration-file.md)</ept>/appsettings.json.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>You can configure the HTTPS port for the web node in this file.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>In that file, search for the section starting with: "Kestrel": {</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Update and add properties in the Kestrel section to match the values for the API certificate.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The Subject name can be found as a property of your certificate in the certificate store.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`"Thumbprint"`</ph> to ensure that the correct certificate is loaded if there are multiple certificates on the same system with same name used for different purposes such as IPsec, TLS Web Server Authentication, Client Authentication, Server Authentication, and so on.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If you do not have multiple certificates with same name, you can leave the Thumbprint field empty.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Close and save the file.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Create a firewall rule to open port 443 to the public IP of the web node so that remote machines can access it.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Launch the administration tool/CLI and <bpt id="p1">[</bpt>restart the web node<ept id="p1">](configure-admin-cli-stop-start.md)</ept>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>In the same tool, run the <bpt id="p1">[</bpt>diagnostic test<ept id="p1">](configure-run-diagnostics.md)</ept> to send a test HTTPs request.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Windows: Using IIS to Encrypt</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Make sure the name of the certificate matches the domain name of the web node URL.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>On each machine hosting a web node:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Open the certificate store:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Install the trusted, signed <bpt id="p1">**</bpt>API HTTPS certificate<ept id="p1">**</ept> with a private key in the certificate store.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Make sure the name of the certificate matches the domain name of the web node URL.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Set the private key permissions.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Right click on the certificate and choose Manage private certificate from the menu.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Add a group called <ph id="ph1">`NETWORK SERVICE`</ph> and give that group <ph id="ph2">`Read`</ph> access.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Group</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Launch IIS.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Connections<ept id="p1">**</ept> pane on the left, expand the <bpt id="p2">**</bpt>Sites<ept id="p2">**</ept> folder and select the website.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Click on <bpt id="p1">**</bpt>Bindings<ept id="p1">**</ept> under the <bpt id="p2">**</bpt>Actions<ept id="p2">**</ept> pane on the right.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Click on <bpt id="p1">**</bpt>Add<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Choose <bpt id="p1">**</bpt>HTTPS<ept id="p1">**</ept> as the type and enter the <bpt id="p2">**</bpt>Port<ept id="p2">**</ept>, which is 443 by default.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Take note of the port number.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Select the SSL certificate you installed previously.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept> to create the new HTTPS binding.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Back in the <bpt id="p1">**</bpt>Connections<ept id="p1">**</ept> pane, select the website name.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Click the <bpt id="p1">**</bpt>SSL Settings<ept id="p1">**</ept> icon in the center of the screen to open the dialog.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Select the checkbox to <bpt id="p1">**</bpt>Require SSL<ept id="p1">**</ept> and require a client certificate.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Create a firewall rule to open port 443 to the public IP of the web node so that remote machines can access it.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Run the <bpt id="p1">[</bpt>diagnostic tool<ept id="p1">](configure-run-diagnostics.md)</ept> to send a test HTTPs request.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Restart the node or just run 'iisreset' on the command line.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Repeat on every web node.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>If satisfied with the new HTTPS binding, consider removing the "HTTP" binding to prevent any access via HTTP.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Linux: Encrypting Traffic</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Make sure the name of the certificate matches the domain name of the web node URL.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>On each Linux machine hosting a web node:</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Install the trusted, signed <bpt id="p1">**</bpt>API HTTPS certificate<ept id="p1">**</ept> with a private key in the certificate store.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Install NGINX version 1.11.6 or later.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Enable HTTPS on NGINX as described in these articles:</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Declare the certificate in the NGINX configuration file <ph id="ph1">`nginx.conf`</ph>.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Find the <ph id="ph1">`server`</ph> code block and update the following values:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>with the name of web node</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>with full path to the  <bpt id="p1">**</bpt>API HTTPS certificate<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>with the private key for that certificate</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>In the same <ph id="ph1">`server`</ph> code block, forward the traffic from port 443 to the web node's port 12800 (or another port if you changed it).</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Add the following lines after <ph id="ph1">`ssl_certificate_key`</ph>.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Close and save <ph id="ph1">`nginx.conf`</ph>.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Restart NGINX service.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>If using IPTABLES firewall, add the HTTPS port, which is 443 by default, to the firewall settings to allow communications between the client application and Machine Learning Server.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Launch the administration tool/CLI and <bpt id="p1">[</bpt>restart the web node<ept id="p1">](configure-admin-cli-stop-start.md)</ept>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Repeat on each web node.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Run the <bpt id="p1">[</bpt>diagnostic tool<ept id="p1">](configure-run-diagnostics.md)</ept> to send a test HTTPs request.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Now, you can access Machine Learning Server to operationalize analytics securely on https://&lt;webnode-server-name&gt; from your client applications.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Encrypt Communication between the Web Node and Compute Node</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>This section walks you through the steps for encrypting the traffic between the web node and each of its compute nodes.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>If a compute node is inside the web node's trust boundary, then encryption of this piece is not needed.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>However, if the compute node resides outside of the trust boundary, consider using the compute node certificate to encrypt the traffic between the web node and compute node.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>When encrypting, you have the choice of using one of the following <bpt id="p1">**</bpt>compute node HTTPS certificates<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>One unique certificate per machine hosting a compute node.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>One common Multi-Domain (SAN) certificate with all compute node names declared in the single certificate</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Windows: Using Your Default ASP .NET Core Web Server to Encrypt</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>On each machine hosting a compute node, install the trusted, signed <bpt id="p1">**</bpt>compute node HTTPS certificate<ept id="p1">**</ept> with a private key in the certificate store.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Make sure the name of the certificate matches the domain name of the compute node URL.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Also, take note of the <ph id="ph1">`Subject`</ph> name of the certificate as you need this info later.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>For non production environments, this <bpt id="p1">[</bpt>blog post<ept id="p1">](https://blogs.msdn.microsoft.com/microsoftrservertigerteam/2017/05/19/using-certificates-in-r-server-operationalization-for-linux/)</ept> demonstrates how to use a self-signed certificate in Linux.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>However, self-signed certificates are NOT recommended for production usage.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Update the external JSON configuration file, appsettings.json to configure the HTTPS port for the compute node:</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Open the configuration file, <bpt id="p1">[</bpt><ph id="ph1">\&lt;</ph>compute-node-install-path&gt;<ept id="p1">](../operationalize/configure-find-admin-configuration-file.md)</ept>/appsettings.json.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>In that file, search for the section starting with: "Kestrel": {</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Update and add properties in that section to match the values for the compute node certificate.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`Subject`</ph> name can be found as a property of your certificate in the certificate store.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`"Thumbprint"`</ph> to ensure that the correct certificate is loaded if there are multiple certificates on the same system with same name used for different purposes such as IPsec, TLS Web Server Authentication, Client Authentication, Server Authentication, and so on.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>If you do not have multiple certificates with same name, you can leave the Thumbprint field empty.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Close and save the file.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Launch the administration tool/CLI and <bpt id="p1">[</bpt>restart the compute node<ept id="p1">](configure-admin-cli-stop-start.md)</ept>.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>In the same tool, run the <bpt id="p1">[</bpt>diagnostic test<ept id="p1">](configure-run-diagnostics.md)</ept> to send a test HTTPs request.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Windows: Using IIS to Encrypt</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>On each machine hosting a compute node, install the trusted, signed <bpt id="p1">**</bpt>compute node HTTPS certificate<ept id="p1">**</ept> with a private key in the certificate store.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Make sure the name of the certificate matches the domain name of the compute node URL.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Launch IIS and follow the <bpt id="p1">[</bpt>instructions above<ept id="p1">](#iis)</ept>.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Restart the node or just run 'iisreset' on the command line.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Linux: Encrypting Traffic between Web Node and Compute Node</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Make sure the name of the certificate matches the domain name of the web node URL.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>On each Linux machine hosting a compute node:</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Install the trusted, signed <bpt id="p1">**</bpt>compute node HTTPS certificate<ept id="p1">**</ept> with a private key in the certificate store.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Install NGINX version 1.11.6 or later.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Enable HTTPS on NGINX as described in these articles:</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Declare the certificate in the NGINX configuration file <ph id="ph1">`nginx.conf`</ph>.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Find the <ph id="ph1">`server`</ph> code block and update the following values:</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>with the name of web node</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>with full path to the  <bpt id="p1">**</bpt>compute node HTTPS certificate<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>with the private key for that certificate</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>In the same <ph id="ph1">`server`</ph> code block, forward all the traffic (<ph id="ph2">`location /`</ph>) from port 443 to the compute node's port 12805 (or another port if you changed it).</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Add the following lines after <ph id="ph1">`ssl_certificate_key`</ph>.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Close and save <ph id="ph1">`nginx.conf`</ph>.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Restart NGINX service.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Launch the administration tool/CLI and <bpt id="p1">[</bpt>restart the compute node<ept id="p1">](configure-admin-cli-stop-start.md)</ept>.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Repeat on each compute node.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>On each web node, update the compute node URIs so they can be found.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Log in to each web node machine.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>For Machine Learning Server<ept id="p1">**</ept>, <bpt id="p2">[</bpt>declare the new URIs in administration tool/CLI<ept id="p2">](configure-admin-cli-compute-uris.md)</ept>.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>For R Server 9.x<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Open the configuration file, <bpt id="p1">[</bpt><ph id="ph1">\&lt;</ph>web-node-install-path&gt;<ept id="p1">](../operationalize/configure-find-admin-configuration-file.md)</ept>/appsettings.json.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Update the <ph id="ph1">`"Uris": {`</ph> properties so that declared compute node now points to <ph id="ph2">`https://&lt;compute-node-ip&gt;`</ph> (without the port number):</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>Close and save the file.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Launch the administration tool/CLI and <bpt id="p1">[</bpt>restart the web node<ept id="p1">](configure-admin-cli-stop-start.md)</ept>.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Verify the configuration by running <bpt id="p1">[</bpt>diagnostic test<ept id="p1">](configure-run-diagnostics.md)</ept> in the administration tool/CLI on the web node.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>Repeat on each web node.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Authenticate the Web Node with the Compute Node</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>This section walks you through the steps for authenticating the web node with the compute node so that only the web node can communicate with the compute node.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>If a compute node is inside the web node's trust boundary, then this certificate is not needed.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>However, if the compute node resides outside of the trust boundary, consider using the compute node certificate to encrypt the traffic between the web node and compute node.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>On each web node:</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Install the trusted, signed <bpt id="p1">**</bpt>HTTPS authentication certificate<ept id="p1">**</ept> with both private and public keys in the certificate store.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Take note of the <ph id="ph1">`Subject`</ph> name of the certificate as you need this info later.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Open the configuration file, <bpt id="p1">[</bpt><ph id="ph1">\&lt;</ph>web-node-install-path&gt;<ept id="p1">](../operationalize/configure-find-admin-configuration-file.md)</ept>/appsettings.json.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>You can configure the HTTPS port for the web node in this file.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>In the file, search for the section starting with: "BackEndConfiguration": {</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Enable this section with <ph id="ph1">`"Enabled": true`</ph> and update the properties to match the values for the <bpt id="p1">**</bpt>Authentication certificate<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`"Thumbprint"`</ph> to ensure that the correct certificate is loaded if there are multiple certificates on the same system with same name used for different purposes such as IPsec, TLS Web Server Authentication, Client Authentication, Server Authentication, and so on.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>If you do not have multiple certificates with same name, you can leave the Thumbprint field empty.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Close and save the file.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>Launch the administration tool/CLI and <bpt id="p1">[</bpt>restart the web node<ept id="p1">](configure-admin-cli-stop-start.md)</ept>.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>Repeat on each web node.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>On each compute node:</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>These steps assume the trusted, signed HTTPS authentication certificate is already installed on the machine hosting the web node with a <bpt id="p1">_</bpt>private<ept id="p1">_</ept> key.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Open the configuration file, <bpt id="p1">[</bpt><ph id="ph1">\&lt;</ph>compute-node-install-path&gt;<ept id="p1">](../operationalize/configure-find-admin-configuration-file.md)</ept>/appsettings.json.</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>In the file, search for the section starting with: "BackEndConfiguration": {</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>Enable this section with <ph id="ph1">`"Enabled": true`</ph> and match the properties to the values for the <bpt id="p1">**</bpt>Authentication certificate<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>Close and save the file.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Launch the administration tool/CLI and <bpt id="p1">[</bpt>restart the compute node<ept id="p1">](configure-admin-cli-stop-start.md)</ept>.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>Repeat on each compute node.</source>
        </trans-unit></group></body></file></xliff>