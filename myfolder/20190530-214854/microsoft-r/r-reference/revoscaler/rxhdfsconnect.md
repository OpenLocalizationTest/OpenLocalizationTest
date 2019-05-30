<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxhdfsconnect.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e9440363f6ff8ab5b0f3cab8a7c417bb38885cd7d.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9440363f6ff8ab5b0f3cab8a7c417bb38885cd7d</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxhdfsconnect.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxHdfsConnect function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Establishes a connection from RevoScaleR to the Hadoop Distributed File System (HDFS).</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxHdfsConnect, file, connection</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxHdfsConnect:  Establish a Connection to the Hadoop Distributed File System</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Establishes a connection from RevoScaleR to the Hadoop Distributed File System (HDFS).</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>character string specifying the host name of your Hadoop name node.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>integer scalar specifying the port number of your Hadoop name node.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If you accept the install time option to specify a default HDFS connection, you are prompted for a host name and port number for your Hadoop name node, which are stored as environment variables <ph id="ph1">`REVOHADOOPHOST`</ph> and <ph id="ph2">`REVOHADOOPPORT`</ph>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If these environment variables are set, this function is called by Rprofile.site on startup.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>After establishing the connection, this function sets the <ph id="ph1">`rxOptions`</ph> for <ph id="ph2">`hdfsHost`</ph> and <ph id="ph3">`hdfsPort`</ph>, and subsequent calls to <ph id="ph4">`RxHdfsFileSystem`</ph> should be done using the default values of <ph id="ph5">`hostName`</ph> and <ph id="ph6">`port`</ph>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>It is important that this function be called before any functions that call into <bpt id="p1">**</bpt>rJava<ept id="p1">**</ept>, in particular before initializing <bpt id="p2">**</bpt>rhdfs<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>invisibly, the return value of <ph id="ph1">`rxOptions`</ph>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxOptions<ept id="p1">](rxOptions.md)</ept>,</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>