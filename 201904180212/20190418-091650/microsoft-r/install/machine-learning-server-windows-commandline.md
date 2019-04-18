<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="machine-learning-server-windows-commandline.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b453e2d856713e4454849467a9ae62001d17285c97.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">53e2d856713e4454849467a9ae62001d17285c97</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\machine-learning-server-windows-commandline.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Windows command line installation for Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to install Machine Learning Server for Windows on the command line.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Command-line install for Machine Learning Server for Windows</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:  Machine Learning Server 9.2.1 | 9.3<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>This article provides syntax and examples for running Machine Learning Server <bpt id="p1">**</bpt>ServerSetup.exe<ept id="p1">**</ept> from the command line.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>You can use command-line parameters for an internet-connected or offline installation.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>A command-line installation requires administrator permissions.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Before you start, review  <bpt id="p1">[</bpt>Install Machine Learning Server on Windows<ept id="p1">](machine-learning-server-windows-install.md)</ept> for:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>System and operational requirements</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Download and file extraction information</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>A summary of what is installed</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Steps for validating your installation</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>This article assumes you have already downloaded and extracted the setup program.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Command-line options</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>You can run ServerSetup.exe from the command line with options to expose or hide the wizard, set an install mode, or specify options for adding features or using custom folder locations.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>User Interaction Options<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Parameter</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Invokes the wizard.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Hides the wizard, running a silent installation with no interaction or prompts.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>EULA acceptance is automatic for both the server and all open-source distributions of R and Python.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Equivalent to <ph id="ph1">`/quiet`</ph> in this release.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Install Modes<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Parameter</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Runs ServerSetup.exe in install mode, used to add R_SERVER, PYTHON_SERVER, or the <bpt id="p1">[</bpt>pre-trained machine learning models<ept id="p1">](microsoftml-install-pretrained-models.md)</ept></source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Removes an existing installation of any component previously installed.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Runs ServerSetup.exe in modify mode.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Setup looks for an existing installation and offers options for changing an installation (for example, you could add the pre-trained models).</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Use this option if you want to rerun (or repair) an installation.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Install Options<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Parameter</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Install just the R feature.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Use with <ph id="ph1">`/install`</ph>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Applies to version 9.3 only.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Install just the Python feature.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Use with <ph id="ph1">`/install`</ph>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Applies to version 9.3 only.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Instructs setup to find <bpt id="p1">[</bpt>.cab files<ept id="p1">](#cab-files)</ept> on the local system in the <ph id="ph1">`mediadir`</ph> location.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>This option requires that the server is disconnected from the internet.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Specifies the installation directory.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>By default, this is C:\Program Files\Microsoft\R Server\R_SERVER.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>A download location for the .cab files.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>By default, setup uses <ph id="ph1">`%temp%`</ph> for the local admin user.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Assuming an online installation scenario, you can set this parameter to have setup download the .cabs to the folder you specify.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The .cab file location setup uses to find .cab files in an offline installation.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>By default, setup uses <ph id="ph1">`%temp%`</ph> for local admin.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Adds the <bpt id="p1">[</bpt>pre-trained machine learning models<ept id="p1">](microsoftml-install-pretrained-models.md)</ept>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Use with <ph id="ph1">`/install`</ph>.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Default installation</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>A default installation includes R and Python, but not the pre-trained models.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>You must explicitly add <ph id="ph1">`/models`</ph> to an installation to add this feature.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The command-line equivalent of a double-click invocation of ServerSetup.exe is <ph id="ph1">`serversetup.exe /install /full`</ph>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Run setup in unattended mode with no prompts or user interaction, to install everything.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>For version 9.2.1, both R Server and Python Server are included in every installation; the pre-trained models are optional and have to be explicitly specified to include them in the installation.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>For version 9.3 only, you can set flags to install individual components: R, Python, pre-trained models:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Add the <bpt id="p1">[</bpt>pre-trained machine learning models<ept id="p1">](microsoftml-install-pretrained-models.md)</ept> to an existing installation.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>You cannot install them as a standalone component.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The models require R or Python.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>During installation, the pre-trained models are inserted into the MicrosoftML (R) and microsoftml (Python) libraries, or both if you add both languages.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Once installed, you cannot incrementally remove them.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Removal will require uninstall and reinstall of Python or R Server.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Uninstall the software in unattended mode.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Unattended offline install requires .cab files that provide open-source distributions and other dependencies.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`/offline`</ph> parameter instructs setup to look for the .cab files on the local system.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>By default, setup looks for the .cab files in the <ph id="ph1">`%temp%`</ph> directory of local admin, but you could also set the media directory if the .cab files are in a different folder.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>For more information and .cab download links, see <bpt id="p1">[</bpt>Offline installation<ept id="p1">](machine-learning-server-windows-offline.md)</ept>.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>9.3 CAB file list</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>For unattended setup or offline setup, copy the .cab files to either the setup user's temp directory (<bpt id="p1">**</bpt>C:\Users<ph id="ph1">\&lt;</ph>user-name&gt;\AppData\Local\Temp<ept id="p1">**</ept>) or to a folder specified via the <ph id="ph2">`/mediadir`</ph> flag.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Component</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Download</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Used for</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>MLM</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>MLM_9.3.0.0_1033.cab<ept id="p1">](https://go.microsoft.com/fwlink/?LinkId=859053&amp;clcid=1033)</ept></source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Pre-trained models, R or Python</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Microsoft R Open</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SRO_3.4.3.0_1033.cab<ept id="p1">](https://go.microsoft.com/fwlink/?LinkId=867186&amp;clcid=1033)</ept></source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>R</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Microsoft Python Open</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SPO_9.3.0.0_1033.cab<ept id="p1">](https://go.microsoft.com/fwlink/?LinkId=859054&amp;clcid=1033)</ept></source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Python</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>There is no separate Python Server package in the 9.3 version.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>9.2.1 CAB file list</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>For unattended setup or offline setup, copy the .cab files to either the setup user's temp directory (<bpt id="p1">**</bpt>C:\Users<ph id="ph1">\&lt;</ph>user-name&gt;\AppData\Local\Temp<ept id="p1">**</ept>) or to a folder specified via the <ph id="ph2">`/mediadir`</ph> flag.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Component</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Download</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Used for</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>MLM</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>MLM_9.2.1.0_1033.cab<ept id="p1">](https://go.microsoft.com/fwlink/?LinkId=852727&amp;clcid=1033)</ept></source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Pre-trained models, R or Python</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Microsoft R Open</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SRO_3.4.1.0_1033.cab<ept id="p1">](https://go.microsoft.com/fwlink/?LinkId=852724&amp;clcid=1033)</ept></source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>R</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Microsoft Python Open</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SPO_9.2.1.0_1033.cab<ept id="p1">](https://go.microsoft.com/fwlink/?LinkId=852723&amp;clcid=1033)</ept></source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Python</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Microsoft Python Server</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SPS_9.2.1.0_1033.cab<ept id="p1">](https://go.microsoft.com/fwlink/?LinkId=852726&amp;clcid=1033)</ept></source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Python</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>We recommend continuing with any Quickstart tutorial listed in the contents pane.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Machine Learning Server<ept id="p1">](r-server-install.md)</ept></source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>What's new in Machine Learning Server<ept id="p1">](../whats-new-in-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Supported platforms<ept id="p1">](r-server-install-supported-platforms.md)</ept></source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Known Issues<ept id="p1">](../resources-known-issues.md)</ept></source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Configure Machine Learning Server to operationalize your analytics<ept id="p1">](../what-is-operationalization.md)</ept></source>
        </trans-unit></group></body></file></xliff>