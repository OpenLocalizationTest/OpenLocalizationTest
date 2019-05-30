<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="install-on-linux.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3ee57e4a1c33a829b26ece544ef9c8c3bce5bb29f9.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">e57e4a1c33a829b26ece544ef9c8c3bce5bb29f9</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-client\install-on-linux.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install Microsoft R Client on Linux - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Guide to installing Microsoft R Client on Linux.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Client is a free, data science tool for high performance analytics.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Client, R IDE configuration, RTVS,  Microsoft R Client Linux</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Client on Linux</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Microsoft R Client is a free data science tool for high-performance analytics that you can install on popular Linux operating systems, including CentOS, Red Hat, and Ubuntu.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>R Client is built on top of <bpt id="p1">[</bpt>Microsoft R Open<ept id="p1">](https://mran.microsoft.com/open)</ept> so you can use any open-source R packages to build your analytics, and includes the <bpt id="p2">[</bpt>R function libraries from Microsoft<ept id="p2">](../r-reference/introducing-r-server-r-package-reference.md#r-function-libraries)</ept> that execute locally on R Client or remotely on a more powerful <bpt id="p3">[</bpt>Machine Learning Server<ept id="p3">](../what-is-machine-learning-server.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>R Client allows you to work with production data locally using the full set of RevoScaleR functions, with these constraints: data must fit in local memory, and processing is capped at two threads for RevoScaleR functions.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>For information about the current release, see <bpt id="p1">[</bpt>What's new in R Client<ept id="p1">](what-is-microsoft-r-client.md#r-client-whats-new)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>System Requirements</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Operating Systems</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Supported versions include:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>- Red Hat Enterprise Linux (RHEL) and CentOS 6.x and 7.x</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>- Ubuntu 14.04 and 16.04</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>- SUSE Linux Enterprise Server 11 (SLES11)</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Must be a supported version of Linux on a 64-bit with x86-compatible architecture (variously known as AMD64, Intel64, x86-64, IA-32e, EM64T, or x64 chips).</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Itanium-architecture chips (also known as IA-64) are not supported.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Multiple-core chips are recommended.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Available RAM</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>2 GB of RAM is required; 8 GB or more are recommended</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Free disk space</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>600 MB recommended, after installation of all prerequisites</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>1.2 GB recommended if pre-trained models are installed</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Internet access</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Needed to download R Client and any dependencies.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If you do not have an internet connection, for the instructions for an <bpt id="p1">[</bpt>offline installation<ept id="p1">](#offline)</ept></source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>MRO (R) and R Client version matrix</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Included and required for R Client setup is <bpt id="p1">[</bpt>Microsoft R Open (MRO)<ept id="p1">](https://mran.microsoft.com/open)</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Microsoft R Open is a built-in dependency of Microsoft R Client.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>In offline scenarios when no internet connection is available on the target machine, you must manually download the MRO installer <bpt id="p1">*</bpt>of the version required by R Client<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Use only the link specified in the installer or in this article.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Do NOT go to MRAN and download it from there or you may inadvertently get the wrong version for your Microsoft R product.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>You can use links and instructions in this article to install either 3.4.1 or 3.4.3 versions of R Client.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>R version</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>MRO version</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>R Client version</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>R Server version</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>3.4.3</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>3.4.3</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>3.4.3</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>9.3</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>3.4.1</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>3.4.1</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>3.4.1</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>9.2.1</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Setup Requirements</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Use a package manager from this list:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Package manager</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Platform</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>yum</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>RHEL, CentOS</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>apt</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Ubuntu online</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>dpkg</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Ubuntu offline</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>zypper</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>SUSE</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>rpm</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>RHEL, CentOS, SUSE</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Root or super user permissions are required.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>You must install Microsoft R Client to a local drive on your computer.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>You may need to disable your antivirus software.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>If you do, please turn it back on as soon as you are finished.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Installation paths</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>After installation completes, software can be found at the following paths:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Install root: /opt/microsoft/rclient/3.4.3 (or 3.4.1)</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Microsoft R Open root: /opt/microsoft/ropen/3.4.3 (or 3.4.1)</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Executables like Revo64 are under /usr/bin</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>There is no support for side-by-side installations of older and newer versions.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>How to install (with internet access)</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>This section walks you through an R Client deployment.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Under these instructions, your installation includes the ability to use the RevoScaleR, MicrosoftML, and mrsdeploy (mrsdeploy is server-side; calls to mrsdeploy must also include remote compute context functions that shift execution to a remote server).</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>The package manager downloads packages from the packages.microsoft.com repo, determines dependencies, retrieves additional packages, sets the installation order, and installs the software.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>For example syntax on setting the repo, see <bpt id="p1">[</bpt>Linux Software Repository for Microsoft Products<ept id="p1">](https://docs.microsoft.com/windows-server/administration/linux-package-repository-for-microsoft-software)</ept>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>If the repository configuration file is not present in the /etc directory, try <bpt id="p1">[</bpt>manual configuration<ept id="p1">](https://docs.microsoft.com/windows-server/administration/linux-package-repository-for-microsoft-software#manual-configuration)</ept> for repository registration.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>On Ubuntu 14.04 - 16.04</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>With root or sudo permissions, run the following commands:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Red Hat and CentOS 6/7</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>With root or sudo permissions, run the following commands:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>SUSE Linux Enterprise Server 11</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>With root or sudo permissions, run the following commands:</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>You can now <bpt id="p1">[</bpt>set up your IDE and try out some sample code<ept id="p1">](../r-client-get-started.md)</ept>.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>How to install offline (without internet access)</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>By default, installers connect to Microsoft download sites to get required and updated components.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>If firewall restrictions or limits on internet access prevent the installer from reaching these sites, you can download individual components on a computer that has internet access, copy the files to another computer behind the firewall, manually install prerequisites and packages, and then run setup.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>If you previously installed version 3.4.1, it will be replaced with the 3.4.3 version.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Packages for all supported versions of Linux can be found at <bpt id="p1">[</bpt>packages.microsoft.com<ept id="p1">](https://packages.microsoft.com)</ept>.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Redhat 6:  <ph id="ph1">https://packages.microsoft.com/rhel/6/prod/</ph></source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Redhat 7:  <ph id="ph1">https://packages.microsoft.com/rhel/7/prod/</ph></source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>SLES 11: <ph id="ph1">https://packages.microsoft.com/sles/11/prod/</ph></source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Ubuntu 14.04: <ph id="ph1">https://packages.microsoft.com/ubuntu/14.04/prod/</ph></source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Ubuntu 16.04: <ph id="ph1">https://packages.microsoft.com/ubuntu/16.04/prod/</ph></source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Package list</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>The package list is the same for both 3.4.1 and 3.4.3, with version numbers being the only difference.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>The following packages comprise a full R Client 3.4.3 installation:</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Microsoft R Open is required for R execution:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Additional open-source packages must be installed if a package is required but not found on the system.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>This list varies for each installation.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Here is one example of the additional packages that were added to a clean RHEL image during a connected (online) setup:</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Download packages</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>If your system provides a graphical user interface, you can click a file to download it.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Otherwise, use <ph id="ph1">`wget`</ph>.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>We recommend downloading all packages to a single directory so that you can install all of them in a single command.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>By default, <ph id="ph1">`wget`</ph> uses the working directory, but you can specify an alternative path using the <ph id="ph2">`-outfile`</ph> parameter.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>The following example is for the first package.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Each command references the version number of the platform.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Remember to change the number if your version is different.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Linux Software Repository for Microsoft Products<ept id="p1">](https://docs.microsoft.com/windows-server/administration/linux-package-repository-for-microsoft-software)</ept>.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>R Client 3.4.3 downloads</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Download to CentOS or RHEL 6:</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Download to CentOS or RHEL 7:</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Download to SUSE:</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Download to Ubuntu 14.04:</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Download to Ubuntu 16.04:</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Repeat for each package.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>R Client 3.4.1 downloads</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Download to CentOS or RHEL 6:</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Download to CentOS or RHEL 7:</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Download to SUSE:</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Download to Ubuntu 14.04:</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Download to Ubuntu 16.04:</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Repeat for each package.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Install packages</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>The package manager determines the installation order.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Assuming all packages are in the same folder:</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Install on CentOS or RHEL:</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Install on Ubuntu:</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Install on SUSE:</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>This step completes installation.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Connect and validate</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>List installed packages:</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>On CentOS and RHEL:</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>On Ubuntu:</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>On SLES11:</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Once you have a package name, you can obtain verbose version information.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>On CentOS and RHEL:</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>On Ubuntu:</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>On SLES:</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Output on Ubuntu is as follows:</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>You can now <bpt id="p1">[</bpt>set up your IDE and try out some sample code<ept id="p1">](../r-client-get-started.md)</ept>.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Also, consider package management as described in the next section.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Set a MKL_CBWR variable</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Set an MKL_CBWR environment variable to ensure consistent output from Intel Math Kernel Library (MKL) calculations.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>Edit or create a file named <bpt id="p1">**</bpt>.bash_profile<ept id="p1">**</ept> in your user home directory, adding the line <ph id="ph1">`export MKL_CBWR="AUTO"`</ph> to the file.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Execute this file by typing <bpt id="p1">**</bpt>source .bash_profile<ept id="p1">**</ept> at a bash command prompt.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Offline Package Management</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Review the recommendations in <bpt id="p1">[</bpt>Package Management<ept id="p1">](../operationalize/configure-manage-r-packages.md#offline)</ept> for instructions on how to set up a local package repository using MRAN or miniCRAN.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>As we mentioned earlier, you must install the <ph id="ph1">`gcc-c++`</ph> and <ph id="ph2">`gcc-gfortran`</ph> binary packages to be able to build and install packages, including miniCRAN.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>How to uninstall R Client</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>This section walks you through a 3.4.3 uninstall.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>To uninstall 3.4.1, use the same commands, modifying the version.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>On root@, uninstall Microsoft R Open (MRO) first.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>This action removes any dependent packages used only by MRO, which includes packages like microsoft-mlserver-packages-r.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>On RHEL:</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>On Ubuntu:</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>On SUSE:</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Re-list the packages from Microsoft to check for remaining files:</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>On RHEL:</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>On Ubuntu:</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>On SUSE:</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>On Ubuntu, you might have <ph id="ph1">`dotnet-runtime-2.0.0`</ph>.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>NET Core<ept id="p1">](https://docs.microsoft.com/dotnet/core/index)</ept> is a cross-platform, general purpose development platform maintained by Microsoft and the .NET community on GitHub.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>This package could be providing infrastructure to other applications on your computer.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>If R Client is the only Microsoft software you have, you can remove it now.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>After packages are uninstalled, remove remaining files.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>On root@, determine whether additional files still exist:</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Remove the entire directory:</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>RM removes the folder.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Parameter "f" is for force and "r" for recursive, deleting everything under microsoft/rclient.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>This command is destructive and irrevocable, so be sure you have the correct directory before you press Enter.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>Configure RStudio for RevoScaleR</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>If you are using the RStudio IDE, perform the following steps to load RevoScaleR and other R Client libraries.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>Close RStudio if it is already open.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Start a terminal session and sign on as root (<ph id="ph1">`sudo su`</ph>).</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>Open the <bpt id="p1">**</bpt>Renviron<ept id="p1">**</ept> file for editing:</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>Scroll down to <bpt id="p1">**</bpt>R_LIBS_USER<ept id="p1">**</ept> and add a new configuration setting just below it:</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>Save the file.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Start RStudio.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>In the Console window, you should see messages indicating both the Microsoft R Open and Microsoft R Client packages are loaded.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>To confirm RevoScaleR is operational, run the RevoScaleR <bpt id="p1">**</bpt>rxSummary<ept id="p1">**</ept> function to return statistical summary information on the built-in Iris dataset:</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>Learn More</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>You can learn more with these guides:</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>Overview of Microsoft R Client</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Quickstart: Running R code in Microsoft R<ept id="p1">](../r/quickstart-run-r-code.md)</ept> (example)</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>How-to guides in Machine Learning Server</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>RevoScaleR R package reference</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>MicrosoftML R package reference</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>mrsdeploy R package reference</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>Execute code on remote Machine Learning Server</source>
        </trans-unit></group></body></file></xliff>