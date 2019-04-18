<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="machine-learning-server-linux-install.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4dbdb33fffb208893a4b7ffbac846b6f5fff8aac5.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">dbdb33fffb208893a4b7ffbac846b6f5fff8aac5</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\machine-learning-server-linux-install.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install Machine Learning Server for Linux</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to install, connect to, and use Machine Learning Server on computers running a Linux operating system.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server for Linux</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Machine Learning Server 9.2.1 | 9.3<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Machine Learning Server for Linux runs machine learning and data mining solutions written in R or Python in standalone and clustered topologies.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This article explains how to install Machine Learning Server on a standalone Linux server that has an internet connection.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>If your server has restrictions on internet access, see <bpt id="p1">[</bpt>offline installation<ept id="p1">](machine-learning-server-linux-offline.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This article covers the following items:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Package manager overview</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>In-place upgrades of existing installations</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Installation steps</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>An inventory of what's installed</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>System and setup requirements</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Operating system must be a <bpt id="p1">[</bpt>supported version of 64-bit Linux<ept id="p1">](r-server-install-supported-platforms.md)</ept>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Minimum RAM is 2 GB.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Minimum disk space is 500 MB (8 GB or more is recommended).</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>An internet connection.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If you do not have an internet connection, use the <bpt id="p1">[</bpt>offline installation instructions<ept id="p1">](machine-learning-server-linux-offline.md)</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Root or super user permissions</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Licensing</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Machine Learning Server is licensed as a SQL Server supplemental feature, even though SQL Server itself is not installed or required on a standalone Machine Learning Server installation.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>On development workstations, you can install the developer edition at no charge.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>For example, if you are learning how to use the RevoScaleR libraries, or developing a solution that is not in production, you would use this edition.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>On production servers where code supports ongoing business operations or is part of a solution you are selling commercially, you will need the enterprise edition.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The enterprise edition of Machine Learning Server for Windows is licensed by the core.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Enterprise licenses are sold in 2-core packs, and you must have a license for every core on the machine.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>For example, on an 8-core server, you would need four 2-core packs.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If you have questions, <bpt id="p1">[</bpt>review the pricing page or contact Microsoft<ept id="p1">](https://www.microsoft.com/sql-server/sql-server-2017-pricing)</ept> for more information.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>When you purchase an enterprise license of Machine Learning Server for Linux, you can install <bpt id="p1">[</bpt>Machine Learning Server for Hadoop<ept id="p1">](machine-learning-server-hadoop-install.md)</ept> for free (5 nodes for each core licensed under enterprise licensing).</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Package managers</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Setup is through package managers that retrieve distributions from Microsoft web sites and install the software.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Unlike previous releases, there is no install.sh script.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>You must have one of these package managers to install Machine Learning Server for Linux.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Package manager</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Platform</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>yum<ept id="p1">](https://access.redhat.com/documentation/Red_Hat_Enterprise_Linux/6/html/Deployment_Guide/ch-yum.html)</ept></source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>RHEL, CentOS</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>apt<ept id="p1">](https://help.ubuntu.com/lts/serverguide/apt.html)</ept></source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Ubuntu online</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>dpkg<ept id="p1">](https://help.ubuntu.com/lts/serverguide/dpkg.html)</ept></source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Ubuntu offline</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>zypper<ept id="p1">](https://www.suse.com/documentation/opensuse111/opensuse111_reference/data/sec_zypper.html)</ept></source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>SUSE</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rpm<ept id="p1">](https://en.wikipedia.org/wiki/Rpm_(software))</ept></source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>RHEL, CentOS, SUSE</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The package manager downloads packages from the <bpt id="p1">[</bpt>packages.microsoft.com<ept id="p1">](https://packages.microsoft.com)</ept> repo, determines dependencies, retrieves additional packages, sets the installation order, and installs the software.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>For example syntax on linking to the repo, see <bpt id="p1">[</bpt>Linux Software Repository for Microsoft Products<ept id="p1">](https://docs.microsoft.com/windows-server/administration/linux-package-repository-for-microsoft-software)</ept>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Machine Learning Server activation is a separate step <bpt id="p1">*</bpt>not<ept id="p1">*</ept> performed by the package manager.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>If you forget to activate, the server works, but the following error appears when you call an API: "Express Edition will continue to be enforced."</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Upgrade existing installations</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If your existing server was configured for <bpt id="p1">[</bpt>operationalization<ept id="p1">](../what-is-operationalization.md)</ept>, follow these alternative steps for upgrade: <bpt id="p2">[</bpt>Configure Machine Learning Server to operationalize analytics (One-box) &gt; How to upgrade<ept id="p2">](../operationalize/configure-machine-learning-server-one-box.md#how-to-upgrade)</ept> or <bpt id="p3">[</bpt>Configure Machine Learning Server to operationalize analytics (Enterprise) &gt; How to upgrade<ept id="p3">](../operationalize/configure-machine-learning-server-enterprise.md#how-to-upgrade)</ept>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>For all other configurations, Setup performs an in-place upgrade on an existing installation.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Although the installation path is new (<ph id="ph1">`/opt/microsoft/mlserver/9.3`</ph>), when R Server 9.x is present, Machine Learning Server 9.3 finds R Server at the old path (<ph id="ph2">`/usr/lib64/microsoft-r/9.1.0`</ph>) and upgrades it to the new version.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>There is no support for side-by-side installations of older and newer versions, nor is there support for hybrid versions (such as R Server 9.1 and Python 9.3).</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>An installation is either entirely 9.3 or an earlier version.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Installation paths</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>After installation completes, software can be found at the following paths:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Install root: <ph id="ph1">`/opt/microsoft/mlserver/9.3.0`</ph></source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Microsoft R Open root: <ph id="ph1">`/opt/microsoft/ropen/3.4.3`</ph></source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Executables like Revo64 and mlserver-python are at <ph id="ph1">`/usr/bin`</ph></source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;a name="redhat"&gt;</bpt>Install on Red Hat or CentOS<ept id="p1">&lt;/a&gt;</ept></source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Run the following commands to install Machine Learning Server for Linux on Red Hat Enterprise (RHEL) and CentOS (6.x - 7.x).</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If you run into problems, try <bpt id="p1">[</bpt>manual configuration<ept id="p1">](https://docs.microsoft.com/windows-server/administration/linux-package-repository-for-microsoft-software#manual-configuration)</ept> instead.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;a name="ubuntu"&gt;</bpt>Install on Ubuntu <ept id="p1">&lt;/a&gt;</ept></source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Follow these instructions for Machine Learning Server for Linux on Ubuntu (14.04 - 16.04 only).</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;a name="suse"&gt;</bpt>Install on SUSE <ept id="p1">&lt;/a&gt;</ept></source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Follow these instructions for Machine Learning Server for Linux on SUSE (SLES11 only).</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Set a MKL_CBWR variable</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Set an MKL_CBWR environment variable to ensure consistent output from Intel Math Kernel Library (MKL) calculations.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Edit or create a file named <bpt id="p1">**</bpt>.bash_profile<ept id="p1">**</ept> in your user home directory, adding the line <ph id="ph1">`export MKL_CBWR="AUTO"`</ph> to the file.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Execute this file by typing <bpt id="p1">**</bpt>source .bash_profile<ept id="p1">**</ept> at a bash command prompt.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Start Revo64</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>As another verification step, run the <bpt id="p1">**</bpt>Revo64<ept id="p1">**</ept> program.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>By default, <bpt id="p1">**</bpt>Revo64<ept id="p1">**</ept> is installed in the /usr/bin directory, available to any user who can log in to the machine:</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>From /Home or any other working directory:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Run a RevoScaleR function, such as <bpt id="p1">**</bpt>rxSummary<ept id="p1">**</ept> on a dataset.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Many sample datasets, such as the iris dataset, are ready to use because they are installed with the software:</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Output from the iris dataset should look similar to the following:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>To quit the program, type <ph id="ph1">`q()`</ph> at the command line with no arguments.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Start Python</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>From Home or any other user directory:</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Run a revoscalepy function, such as <bpt id="p1">**</bpt>rx_Summary<ept id="p1">**</ept> on a dataset.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Many sample datasets are built in.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>At the Python command prompt, paste the following script:</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Output from the sample dataset should look similar to the following:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>To quit the program, type <ph id="ph1">`quit()`</ph> at the command line with no arguments.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Verify CLI</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Open an Administrator command prompt.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Enter the following command to check availability of the CLI: <ph id="ph1">`az ml admin --help`</ph>.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>If you receive the following error: <ph id="ph1">`az: error argument _command_package: invalid choice: ml`</ph>, follow the <bpt id="p1">[</bpt>instructions to re-add the extension to the CLI<ept id="p1">](https://docs.microsoft.com/en-us/machine-learning-server/resources-known-issues#1-missing-azure-ml-admin-cli-extension-on-dsvm-environments
)</ept>.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Enable web service deployment and remote connections</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>After you confirm the basic install, continue with the next step: <bpt id="p1">[</bpt>configuring the server for operationalization<ept id="p1">](../operationalize/configure-start-for-administrators.md#configure-server-for-operationalization)</ept> to enable additional functionality, including logging, diagnostics, and web service hosting.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>You can use the <ph id="ph1">`bootstrap`</ph> command for this step.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>This command enables operationalization features on a standalone server.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>It creates and starts a web node and compute node, and runs a series of diagnostic tests against the configuration to confirm the internal data storage is functional and that web services can be successfully deployed.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Alternatively, if you have multiple servers, you can designate each one as either a web node or compute node, and then link them up.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>For instructions, see <bpt id="p1">[</bpt>Configure Machine Learning Server (Enterprise)<ept id="p1">](../operationalize/configure-machine-learning-server-enterprise.md)</ept>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Open an Administrator command prompt.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Enter the following command to invoke the Administrator Command Line Interface (CLI) and configure the server: <ph id="ph1">`az ml admin bootstrap`</ph></source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Set a password used to protect your configuration settings.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Later, after configuration is finished, anyone who wants to use the CLI to modify a configuration must provide this password to gain access to settings and operations.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>The password must meet these requirements: 8-16 characters long, with at least one upper-case letter, one lower-case letter, one number, and one special character.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>After you provide the password, the tool does the rest.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Your server is fully operationalized once the process is complete.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>For more information about the benefits of operationalization:</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Deploy Python and R script as a web service<ept id="p1">](../operationalize/concept-what-are-web-services.md)</ept></source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Connect to a remote R server for code execution<ept id="p1">](../r/how-to-execute-code-remotely.md)</ept>.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Remote execution makes the server accessible to client workstations running <bpt id="p1">[</bpt>R Client<ept id="p1">](../r-client/install-on-linux.md)</ept> or other Machine Learning Server nodes on your network.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Python support is new and there are a few limitations in remote computing scenarios.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Remote execution is not supported on Windows or Linux in Python code.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Additionally, you cannot set a <bpt id="p1">[</bpt>remote compute context<ept id="p1">](../r/concept-what-is-compute-context.md)</ept> to HadoopMR in Python.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>What's installed</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>An installation of Machine Learning Server includes some or all of the following components.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Component</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Microsoft R Open (MRO)</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>An open-source distribution of the base R language, plus the Intel Math Kernel library (int-mkl).</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>R proprietary libraries and script engine</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Properietary R libraries are co-located with R base libraries.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Libraries include RevoScaleR, MicrosoftML, mrsdeploy, olapR, RevoPemaR, and others listed in <bpt id="p1">[</bpt>R Package Reference<ept id="p1">](../r-reference/introducing-r-server-r-package-reference.md)</ept>.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>On Linux, the default R installation directory is <ph id="ph1">`/opt/microsoft/mlserver/9.3.0`</ph>.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>RevoScaleR is engineered for distributed and parallel processing for all multi-threaded functions, utilizing available cores and disk storage of the local machine.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>RevoScaleR also supports the ability to transfer computations to other RevoScaleRr instances on other computers and platforms through compute context instructions.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Python proprietary libraries</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Proprietary packages provide modules of class objects and static functions.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Libraries include revoscalepy, microsoftml, and azureml-model-management-sdk.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Anaconda 4.2 with Python 3.5.2</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>An open-source distribution of Python.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Admin CLI<ept id="p1">](../operationalize/configure-admin-cli-launch.md)</ept></source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Used for enabling remote execution and web service deployment, operationalizing analytics, and configuring web and compute nodes.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Pre-trained models<ept id="p1">](microsoftml-install-pretrained-models.md)</ept></source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Used for sentiment analysis and image detection.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Consider adding a development tool on the server to build script or solutions using R Server features:</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Visual Studio 2017<ept id="p1">](https://www.visualstudio.com/downloads/)</ept> followed by the <bpt id="p2">[</bpt>R Tools for Visual Studio (RTVS) add-in<ept id="p2">](https://docs.microsoft.com/visualstudio/rtvs/installation)</ept> and the <bpt id="p3">[</bpt>Python for Visual Studio (PTVS)<ept id="p3">](https://www.visualstudio.com/vs/python/)</ept>.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Package list</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>The following packages comprise a full Machine Learning Server installation:</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>The microsoft-mlserver-python-9.3.0 package provides Anaconda 4.2 with Python 3.5, executing as mlserver-python, found in <ph id="ph1">`/opt/microsoft/mlserver/9.3.0/bin/python/python`</ph></source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Microsoft R Open is required for R execution:</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Microsoft .NET Core 2.0, used for operationalization, must be added to Ubuntu:</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Additional open-source packages are installed if a package is required but not found on the system.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>This list varies for each installation.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Refer to <bpt id="p1">[</bpt>offline installation<ept id="p1">](machine-learning-server-linux-offline.md)</ept> for an example list.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Configure RStudio for RevoScaleR</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>If you are using the RStudio IDE, perform the following steps to load RevoScaleR and other R Client libraries.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Close RStudio if it is already open.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Start a terminal session and sign on as root (<ph id="ph1">`sudo su`</ph>).</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Open the <bpt id="p1">**</bpt>Renviron<ept id="p1">**</ept> file for editing:</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Scroll down to <bpt id="p1">**</bpt>R_LIBS_USER<ept id="p1">**</ept> and add a new configuration setting just below it:</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Save the file.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Start RStudio.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>In the Console window, you should see messages indicating both the Microsoft R Open and Microsoft R Client packages are loaded.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>To confirm RevoScaleR is operational, run the RevoScaleR <bpt id="p1">**</bpt>rxSummary<ept id="p1">**</ept> function to return statistical summary information on the built-in Iris dataset:</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>We recommend starting with any Quickstart tutorial listed in the contents pane.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Machine Learning Server<ept id="p1">](r-server-install.md)</ept></source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>What's new in Machine Learning Server<ept id="p1">](../whats-new-in-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Supported platforms<ept id="p1">](r-server-install-supported-platforms.md)</ept></source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Known Issues<ept id="p1">](../resources-known-issues.md)</ept></source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure Machine Learning Server to operationalize your analytics<ept id="p1">](../what-is-operationalization.md)</ept></source>
        </trans-unit></group></body></file></xliff>