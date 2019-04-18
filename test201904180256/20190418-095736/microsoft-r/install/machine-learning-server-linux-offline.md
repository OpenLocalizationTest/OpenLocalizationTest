<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="machine-learning-server-linux-offline.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c6a4ba86b261fed2276b4b29779da382226ac2172.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">6a4ba86b261fed2276b4b29779da382226ac2172</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\machine-learning-server-linux-offline.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Linux offline installation for Machine Learning Server 9.3</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to install Machine Learning Server for Linux with no internet connection.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Offline installation Machine Learning Server for Linux</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Machine Learning Server 9.2.1 | 9.3<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>By default, installers connect to Microsoft download sites to get required and updated components for Machine Learning Server 9.x for Linux.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>If firewall constraints prevent the installer from reaching these sites, you can use an internet-connected device to download files, transfer files to an offline server, and then run setup.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Before you start, review the following article for general information about setup: <bpt id="p1">[</bpt>Install Machine Learning Server on Linux<ept id="p1">](machine-learning-server-linux-install.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Package managers</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>In contrast with previous releases, there is no install.sh script.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Package managers are used for installation.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Package manager</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Platform</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>yum<ept id="p1">](https://access.redhat.com/documentation/Red_Hat_Enterprise_Linux/6/html/Deployment_Guide/ch-yum.html)</ept></source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>RHEL, CentOS</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>apt<ept id="p1">](https://help.ubuntu.com/lts/serverguide/apt.html)</ept></source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Ubuntu online</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>dpkg<ept id="p1">](https://help.ubuntu.com/lts/serverguide/dpkg.html)</ept></source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Ubuntu offline</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>zypper<ept id="p1">](https://www.suse.com/documentation/opensuse111/opensuse111_reference/data/sec_zypper.html)</ept></source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>SUSE</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rpm<ept id="p1">](https://en.wikipedia.org/wiki/Rpm_(software))</ept></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>RHEL, CentOS, SUSE</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Package location</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Packages for all supported versions of Linux can be found at <bpt id="p1">[</bpt>packages.microsoft.com<ept id="p1">](https://packages.microsoft.com)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><ph id="ph1">https://packages.microsoft.com/rhel/6/prod/</ph> (CentOS 6)</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><ph id="ph1">https://packages.microsoft.com/rhel/7/prod/</ph> (CentOS 7)</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><ph id="ph1">https://packages.microsoft.com/sles/11/prod/</ph> (SLES 11)</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><ph id="ph1">https://packages.microsoft.com/ubuntu/14.04/prod/pool/main/m/</ph> (Ubuntu 14.04)</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><ph id="ph1">https://packages.microsoft.com/ubuntu/16.04/prod/pool/main/m/</ph> (Ubuntu 16.04)</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Package list</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The following packages comprise a full Machine Learning Server installation:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The microsoft-mlserver-python-9.3.0 package provides Anaconda 4.2 with Python 3.5, executing as mlserver-python, found in <ph id="ph1">`/opt/microsoft/mlserver/9.3.0/bin/python/python`</ph></source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Microsoft R Open is required for R execution:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Microsoft .NET Core 2.0, used for operationalization, must be added to Ubuntu:</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Additional open-source packages must be installed if a package is required but not found on the system.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>This list varies for each installation.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Here is one example of the additional packages that were added to a clean RHEL image during a connected (online) setup:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Download packages</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If your system provides a graphical user interface, you can click a file to download it.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Otherwise, use <ph id="ph1">`wget`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>We recommend downloading all packages to a single directory so that you can install all of them in a single command.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>By default, <ph id="ph1">`wget`</ph> uses the working directory, but you can specify an alternative path using the <ph id="ph2">`-outfile`</ph> parameter.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The following example is for the first package.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Each command references the version number of the platform.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Remember to change the number if your version is different.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Linux Software Repository for Microsoft Products<ept id="p1">](https://docs.microsoft.com/windows-server/administration/linux-package-repository-for-microsoft-software)</ept>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Download to CentOS or RHEL: <ph id="ph1">`wget https://packages.microsoft.com/rhel/7/prod/microsoft-mlserver-packages-r-9.3.0.rpm`</ph></source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Download to Ubuntu 16.04: <ph id="ph1">`wget https://packages.microsoft.com/ubuntu/16.04/prod/pool/main/m/microsoft-mlserver-packages-r-9.3.0/microsoft-mlserver-packages-r-9.3.0.deb`</ph></source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Download to SUSE: <ph id="ph1">`wget https://packages.microsoft.com/sles/11/prod/microsoft-mlserver-packages-r-9.3.0.rpm`</ph></source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Repeat for each package in the <bpt id="p1">[</bpt>package list<ept id="p1">](#Package%20list)</ept>.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Install packages</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The package manager determines the installation order.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Assuming all packages are in the same folder:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Install on CentOS or RHEL: <ph id="ph1">`yum install *.rpm`</ph></source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Install on Ubuntu: <ph id="ph1">`dpkg -i *.deb`</ph></source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Install on SUSE: <ph id="ph1">`zypper install *.rpm`</ph></source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>This step completes installation.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Activate the server</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Run the activation script from either the R or Python directory:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>or <ph id="ph1">`/opt/microsoft/mlserver/9.3.0/bin/python/activate.sh`</ph></source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Connect and validate</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>List installed packages:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>On CentOS and RHEL: <ph id="ph1">`rpm -qa | grep microsoft`</ph></source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>On Ubuntu: <ph id="ph1">`apt list --installed | grep microsoft`</ph></source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>On SLES11: <ph id="ph1">`zypper se microsoft`</ph></source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Once you have a package name, you can obtain verbose version information.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>On CentOS and RHEL: <ph id="ph1">`$ rpm -qi microsoft-mlserver-packages-r-9.3.0`</ph></source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>On Ubuntu: <ph id="ph1">`$ dpkg --status microsoft-mlserver-packages-r-9.3.0`</ph></source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>On SLES: <ph id="ph1">`zypper info microsoft-mlserver-packages-r-9.3.0`</ph></source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Output on Ubuntu is as follows:</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Set a MKL_CBWR variable</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Set an MKL_CBWR environment variable to ensure consistent output from Intel Math Kernel Library (MKL) calculations.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Edit or create a file named <bpt id="p1">**</bpt>.bash_profile<ept id="p1">**</ept> in your user home directory, adding the line <ph id="ph1">`export MKL_CBWR="AUTO"`</ph> to the file.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Execute this file by typing <bpt id="p1">**</bpt>source .bash_profile<ept id="p1">**</ept> at a bash command prompt.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Start Revo64</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>As another verification step, run the Revo64 program.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>By default, Revo64 is linked to the /usr/bin directory, available to any user who can log in to the machine:</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>From /Home or any other working directory:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Run a RevoScaleR function, such as <bpt id="p1">**</bpt>rxSummary<ept id="p1">**</ept> on a dataset.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Many sample datasets, such as the iris dataset, are ready to use because they are installed with the software:</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Output from the iris dataset should look similar to the following:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>To quit the program, type <ph id="ph1">`q()`</ph> at the command line with no arguments.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Start Python</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>From Home or any other user directory:</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Run a revoscalepy function, such as <bpt id="p1">**</bpt>rx_Summary<ept id="p1">**</ept> on a dataset.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Many sample datasets are built in.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>At the Python command prompt, paste the following script:</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Output from the sample dataset should look similar to the following:</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>To quit the program, type <ph id="ph1">`quit()`</ph> at the command line with no arguments.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Verify CLI</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Open an Administrator command prompt.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Enter the following command to check availability of the CLI: <ph id="ph1">`az ml admin --help`</ph>.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>If you receive the following error: <ph id="ph1">`az: error argument _command_package: invalid choice: ml`</ph>, follow the <bpt id="p1">[</bpt>instructions to re-add the extension to the CLI<ept id="p1">](https://docs.microsoft.com/en-us/machine-learning-server/resources-known-issues#1-missing-azure-ml-admin-cli-extension-on-dsvm-environments
)</ept>.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>We recommend starting with any Quickstart tutorial listed in the contents pane.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Machine Learning Server<ept id="p1">](r-server-install.md)</ept></source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>What's new in Machine Learning Server<ept id="p1">](../whats-new-in-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Supported platforms<ept id="p1">](r-server-install-supported-platforms.md)</ept></source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Known Issues<ept id="p1">](../resources-known-issues.md)</ept></source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure Machine Learning Server to operationalize your analytics<ept id="p1">](../what-is-operationalization.md)</ept></source>
        </trans-unit></group></body></file></xliff>