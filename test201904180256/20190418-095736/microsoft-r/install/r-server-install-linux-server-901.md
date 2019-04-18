<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-linux-server-901.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c397788fe65eeb0f5b3acec5ae26795a832ed2c85.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">397788fe65eeb0f5b3acec5ae26795a832ed2c85</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-linux-server-901.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Server 9.0.1 installation for Linux systems</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install Microsoft R Server 9.0.1 on Linux.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>R Server 9.0.1 Installation for Linux Systems</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Older versions of R Server for Linux are no longer available on the Microsoft download sites, but if you already have an older distribution, you can follow these instructions to deploy version 8.0.5.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>For the current release, see <bpt id="p1">[</bpt>Install R Server for Linux<ept id="p1">](r-server-install-linux-server.md)</ept>.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Side-by-side Installation<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>You can install major versions of R Server (such as an 8.x and 9.x) side-by-side on Linux, but not minor versions.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>For example, if you already installed Microsoft R Server 8.0, you must uninstall it before you can install 8.0.5.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Upgrade Versions<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If you want to replace an older version rather than run side-by-side, you can uninstall the older distribution before installing the new version (there is no in-place upgrade).</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>Uninstall Microsoft R Server to upgrade to a newer version<ept id="p1">](r-server-install-uninstall-upgrade.md)</ept> for instructions.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Requirements<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Installer requirements include the following:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>An internet connection</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>A package manager (yum for RHEL systems, zypper for SLES systems)</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Root or as super user permissions</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If these requirements cannot be met, you can install R Server manually.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>First, verify that your system meets system requirements and satisfies the <bpt id="p1">[</bpt>package prerequisites<ept id="p1">](r-server-install-linux-hadoop-packages.md)</ept>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>You can then follow the more detailed installation instructions described in <bpt id="p1">[</bpt>Managing Your Microsoft R Server Installation<ept id="p1">](#manage-installation)</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>System Requirements</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Processor:<ept id="p1">**</ept> 64-bit processor with x86-compatible architecture (variously known as AMD64, Intel64, x86-64, IA-32e, EM64T, or x64 chips).</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Itanium-architecture chips (also known as IA-64) are not supported.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Multiple-core chips are recommended.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Operating System:<ept id="p1">**</ept> Microsoft R for Linux can be installed on Red Hat Enterprise Linux (RHEL) or a fully compatible operating system like CentOS, or SUSE Linux Enterprise Server.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Microsoft R Server has different operating system requirements depending on the version you install.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>Supported platforms<ept id="p1">](r-server-install-supported-platforms.md)</ept> for specifics.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Only 64-bit operating systems are supported.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Memory:<ept id="p1">**</ept> A minimum of 2 GB of RAM is required; 8 GB or more are recommended.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Disk Space:<ept id="p1">**</ept> A minimum of 500 MB of disk space is required.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Unpack the distribution</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Download the software to a writable directory, such as <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept>, unpack the distribution and then run the installation script.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The distribution includes one installer for Microsoft R Server.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>For a gzipped TAR file, you should unpack the file as follows (be sure you have downloaded the file to a writable directory, such as <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept>):</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Log in as root or a user with sudo privileges.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Switch to the <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept> directory (assuming it's the download location)</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Unpack the file:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Run the MRS install script</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>R Server for Linux is deployed by running the install script with no parameters.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Change to the <ph id="ph1">`MRS90LINUX`</ph> directory containing the installation script:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Run the script.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>When prompted to accept the license terms for Microsoft R Server, click Enter to read the EULA, click <bpt id="p1">**</bpt>q<ept id="p1">**</ept> when you are finished reading, and then click <bpt id="p2">**</bpt>y<ept id="p2">**</ept> to accept the terms.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Installer output shows the packages and location of the log file.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Verify installation</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>List installed packages and get package names:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Check the version of Microsoft R Open using <ph id="ph1">`rpm -qi`</ph>:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Check the version of Microsoft R Server:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Partial output is as follows (note version 9.0.1):</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Name        : microsoft-r-server-packages-9.0     Relocations: /usr/lib64 Version     : 9.0.1                               Vendor: Microsoft .</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Start Revo64</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>As a verification step, run the Revo64 program.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Switch to the directory containing the executable:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Start the program:</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Run an R function, such as <bpt id="p1">**</bpt>rxSummary<ept id="p1">**</ept> on a dataset.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Many sample datasets, such as the iris dataset, are ready to use because they are installed with the software:</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Output from the iris dataset should look similar to the following:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>To quit the program, type <ph id="ph1">`q()`</ph> at the command line with no arguments.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Configure R Server to operationalize your analytics</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The server can be used as-is if you install and use an R IDE on the same box, but to benefit from the deployment and consumption of web services with Microsoft R Server, then you must configure R Server after installation to act as a deployment server and host analytic web services.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Possible configurations are a <bpt id="p1">[</bpt>one-box setup<ept id="p1">](operationalize-r-server-one-box-config.md)</ept> or an <bpt id="p2">[</bpt>enterprise setup<ept id="p2">](operationalize-r-server-enterprise-config.md)</ept>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Doing so also enables remote execution, allowing you to connect to R Server from an R Client workstation and execute code on the server.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Manage your installation</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>In this section, we discuss file management for your Microsoft R Server installation, including file ownership, file permissions, and so on.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>File ownership</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>If you followed the instructions provided, the installed files are all owned by root.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>For single-user workstations where the user has either sudo privileges or access to the root password, this is normally fine.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>In enterprise environments, however, it's common to have third-party applications such as Microsoft R Server installed into an account owned by a non-root user; this can make maintenance easier and reduce security concerns.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>In such an environment, you may wish to create an "RUser" account, and change ownership of the files to that user.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>You can do that as follows:</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Server as root, as usual.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Create the "RUser" account if it does not already exist.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Assign this user to a suitable group, if desired.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">**</bpt>chown<ept id="p1">**</ept> command to change ownership of the files (in the example below, we assume RUser has been made a member of the dev group; this command requires root privileges):</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Here we show the default path /usr/lib64/MRS90LINUX; if you have specified an alternate installation path, use that in this command as well.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Unattended installs</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>You can bypass the interactive install steps of the Microsoft R Server install script with the -y flag ("yes" or "accept default" to all prompts except that you also agree to the license agreement).</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Additional flags can be used to specify which of the usual install options you want, as follows:</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>flag</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Option</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>-a</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>--accept-eula</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Accept all end user license agreements.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>-d</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>--download-mro</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Download microsoft r open for distribution to an offline system.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>-p</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>--hadoop-components</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Install Hadoop components.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>-s</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>--silent</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Perform a silent, unattended install.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>-u</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>--unattended</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Perform an unattended install.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>-h</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>--help</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Print this help text.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>For a standard unattended install, run the following script:</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>File permissions</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Normally, ordinary Microsoft R Server files are installed with read/write permission for owner and read-only permission for group and world.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Directories are installed with execute permission as well, to permit them to be traversed.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>You can modify these permissions using the <bpt id="p1">**</bpt>chmod<ept id="p1">**</ept> command.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>(For files owned by root, this command requires root privileges.)</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Installing to a read-only file system</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>In enterprise environments, it is common for enterprise utilities to be mounted as read-only file systems, so that ordinary operations cannot corrupt the tools.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Obviously, new applications can be added to such systems only by first unmounting them, then re-mounting them for read/write, installing the software, and then re-mounting as read-only.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>This must be done by a system administrator.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Setting up a package repository</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>One of the strengths of the R language is the thousands of third-party packages that have been made publicly available via CRAN, the Comprehensive R Archive Network.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>R includes a number of functions that make it easy to download and install these packages.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>However, in many enterprise environments, access to the Internet is limited or non-existent.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>In such environments, it is useful to create a local package repository that users can access from within the corporate firewall.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Your local repository may contain source packages, binary packages, or both.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>If some or all of your users will be working on Windows systems, you should include Windows binaries in your repository.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Windows binaries are R-version-specific; if you are running R 3.2.2, you need Windows binaries built under R 3.2.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>These versioned binaries are available from CRAN and other public repositories.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>If some or all of your users will be working on Linux systems, you must include source packages in your repository.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>The Microsoft Managed R Archive Network (MRAN) provides daily snapshots of all of CRAN, and together with the Microsoft-developed open-source package miniCRAN can be used to easily build a local package repository containing source packages, binary packages, or both.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>There are two ways to create the package repository: either copy all the packages from a given MRAN snapshot, or create a new repository and populate it with just those packages you want to be available to your users.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>We will describe both procedures using MRAN and miniCRAN.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Note:<ept id="p1">**</ept> The miniCRAN package itself is dependent on 18 other CRAN packages, among which is the RCurl package, which has a system dependency on the curl-devel package.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Similarly, package XML has a dependency on libxml2-devel.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>We recommend, therefore, that you build your local repository initially on a machine with full Internet access, so that you can easily satisfy all these dependencies.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>After created, you can either move the repository to a different location within your firewall, or simply disable the machine’s Internet access.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Installing miniCRAN</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>On a system with Internet access, the easiest way to install the miniCRAN package (or any R package) is to start R and use the install.packages function:</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>If your system already contains all the system prerequisites, this will normally download and install all of miniCRAN’s R package dependencies as well as miniCRAN itself.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>If a system dependency is missing, compilation of the first package that needs that dependency will fail, typically with a specific but not particularly helpful message.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>In our testing, we have found that an error about curl-config not being found indicates that the curl-devel package is missing, and an error about libxml2 indicates the libxml2-devel package is missing.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>If you get such an error, exit R, use yum or zypper to install the missing package, then restart R and retry the install.packages command.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Create a repository from an MRAN snapshot</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Creating a repository from an MRAN snapshot is very straightforward:</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Choose a location for your repository somewhere on your local network.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>If you have a corporate intranet, this is usually a good choice, provided URLs have the prefix http:// and not https://.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Any file system that is mounted for all users can be used; file-based URLs of the form file:// are supported by the R functions.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>In this example, we suppose the file system /local is mounted on all systems and we will create our repository in the directory /local/repos.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Start R and load the miniCRAN package:</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Specify an MRAN snapshot:</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Set your MRAN snapshot as your CRAN repo:</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Use miniCRAN’s pkgAvail function to obtain a list of (source) packages in your MRAN snapshot:</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Use miniCRAN’s makeRepo function to create a repository of these packages in your /local/repos directory:</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Create a custom repository</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>As mentioned above, a custom repository gives you complete control over which packages are available to your users.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Here, too, you have two basic choices in terms of populating your repository: you can either use makeRepo to select specific packages from an existing MRAN snapshot, or you can combine your own locally developed packages with packages from other sources.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>The latter option gives you the greatest control, but typically means you need to manage the contents using home-grown tools.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Create a custom package directory</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Your custom package directory can contain source packages, binary packages, or both.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Windows binary packages should have a path of the form</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>while source packages should have a path of the form:</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>Windows binary packages should be built with your current R version.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>Windows binary files will be zip files, package source files will be tar.gz files.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Move the desired packages to the appropriate directories, then run the R function write<ph id="ph1">\_</ph>PACKAGES in the tools package to create the PACKAGES and PACKAGES.gz index files:</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Configure R to use a local repository</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>To make your local repository available to your R users:</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Open the file Rprofile.site in the /etc directory of your installed R (if you installed to the default /usr prefix, the path is /usr/lib64/MRO-for-MRS-8.0.0/R-3.2.2/lib64/R/etc/Rprofile.site).</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Find the following line in the Rprofile.site file:</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Add your repository as follows:</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>If you added more than one repository and used R version numbers, add multiple lines of the form LOCAL<ph id="ph1">\_</ph>VER="file:///local/repos/VER", for example:</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>Save the file and your repository is ready for use.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>If you are in a locked-down environment without access to the standard Microsoft repository, <bpt id="p1">*</bpt>replace<ept id="p1">*</ept> the Revo repository with your local repository (or repositories).</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>Remove Microsoft R Server</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>For instructions on rolling back your installation, see <bpt id="p1">[</bpt>Uninstall Microsoft R Server to upgrade to a newer version<ept id="p1">](r-server-install-uninstall-upgrade.md)</ept>.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>Manage multiple R installations</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>You can install the latest Microsoft R Server side-by-side with an existing Microsoft R Server.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>In this section, we discuss maintaining multiple versions of Microsoft R Server, together with instructions for maintaining Microsoft R Server alongside versions of R obtained from CRAN or third-party repositories such as <ph id="ph1">&lt;http://dl.fedoraproject.org/pub/epel&gt;</ph>.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>(Note, however, that patch releases such as Microsoft R Server 7.4.1 are intended to replace their associated main release, not live side by side with it.</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>You must uninstall and reinstall such releases.)</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Using Microsoft R Server with other R installations</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>If you have an installed R script in your /usr/bin directory and then install Microsoft R Server, the automated installer detects that R exists and does not prompt you to link R to Revo64.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>In this case, you can use both versions of R simply by calling them by their respective script names, “R” and “Revo64”.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>To have Microsoft R Server become your default R, do the following:</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>Rename the R script by appending the R version, for example 3.2.2:</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Create a symbolic link from the Revo64 script to R:</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>If you have installed Microsoft R Server and then install base R, again there should be no conflict; R and Revo64 point to their respective installations, as usual.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>You can use the above procedure to make Microsoft R Server your default version of R.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install R Server 8.0.5 for Linux<ept id="p1">](r-server-install-linux-server-805.md)</ept></source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install R on Hadoop overview<ept id="p1">](r-server-install-hadoop.md)</ept></source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install R Server 8.0.5 for Hadoop<ept id="p1">](r-server-install-hadoop-805.md)</ept></source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Uninstall Microsoft R Server to upgrade to a newer version<ept id="p1">](r-server-install-uninstall-upgrade.md)</ept></source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Troubleshoot R Server installation problems on Hadoop<ept id="p1">](r-server-install-hadoop-troubleshoot.md)</ept></source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure R Server to operationalize analytics<ept id="p1">](operationalize-r-server-one-box-config.md)</ept></source>
        </trans-unit></group></body></file></xliff>