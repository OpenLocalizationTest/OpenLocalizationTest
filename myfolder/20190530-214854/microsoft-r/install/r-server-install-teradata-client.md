<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-teradata-client.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3ef769a88e398ac89fe782ab136465640da875f804.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">f769a88e398ac89fe782ab136465640da875f804</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-teradata-client.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Server Client Installation Guide for Teradata</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Microsoft R Server install guide for Teradata clients.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>R Server Client Installation Guide for Teradata</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Microsoft R Server for Teradata is an R-based analytical engine embedded in your Teradata data warehouse.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Together with a Microsoft R Server client, it provides a comprehensive set of tools for interacting with the Teradata database and performing in-database analytics.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This manual provides detailed instructions for configuring local workstations to submit jobs to run within your Teradata data warehouse.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>For installing Microsoft R Server for Teradata in the Teradata data warehouse, see the companion manual <bpt id="p1">[</bpt><bpt id="p2">*</bpt>Microsoft R Server Server Installation Manual for Teradata<ept id="p2">*</ept><ept id="p1">](r-server-install-teradata-client.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The Teradata compute context was discontinued in Machine Learning Server 9.2.1.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>If you have R Server 9.1 and use the Teradata compute context, you are covered by Microsoft's <bpt id="p1">[</bpt>service support policy<ept id="p1">](../resources-servicing-support.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>For future compatibility, we recommend modifying existing code to run in other compute contexts, and create a Teradata data source object to work with your data.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>For more information about Teradata as a data source, see <bpt id="p1">[</bpt>RxTeradata<ept id="p1">](../r-reference/revoscaler/rxteradata.md)</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>System Requirements</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Microsoft R Server for Windows has the following system requirements:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Processor:<ept id="p1">**</ept> 64-bit processor with x86-compatible architecture (variously known as AMD64, Intel64, x86-64, IA-32e, EM64T, or x64 chips).</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Itanium-architecture chips (also known as IA-64) are not supported.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Multiple-core chips are recommended.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Operating System:<ept id="p1">**</ept> 64-bit Windows Vista, Windows 7, Windows 8, Windows Server 2008, Windows Server 2012, and HPC Server 2008 R2.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Distributed computing features require access to a cluster running HPC Server Pack 2012 or HPC Server 2008.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Only 64-bit operating systems are supported.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Teradata Version:<ept id="p1">**</ept> Teradata  Tools and Utilities 15.00 or 14.10.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Memory:<ept id="p1">**</ept> A minimum of 1 GB of RAM is required; 4 GB or more are recommended.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Disk Space:<ept id="p1">**</ept> A minimum of 500 MB of disk space is required.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Microsoft R Server on Linux systems has the following system requirements:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Processor:<ept id="p1">**</ept> 64-bit processor with x86-compatible architecture (variously known as AMD64, Intel64, x86-64, IA-32e, EM64T, or x64 chips).</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Itanium-architecture chips (also known as IA-64) are not supported.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Multiple-core chips are recommended.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Operating System:<ept id="p1">**</ept> SUSE Linux Enterprise Server 11, Red Hat Enterprise Linux 5, Red Hat Enterprise Linux 6, or fully compatible equivalents.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Only 64-bit operating systems are supported.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Teradata Version:<ept id="p1">**</ept> Teradata Tools and Utilities 15.00 or 14.10.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Memory:<ept id="p1">**</ept> A minimum of 1 GB of RAM is required; 4 GB or more are recommended.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Disk Space:<ept id="p1">**</ept> A minimum of 500 MB of disk space is required.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Installing the Client Software</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The Teradata client software for Windows is available from the <bpt id="p1">[</bpt>Teradata At Your Service<ept id="p1">](https://tays.teradata.com/)</ept> web site (this web site requires a customer login).</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Installing the Teradata Client on Windows</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If you are using the 14.10 client:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The Teradata 14.10 Client for Windows is contained in the file BCD0-1560-0000-Windows_14.10.00_V1-1.exe, Teradata Tools and Utilities Windows (the exact file name will change with update releases; the basic process should be similar for all updates of a given major release).</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Download this file and run it to start the installation process.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Accept defaults until you reach the “Select Features” dialog.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Choose the following items:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>ODBC Driver for Teradata</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Teradata Parallel Transporter Base</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Teradata Parallel Transporter Stream</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>BTEQ (optional)</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>FastExport (optional)</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>FastLoad (optional)</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Teradata SQL Assistant (optional)</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Teradata Administrator (optional)</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Complete the installation.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>You may want to define a DSN connection, but this is not required for use with RxTeradata (but can be useful for testing your client and troubleshooting installation problems).</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>If you are using the 15.00 client:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The Teradata 15.00 Client for Windows is contained on Teradata At Your Service in the file BCD0-1740-0000-Windows_15.00.00_V1-1.zip, Teradata Tools and Utilities Windows (the exact file name will change with update releases; the basic process should be similar for all updates of a given major release).</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>To start the installation process, download this file, extract the files from the zip, then run the TTU.exe in the TTU_Foundation_windows\Windows subdirectory.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Accept defaults until you reach the “Select Features” dialog.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Choose the following items:</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>ODBC Driver for Teradata</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Teradata Parallel Transporter Base</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Teradata Parallel Transporter Stream</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>BTEQ (optional)</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>FastExport (optional)</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>FastLoad (optional)</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Teradata SQL Assistant (optional)</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Teradata Administrator (optional)</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Complete the installation.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>You may want to define a DSN connection, but this is not required for use with RxTeradata (but can be useful for testing your client and troubleshooting installation problems).</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Creating a Teradata DSN:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>A DSN is a common way of encapsulating database connection information.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>On Windows, you create DSNs with the ODBC Data Source Administrator, found under Administrative Tools in the System and Security section of the Windows Control Panel.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>To create the DSN, do the following:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Launch the 64-bit ODBC Data Source Administrator.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>System DSN<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Add…<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Teradata<ept id="p1">**</ept> in the list view and then click <bpt id="p2">**</bpt>Finish<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>The ODBC Driver Setup for Teradata Database dialog appears.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Name<ept id="p1">**</ept> field, type <bpt id="p2">**</bpt>TDDSN<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Teradata Server Info<ept id="p1">**</ept> field, enter the fully qualified domain name or IP address of the Teradata server.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept> to complete the DSN.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept> to close the ODBC Data Source Administrator.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Testing the ODBC Connection:</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>To test that you can communicate with your Teradata server using your Teradata ODBC driver, use the Teradata client program tdxodbc.exe, as follows:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Open a Command Prompt as Administrator.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Change directory to the directory containing the tdxodbc.exe program (you may need to quote the path:</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Start the program by typing its name:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>At the prompt, enter the DSN name TDDSN.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>At the prompt, enter your database user name.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>At the prompt, enter your database user password.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>If your ODBC connection is successful, you will see something like the following, followed by a prompt to enter a SQL string:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Enter “quit” to exit.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Installing the Teradata Client on Linux</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>If you are using the 14.10 client:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The Teradata 14.10 Client for Linux, also known as the TTU 14.10 Teradata Tool and Utilities, is contained in the file BCD0-1560-0000-Linux-i386-x8664_14.10.00_V1-1_101747728.tar.gz, available from the <bpt id="p1">[</bpt>Teradata At Your Service<ept id="p1">](https://tays.teradata.com/)</ept> web site (this web site requires a customer login).</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Download this file to a temporary directory, such as /tmp/Teradata, and unpack it using the following commands:</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>The Teradata client setup script is designed to use ksh; if your system does not have ksh, you can install it using yum as follows (you must be root or a sudo user to run yum):</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>By default, yum installs ksh into /bin/ksh, but the Teradata setup script expects it in /usr/bin; if necessary, create a symbolic link as follows:</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Verify that the zip program is installed, as this is required by Microsoft R Server InTeradata operation:</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Change directory to the ttu directory created when you unpacked the tarball:</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>As root, or as a sudo user, run the setup script as follows:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>At the prompt “Enter one or more selections (separated by space):”, enter “9 12” to specify the ODBC drivers and the TPT Stream package.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>You should see the following warnings:</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>This indicates that the necessary dependencies will also be installed.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>If the setup script fails, you can try installing the packages using rpm directly.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>The rpm files are located in subdirectories of the Linux/ i386-x8664/ directory created under your /tmp/Teradata directory (again, these commands should be run as root or as a sudo user):</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Install the tdicu package:</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Source /etc/profile:</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Install the TeraGSS package:</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>On RHEL6 systems, TeraGSS may not install cleanly.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>If you see an error about a bad XML file, try copying /opt/Teradata/teragss/linux-i386/14.10.00.00/etc/TdgssUserConfigFile.xml to /opt/teradata/teragss/site, then run /usr/teragss/linux-x8664/14.10.00.00/bin/run_tdgssconfig.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>This should then complete with a message about something being written to a binary file.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Then proceed to the next step.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Install the tdodbc package:</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Install the cliv2 package:</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Install the tptbase package:</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Install the tptstream package:</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>On RHEL6 systems, tptstream may complain about missing glibc and nsl dependencies; these can be resolved by using the “yum provides” command to find a package or packages that can provide the missing dependencies, then using yum to install those packages.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>After installing the tptstream package, update your system LD_LIBRARY_PATH environment variable to include the path to the 64-bit version of libtelapi.so (typically /opt/teradata/client/14.10/tbuild/lib64) and the path to your unixODBC 2.3 libraries (typically /usr/lib64).</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>(This is most effectively done in the /etc/profile file; be sure to source the file after making any changes to it.)</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>If you are using the 15.00 client:</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>The Teradata 15.00 Client for Linux, also known as the TTU 15.00 Teradata Tool and Utilities, is contained in the file BCD0-1740-0000-Linux-i386_15.00.00_V1-1_2291720869.tar.gz.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>, available from the <bpt id="p1">[</bpt>Teradata At Your Service<ept id="p1">](https://tays.teradata.com/)</ept> web site (this web site requires a customer login).</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Download this file to a temporary directory, such as /tmp/Teradata, and unpack it using the following commands:</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>The Teradata client setup script is designed to use ksh; if your system does not have ksh, you can install it using yum as follows (you must be root or a sudo user to run yum):</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>By default, yum installs ksh into /bin/ksh, but the Teradata setup script expects it in /usr/bin; if necessary, create a symbolic link as follows:</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Verify that the zip program is installed, as this is required by Microsoft R Server InTeradata operation:</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Change directory to the ttu directory created when you unpacked the tarball:</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>As root, or as a sudo user, run the setup script as follows:</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>At the prompt “Enter one or more selections (separated by space):”, enter “9 12” to specify the ODBC drivers and the TPT Stream package.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>You should see the following warnings:</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>This indicates that the necessary dependencies will also be installed.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>After installing the tptstream package, update your system LD_LIBRARY_PATH environment variable to include the path to the 64-bit version of libtelapi.so (typically /opt/teradata/client/15.00/tbuild/lib64) and the path to your unixODBC 2.3 libraries (typically /usr/lib64).</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>(This is most effectively done in the /etc/profile file; be sure to source the file after making any changes to it.) Also, export the NLSPATH environment variable as follows:</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Updating Your ODBC Driver Manager</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Database operations with ODBC depend upon having both an ODBC driver and an ODBC driver manager.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Teradata ODBC drivers are provided in a client package that includes an ODBC driver manager; if you are using Microsoft R Server exclusively with a Teradata database, we recommend that you use this supplied ODBC driver manager.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>If you are using Microsoft R Server with other databases in addition to Teradata, we recommend installing unixODBC 2.3.1 for all your ODBC data management.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Configuring the Teradata ODBC Driver Manager</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>To use the ODBC driver manager supplied with the Teradata client package when you have another ODBC driver manager installed (typically unixODBC):</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Identify the directory where the existing ODBC driver manager libraries reside (almost certainly /usr/lib64) and cd to that directory:</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Rename or remove any existing soft link in that directory named libodbc.so.2:</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Add a soft link, libodbc.so.2, that points to the Teradata driver manager library libodbc.so (almost certainly in /opt/teradata/client/ODBC_64/lib)</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Export an environment variable definition for ODBCINI in the /etc/profile file (which runs for everyone at login), set to the pathname of the currently used odbc.ini file (probably /etc/odbc.ini):</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Logout and log back in so that the profile changes take effect.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Configuring the unixODBC 2.3.1 Driver Manager</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>The unixODBC 2.3.1 driver manager is not available as part of standard RHEL yum repositories.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>You must, therefore, install it from source.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>It is important that unixODBC 2.3.1 be the only unixODBC installation on your system, so be sure to perform the following steps:</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Ensure that you do not currently have unixODBC installed via yum:</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>This should return nothing; if any packages are listed, use yum to remove them:</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Download the unixODBC 2.3.1 sources from www.unixodbc.org.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Unpack the sources, then change directory to the top-level source directory and run the following commands to build and install the source:</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>After installing unixODBC, edit the file /etc/odbcinst.ini and add a section such as the following (making sure the path to the driver matches that on your machine):</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>If you are using RxOdbcData with a DSN, you need to define an appropriate DSN in the file /etc/odbc.ini, such as the following:</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Installing RODBC</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>The RODBC package is not required to use RxTeradata, but it can be useful for timing comparisons with other databases.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>You can download RODBC from the MRAN source package repository at <bpt id="p1">[</bpt><ph id="ph1">https://mran.microsoft.com</ph><ept id="p1">](https://mran.microsoft.com/)</ept>.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Installing Microsoft R Server or R Client on the Client</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>To download and install Microsoft R Server, you need an MSDN subscription or a Microsoft Volume License Center sign-in.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>For development purposes, you can install the free Developer edition of R Server on Linux or Windows:</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Install R Server for Linux</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Install R Server for Windows</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Optionally, you can use Microsoft R Client.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>It also runs on Linux and Windows:</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Install R Client on Linux</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>Install R Client on Windows</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Testing the Client Installation</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>After installing your Teradata client software, you should test that you can communicate with your Teradata database.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>For this, you typically need a connection string, which may look something like the following:</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>The connection string is typically quite long, but should remain contained on a single input line.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>The following commands can be used to verify that your Windows client can communicate with your Teradata data warehouse using the Revolution test database (instructions for creating that database are contained in the <bpt id="p1">[</bpt><bpt id="p2">*</bpt>Microsoft R Server Server Installation Manual for Teradata<ept id="p2">*</ept><ept id="p1">](r-server-install-teradata-server.md)</ept>:</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>ODBC</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>TPT</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>InTeradata</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>For Linux clients, the only change that should need to be made is to the shareDir argument to the RxInTeradata call that creates the myCluster object:</source>
        </trans-unit></group></body></file></xliff>