<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-windows-vm-803-provisioning.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926c36a95f2068057ec8f0a45f6273e489aa9846e57.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">c36a95f2068057ec8f0a45f6273e489aa9846e57</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-windows-vm-803-provisioning.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Provision version 8.0.3 R Server (standalone) SQL Server 2016 Enterprise feature</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Provision the R Server 8.0.3 Only SQL Server 2016 Enterprise VM on Azure</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Provision version 8.0.3 R Server (standalone) SQL Server 2016 Enterprise feature</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies To: Azure Virtual Machines, provisioned as the 8.0.3 version of "R Server Only SQL Server 2016 Enterprise"</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>If you already have an existing 8.0.3 version of "R Server Only SQL Server 2016 Enterprise" Virtual Machine on Azure, these instructions apply to your VM.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>A newer version (9.0.1) is the current VM image on Azure.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>You can no longer obtain the previous version (8.0.3).</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>If installation and provisioning is still ahead of you, we recommend that you get the newest version.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>For instructions, see <bpt id="p1">[</bpt>Provision the R Server Only SQL Server 2016 Enterprise VM on Azure<ept id="p1">](https://msdn.microsoft.com/library/mt759780.aspx)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Provision the R Server 8.0.3 Virtual Machine</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Version 8.0.3 includes DeployR Enterprise, for deploying R analytics inside applications and backend systems.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>About Deploy R<ept id="p1">](https://msdn.microsoft.com/microsoft-r/deployr-about)</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>As a prerequisite, review this article for more information about using the portal and configuring a virtual machine.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Virtual Machines - Getting started<ept id="p1">](https://azure.microsoft.com/en-us/documentation/learning-paths/virtual-machines/)</ept></source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>To create the R Server VM from the Microsoft Azure Marketplace</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Virtual machines<ept id="p1">**</ept>, and in the search box, type <bpt id="p2">*</bpt>R Server<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>R Server Only SQL Server 2016 Enterprise<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Continue to provision the virtual machine as described in this article: <ph id="ph1">https://azure.microsoft.com/documentation/articles/virtual-machines-windows-hero-tutorial/</ph></source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>After the VM has been created and is running, click the <bpt id="p1">**</bpt>Connect<ept id="p1">**</ept> button to open a connection and log into the new machine.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>When you connect, <bpt id="p1">**</bpt>Server Manager<ept id="p1">**</ept> is opened by default, but no additional server configuration is required.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Close <bpt id="p1">**</bpt>Server Manager<ept id="p1">**</ept> to get to the desktop, and proceed with the next steps:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Installing additional R tools or development tools</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Configuring DeployR</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>To locate the R Server VM in the Azure Classic Portal</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Virtual Machines<ept id="p1">**</ept>, and then click <bpt id="p2">**</bpt>NEW<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>New<ept id="p1">**</ept> pane, <bpt id="p2">**</bpt>Compute<ept id="p2">**</ept> and <bpt id="p3">**</bpt>Virtual Machine<ept id="p3">**</ept> should already be selected.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>From Gallery<ept id="p1">**</ept> to locate the VM image.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>You can type <bpt id="p1">*</bpt>R Server<ept id="p1">*</ept> in the search box, or click <bpt id="p2">**</bpt>Microsoft<ept id="p2">**</ept> and then scroll down until you see <bpt id="p3">**</bpt>R Server Only SQL Server 2016 Enterprise<ept id="p3">**</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Install R Tools</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>By default, Microsoft R Server includes all the R tools installed with a base installation of R, including RTerm and RGui.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>A shortcut to RGui has been added to the desktop, if you want to get started using R right away.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>However, you might wish to install additional R tools, such as RStudio, R Tools for Visual Studio, or Microsoft R Client.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>See the following links for download locations and instructions:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>R Tools for Visual Studio<ept id="p1">](https://docs.microsoft.com/visualstudio/rtvs/installation)</ept></source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Microsoft R Client<ept id="p1">](https://msdn.microsoft.com/microsoft-r/r-client-install)</ept></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RStudio for Windows<ept id="p1">](https://www.rstudio.com/products/rstudio/download3/)</ept></source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>After you have installed these tools, be sure to point your tools to the R Server libraries.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Using DeployR on the Virtual Machine</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Some additional steps are required to use the DeployR instance that is installed on this VM.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>To configure the DeployR instance:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>On the VM, open the <bpt id="p1">**</bpt>DeployR Administrator Utility<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Set the DeployR administrator password as described here: <bpt id="p1">[</bpt>Post Installation Steps<ept id="p1">](https://msdn.microsoft.com/microsoft-r/deployr-install-on-windows#post-installation-steps)</ept> Set the DeployR Web context.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>DeployR Admin Installation in the Cloud<ept id="p1">](https://msdn.microsoft.com/microsoft-r/deployr-admin-install-in-cloud)</ept> Open the appropriate ports on the VM as described here: <bpt id="p2">[</bpt>Configuring Azure Endpoints<ept id="p2">](https://msdn.microsoft.com/microsoft-r/deployr-admin-install-in-cloud#configuring-azure-endpoints)</ept> Update the Windows Firewall as described here: <bpt id="p3">[</bpt>Updating the firewall<ept id="p3">](https://msdn.microsoft.com/microsoft-r/deployr-admin-install-in-cloud#updating-the-firewall)</ept></source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Accessing Data in an Azure Storage Account</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>When you need to use data from your Azure storage account, there are several options for accessing or moving the data:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Copy the data from your storage account to the local file system using a utility, such as <bpt id="p1">[</bpt>AzCopy<ept id="p1">](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy#copy-files-in-azure-file-storage-with-azcopy-preview-version-only)</ept>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Add the files to a file share on your storage account and then mount the file share as a network drive on your VM.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Mounting Azure files<ept id="p1">](https://docs.microsoft.com/en-us/azure/storage/storage-dotnet-how-to-use-files)</ept>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Resources</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Additional documentation about Microsoft R can be found in the MSDSN library: <bpt id="p1">[</bpt>R Server and Scale R<ept id="p1">](https://msdn.microsoft.com/en-us/microsoft-r/microsoft-r-getting-started)</ept></source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>See these additional resources to learn about R in general:</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>DataCamp<ept id="p1">](https://www.datacamp.com/)</ept> Provides a free introductory and intermediate course in R, and a course on working with big data using Revolution R.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Stack Overflow<ept id="p1">](http://stackoverflow.com/)</ept> A good resource for R programming and ML tools questions.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Cross Validated<ept id="p1">](https://stats.stackexchange.com/)</ept> Site for questions about statistical issues in machine learning.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>R Help mailing list archives<ept id="p1">](https://www.r-project.org/mail.html)</ept> Good resource of historical information.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>MRAN website<ept id="p1">](https://mran.microsoft.com/documents/getting-started/)</ept> Many other R resources.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SQL Server Machine Learning Services<ept id="p1">](https://msdn.microsoft.com/library/mt604845.aspx)</ept></source>
        </trans-unit></group></body></file></xliff>