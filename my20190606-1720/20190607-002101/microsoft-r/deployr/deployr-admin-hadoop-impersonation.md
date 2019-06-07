<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-admin-hadoop-impersonation.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37021be588c93a9d9bc3a983d4bfbb483c7b518274.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">021be588c93a9d9bc3a983d4bfbb483c7b518274</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-admin-hadoop-impersonation.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Using Hadoop Impersonation - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>DeployR and Hadoop Impersonation</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Using Hadoop Impersonation and DeployR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Typically when invoking system commands from R, those commands run as the user that started R. In the case of Hadoop, if user <ph id="ph1">`abc`</ph> logs in to a node on a Hadoop cluster and starts R, any <bpt id="p1">*</bpt>system<ept id="p1">*</ept> commands, such as <ph id="ph2">`system("hadoop fs -ls /")`</ph>, run as user <ph id="ph3">`abc`</ph>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>File permissions in HDFS are honored accordingly.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>For example, user <ph id="ph1">`abc`</ph> cannot access files in HDFS if that user does not have proper permissions.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>However when using DeployR, every R session is started as the same user.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>This is an artifact of the Rserve component that was used to create and interact with R sessions.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>In order to work around this circumstance, <bpt id="p1">[</bpt>Hadoop Impersonation<ept id="p1">](https://issues.apache.org/jira/browse/HADOOP-8561)</ept> is used.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Hadoop impersonation is employed by standard Hadoop services like Hue and WebHDFS.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The idea behind impersonation is that R sets an environment variable that tells Hadoop to run commands as a different user than the user who started the R session.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>You can use one of two Hadoop-supported environment variables:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>for non-kerberos secured clusters</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>for clusters secured with Kerberos.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>This document assumes we are working with a Kerberos secured cluster.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The rest of the document focuses on the steps needed to get Hadoop Impersonation to work with DeployR.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Creating the 'rserve' User</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Since the DeployR Rserve component runs by default as the <ph id="ph1">`apache`</ph> user who <bpt id="p1">**</bpt>does not<ept id="p1">**</ept> have a <ph id="ph2">`home`</ph> directory, we recommend that you create a new user that:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Is used when running Rserve</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Has a <ph id="ph1">`home`</ph> directory</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Starts a bash shell</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>In this example, we create the user <ph id="ph1">`rserve`</ph> and change which user used to run Rserve.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Non Root Installation</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If DeployR was installed as non-root, then you must ensure that the user that starts DeployR has a <ph id="ph1">`home`</ph> directory and starts a bash shell.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Nothing else is required.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Root Installation</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If DeployR was installed as user <ph id="ph1">`root`</ph>, do the following:</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Create the Linux user <ph id="ph1">`rserve`</ph>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Go to the directory where DeployR is installed.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Go the <ph id="ph1">`rserve`</ph> subdirectory and open <ph id="ph2">`rserve.sh`</ph> in an editor.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Replace all instances of <ph id="ph1">`apache`</ph> with <ph id="ph2">`rserve`</ph>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>There are two instances of the string <ph id="ph1">`apache`</ph> in the file.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Give full write permissions to directory <ph id="ph1">`workdir`</ph>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Edit <ph id="ph1">`/etc/group`</ph> and add <ph id="ph2">`rserve`</ph> as a member of group <ph id="ph3">`apache`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Restart Rserve.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Setting Up the Environment for the 'rserve' User</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>ScaleR<ept id="p1">**</ept>: If you are using ScaleR inside Hadoop, add the following line to <ph id="ph1">`.bash_profile`</ph> for user <ph id="ph2">`rserve`</ph>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>This ensures all environment variables needed by ScaleR are set properly.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Kerberos<ept id="p1">**</ept>: If your Hadoop cluster is secured using Kerberos, obtain a Kerberos ticket for principal <ph id="ph1">`hdfs`</ph>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>This ticket acts as the proxy for all other users.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Be sure you are the Linux user <ph id="ph1">`rserve`</ph> when obtaining the ticket.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>We recommend that you use a <ph id="ph1">`cron`</ph> job or equivalent to renew this ticket periodically to keep it from expiring.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Testing the Environment</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Create a private file in HDFS.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>In the following example, user <ph id="ph1">`revo`</ph> owns the file:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Create a sample RScript that tries to access the file.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>When you run this program from the R console as user <ph id="ph1">`rserve`</ph>, it works because principal <ph id="ph2">`hdfs`</ph> has a valid Kerberos ticket for the Linux user <ph id="ph3">`rserve`</ph>.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Modify the script to use the <ph id="ph1">`HADOOP_PROXY_USER`</ph> environment variable.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>For example, add <ph id="ph1">`Sys.setenv(HADOOP_PROXY_USER='rserve')`</ph>:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Unlike the previous step, when you run the script now, it will fail.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>This is due to the fact that the principal <ph id="ph1">`hdfs`</ph> is no longer acting as a <bpt id="p1">*</bpt>superuser<ept id="p1">*</ept> for the command.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Instead, it is acting as proxy for the user <ph id="ph1">`rserve`</ph>.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>This is a subtle but important difference.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>RScript for DeployR - We don't want to leave line of code that sets the HADOOP<ph id="ph1">\_</ph>PROXY<ph id="ph2">\_</ph>USER in our R Script.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>So we remove it and revert back to our original script.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>In addition, we pass the filename into the script from our DeployR client application.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>So, the script simply becomes:</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>We can now upload the script to DeployR using the Repository Manager.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>In our example, user <ph id="ph1">`testuser`</ph> creates a directory called <ph id="ph2">`demo`</ph> in the DeployR Repository Manager and name our RScript <ph id="ph3">`piperead.R`</ph>.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Creating a DeployR Client</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Create a DeployR client application to control which user is running the script.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>This example code is written in Visual Basic using the DeployR .NET client library.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>An equivalent example could be written in C<ph id="ph1">\#</ph>, Java or JavaScript.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Extending the Example</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>We can now extend this example to include two more RScripts for execution.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Second RScript</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>This script demonstrates how to copy a file from HDFS into the working directory of the R session.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>This RScript is uploaded to the DeployR repository as <ph id="ph1">`copy_to_workspace.R`</ph>, in directory <ph id="ph2">`demo`</ph> for user <ph id="ph3">`testuser`</ph>.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Third RScript</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>This script runs a ScaleR algorithm as a MapReduce job in Hadoop.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>This RScript is uploaded to the DeployR repository as <ph id="ph1">`scaleR_hadoop.R`</ph>, in directory <ph id="ph2">`demo`</ph> for user <ph id="ph3">`testuser`</ph>.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Update VB.NET code that executes all three examples</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>This is an update of the <bpt id="p1">[</bpt>code shown here<ept id="p1">](#create-deployr-client)</ept> that now reads in and executes all three scripts.</source>
        </trans-unit></group></body></file></xliff>