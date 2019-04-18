<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxhadoopcommand.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18cbad06ed337bcde8dbf2709599f6891936e146ff8.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">bad06ed337bcde8dbf2709599f6891936e146ff8</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxhadoopcommand.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxHadoopCommand function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Execute arbitrary Hadoop commands and perform standard file operations in Hadoop.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxHadoopCommand, rxHadoopCopy, rxHadoopCopyFromLocal, rxHadoopCopyFromClient, rxHadoopCopyToLocal, rxHadoopFileExists, rxHadoopListFiles, rxHadoopMakeDir, rxHadoopMove, rxHadoopRemove, rxHadoopRemoveDir, rxHadoopVersion, file</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxHadoopCommand:  Execute Hadoop Commands</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Execute arbitrary Hadoop commands and perform standard file operations in Hadoop.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A character string containing a valid Hadoop command, that is, the <ph id="ph1">`cmd`</ph> portion of <ph id="ph2">`hadoop cmd`</ph>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Embedded quotes are not permitted.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Run against this compute context.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Default to the current compute context as returned by <bpt id="p1">[</bpt>rxGetComputeContext<ept id="p1">](rxSetComputeContext.md)</ept> .</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>character string specifying the username for making an ssh connection to the Hadoop cluster.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>character string specifying the hostname or IP address of the Hadoop cluster node or edge node that the client will log into for launching Hadoop commands.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>character string specifying any switches needed for making an ssh connection to the Hadoop cluster.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Optional character string specifying the absolute path to a profile script that will exist on the <ph id="ph1">`sshHostname`</ph> host.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>This is used when the target ssh host does not automatically read in a <ph id="ph1">`.bash_profile`</ph>, <ph id="ph2">`.profile`</ph> or other shell environment configuration file for the definition of requisite variables.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>logical (not <ph id="ph1">`NA`</ph>) specifying whether to capture the output of a Hadoop command as an R character vector in a local compute context.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>(When using the <ph id="ph1">`RxHadoopMR`</ph> compute context, any output is always returned as an R character vector.)</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>character vector specifying file(s) to be copied or moved.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>character string specifying the destination of a copy or move.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`source`</ph> includes more than one file, <ph id="ph2">`dest`</ph> must be a directory.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>character string specifying a directory in the Hadoop cluster's native file system, to be used as an intermediate location for file(s) copied from a client machine.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>character string specifying a directory in the Hadoop Distributed File System.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>character vector specifying location of one or more files or directories.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Deprecation Warning: the <ph id="ph1">`print`</ph> argument in <ph id="ph2">`rxHadoopListFiles`</ph> is now deprecated and is going to be removed in the next release.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, <ph id="ph2">`rxHadoopListFiles`</ph> will return a <ph id="ph3">`character`</ph> vector of paths; by default it prints paths to the console.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, directory listings are recursive.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, removal via <ph id="ph2">`rxHadoopRemove`</ph> and <ph id="ph3">`rxHadoopRemoveDir`</ph> bypasses the trash folder, if one has been set up.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the <ph id="ph1">`rxHadoopCommand`</ph> function.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxHadoopCommand`</ph> allows you to run basic Hadoop commands.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxCopyFromClient`</ph> allows a file to be copied from a remote client to the Hadoop Distributed File System on the Hadoop cluster.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxHadoopVersion`</ph> calls the Hadoop <ph id="ph2">`version`</ph> command and extracts and returns the version number only.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The remaining functions are wrappers for various Hadoop file system commands:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxHadoopCopyFromLocal`</ph> wraps the Hadoop <ph id="ph2">`fs -copyFromLocal`</ph> command.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxHadoopCopyToLocal`</ph> wraps the Hadoop <ph id="ph2">`fs -copyToLocal`</ph> command.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxHadoopListFiles`</ph> wraps the Hadoop <ph id="ph2">`fs -ls`</ph> or <ph id="ph3">`fs -lsr`</ph> command.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxHadoopRemove`</ph> wraps the Hadoop <ph id="ph2">`fs -rm`</ph> command.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxHadoopCopy`</ph> wraps the Hadoop <ph id="ph2">`fs -cp`</ph> command.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxHadoopMove`</ph> wraps the Hadoop <ph id="ph2">`fs -mv`</ph> command.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxHadoopMakeDir`</ph> wraps the Hadoop <ph id="ph2">`fs -mkdir`</ph> command.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxHadoopRemoveDir`</ph> wraps the Hadoop <ph id="ph2">`fs -rm -r`</ph> command.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>These functions are executed for their side effects and typically return <ph id="ph1">`NULL`</ph> invisibly.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>RxHadoopMR.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>