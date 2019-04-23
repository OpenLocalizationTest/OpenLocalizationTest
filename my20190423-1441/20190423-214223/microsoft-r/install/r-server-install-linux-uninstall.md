<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-linux-uninstall.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86dae0916e0cdca74bce1c3a45061f6a77dcbf5227.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">dae0916e0cdca74bce1c3a45061f6a77dcbf5227</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-linux-uninstall.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Uninstall R Server on Linux to upgrade to a newer version</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Upgrade Microsoft R Server and the RevoScaleR package by uninstalling the existing version and installing a newer version.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Uninstall R Server on Linux to upgrade to a newer version</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>This article explains how to uninstall Microsoft R Server on Linux.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Unless you are upgrading from 9.0.1 to the <bpt id="p1">[</bpt>the latest version 9.1<ept id="p1">](r-server-install-linux-server.md)</ept>, upgrade requires that you first uninstall the existing deployment before installing a new distribution.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>For 9.0.1-to-9.1, the install script automatically removes previous versions of R Server or Microsoft R Open 3.3.2 if they are detected so that setup can install newer versions.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Program version and file locations</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>As a first step, use your package manager to list the currently installed R Server packages.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Typically, CentOS and Red Hat systems use <bpt id="p1">**</bpt>yum<ept id="p1">**</ept>, Ubuntu systems use <bpt id="p2">**</bpt>apt-get<ept id="p2">**</ept>, and SLES systems use <bpt id="p3">**</bpt>zypper<ept id="p3">**</ept>:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>List the packages from Microsoft.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>On RHEL:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>On Ubuntu:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>On SUSE:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>On a 9.1 installation, you will see about 9 packages.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Since multiple major versions can coexist, the package list could be much longer.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Given a list of packages, you can get verbose version information for particular packages in the list.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The following examples are for Microsoft R Open version 3.3.3:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>On RHEL:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>On Ubuntu:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>On SUSE:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If R Server was installed on Cloudera using parcel installation, program information looks like this:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>and <ph id="ph1">`/opt/cloudera/parcels/MRS-9.0.1`</ph> (applies to 9.0.1)</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>and <ph id="ph1">`/opt/cloudera/parcels/MRS-8.0.5`</ph> (applies to 8.0.5)</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>and <ph id="ph1">`/opt/cloudera/parcels/MRS-8.0.0-1`</ph> (applies to 8.0)</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>General instructions for all versions</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Packages are registered in a database that tracks all package installations in the cluster.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>To update the database, use a package manager to remove the package: <bpt id="p1">**</bpt>yum<ept id="p1">**</ept> for Red Hat and CentOS, <bpt id="p2">**</bpt>apt<ept id="p2">**</ept> for Ubuntu, or <bpt id="p3">**</bpt>zypper<ept id="p3">**</ept> for SUSE.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Log in as root or a user with <ph id="ph1">`sudo`</ph> privileges.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If you are using <ph id="ph1">`sudo`</ph>, precede commands requiring root privileges with <ph id="ph2">`sudo`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The Revo64 program runs on demand so stopping and disabling the server is not required.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>How to uninstall 9.x</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Uninstall Microsoft R Open (MRO) and remove any dependent packages used only by MRO:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>On RHEL:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>On Ubuntu:</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>On SUSE:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Most packages are uninstalled, including Microsoft R Server.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>List the remaining packages to see what's left.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>On a 9.1.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>installation, you should see only those packages used for operationalizing R Server analytics.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>On a 9.0.1 install, you might see just mrsdeploy.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Using the syntax from the previous step, uninstall remaining packages.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>For 9.1, uninstall packages in the following order:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Microsoft-r-server-adminutil-9.1.x86_64</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Microsoft-r-server-webnode-9.1.x86_64</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Microsoft-r-server-computenode-9.1.x86_64</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Microsoft-r-server-config-rserve-9.1.x86_64</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>After packages are removed, you can remove remaining files.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>On the root node, verify the location of other files that need to be removed:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Remove the entire directory:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>RM removes the folder.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Parameter "f" is for force and "r" for recursive, deleting everything under microsoft-r.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>This command is destructive and irrevocable, so be sure you have the correct directory before you press Enter.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>How to uninstall 8.0.5</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Uninstall Microsoft R Open (MRO) and remove any dependent packages used only by MRO:</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>On the root node, verify the location of other files that need to be removed: `</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Remove the entire directory:</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>RM removes the folder.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Parameter "f" is for force and "r" for recursive, deleting everything under microsoft-r.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>This command is destructive and irrevocable, so be sure you have the correct directory before you press Enter.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>How to uninstall 8.0.0</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Uninstall the Microsoft R Open for Microsoft R Server (MRO-for-MRS) package:</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Remove directories of MRS and MRO, in this order:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Remove symlinks:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>How to uninstall individual packages</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>If you remove Microsoft R Open (microsoft-r-server-mro-8.0-8.0.5-1.x86_64), you will also remove any dependent packages used only by R Open.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Uninstall order is important.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Due to package dependencies, be sure to remove the packages in the order given below.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Install R on Hadoop overview</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Install R Server 8.0.5 on Hadoop</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Microsoft R Server on Linux<ept id="p1">](r-server-install-linux-server.md)</ept> <bpt id="p2">[</bpt>Troubleshoot R Server installation problems on Hadoop<ept id="p2">](r-server-install-hadoop-troubleshoot.md)</ept></source>
        </trans-unit></group></body></file></xliff>