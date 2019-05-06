<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-developer-manage-threads.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc775030209c83085dc65c525727512e783ba6f33bb5c9.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">30209c83085dc65c525727512e783ba6f33bb5c9</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-developer-manage-threads.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Manage threads in RevoScaleR (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How ScaleR establishes and manages thread pools for parallel processing.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Managing threads in RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RevoScaleR provides functions for managing the thread pool used for parallel execution.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>On Windows, thread pool management is enabled and should not be turned off.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>On Linux, thread pool management is turned off by default to avoid interfering with how Unix systems fork processes.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Process forking is only available on Unix-based systems.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>You can turn the thread pool on if you do not fork your R process.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>RevoScaleR provides an interface to activate the thread pool:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Similarly, the thread pool may be disabled as follows:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If you want to ensure that the RevoScaleR thread pool is always enabled on Linux, you can add the preceding command to a <bpt id="p1">*</bpt>.First<ept id="p1">*</ept> function defined in either your own Rprofile startup file, or the system Rprofile.site file.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>For example, you can add the following lines after the closing right parenthesis of the existing Rprofile.site file:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>.First.sys<ept id="p1">*</ept> function is normally run after all other initialization is complete, including the evaluation of the <bpt id="p2">*</bpt>.First<ept id="p2">*</ept> function.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>We need the call to <bpt id="p1">*</bpt>rxSetEnableThreadPool<ept id="p1">*</ept> to occur after RevoScaleR is loaded.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>That is done by <bpt id="p1">*</bpt>.First.sys<ept id="p1">*</ept>, so we call <bpt id="p2">*</bpt>.First.sys<ept id="p2">*</ept> first.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Machine Learning Server</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>How-to guides in Machine Learning Server</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>RevoScaleR Functions</source>
        </trans-unit></group></body></file></xliff>