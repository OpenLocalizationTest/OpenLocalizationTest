<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-cloudera-generate-parcel.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750d99f7cd1ca7b9f1f2741b3edc7110572b16bb535.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d99f7cd1ca7b9f1f2741b3edc7110572b16bb535</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-cloudera-generate-parcel.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Generate a parcel for R Server 9.1 on CDH</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Generate a parcel to install Microsoft R Server 9.1 on the Cloudera distribution of Apache Hadoop (CDH).</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Generate a parcel</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:<ept id="p1">**</ept> R Server 9.1 on the Cloudera distribution of Apache Hadoop (CDH)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>When performing a parcel installation in CDH, you use the <bpt id="p1">**</bpt>generate_mrs_parcel.sh<ept id="p1">**</ept> instead of <bpt id="p2">**</bpt>install.sh<ept id="p2">**</ept>. You will also use support files provided in the R Server 9.1 distribution, followed by Cloudera Manager to complete the deployment.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>The instructions in this article walk you through steps performed at the console, prior to using Cloudera Manager.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>In previous releases, parcel installation required downloading two pre-built parcel files.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The 9.1 release improves upon this experience by providing a parcel generator script.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The script produces the following output:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>a parcel</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>a checksum</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>a Custom Service Descriptor (CSD) that integrates Microsoft R Server as a managed service in Cloudera</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Before you start, be aware of the following limitations:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>MicrosoftML can only be included in the parcel if CDH is running on RHEL 7.x or later.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>mrsdeploy features (remote execution, web service deployment), plus web node and compute node configurations, are not supported at all.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>A workaround is to install the packages manually.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>For instructions, see <bpt id="p1">[</bpt>Manual package installation<ept id="p1">](r-server-install-hadoop-manual-package.md)</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Step 1: Download</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The first step is to download a gzipped tar file of the R Server 9.1 distribution to the master node from one of the following download sites.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Site</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Edition</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Visual Studio Dev Essentials</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Developer (free)</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>This option provides a zipped file, free when you sign up for Visual Studio Dev Essentials.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Developer edition has the same features as Enterprise, except it is licensed for development scenarios.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Volume Licensing Service Center (VLSC)</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Enterprise</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Sign in, search for R Server for Hadoop.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>A selection for <bpt id="p1">**</bpt>R Server 9.1.0 for Hadoop<ept id="p1">**</ept> is provided on this site.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>For downloads from <bpt id="p1">[</bpt>Visual Studio Dev Essentials<ept id="p1">](https://www.visualstudio.com/dev-essentials/)</ept>:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Join or access now<ept id="p1">**</ept> to sign up for download benefits.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Check the URL to verify it changed to <bpt id="p1">*</bpt><ph id="ph1">https://my.visualstudio.com/</ph><ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> to search for R Server.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Downloads<ept id="p1">**</ept> for a specific version to select the platform.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Download page on Visual Studio benefits page</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Step 2: Unpack</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>After downloading the software to a writable directory, such as <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept>, the second step is to unpack the distribution.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>On the master node, log in as root or a user with super user privileges (<ph id="ph1">`sudo su`</ph>).</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>In our examples, the master node is a machine named <ph id="ph1">`cdh4-mn0`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Switch to the <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept> directory (assuming it's the download location):</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Unpack the file:      <ph id="ph1">`[root@cdh4-mn0 tmp] $ tar zxvf en_microsoft_r_server_910_for_hadoop_x64_10323951.tar.gz`</ph></source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The distribution is unpacked into an <ph id="ph1">`MRS91Hadoop`</ph> folder at the download location.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The distribution includes the following files:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>File</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Script for installing R Server.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Do not use this for a parcel install.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Script for generating a parcel used for installing R Server on CDH.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>End user license agreements for each separately licensed component.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>DEB folder</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Contains Microsoft R packages for deployment on Ubuntu.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>RPM folder</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Contains Microsoft R packages for deployment on CentOS/RHEL and SUSE</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Parcel folder</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Contains files used to generate a parcel for installation on CDH.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Step 3: Dry run</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The parcel generator script is now available in the <bpt id="p1">**</bpt>tmp<ept id="p1">**</ept> directory.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>The script includes a <bpt id="p1">**</bpt>-n<ept id="p1">**</ept> flag that steps through actions without actually deploying anything.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>We recommend you start with the <bpt id="p1">**</bpt>-n<ept id="p1">**</ept> parameter to review the prompts.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The script downloads Microsoft R Open and builds a parcel by extracting information from RPM packages.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>You can append flags to run unattended setup or customize feature selections.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Switch to the MRS91Hadoop directory:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Run the script without actually invoking its operations:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>You will be prompted to read and accept license agreements.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>You are also asked to specify the underlying operating system.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>If the platform supports it, the parcel generator adds installation instructions for features having a dependency on .NET Core.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Namely, these features include Microsoft machine learning and application components used for remote execution, web service deployment, web node, and compute node configurations.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>RHEL 7.x is the platform with .NET Core support.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>When the script is finished, the location of the parcel, checksum, and CSD is printed to the console.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Remember the files do not yet exist.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>This is just a dry run.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Running the script without -n generates the files.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>console output messages</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Step 4: Review flags</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>You can run parcel generator with the following flags.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>flag</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Option</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>-m</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>--distro-name [DISTRO]</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Target Linux distribution for this parcel, one of: el6 el7 sles11</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>-l</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>--add-mml</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Add Microsoft ML to the Parcel regardless of the target system.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>-a</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>--accept-eula</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Accept all end user license agreements.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>-d</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>--download-mro</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Download Microsoft r open for distribution to an offline system.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>-s</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>--silent</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Perform a silent, unattended install.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>-u</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>--unattended</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Perform an unattended install.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>-n</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>--dry-run</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Don't do anything, just show what would be done.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>-h</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>--help</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Print this help text.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Step 4: Actual run</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Repeat the command without <bpt id="p1">**</bpt>-n<ept id="p1">**</ept> parameter.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>This time, the parcel, .sha, and CSD file are actually created.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Step 5: Copy parcel</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>By default, Cloudera Manager finds parcels in the Cloudera parcel repository.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>In this step, copy the parcel you generated to the repository.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Copy <ph id="ph1">`MRS-9.1.0-el7.parcel`</ph> and <ph id="ph2">`MRS-9.1.0-el7.parcel.sha`</ph> to the Cloudera parcel repository, typically /opt/cloudera/parcels.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Step 6: Copy CSD</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>The Custom Service Descriptor (CSD) enables MRS monitoring and administration from within Cloudera Manager.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>In this step, copy the CSD (a .jar file) to the Cloudera repository for CSD files.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Copy the CSD file <ph id="ph1">`MRS-9.1.0-el7-CONFIG.jar`</ph> to the Cloudera CSD directory, typically /opt/cloudera/csd.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Modify the permissions of CSD file as follows:</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Restart the cloudera-scm-server service:</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>After you generate a parcel and CSD and copy the files to the appropriate repositories, the next steps are performed in Cloudera Manager.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Start at the Home page to <bpt id="p1">[</bpt>deploy the parcel and activate Microsoft R Server in CDH<ept id="p1">](r-server-install-cloudera-deploy-activate.md)</ept>.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Install R Server 9.1.0 on the Cloudera distribution of Apache Hadoop (CDH)</source>
        </trans-unit></group></body></file></xliff>