<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-linux-manage-install.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c43170601c936c1669d86f1d7c66e76b7b7b1161f.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">43170601c936c1669d86f1d7c66e76b7b7b1161f</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-linux-manage-install.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Manage an R Server installation on Linux</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Manage an R Server installation on Linux</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Manage your Microsoft R Server installation on Linux</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Covers file management (ownership and permissions), creating a local package repository for production servers deployed behind a firewall, and how to make RevoScaleR the default R script engine.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>File permissions</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>By default, R Server files are installed with read-write permission for owner and read-only permission for group and world.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Directories are installed with execute permission as well, to permit them to be traversed.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>If you need to modify these permissions, you can use the <bpt id="p1">[</bpt><bpt id="p2">**</bpt>chmod<ept id="p2">**</ept> command<ept id="p1">](https://en.wikipedia.org/wiki/Chmod)</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>For files owned by root, use <bpt id="p1">**</bpt>chmod<ept id="p1">**</ept> with root privileges.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>File ownership</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>By default, R Server files are owned by root.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>For single-user workstations where the user has either sudo privileges or access to the root password, this is normally fine.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>In enterprise environments, however, it's common to have third-party applications such as Microsoft R Server installed into an account owned by a non-root user as a security precaution.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>In such an environment, you might want to create an "RUser" account, and change ownership of the files to that user.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>You can do that as follows:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Server as root, as usual.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Login as root or super user to create accounts or change file ownership.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Create the "RUser" account if it does not already exist.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Assign this user to a suitable group, if desired.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">[</bpt><bpt id="p2">**</bpt>chown<ept id="p2">**</ept> command<ept id="p1">](https://en.wikipedia.org/wiki/Chown)</ept> to change ownership of the files.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>In the following example, we assume RUser has been made a member of the dev group:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Use Revo64 as the default R script engine</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If you installed base R first, followed by Microsoft R Server, the automated installer detects that R exists and does not prompt you to link R to Revo64.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>In this case, you can use both versions of R simply by calling them by their respective script names: “R” and “Revo64”.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>To make R Server the default R script engine, do the following:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Rename the R script by appending the R version, for example 3.3.3:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Create a symbolic link from the Revo64 script to R:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Set up a local package repository behind a firewall</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>One of the strengths of the R language is the thousands of third-party packages that have been made publicly available via CRAN, the Comprehensive R Archive Network.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>R includes a number of functions that make it easy to download and install these packages.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>However, in many enterprise environments, access to the Internet is limited or non-existent.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>In such environments, it is useful to create a local package repository that users can access from within the corporate firewall.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>A local repository may contain source packages, binary packages, or both.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If some or all of your users will be working on Windows systems, you should include Windows binaries in your repository.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Windows binaries are R-version-specific; if you are running R 3.3.3, you need Windows binaries built under R 3.3.3.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>These versioned binaries are available from CRAN and other public repositories.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If some or all of your users will be working on Linux systems, you must include source packages in your repository.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The Microsoft Managed R Archive Network (MRAN) provides daily snapshots of all of CRAN, and together with the Microsoft-developed open-source package miniCRAN can be used to easily build a local package repository containing source packages, binary packages, or both.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>There are two ways to create the package repository: either copy all the packages from a given MRAN snapshot, or create a new repository and populate it with just those packages you want to be available to your users.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>We will describe both procedures using MRAN and miniCRAN.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The miniCRAN package itself is dependent on 18 other CRAN packages, among which is the RCurl package, which has a system dependency on the curl-devel package.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Similarly, package XML has a dependency on libxml2-devel.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>We recommend, therefore, that you build your local repository initially on a machine with full Internet access, so that you can easily satisfy all these dependencies.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>After created, you can either move the repository to a different location within your firewall, or simply disable the machine’s Internet access.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Approach 1: use miniCRAN</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>On a system with Internet access, the easiest way to install the miniCRAN package (or any R package) is to start R and use the install.packages function:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If your system already contains all the system prerequisites, this will normally download and install all of miniCRAN’s R package dependencies as well as miniCRAN itself.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If a system dependency is missing, compilation of the first package that needs that dependency will fail, typically with a specific but not particularly helpful message.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>In our testing, we have found that an error about curl-config not being found indicates that the curl-devel package is missing, and an error about libxml2 indicates the libxml2-devel package is missing.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>If you get such an error, exit R, use yum or zypper to install the missing package, then restart R and retry the install.packages command.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Approach 2: use an MRAN snapshot</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Creating a repository from an MRAN snapshot is very straightforward:</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Choose a location for your repository somewhere on your local network.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>If you have a corporate intranet, this is usually a good choice, provided URLs have the prefix http:// and not https://.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Any file system that is mounted for all users can be used; file-based URLs of the form file:// are supported by the R functions.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>In this example, we suppose the file system /local is mounted on all systems and we will create our repository in the directory /local/repos.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Start R and load the miniCRAN package:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Specify an MRAN snapshot:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Set your MRAN snapshot as your CRAN repo:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Use miniCRAN’s pkgAvail function to obtain a list of (source) packages in your MRAN snapshot:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Use miniCRAN’s makeRepo function to create a repository of these packages in your /local/repos directory:</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Create a custom repository</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>You can customize a package repository to include specific packages rather than all-inclusive snapshots providing more packages than you need.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>A custom repository gives you complete control over which packages are available to your users.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Here, too, you have two basic choices in terms of populating your repository: you can either use the previously described miniCRAN makeRepo function to select specific packages from an existing MRAN snapshot</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Alternatively, you can combine your own locally developed packages with packages from other sources.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The second option offers the greatest control, but typically means you need to manage the contents using home-grown tools.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Recommendations for Windows binary packages</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>If using your own tools to create a custom package directory, your Windows binary packages should have a path of the form:</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>while source packages should have a path of the form:</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Windows binary packages should be built with your current R version.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Windows binary files will be zip files.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Package source files will be tar.gz files.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Move the desired packages to the appropriate directories, then run the R function write<ph id="ph1">\_</ph>PACKAGES in the tools package to create the PACKAGES and PACKAGES.gz index files:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Configure R to use a local repository</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>To make your local repository available to your R users:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Open the file Rprofile.site in the /etc directory of your installed R (if you installed to the default /usr prefix, the path is /usr/lib64/MRO-for-MRS-9.0.1/R-3.3.3/lib64/R/etc/Rprofile.site).</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Find the following line in the Rprofile.site file:</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Add your repository as follows:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>If you added more than one repository and used R version numbers, add multiple lines of the form LOCAL<ph id="ph1">\_</ph>VER="file:///local/repos/VER", for example:</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Save the file and your repository is ready for use.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>If you are in a locked-down environment without access to the standard Microsoft repository, <bpt id="p1">*</bpt>replace<ept id="p1">*</ept> the Revo repository with your local repository (or repositories).</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install R Server 8.0.5 for Linux<ept id="p1">](r-server-install-linux-server-805.md)</ept></source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install R Server 9.0.1 for Linux<ept id="p1">](r-server-install-linux-server-901.md)</ept></source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install R on Hadoop overview<ept id="p1">](r-server-install-hadoop.md)</ept></source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Uninstall Microsoft R Server to upgrade to a newer version<ept id="p1">](r-server-install-linux-uninstall.md)</ept></source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Troubleshoot R Server installation problems on Hadoop<ept id="p1">](r-server-install-hadoop-troubleshoot.md)</ept></source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure R Server to operationalize analytics<ept id="p1">](operationalize-r-server-one-box-config.md)</ept></source>
        </trans-unit></group></body></file></xliff>