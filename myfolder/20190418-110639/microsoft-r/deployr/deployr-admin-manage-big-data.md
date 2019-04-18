<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-admin-manage-big-data.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f02d70ce9070eafef6a2b68091bbe2312dd37200a.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">02d70ce9070eafef6a2b68091bbe2312dd37200a</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-admin-manage-big-data.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Managing External Directories for Big Data - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Big Data in DeployR - Managing External Directories for Big Data</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>big data, DeployR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Managing External Directories for Big Data</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>There may be times when your DeployR user community needs access to genuinely large data files, or big data.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>These data files might be too big to be copied from the Web or copied from their local machines to the server.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>When such files are stored in the DeployR Repository or at any network-accessible URI, the R code executing on the DeployR server can load the desired file data on-demand.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>However, physically moving big data is expensive both in terms of bandwidth and throughput.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>To alleviate this overhead, the DeployR server supports a set of NFS-mounted directories dedicated to managing large data files.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>We refer to these directories as 'big data' external directories.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>As an administrator, you can enable this service by:</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configuring<ept id="p1">](#setting-up-nfs-setup)</ept> the big data directories within your deployment.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Informing your DeployR users that they must use <bpt id="p1">[</bpt>the <ph id="ph1">`deployrExternal`</ph> R function<ept id="p1">](#deployrexternal)</ept> from the <ph id="ph2">`deployrUtils`</ph> package in their R code to reference the big data files within these directories.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>It is the responsibility of the DeployR administrator to configure and manage these 'big data' external directories and the data files within them.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Setting up NFS Setup</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>NFS configuration for external directories is required only if your DeployR environment has multiple grid nodes.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>To benefit from external directory support in a multi-grid node DeployR environment, you (the administrator) must install and configure a Network File System (NFS) shared directory on the DeployR main server as well as any grid node from which they want to access to these big data files.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Configure NFS on Windows</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>NFS mount the <ph id="ph1">`&lt;INSTALL_DIR&gt;/deployr/external`</ph> directory on both the DeployR main server and each grid node.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`&lt;INSTALL_DIR&gt;`</ph> is the full path to directory into which you installed DeployR, which is <ph id="ph2">`C:\Program Files\Microsoft\DeployR-&lt;version&gt;\`</ph> by default.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Open the Windows firewall ports as described in the Windows NFS documentation for your platform.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Configure NFS on Linux</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If you do not have access to the Internet, you’ll have to copy the install files to this machine using another method.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Log into the operating system as <ph id="ph1">`root`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Install NFS.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>For Redhat:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>For SLES:</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Open the file <ph id="ph1">`/etc/sysconfig/nfs`</ph> and add these lines to the end of the file:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>In IPTABLES, open the following ports for NFS for external directory support:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Restart IPTABLES.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Set up the automatic start of NFS and <ph id="ph1">`portmap/rpcbind`</ph> at boot time.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>At the prompt, type:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>For both the main server and any grid machines on Redhat 5, type:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>For both the main server and any grid machines on Redhat 6, type:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>For the main server on SLES, type the following at the prompt:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>For a grid machine on SLES, type the following at the prompt:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>To create a new NFS directory share, run the following commands.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>To update an existing NFS share, see the next step instead.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>On the DeployR main server:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Add a line to the file <ph id="ph1">`/etc/exports`</ph> as follows where <ph id="ph2">&lt;VERSION&gt;</ph> is the installed version of DeployR.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Broadcast the new directory.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>At the prompt, type:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>On the DeployR grid node machine:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Add a line to the end of the fstab file, where <ph id="ph1">`&lt;DeployR_server_ip&gt;`</ph> is the IP or hostname of the machine on which you installed DeployR,</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Attempt to mount the contents of the file and verify the NFS points to the correct address.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>At the prompt, type:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>To use an existing NFS directory share, do the following for the main server and each grid node.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Add the following line to <ph id="ph1">`/etc/fstab`</ph>, where <ph id="ph2">`&lt;nfs_share_hostname&gt;`</ph> and <ph id="ph3">`&lt;nfs_share_directory&gt;`</ph> is the IP or hostname and directory of the machine where the NFS share site exists:</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Try to mount the contents of the file and verify the NFS points to the correct address.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>At the prompt, type:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>External Directory Structure</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>While it suffices for users to store their local copy of the data in the current working directory of their R session, the external directory structure in the DeployR server environment is not transparent to the users.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>For this reason, you need to <bpt id="p1">[</bpt>put the files into the external directories for them<ept id="p1">](#adding-files-to-external-directories)</ept>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>The external directory structure is really a tree of public and private directories hanging off a common base directory managed by you, the DeployR administrator.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The default base directory for the external directory structure might be:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>On Windows, <ph id="ph1">`C:/Program Files/Microsoft/DeployR-&lt;version&gt;/deployr/external/data/`</ph></source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>On Linux, <ph id="ph1">`/home/deployr-user/deployr/&lt;version&gt;/deployr/external/data`</ph></source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>On Mac OS X (DeployR Open only), <ph id="ph1">`/Users/deployr-user/deployr/&lt;version&gt;/deployr/external/data`</ph></source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Two external subdirectories are automatically created by the server the first time the corresponding user logs into the system.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>The first directory is called <ph id="ph1">`/public`</ph> and contains the files that can be read by any authenticated users on the server.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>The second directory is the user’s private directory.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Each private external directory can be found at <ph id="ph1">`&lt;DeployR_Install_Dir&gt;/external/data/{deployr_username_private_directory}`</ph>.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Files in each private directory are available only to that authenticated user during a live session.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The administrator can also manually create these subdirectories in advance.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>The names of the directories are case-sensitive.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>For example, the user <ph id="ph1">`testuser`</ph> would have access to the files under:</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The private external directory, <ph id="ph1">`&lt;DeployR_Install_Dir&gt;/deployr/external/data/testuser`</ph></source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`/public`</ph> directory, <ph id="ph2">`&lt;DeployR_Install_Dir&gt;/deployr/external/data/public`</ph></source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>It is up to the administrator to inform each user of which files are available in the <ph id="ph1">`/public`</ph> directory and which files are in their private directory.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Adding Files to External Directories</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>A file can be added to the external directories in one of two ways:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>You can place the file, on the user's behalf, into his or her private external directories or into the <ph id="ph1">`/public`</ph> external directory so that it can be access when running R code.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>A user can execute R code that will write a file directly into his or her private external directory.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Ultimately, the administrator is responsible for moving and managing files in the external directories as well as informing users that the files exist and their whereabouts.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>To reference one of these files in the code, a user must declare and, therefore, know if the given file is stored in the <ph id="ph1">`/public`</ph> external subdirectory or the user's private subdirectory.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>This declaration is done using the <ph id="ph1">`deployrExternal`</ph> function in the <ph id="ph2">`deployrUtils`</ph> package.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>This function provides read and write access to big data files in a portable way whether the R code is run locally or in the remote DeployR server environment.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>For more information, point your users to the <bpt id="p1">[</bpt>Writing Portable R Code<ept id="p1">](deployr-data-scientist-write-portable-r-code.md#portable-access-to-data-files)</ept> guide and the package help for this function (<ph id="ph1">`??deployrUtils::deployrExternal`</ph>).</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Currently there is no user interface to display the names of the files in this directory.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Additionally, due to the potentially large size of the data, we do not expose any API or other facility for moving data into the external directories.</source>
        </trans-unit></group></body></file></xliff>