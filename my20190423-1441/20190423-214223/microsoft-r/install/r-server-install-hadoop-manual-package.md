<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-hadoop-manual-package.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca860bbeabf8fec518e627d55d8159fb89594ace1c84.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">0bbeabf8fec518e627d55d8159fb89594ace1c84</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-hadoop-manual-package.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Manual package install on R Server for Linux or Hadoop</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install individual packages on R Server on Linux or Hadoop</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Manual package installation (Microsoft R Server for Linux or Hadoop)</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>An alternative to running the install.sh script at the command line is to manually install each package and component.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Syntax</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>With root privilege, you can use a package manager to install each package in the R Server distribution.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The following example illustrates the syntax.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>On RHEL:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>On Ubuntu:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>On SUSE:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>A manual package installation is similar to an offline installation.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>As a first step, review the instructions for <bpt id="p1">[</bpt>offline installation<ept id="p1">](r-server-install-hadoop-offline.md)</ept> for system prerequisites and for downloading and unpacking the distribution.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>After you unpack the distribution, you should see packages for RPM and DEB in the /tmp/MRS91Hadoop directory.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Steps</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Log in as root or as a user with super user privileges (<ph id="ph1">`sudo -s`</ph>).</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The following instructions assume user privileges with the sudo override.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Use a package manager to verify system repositories are up-to-date:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>On RHEL use <bpt id="p1">[</bpt>yum<ept id="p1">](https://access.redhat.com/documentation/Red_Hat_Enterprise_Linux/6/html/Deployment_Guide/sec-Working_with_Yum_Cache.html)</ept>:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>On Ubuntu use <bpt id="p1">[</bpt>apt-get<ept id="p1">](https://help.ubuntu.com/community/AptGet/Howto)</ept>:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Install the .NET Core package from <bpt id="p1">[</bpt><ph id="ph1">https://www.microsoft.com/net/core</ph><ept id="p1">](https://www.microsoft.com/net/core)</ept>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This component is required for machine learning, remote execution, web service deployment, and configuration of web and compute nodes.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Server packages.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>You should have the following packages, which should be installed in this order:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>microsoft-r-open-mro-3.3.3.x86_64.rpm</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>microsoft-r-server-packages-9.1.rpm</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>microsoft-r-server-hadoop-9.1.rpm</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>microsoft-r-server-mml-9.1.rpm</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>microsoft-r-server-mlm-9.1.rpm</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>microsoft-r-server-config-rserve-9.1.rpm</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>microsoft-r-server-computenode-9.1.rpm</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>microsoft-r-server-webnode-9.1.rpm</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>microsoft-r-server-adminutil-9.1.rpm</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Create folders and set permissions</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>A manual or custom installation must create the appropriate folders and set permissions.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>RPM or DEB Installers</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>and <ph id="ph1">`hdfs://user/RevoShare`</ph> must exist and have folders for each user running Microsoft R Server in Hadoop or Spark.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>and <ph id="ph1">`hdfs://user/RevoShare/&lt;user&gt;`</ph> must have full permissions (all read, write, and executive permissions for all users).</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Cloudera Parcel Installers</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Create <ph id="ph1">`/var/RevoShare/`</ph> and <ph id="ph2">`hdfs://user/RevoShare`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Parcels cannot create them for you.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Give <ph id="ph1">`/var/RevoShare/&lt;user&gt;`</ph> and <ph id="ph2">`hdfs://user/RevoShare/&lt;user&gt;`</ph> for each user.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Grant full permissions to both <ph id="ph1">`/var/RevoShare/&lt;user&gt;`</ph> and <ph id="ph2">`hdfs://user/RevoShare/&lt;user&gt;`</ph>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Install additional packages on each node using rxExec</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Once you have R Server installed on a node, you can use the <ph id="ph1">`rxExec`</ph> function in <bpt id="p1">[</bpt>RevoScaleR<ept id="p1">](~/r-reference/revoscaler/revoscaler.md)</ept> to install additional packages, including third-party packages from CRAN or another repository.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>For example, to install the <ph id="ph1">`SuppDists`</ph> package on all the nodes of your cluster, call <ph id="ph2">`rxExec`</ph> as follows:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Enable Remote Connections and Analytic Deployment</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The server can be used as-is if you install and use an R IDE on the same box, but to benefit from the deployment and consumption of web services with Microsoft R Server, then you must configure R Server after installation to act as a deployment server and host analytic web services.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Possible configurations are a <bpt id="p1">[</bpt>one-box setup<ept id="p1">](operationalize-r-server-one-box-config.md)</ept> or an <bpt id="p2">[</bpt>enterprise setup<ept id="p2">](operationalize-r-server-enterprise-config.md)</ept>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Doing so also enables remote execution, allowing you to connect to R Server from an R Client workstation and execute code on the server.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Next Steps</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Review the following walkthroughs to move forward with using R Server and the RevoScaleR package in Spark and MapReduce processing models.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Practice data import and exploration on Spark</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Practice data import and exploration on MapReduce</source>
        </trans-unit></group></body></file></xliff>