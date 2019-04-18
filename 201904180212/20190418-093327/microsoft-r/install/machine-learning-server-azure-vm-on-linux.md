<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="machine-learning-server-azure-vm-on-linux.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4217e6d034ac01dd33073cbd00d7cf695e37c3aa0.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">217e6d034ac01dd33073cbd00d7cf695e37c3aa0</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\machine-learning-server-azure-vm-on-linux.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to use Machine Learning Server on Linux VM in Azure (Virtual Machine) - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn how to work with Machine Learning Server / R Server on Linux by using a virtual machine in Azure.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Machine Learning Server, R Server, linux, virtual machine</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Machine Learning Server on Azure Virtual Machines</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Machine Learning Server, formerly known as R Server, is pre-installed on Azure virtual machines (VM) images running either a Windows or Linux operating system.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>An excellent alternative to selecting an existing VM image is to provision a VM yourself using a resource template.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The template includes extra configuration steps for both the VM and Machine Learning Server itself, resulting in a VM that is ready-to-use with no additional work on your part.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>VM images on Azure</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The following procedure explains how to use the Azure portal to view the full range of VM images that provide Machine Learning Server.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Sign in to the <bpt id="p1">[</bpt>Azure portal<ept id="p1">](https://portal.azure.com)</ept>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create a resource<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Search for <bpt id="p1">*</bpt>Machine Learning Server<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The following list shows partial search results.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>VM images include current and previous versions of Machine Learning Server on several common Linux operating systems as well as Windows Server 2016.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>VM images on Azure</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>VM images include the custom <bpt id="p1">[</bpt>R packages<ept id="p1">](../r-reference/introducing-r-server-r-package-reference.md)</ept> and <bpt id="p2">[</bpt>Python libraries<ept id="p2">](../python-reference/introducing-python-package-reference.md)</ept> from Machine Learning Server that offer machine learning algorithms, R and Python helpers for deploying analytics, and portable, scalable, and distributable data analysis functions.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>How to provision with templates</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The easiest approach is to use an ARM template that both installs and configures the VM and Machine Learning Server.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The template defines a resource group, the virtual network, a DNS name.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>ARM templates are available on GitHub, with options for a single-server install or distributed installation that places web nodes and compute nodes on different VMs within the same virtual network.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>There are also template options for data Science VMs, which include a broader selection of tools and technologies, of which Machine Learning Server is just one.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>When you use a template, the server is operationalized for remote connections, web service deployment, logging, and so forth.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Operationalize analytics with Machine Learning Server<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Go to the GitHub repo containing the templates: <bpt id="p1">[</bpt><ph id="ph1">https://github.com/Microsoft/microsoft-r/tree/master/mlserver-arm-templates</ph><ept id="p1">](https://github.com/Microsoft/microsoft-r/tree/master/mlserver-arm-templates)</ept></source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Choose your configuration.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>one-box configuration<ept id="p1">**</ept> to install all packages and features on a single VM, or click <bpt id="p2">**</bpt>enterprise-configuration<ept id="p2">**</ept> if you need a cluster.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Choose the operating system: Windows, Linux, Windows Data Science VM, or Linux Data Science VM.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>On the readme page for the option you selected, click <bpt id="p1">**</bpt>Deploy to Azure<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>You are prompted for input values necessary to complete the deployment, including passwords and the level of physical resources used by the VM.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Deploy button on the readme page</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>How to provision in the portal</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If you are new to using Azure VMs, we recommend that you review <bpt id="p1">[</bpt>this article<ept id="p1">](https://azure.microsoft.com/documentation/services/virtual-machines/linux/)</ept> for more information about using the portal and configuring a virtual machine.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Sign in to the <bpt id="p1">[</bpt>Azure portal<ept id="p1">](https://portal.azure.com)</ept>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create a resource<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Search for <bpt id="p1">*</bpt>Machine Learning Server<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>From the list of virtual machines, choose the VM image providing the operating system and version of Machine Learning Server you want to install.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Accept the terms and get started by clicking <bpt id="p1">**</bpt>Create<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Follow the onscreen prompts to provision the VM.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>After the VM is deployed and running, <bpt id="p1">[</bpt>connect<ept id="p1">](#connect)</ept> to the VM to begin interacting with Machine Learning Server.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>At this point, you can also:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install an R IDE<ept id="p1">](#ride)</ept> or a Python interpreter.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Configure Machine Learning Server to <bpt id="p1">[</bpt>operationalize your analytics<ept id="p1">](#o16n)</ept> so it acts as a deployment server and host analytic web services.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Connect to the Virtual Machine</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Once the VM is deployed, you can open the portal page for that VM and click <bpt id="p1">**</bpt>Connect<ept id="p1">**</ept> to obtain connection information in the form of the IP address and port.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>You can further configure the VM to use a domain name or static IP, but for an initial connection, the dynamic IP is sufficient.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Many people have success connecting using an open-source SSH client.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>A few examples include <bpt id="p1">[</bpt>PuTTY<ept id="p1">](https://www.putty.org/)</ept>, <bpt id="p2">[</bpt>SmarTTY<ept id="p2">](http://smartty.sysprogs.com/download/)</ept>, and <bpt id="p3">[</bpt>WinCP<ept id="p3">](https://winscp.net/eng/download.php)</ept>.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Launch R Server</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>On Linux, simple type <ph id="ph1">`R`</ph> at the command prompt to invoke the R interpreter, or <ph id="ph2">`Revo64`</ph> to run R Server in a console session.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>On Windows, open an R console session by entering <bpt id="p1">*</bpt>RGUI<ept id="p1">*</ept> in the Cortana search bar.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Configure an R IDE</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>With Machine Learning Server installed, you can configure your favorite R integrated development environment (IDE) to point to the Machine Learning Server R executable.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>This way, whenever you execute your R code, you do so using Machine Learning Server and benefit from its proprietary packages.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Machine Learning Server works well with popular IDEs such as <bpt id="p1">[</bpt>RStudio<ept id="p1">](https://www.rstudio.com)</ept> Desktop or Server.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Configure RStudio for Machine Learning Server</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Launch RStudio.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Update the path to R<ept id="p1">](https://support.rstudio.com/hc/en-us/articles/200486138-Using-Different-Versions-of-R)</ept>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>When you launch RStudio, Machine Learning Server is now the default R engine.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Open Ports needed to Use RStudio Server</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>RStudio Server uses port 8787.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The default configuration for the Azure VM does not open this port.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>To do that, you must go to the Azure portal and elect the proper Network Security Group.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Select the <bpt id="p1">**</bpt>All Settings<ept id="p1">**</ept> option and choose <bpt id="p2">**</bpt>Inbound security rules<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Add a new rule for RStudio.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Name the rule, choose <bpt id="p1">**</bpt>Any<ept id="p1">**</ept> for the Protocol, and add port 8787 to the destination port range.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept> to save your changes.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>You should now be able to access RStudio using a browser.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Assign a Fully Qualified Domain Name to the VM for Accessing RStudio Server</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>No cloud service is created to contain the public resources for the VM so there is no fully qualified domain name assigned to the dynamic public IP by default.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>One can be created and added to the image after deployment using the Azure PowerShell.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>The format of the hostname is <ph id="ph1">````domainnamelabel; region;.cloudapp.azure.com````</ph>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>For example, to add a public hostname using PowerShell for a VM named <ph id="ph1">`rservercloudvm`</ph> with resource group <ph id="ph2">`rservercloudrg`</ph> and desired hostname of <ph id="ph3">`rservercloud`</ph>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>After adding access to port TCP/8787 to the inbound security rules, RStudio Server can be accessed at <ph id="ph1">&lt;http://rservercloud.southcentralus.cloudapp.azure.com:8787/&gt;</ph></source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Some related articles are:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Azure Compute, Network, and Storage Providers for Windows applications under Azure Resource Manager deployment model<ept id="p1">](https://azure.microsoft.com/en-gb/documentation/articles/virtual-machines-azurerm-versus-azuresm/)</ept></source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Creating Azure VMs with Azure Resource Manager PowerShell cmdlets<ept id="p1">](http://blogs.msdn.com/b/cloud_solution_architect/archive/2015/05/05/creating-azure-vms-with-arm-powershell-cmdlets.aspx)</ept></source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Operationalize R and Python Analytics with Machine Learning Server on the VM</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>In order to operationalize your analytics with Machine Learning Server, you can <bpt id="p1">[</bpt>configure Machine Learning Server<ept id="p1">](operationalize-r-server-one-box-config.md)</ept> after installation to act as a deployment server and host analytic web services.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Access Data in an Azure Storage Account</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>When you need to use data from your Azure storage account, there are several options for accessing or moving the data:</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Copy the data from your storage account to the local file system using a utility, such as <bpt id="p1">[</bpt>AzCopy.<ept id="p1">](https://azure.microsoft.com/en-us/documentation/articles/storage-use-azcopy/)</ept></source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Add the files to a file share on your storage account and then mount the file share as a network drive on your VM.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Mounting Azure files.<ept id="p1">](https://azure.microsoft.com/en-us/documentation/articles/storage-how-to-use-files-linux/)</ept></source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Resources &amp; Documentation</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Additional documentation about Machine Learning can be found on this documentation site using the table of contents on your left.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>See these additional resources to learn about R in general:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>DataCamp<ept id="p1">](http://www.datacamp.com/)</ept>: A free introductory and intermediate course in R, and a course on working with big data using Revolution R</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Stack Overflow<ept id="p1">](http://www.stackoverflow.com/)</ept>: A good resource for R and Python programming and ML tools questions</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Cross Validated<ept id="p1">](https://stats.stackexchange.com/)</ept>: A site for questions about statistical issues in machine learning</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>R Help mailing list<ept id="p1">](https://www.r-project.org/mail.html)</ept>: The list and its archives offer a good resource of historical information</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>MRAN website<ept id="p1">](https://mran.microsoft.com/documents/getting-started/)</ept>: Many other R resources.</source>
        </trans-unit></group></body></file></xliff>