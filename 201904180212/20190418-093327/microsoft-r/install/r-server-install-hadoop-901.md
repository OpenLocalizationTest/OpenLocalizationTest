<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-hadoop-901.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b41ed00b5ec2453c05884520b0c87855f297297426.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1ed00b5ec2453c05884520b0c87855f297297426</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-hadoop-901.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install Microsoft R Server 9.0.1 on Hadoop</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Installation and configuration Microsoft R Server 9.0.1 on Hadoop</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Server 9.0.1 on Hadoop</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>The following instructions are for installation of R Server 9.0.1 for Hadoop.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Side-by-side Installation<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>You can install major versions of R Server (such as an 8.x and 9.x) side-by-side on Hadoop, but not minor versions.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>For example, you already installed Microsoft R Server 8.0, you must uninstall it before installing 8.0.5.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Upgrade Versions<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>If you want to replace an older version rather than run side-by-side, you can uninstall the older distribution before installing the new version (there is no in-place upgrade).</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>Uninstall Microsoft R Server to upgrade to a newer version<ept id="p1">](r-server-install-uninstall-upgrade.md)</ept> for instructions.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Installation Steps<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>A summary of setup tasks is as follows:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Download software.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Unzip to extract packages and an install script (install.sh)</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Run the install script with a -p parameter (for Hadoop)</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Verify the installation</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The install script downloads and installs Microsoft R Open (microsoft-r-server-mro-9.0.x86_64.rpm).</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>This distribution provides the following packages that are new in this version:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>microsoft-r-server-intel-mkl-9.0.rpm</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>microsoft-r-server-packages-9.0.rpm</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>microsoft-r-server-hadoop-9.0.rpm</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>In contrast with previous releases, this version  comes with a requirement for <ph id="ph1">`root`</ph> installation.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Non-root installations are not supported.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Recommendations for installation</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>We recommend installing R Server on all nodes of the cluster to avoid Hadoop queuing up jobs on nodes that don't actually have R Server.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Although the task will eventually get reassigned to a node that has R Server, you will see errors from the worker node and experience unnecessary delay while waiting for the error to resolve.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Microsoft Azure offers virtual machines with Hadoop templates.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If you don't have a Hadoop cluster, you can purchase and provision virtual machines on Azure using templates provided by several vendors.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Sign in to <bpt id="p1">[</bpt>Azure portal<ept id="p1">](https://ms.portal.azure.com)</ept>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>New<ept id="p1">**</ept> in the top left side bar.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>In the search box, type the name of one of these vendors: Cloudera, HortonWorks, and MapR.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Several of these vendors offer sandbox deployments that make it easier to get started.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>System requirements</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>R Server must be installed on at least one master or client node which will serve as the submit node; it should be installed on as many workers as is practical to maximize the available compute resources.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Nodes must have the same version of R Server within the cluster.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Setup checks the operating system and detects the Hadoop cluster, but it doesn't check for specific distributions.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Microsoft R Server works with the Hadoop distributions listed here: <bpt id="p1">[</bpt>Supported platforms<ept id="p1">](r-server-install-supported-platforms.md)</ept></source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Microsoft R Server requires Hadoop MapReduce, the Hadoop Distributed File System (HDFS), and Apache YARN.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Optionally, Spark version 1.6-2.0 is supported for Microsoft R Server 9.0.1.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>In this version, the installer should provide most of the dependencies required by R Server, but if the installer reports a missing dependency, see <bpt id="p1">[</bpt>Package Dependencies for Microsoft R Server installations on Linux and Hadoop<ept id="p1">](r-server-install-linux-hadoop-packages.md)</ept> for a complete list of the dependencies required for installation.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Minimum system configuration requirements for Microsoft R Server are as follows:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Processor:<ept id="p1">**</ept> 64-bit CPU with x86-compatible architecture (variously known as AMD64, Intel64, x86-64, IA-32e, EM64T, or x64 CPUs).</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Itanium-architecture CPUs (also known as IA-64) are not supported.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Multiple-core CPUs are recommended.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Memory:<ept id="p1">**</ept> A minimum of 8 GB of RAM is required for Microsoft R Server; 16 GB or more are recommended.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Hadoop itself has substantial memory requirements; see your Hadoop distribution’s documentation for specific recommendations.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Disk Space:<ept id="p1">**</ept> A minimum of 500 MB of disk space is required on each node for R Server.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Hadoop itself has substantial disk space requirements; see your Hadoop distribution’s documentation for specific recommendations.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Unpack the distribution</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Download the software to a writable directory, such as <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept>, unpack the distribution and then run the installation script.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The distribution includes one installer for Microsoft R Server.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>For a gzipped TAR file, you should unpack the file as follows (be sure you have downloaded the file to a writable directory, such as <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept>):</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Log in as root or a user with sudo privileges.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Switch to the <bpt id="p1">**</bpt>/tmp<ept id="p1">**</ept> directory (assuming it's the download location)</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Unpack the file:      <ph id="ph1">`[tmp] $ tar zxvf en_r_server_901_for_hadoop_x64_9648875.gz`</ph></source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Run the install script</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Microsoft R Server 2016 for Hadoop is deployed by running the install script with the <bpt id="p1">**</bpt>-p<ept id="p1">**</ept> parameter, which you can install at the root, or as super user via <ph id="ph1">`sudo`</ph>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Log in as root or a user with sudo privileges (<ph id="ph1">`sudo su`</ph>).</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>The following instructions assume user privileges with the sudo override.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Verify system repositories are up-to-date:      [username] $ <ph id="ph1">`sudo yum clean all`</ph></source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Change to the directory to which you mounted or unpacked the installer (for example, /mnt/mrsimage for an .img file, or /tmp/MRS90HADOOP if you unpacked the tar.gz file):      [username] $ <ph id="ph1">`cd /tmp`</ph> [username tmp] $ <ph id="ph2">`cd /MRS90HADOOP`</ph></source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Run the script with the <bpt id="p1">**</bpt>-p<ept id="p1">**</ept> parameter, specifying the Hadoop component:      [username tmp MRS90HADOOP] $ <ph id="ph1">`sudo bash install.sh -p`</ph></source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>When prompted to accept the license terms for Microsoft R Open, click Enter to read the EULA, click <bpt id="p1">**</bpt>q<ept id="p1">**</ept> when you are finished reading, and then click <bpt id="p2">**</bpt>y<ept id="p2">**</ept> to accept the terms.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Repeat to accept license terms for Microsoft R Server.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Installer output shows the packages and location of the log file.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Verify installation</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>List installed packages and get package names:      [MRS90HADOOP] $ <ph id="ph1">`yum list \*microsoft\*`</ph> [MRS90HADOOP] $ <ph id="ph2">`yum list \*deployr\*`</ph></source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Check the version of Microsoft R Open using <ph id="ph1">`rpm -qi`</ph>:      [MRS90HADOOP] $ <ph id="ph2">`rpm -qi microsoft-r-open-mro-3.3.x86_64`</ph></source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Check the version of Microsoft R Server:      [MRS90HADOOP] $ <ph id="ph1">`rpm -qi microsoft-r-server-packages-9.0.x86_64`</ph></source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Partial output is as follows (note version 9.0.1):</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>For further verification, check folders and permissions.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Following that, you should run the Revo64 program, a sample Hadoop job, and if applicable, a sample Spark job.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Check folders and permissions<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Each user should ensure that the appropriate user directories exist, and if necessary, create them with the following shell commands:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>The HDFS directory can also be created in a user’s R session (provided the top-level /user/RevoShare has the appropriate permissions) using the following RevoScaleR commands (substitute your actual user name for "username").</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Run the RevoScaleR commands in a Revo64 session.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Output for each command should be <ph id="ph1">`[1] TRUE`</ph>.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>As part of this process, make sure the base directories /user and /user/RevoShare have <ph id="ph1">`uog+rwx`</ph> permissions as well.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Run programs and sample jobs using sample data<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The next procedure loads sample data and runs the Revo64 program to further verify the installation.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Send sample data to HDFS.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Start Revo64.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Run a simple local computation.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>This step uses the proprietary Microsoft libraries.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Partial output is as follows (showing the first 4 lines).</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Run a sample local job.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>This step uses the sample dataset and downloads data from HDFS, confirming that your local session can access HDFS.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Paste the following code into your Revo64 session.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Partial output is as follows (showing the last 8 lines).</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Run a sample Hadoop job.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>This step uses the sample dataset to run a Hadoop job.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Paste the following code into your Revo64 session.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>This snippet differs from the previous snippet by the first line.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Partial output is as follows (showing the first 10 lines).</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Run a sample Spark job.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>To quit the program, type <ph id="ph1">`q()`</ph> at the command line with no arguments.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Manual Installation</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>An alternative to running the install.sh script is manual installation of each package and component, or building a custom script that satisfies your technical or operational requirements.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Assuming that the packages for Microsoft R Open and Microsoft R Server are already unpacked, a manual or custom installation must create the appropriate folders and set permissions.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RPM or DEB Installers<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`/var/RevoShare/`</ph> and <ph id="ph2">`hdfs://user/RevoShare`</ph> must exist and have folders for each user running Microsoft R Server in Hadoop or Spark.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`/var/RevoShare/&lt;user&gt;`</ph> and <ph id="ph2">`hdfs://user/RevoShare/&lt;user&gt;`</ph> must have full permissions (all read, write, and executive permissions for all users).</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Cloudera Parcel Installers<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Create <ph id="ph1">`/var/RevoShare/`</ph> and <ph id="ph2">`hdfs://user/RevoShare`</ph>.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Parcels cannot create them for you.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Give <ph id="ph1">`/var/RevoShare/&lt;user&gt;`</ph> and <ph id="ph2">`hdfs://user/RevoShare/&lt;user&gt;`</ph> for each user.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Grant full permissions to both <ph id="ph1">`/var/RevoShare/&lt;user&gt;`</ph> and <ph id="ph2">`hdfs://user/RevoShare/&lt;user&gt;`</ph>.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Distributed Installation</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>If you have multiple nodes, you can automate the installation across nodes using any distributed shell.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>(You can, of course, automate installation with a non-distributed shell such as bash using a for-loop over a list of hosts, but distributed shells usually provide the ability to run commands over multiple hosts simultaneously.) Examples include <bpt id="p1">[</bpt>dsh ("Dancer’s shell")<ept id="p1">](http://www.netfort.gr.jp/~dancer/software/dsh.html.en)</ept>, <bpt id="p2">[</bpt>pdsh (Parallel Distributed Shell)<ept id="p2">](http://sourceforge.net/projects/pdsh/)</ept>, <bpt id="p3">[</bpt>PyDSH (the Python Distributed Shell)<ept id="p3">](http://pydsh.sourceforge.net/)</ept>, and <bpt id="p4">[</bpt>fabric<ept id="p4">](http://www.fabfile.org/)</ept>.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Each distributed shell has its own methods for specifying hosts, authentication, and so on, but ultimately all that is required is the ability to run a shell command on multiple hosts.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>(It is convenient if there is a top-level copy command, such as the pdcp command that is part of pdsh, but not necessary.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>The “cp” command can always be run from the shell.)</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Download Microsoft R Open rpm and the Microsoft R Server installer tar.gz file and copy all to /tmp.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Mount the IMG file.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>The following commands create a mount point and mount the file to that mount point:</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>For RHEL/CENTOS systems;      tar zxvf MRS80RHEL.tar.gz</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>For SLES systems;      tar zxvf MRS80SLES.tar.gz</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Copy the installer gzipped tar file to a writable directory, such as /tmp:</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>From the mounted img file:      cp /mnt/mrsimage/Microsoft-R-Server-<ph id="ph1">`*`</ph>.tar.gz /tmp</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>From the unpacked tar file:      cp /tmp/MRS80<ph id="ph1">&lt;em&gt;</ph>/Microsoft-R-Server-<ph id="ph2">`&lt;/em&gt;`</ph>.tar.gz /tmp</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>The following commands use pdsh and pdcp to distribute and install Microsoft R Server (ensure that each command is run on a single logical line, even if it spans two lines below due to space constraints; lines beginning with “<ph id="ph1">&amp;gt;</ph>” indicate commands typed into an interactive pdsh session):</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Install additional packages on each node using rxExec</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Once you have R Server installed on a node, you can the <ph id="ph1">`rxExec`</ph> function in RevoScaleR to install additional packages, including third-party packages from CRAN or another repository.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>For example, to install the <ph id="ph1">`SuppDists`</ph> package on all the nodes of your cluster, call <ph id="ph2">`rxExec`</ph> as follows:</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Configure R Server to operationalize your analytics</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Developers might want to configure R Server after its installation to benefit from the deployment and consumption of web services on your Hadoop cluster.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>This optional feature provides a server-based framework for running R code in real time.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>We recommend that you set up the <bpt id="p1">[</bpt>"one-box configuration"<ept id="p1">](operationalize-r-server-one-box-config.md#onebox)</ept>, where the compute node and web node are on the same machine.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>If you need to scale the configuration, then you can add web nodes and compute nodes on the other edge nodes.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Do not configure a web node or compute node on any data nodes since they are not YARN resources.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install R on Hadoop overview<ept id="p1">](r-server-install-hadoop.md)</ept></source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Microsoft R Server on Linux<ept id="p1">](r-server-install-linux-server.md)</ept></source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Uninstall Microsoft R Server to upgrade to a newer version<ept id="p1">](r-server-install-uninstall-upgrade.md)</ept></source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Troubleshoot R Server installation problems on Hadoop<ept id="p1">](r-server-install-hadoop-troubleshoot.md)</ept></source>
        </trans-unit></group></body></file></xliff>