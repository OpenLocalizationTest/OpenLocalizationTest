<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="machine-learning-server-linux-uninstall.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b49baee03cf403c01666b8b1bb0ed135ffb5103ada.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9baee03cf403c01666b8b1bb0ed135ffb5103ada</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\machine-learning-server-linux-uninstall.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Uninstall Machine Learning Server for Linux</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to uninstall Machine Learning Server for Linux.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Uninstall Machine Learning Server for Linux</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Machine Learning Server 9.2.1 | 9.3<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>This article explains how to uninstall Machine Learning Server for Linux.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>For upgrade purposes, uninstall is not necessary unless the existing version is 8.x.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Upgrading from 9.x is an in-place upgrade that overwrites the previous version.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Upgrading from 8.x requires that you uninstall R Server 8.x first.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Gather information</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Uninstall reverses the installation steps, including uninstalling any package dependencies used only by the server.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Start by collecting information about your installation.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>List the packages from Microsoft.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>On RHEL: <ph id="ph1">`yum list \*microsoft\*`</ph></source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>On Ubuntu: <ph id="ph1">`apt list --installed | grep microsoft`</ph></source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>On SUSE: <ph id="ph1">`zypper search \*microsoft-r\*`</ph></source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Get package version information.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>On a 9.3.0 installation, you should see about <bpt id="p1">[</bpt>17 packages<ept id="p1">](#installed-packages)</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Since multiple major versions can coexist, the package list could be much longer.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Given a list of packages, you can get verbose version information for particular packages in the list.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The following examples are for Microsoft R Open version 3.4.3:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>On RHEL: <ph id="ph1">`rpm -qi microsoft-r-open-mro-3.4.3`</ph></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>On Ubuntu: <ph id="ph1">`dpkg --status microsoft-r-open-mro-3.4.3`</ph></source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>On SUSE: <ph id="ph1">`zypper info microsoft-r-open-mro-3.4.3`</ph></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Uninstall 9.3.0</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>On root@, uninstall Microsoft R Open (MRO) first.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>This action removes any dependent packages used only by MRO, which includes packages like microsoft-mlserver-packages-r.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>On RHEL: <ph id="ph1">`yum erase microsoft-r-open-mro-3.4.3`</ph></source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>On Ubuntu: <ph id="ph1">`apt-get purge microsoft-r-open-mro-3.4.3`</ph></source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>On SUSE: <ph id="ph1">`zypper remove microsoft-r-open-mro-3.4.3`</ph></source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Remove the Machine Learning Server Python packages:</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>On RHEL: <ph id="ph1">`yum erase microsoft-mlserver-python-9.3.0`</ph></source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>On Ubuntu: <ph id="ph1">`apt-get purge microsoft-mlserver-python-9.3.0`</ph></source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>On SUSE: <ph id="ph1">`zypper remove microsoft-mlserver-python-9.3.0`</ph></source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Remove the Hadoop package:</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>On RHEL: <ph id="ph1">`yum erase microsoft-mlserver-hadoop-9.3.0`</ph></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>On Ubuntu: <ph id="ph1">`apt-get purge microsoft-mlserver-hadoop-9.3.0`</ph></source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>On SUSE: <ph id="ph1">`zypper remove microsoft-mlserver-hadoop-9.3.0`</ph></source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>You have additional packages if you installed the operationalization feature.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>On a 9.3.0 installation, this is the <bpt id="p1">[</bpt>azureml-model-management library<ept id="p1">](../python-reference/azureml-model-management-sdk/azureml-model-management-sdk.md)</ept> or <bpt id="p2">[</bpt>mrsdeploy<ept id="p2">](../r-reference/mrsdeploy/mrsdeploy-package.md)</ept>, which you can uninstall using the syntax from the previous step.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Multiple packages provide the feature.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Uninstall each one in the following order:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>microsoft-mlserver-adminutil-9.3</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>microsoft-mlserver-webnode-9.3</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>microsoft-mlserver-computenode-9.3</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Re-list the packages from Microsoft to check for remaining files:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>On RHEL: <ph id="ph1">`yum list \*microsoft\*`</ph></source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>On Ubuntu: <ph id="ph1">`apt list --installed | grep microsoft`</ph></source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>On SUSE: <ph id="ph1">`zypper search \*microsoft-r\*`</ph></source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>On Ubuntu, you have <ph id="ph1">`dotnet-runtime-2.0.0`</ph>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>NET Core<ept id="p1">](https://docs.microsoft.com/dotnet/core/index)</ept> is a cross-platform, general purpose development platform maintained by Microsoft and the .NET community on GitHub.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>This package could be providing infrastructure to other applications on your computer.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If Machine learning Server is the only Microsoft software you have, you can remove it now.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>After packages are uninstalled, remove remaining files.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>On root@, determine whether additional files still exist:</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Remove the entire directory:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>RM removes the folder.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Parameter "f" is for force and "r" for recursive, deleting everything under microsoft/mlserver.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>This command is destructive and irrevocable, so be sure you have the correct directory before you press Enter.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Package list</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Machine Learning Server for Linux adds the following packages at a minimum.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>When uninstalling software, refer to this list when searching for packages to remove.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Machine Learning Server<ept id="p1">](r-server-install.md)</ept></source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Supported platforms<ept id="p1">](r-server-install-supported-platforms.md)</ept></source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Known Issues<ept id="p1">](../resources-known-issues.md)</ept></source>
        </trans-unit></group></body></file></xliff>