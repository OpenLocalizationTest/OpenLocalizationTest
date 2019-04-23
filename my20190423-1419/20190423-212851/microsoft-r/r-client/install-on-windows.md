<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="install-on-windows.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a117788344c1330c274d9024d5d3c5590826645e5.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">117788344c1330c274d9024d5d3c5590826645e5</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-client\install-on-windows.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install Microsoft R Client on Windows</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Guide to installing Microsoft R Client on Windows.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Client is a free, data science tool for high performance analytics.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Client, R IDE configuration, RTVS, R Tools for Visual Studio, Microsoft R Client</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Client on Windows</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Microsoft R Client is a free, data science tool for high-performance analytics that you can install on Windows client operating systems.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>R Client is built on top of <bpt id="p1">[</bpt>Microsoft R Open<ept id="p1">](https://mran.microsoft.com/open)</ept> so you can use any open-source R packages to build your analytics, and includes the <bpt id="p2">[</bpt>R function libraries from Microsoft<ept id="p2">](../r-reference/introducing-r-server-r-package-reference.md#r-function-libraries)</ept> that execute locally on R Client or remotely on a more powerful <bpt id="p3">[</bpt>Machine Learning Server<ept id="p3">](../what-is-machine-learning-server.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>R Client allows you to work with production data locally using the full set of RevoScaleR functions, with these constraints: data must fit in local memory, and processing is capped at two threads for RevoScaleR functions.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>For information about the current release, see <bpt id="p1">[</bpt>What's new in R Client<ept id="p1">](what-is-microsoft-r-client.md#r-client-whats-new)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>System Requirements</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Operating<ph id="ph1">&amp;nbsp;</ph>Systems</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>64-bit versions of Microsoft Windows 7, 8.1, and 10</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Free disk space</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>600 MB recommended, after installation of all prerequisites</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If pre-trained models are installed, 1.2 GB is recommended</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Available RAM</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>4+ GB recommended</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Internet access</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Needed to download R Client and any dependencies</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>.NET Framework 4.5.2</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Framework component must be installed to run setup.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Use the link provided in the setup wizard.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Installing this component requires a computer restart.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The following additional components are included in Setup and required:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Microsoft R Open 3.4.3</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Microsoft MPI 8.1</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>AS OLE DB (SQL Server 2016) provider</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Microsoft Visual C++ 2015 Redistributable</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Optionally, you can install the <bpt id="p1">[</bpt>pre-trained models<ept id="p1">](../install/microsoftml-install-pretrained-models.md)</ept> for sentiment analysis and image detection.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Setup Requirements</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>On the machine onto which you are installing, follow this guidance before you begin installing:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Always install Microsoft R Client to a local drive on your computer.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>You may need to disable your antivirus software.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If you do, be sure to turn it back on immediately after installing.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Close any other programs running on the system.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>How to install (with internet access)</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Log in to the machine with administrator privileges.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Download Microsoft R Client from the following link: <ph id="ph1">https://aka.ms/rclient/</ph></source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Launch the Microsoft R Client setup and follow the prompts.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Accept the default installation path for Microsoft R Client or choose another location.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Review the components that are installed as part of Microsoft R Client.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>While most are required, you can choose to add additional components such as <bpt id="p1">[</bpt><bpt id="p2">**</bpt>pre-trained models<ept id="p2">**</ept><ept id="p1">](../install/microsoftml-install-pretrained-models.md)</ept>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Accept the Microsoft R Client license terms.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Accept the Microsoft R Open license term.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Microsoft R Client is built on Microsoft R Open, Microsoft's enhanced distribution of R. Setup installs the correct version of R Open for you automatically.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Finish<ept id="p1">**</ept> when installation is finished.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>A welcome screen opens to introduce you to the product and documentation.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>How to offline install (without internet access)</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Microsoft R Open is a requirement of Microsoft R Client.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>In offline scenarios when no internet connection is available on the target machine, you must manually download the R Open installer.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Use only the link specified in the installer or installation guide.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Do NOT go to MRAN and download it from there or you may inadvertently get the wrong version for your Microsoft R product.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>On a machine with <bpt id="p1">_</bpt><bpt id="p2">**</bpt>unrestricted<ept id="p2">**</ept><ept id="p1">_</ept> internet access:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Download Microsoft R Client from <ph id="ph1">https://aka.ms/rclient/</ph>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Download the Microsoft R Open (*.cab) needed to install R Client from <ph id="ph1">https://go.microsoft.com/fwlink/?LinkId=867186</ph>.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Download .NET Framework 4.5.2 from <ph id="ph1">https://www.microsoft.com/download/details.aspx?id=42642</ph>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Download, if desired, the .cab file for pre-trained machine learning models from: <ph id="ph1">https://go.microsoft.com/fwlink/?LinkId=852727</ph>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Learn more about these <bpt id="p1">[</bpt>pre-trained models<ept id="p1">](../install/microsoftml-install-pretrained-models.md)</ept>.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Copy the downloaded files to a network share or portable drive.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>On the machine with <bpt id="p1">_</bpt><bpt id="p2">**</bpt>restricted<ept id="p2">**</ept><ept id="p1">_</ept> internet access:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Log in with administrator privileges.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Copy the .cab file and R Client installer from the network share/portable drive on the first machine to the machine that has restricted internet access.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Put the CAB files in the setup user's temp folder under <ph id="ph1">`%temp%`</ph>.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Copy and install the .NET Framework.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Restart your computer if you installed the .NET Framework.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Run <ph id="ph1">`RClientSetup.exe`</ph>, which finds the cab file in the temp folder for you.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Accept the default installation path for Microsoft R Client or choose another location.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Review the components that are installed as part of Microsoft R Client.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>While most are required, you can choose to add additional components such as <bpt id="p1">[</bpt><bpt id="p2">**</bpt>pre-trained models<ept id="p2">**</ept><ept id="p1">](../install/microsoftml-install-pretrained-models.md)</ept>.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Accept the Microsoft R Client license terms.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Accept the Microsoft R Open license term.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Microsoft R Client is built on Microsoft R Open, Microsoft's enhanced distribution of R. Setup installs the correct version of R Open for you automatically.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Without internet access, we recommend disabling the <bpt id="p1">_</bpt>auto-update check<ept id="p1">_</ept> feature so that R Client can launch more quickly.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Do so in the <ph id="ph1">`Rprofile.site`</ph> file by adding a comment character (#) at the start of the line: mrupdate::mrCheckForUpdates()</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Review the recommendations in <bpt id="p1">[</bpt>Package Management<ept id="p1">](../operationalize/configure-manage-r-packages.md#offline)</ept> for instructions on how to set up a local package repository using MRAN or miniCRAN.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Silent and Passive Installs</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>To install Microsoft R Client from a script on Windows, use the following command-line switches:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Mode</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Install Command</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Passive</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>No prompts, but a progress indicator</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Silent</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>No prompts nor progress indicator</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Set environment variables</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Create an <bpt id="p1">**</bpt>MKL_CBWR<ept id="p1">**</ept> environment variable to <bpt id="p2">[</bpt>ensure consistent output<ept id="p2">](https://software.intel.com/articles/introduction-to-the-conditional-numerical-reproducibility-cnr)</ept> from Intel Math Kernel Library (MKL) calculations.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>In Control Panel, click <bpt id="p1">**</bpt>System and Security<ept id="p1">**</ept><ph id="ph1"> &gt; </ph><bpt id="p2">**</bpt>System<ept id="p2">**</ept><ph id="ph2"> &gt; </ph><bpt id="p3">**</bpt>Advanced System Settings<ept id="p3">**</ept><ph id="ph3"> &gt; </ph><bpt id="p4">**</bpt>Environment Variables<ept id="p4">**</ept>.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Create a new User or System variable.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Set variable name to</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Set the variable value to</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>This step requires a computer restart.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>What's Installed with R Client</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Microsoft R Client installs the R base packages and a set of enhanced and proprietary R packages that support parallel processing, improved performance, and connectivity to data sources including SQL Server and Hadoop.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>The R libraries are installed under the R Client installation directory, <ph id="ph1">`C:\Program Files\Microsoft\R Client\R_SERVER`</ph>.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Additionally, this directory contains the documentation for the R base packages, sample data, and the R library.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>All tools for the standard base R (RTerm, Rgui.exe, and RScript) are also included with Microsoft R Client under <ph id="ph1">`&lt;install-directory&gt;\bin`</ph>.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Documentation for these tools can be found in the setup folder: <ph id="ph1">`&lt;install-directory&gt;\doc`</ph> and in <ph id="ph2">`&lt;install-directory&gt;\doc\manual`</ph>.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>One easy way to open these files is to open <ph id="ph1">`RGui`</ph>, click <bpt id="p1">**</bpt>Help<ept id="p1">**</ept>, and select one of the options.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>By default, telemetry data is collected during your usage of R Client.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>To turn off this feature, use the RevoScaleR package function <ph id="ph1">`rxPrivacyControl(FALSE)`</ph>.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>To turn it back on, change the setting to <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>How to uninstall</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Remove Microsoft R Client like other applications using the Add/Remove dialog on Windows.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Alternately, you can use the same setup file used to install R Client to remove the program by specifying the /uninstall option on the command line such as: <ph id="ph1">```RClientSetup.exe /uninstall```</ph></source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Learn More</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>You can learn more with these guides:</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Overview of Microsoft R Client</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Quickstart: Running R code in Microsoft R<ept id="p1">](../r/quickstart-run-r-code.md)</ept> (example)</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>How-to guides in Machine Learning Server</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>RevoScaleR R package reference</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>MicrosoftML R package reference</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>mrsdeploy R package reference</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Execute code on remote Machine Learning Server</source>
        </trans-unit></group></body></file></xliff>