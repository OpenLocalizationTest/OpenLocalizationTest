<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="machine-learning-server-windows-uninstall.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca867cfc0c42314ce58ddef7083cd05f6fc9c8ab6dd6.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">7cfc0c42314ce58ddef7083cd05f6fc9c8ab6dd6</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\machine-learning-server-windows-uninstall.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Uninstall Machine Learning Server for Windows</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to uninstall Machine Learning Server for Windows.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Uninstall Machine Learning Server for Windows</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies to:  Machine Learning Server 9.2.1 | 9.3</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>You can re-run the Windows installer to remove Machine Learning Server for Windows.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Clearing the checkbox for an option in the Configuration page removes that component from your computer.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Redistributable components, such as the Analysis Services OLE DB provider, are not removed because doing so might break other applications using those components.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>If you have ServerSetup.exe in the Downloads folder, double-click the file to start it.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Clear the options.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Install<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>You can also use <bpt id="p1">**</bpt>Add and Remove programs<ept id="p1">**</ept> in Windows to uninstall the software.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Manual uninstall</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If Setup fails to install all of the components, you can run a VB Script that forces uninstall and cleans up residual components.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Run a script that produces a list of all installed products and saves it in a log.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Review log output for Microsoft Machine Learning Server, Microsoft R Server, or Microsoft R Client.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>For either product, find the value for <ph id="ph1">`LocalPackage`</ph>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Run the package at an elevated command prompt with this syntax: <ph id="ph1">`Msiexec /x {LocalPackage.msi} /L*v uninstall.log`</ph>, where local package is the value from the previous step.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Review the uninstall log to confirm the software was removed.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>You can repeat steps 1 and 2 for further verification.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If the script contains no evidence of the program, but the program folder still exists, you can safely delete it.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Program files are located at <ph id="ph1">`\Program Files\Microsoft`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>VBScript listing installers for all installed products</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Copy the following script and save it as <bpt id="p1">**</bpt>msi_lister.vbs<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Install Machine Learning Server</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>What's new in Machine Learning Server</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Supported platforms</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Known Issues</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Configure Machine Learning Server to operationalize your analytics</source>
        </trans-unit></group></body></file></xliff>