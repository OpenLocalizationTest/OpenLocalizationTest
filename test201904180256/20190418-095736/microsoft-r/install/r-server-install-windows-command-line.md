<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-windows-command-line.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c6b91e76c4dcedce03e2d36e402ae6277e9615a6e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">6b91e76c4dcedce03e2d36e402ae6277e9615a6e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-windows-command-line.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Command line install of R Server 9.1 for Windows</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Run unattended or scripted setup of R Server 9.1 on a Windows operating system</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Command-line install of R Server 9.1 for Windows</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>This article provides syntax and examples for running RServerSetup.exe from the command line.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>You can use command-line parameters for an internet-connected or offline installation.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>A command-line installation requires administrator permissions.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Before you start, review the following articles for system requirements, prerequisites, download links, and steps:</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install R Server 9.1. on Windows<ept id="p1">](r-server-install-windows.md)</ept> for an internet-connected installation.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Offline installation<ept id="p1">](r-server-install-windows-offline.md)</ept> for a machine with no internet access.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Command-line options</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>You can run RServerSetup.exe from the command line with options to expose or hide the wizard, set an install mode, or specify options for adding features or using custom folder locations.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>User Interaction Options<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Parameter</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Invokes the wizard.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Hides the wizard, running a silent installation with no interaction or prompts.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>EULA acceptance is automatic for both MRS and MRO.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Equivalent to <ph id="ph1">`/quiet`</ph> in this release.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Install Modes<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Parameter</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Runs RServerSetup.exe in install mode, used to add R Server or the <bpt id="p1">[</bpt>pre-trained machine learning models<ept id="p1">](microsoftml-install-pretrained-models.md)</ept></source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Removes an existing installation of R Server.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Runs RServerSetup.exe in modify mode.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Setup looks for an existing installation of R Server 9.1 and gives you options for changing an installation (for example, you could add the pre-trained models, or uninstall the server).</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Use this option if you want to rerun (or repair) an installation.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Install Options<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Parameter</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Instructs setup to find .cab files on the local system in the <ph id="ph1">`mediadir`</ph> location.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>In this release, two .cab files are required: SRO_3.3.3.0_1033.cab for MRO, and MLM_9.1.0.0_1033.cab for the machine learning models.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Specifies the installation directory.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>By default, this is C:\Program Files\Microsoft\R Server\R_SERVER.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>A download location for the .cab files.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>By default, setup uses <ph id="ph1">`%temp%`</ph> for the local admin user.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Assuming an online installation scenario, you can set this parameter to have setup download the .cabs to the folder you specify.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The .cab file location setup uses to find .cab files in an offline installation.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>By default, setup uses <ph id="ph1">`%temp%`</ph> for local admin.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Adds the <bpt id="p1">[</bpt>pre-trained machine learning models<ept id="p1">](microsoftml-install-pretrained-models.md)</ept>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Use with <ph id="ph1">`/install`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Default installation</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The default installation adds Microsoft R Server (MRS) and its required components: Microsoft R Open (MRO) and .NET Core used for operationalizing analytics and machine learning.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The command-line equivalent of a double-click invocation of RServerSetup.exe is <ph id="ph1">`rserversetup.exe /install /full`</ph>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>A default installation includes the MicrosoftML package, but not the pre-trained models.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>You must explicitly add <ph id="ph1">`/models`</ph> to an installation to add this feature.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Run setup in unattended mode with no prompts or user interaction to install all features, including the pre-trained models.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Add the pre-trained machine learning models to an existing installation.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The pre-trained models are inserted into the MicrosoftML package.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Once installed, you cannot incrementally remove them.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Removal will require uninstall and reinstall of R Server.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Uninstall the software in unattended mode.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Offline install requires two .cab files that provide MRO and other dependencies.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`/offline`</ph> parameter instructs setup to look for the .cab files on the local system.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>By default, setup looks for the .cab files in the <ph id="ph1">`%temp%`</ph> directory of local admin, but you could also set the media directory if the .cab files are in a different folder.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>For more information and .cab download links, see <bpt id="p1">[</bpt>Offline installation<ept id="p1">](r-server-install-windows-offline.md)</ept>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Introduction to R Server<ept id="p1">](../what-is-microsoft-r-server.md)</ept> <bpt id="p2">[</bpt>What's New in R Server<ept id="p2">](../whats-new-in-r-server.md)</ept> <bpt id="p3">[</bpt>Supported platforms<ept id="p3">](r-server-install-supported-platforms.md)</ept></source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Known Issues<ept id="p1">](../resources-known-issues.md)</ept></source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Microsoft R Getting Started Guide<ept id="p1">](../microsoft-r-getting-started.md)</ept><ph id="ph1">  </ph></source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure R Server to operationalize your analytics<ept id="p1">](operationalize-r-server-one-box-config.md)</ept></source>
        </trans-unit></group></body></file></xliff>