<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="install-uninstall.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86203c0f81b45a70ba7dda9d02afa9558555d498d8.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">203c0f81b45a70ba7dda9d02afa9558555d498d8</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-client\install-uninstall.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Uninstall Microsoft R Client to upgrade to a newer version - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Explains how to uninstall Microsoft R Client.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>You do not have to uninstall R Client before installing a more recent version.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Client, Microsoft R Client, remove, uninstall, uninstallation</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Uninstall Microsoft R Client</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This article explains how to uninstall Microsoft R Client.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>You do not have to uninstall R Client before installing a more recent version.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Uninstall on Windows</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Remove Microsoft R Client like other applications using the Add/Remove dialog on Windows.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Alternately, you can use the same setup file used to install R Client to remove the program by specifying the /uninstall option on the command line such as: <ph id="ph1">```RClientSetup.exe /uninstall```</ph></source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Uninstall on Linux</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Program version and file locations</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>As a first step, use your package manager to list the currently installed Machine Learning Server packages.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>(Typically, CentOS and Red Hat systems use <bpt id="p1">**</bpt>yum<ept id="p1">**</ept>, Ubuntu systems use <bpt id="p2">**</bpt>apt-get<ept id="p2">**</ept>, and SLES systems use <bpt id="p3">**</bpt>zypper<ept id="p3">**</ept>):</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If your package manager is <bpt id="p1">**</bpt>yum<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If your package manager is <bpt id="p1">**</bpt>apt-get<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If your package manager is <bpt id="p1">**</bpt>zypper<ept id="p1">**</ept>:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>General instructions for all versions</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Packages are registered in a database that tracks all package installations in the cluster.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>To update the database, use a package manager to remove the package: <bpt id="p1">**</bpt>yum<ept id="p1">**</ept> for Red Hat and CentOS, <bpt id="p2">**</bpt>zypper<ept id="p2">**</ept> for SUSE, or <bpt id="p3">**</bpt>apt-get<ept id="p3">**</ept> for Ubuntu.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Log in as root or a user with <ph id="ph1">`sudo`</ph> privileges.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If you are using <ph id="ph1">`sudo`</ph>, precede commands requiring root privileges with <ph id="ph2">`sudo`</ph> (for example, <ph id="ph3">`sudo yum erase microsoft-r-server-mro-8.0`</ph>).</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>How to uninstall</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Uninstall Microsoft R Open (MRO) and remove any dependent packages used only by MRO:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>where x.x is the version number.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>On the root node, verify the location of other files that need to be removed: `</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Remove the entire directory:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>rm<ept id="p1">**</ept> command removes the folder.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Parameter "f" is for force and "r" for recursive, deleting everything under microsoft-r.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>This command is destructive and irrevocable, so be sure you have the correct directory before you press Enter.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Learn More</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>You can learn more with these guides:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Overview of Microsoft R Client</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Quickstart: Running R code in Microsoft R<ept id="p1">](../r/quickstart-run-r-code.md)</ept> (example)</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>How-to guides in Machine Learning Server</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>RevoScaleR R package reference</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>MicrosoftML R package reference</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>mrsdeploy R package reference</source>
        </trans-unit></group></body></file></xliff>