<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxhdfsfilesystem.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b44c682f3f50ee386cc3a41aedc540dfa22c73fb5d.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">4c682f3f50ee386cc3a41aedc540dfa22c73fb5d</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxhdfsfilesystem.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxHdfsFileSystem function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This is the main generator for RxHdfsFileSystem S3 class.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), RxHdfsFileSystem, print.RxHdfsFileSystem, file, connection</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>RxHdfsFileSystem: RevoScaleR HDFS File System object generator</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This is the main generator for RxHdfsFileSystem S3 class.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>object of class RxHdfsFileSystem.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>This argument is optional.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If supplied, the values of  the other arguments are used to replace those of <ph id="ph1">`object`</ph> and the modified object is returned.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If these arguments are not supplied, they will take their default values.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>character string specifying name of host for HDFS file system.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>integer specifying port number.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>NOT YET IMPLEMENTED Optional Flag indicating whether this is a HDFS or a WebHdfs interface - default FALSE</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>NOT YET IMPLEMENTED Optional list of OAuth2 parameters created using rxOAuthParameters function  (valid only if useWebHdfs is TRUE) - default NULL</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Optional Flag indicating "verbose" mode for WebHdfs HTTP calls (valid only if useWebHdfs is TRUE) - default FALSE</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>an RxHdfsFileSystem object.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>other arguments are passed to the underlying function.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Writing to the HDFS file system can only be done using a RxHadoopMR compute context with an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> data source.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The 'rxHadoop' commands, such as <bpt id="p1">[</bpt>rxHadoopCopy<ept id="p1">](rxHadoopCommand.md)</ept>, can also be used to manipulate data sets in HDFS.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>An RxHdfsFileSystem file system object.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>This object may be used to in <bpt id="p1">[</bpt>rxSetFileSystem<ept id="p1">](rxSetFileSystem.md)</ept>, <bpt id="p2">[</bpt>rxOptions<ept id="p2">](rxOptions.md)</ept>, <bpt id="p3">[</bpt>RxTextData<ept id="p3">](RxTextData.md)</ept>, or <bpt id="p4">[</bpt>RxXdfData<ept id="p4">](RxXdfData.md)</ept> to set the file system.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RxFileSystem<ept id="p1">](RxFileSystem.md)</ept>, <bpt id="p2">[</bpt>RxNativeFileSystem<ept id="p2">](RxNativeFileSystem.md)</ept>, <bpt id="p3">[</bpt>rxSetFileSystem<ept id="p3">](rxSetFileSystem.md)</ept>, <bpt id="p4">[</bpt>rxOptions<ept id="p4">](rxOptions.md)</ept>, <bpt id="p5">[</bpt>RxXdfData<ept id="p5">](RxXdfData.md)</ept>, <bpt id="p6">[</bpt>RxTextData<ept id="p6">](RxTextData.md)</ept>, <bpt id="p7">[</bpt>rxOAuthParameters<ept id="p7">](rxOAuthParameters.md)</ept>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>