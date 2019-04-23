<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="resources-opting-out.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86d709cd1deeb0d32494063f0da76f9fc9d3a169cc.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d709cd1deeb0d32494063f0da76f9fc9d3a169cc</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\resources-opting-out.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Opting out of usage data collection - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn how to turn off telemetry data collection on Machine Learning Server, Microsoft R Server and R Client using the rxPrivacyControl function in RevoScaleR or rx-privacy-control function in revoscalepy.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Opting out of usage data collection</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:<ept id="p1">**</ept> Machine Learning Server, Microsoft R Server 9.x</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>By default, telemetry data is collected during your usage of Machine Learning Server, Microsoft R Server, and R Client for the purpose of improving products and services.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Anonymous usage data includes device information, operating system version, regional and language settings, and errors reports.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Please see the <bpt id="p1">[</bpt>Microsoft privacy statement<ept id="p1">](https://privacy.microsoft.com/privacystatement)</ept> for a detailed explanation.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>To turn data collection on or off, use <bpt id="p1">[</bpt>rxPrivacyControl<ept id="p1">](r-reference/revoscaler/rxprivacycontrol.md)</ept> from <bpt id="p2">[</bpt>RevoScaleR<ept id="p2">](r-reference/revoscaler/revoscaler.md)</ept> on any platform, or <bpt id="p3">[</bpt>rx_privacy_control<ept id="p3">](python-reference/revoscalepy/rx-privacy-control.md)</ept> from <bpt id="p4">[</bpt>revoscalepy<ept id="p4">](python-reference/revoscalepy/revoscalepy-package.md)</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Version Requirements</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Privacy controls are in newer versions of the server.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>To verify server version is 9.x or later (or 3.4.x for R Client), open an R IDE, such the R Console (RGui.exe).</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The console app reports server version information for Microsoft R Open, R Client, and R Server.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>From the console, you can use the <ph id="ph1">`print`</ph> command to return verbose version information:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Permission Requirements</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Opting out of telemetry requires administrator rights.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The instructions below explain how to run console applications as an administrator.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>As an administrator, running the R command <ph id="ph1">`rxPrivacyControl(TRUE)`</ph> will permanently change the setting to TRUE, and <ph id="ph2">`rxPrivacyControl(FALSE)`</ph> will permanently change the setting to FALSE.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>There is no user-facing way to change the setting for a single session.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Without a parameter, running <ph id="ph1">`rxPrivacyControl()`</ph> returns the current setting.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Similarly, if you are not an administrator, <ph id="ph1">`rxPrivacyControl()`</ph> returns just the current setting.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>How to opt out (Python)</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The revoscalepy package providing <ph id="ph1">`rx-privacy-control`</ph> is installed when you add Python support to Machine Learning Server:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Log on as root:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Start a Python session:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Load the library:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Return the current value:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Change the current value:<ph id="ph1">`revoscalepy.rx_privacy_control(TRUE)`</ph> to turn on telemetry data collection.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Otherwise, set it to FALSE.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>How to opt out (R)</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The RevoScaleR package provides<ph id="ph1">`rxPrivacyControl`</ph> is installed and loaded in both R Client and R Server.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>To turn off telemetry data collection, you can use the built-in R console application, which loads RevoScaleR automatically.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>On Linux</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Log on as root:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Start an R session:</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Return the current value:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Change the current value:<ph id="ph1">`rxPrivacyControl(TRUE)`</ph> to turn on telemetry data collection.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Otherwise, set it to FALSE.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>On Windows</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Log in to the computer as an administrator.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Go to C:\Program Files\Microsoft\ML Server\R_SERVER\bin\x64.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Right-click Rgui.exe and select <bpt id="p1">**</bpt>Run as administrator<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`rxPrivacyControl`</ph> to return the current value.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Type <ph id="ph1">`rxPrivacyControl(FALSE)`</ph>to turn off telemetry data collection.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The  <ph id="ph1">`rxPrivacyControl`</ph> command sets the state to be opted-in or out for anonymous usage collection.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Command syntax</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>This command takes one parameter, <ph id="ph1">`optIn`</ph>, set to either ‘TRUE’ or ‘FALSE’ to opt out. Left unspecified, the current setting is returned.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>How to Contact Us</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Please contact Microsoft if you have any questions or concerns.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>For general privacy question or a question for the Chief Privacy Officer of Microsoft or want to request access to your personal information, please contact us by using our <bpt id="p1">[</bpt>Web form<ept id="p1">](https://go.microsoft.com/fwlink/?LinkId=321116)</ept>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>For technical or general support question, please visit <bpt id="p1">[</bpt><ph id="ph1">https://support.microsoft.com/</ph><ept id="p1">](https://support.microsoft.com/)</ept> to learn more about Microsoft Support offerings.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If you have a Microsoft account password question, please visit <bpt id="p1">[</bpt>Microsoft account support<ept id="p1">](https://go.microsoft.com/FWLink/p/?LinkID=320207)</ept>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>By mail: Microsoft Privacy, Microsoft Corporation, One Microsoft Way, Redmond, Washington 98052 USA</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>By Phone: 425-882-8080</source>
        </trans-unit></group></body></file></xliff>