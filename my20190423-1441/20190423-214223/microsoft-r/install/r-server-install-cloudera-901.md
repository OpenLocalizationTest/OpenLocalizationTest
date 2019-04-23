<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-cloudera-901.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86d1e5c6b57e74d994034f99b6a8933df6bd9359cb.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d1e5c6b57e74d994034f99b6a8933df6bd9359cb</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-cloudera-901.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install R Server 9.0.1 on CDH</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install R Server 9.0.1 on Cloudera Distribution Including Apache Hadoop (CDH).</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Install R Server 9.0.1 on Cloudera Distribution Including Apache Hadoop (CDH)</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>We recommend the latest version of <bpt id="p1">[</bpt>R Server for Hadoop<ept id="p1">](r-server-install-cloudera.md)</ept> for the most features and for simplicity of installation, but if you have an older download of R Server for Hadoop 9.0.1, you can use the following instructions to create a parcel in Cloudera Manager.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Multi-node installation is also covered in this article.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Create an R Package Parcel for Cloudera Manager</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>If you are using Cloudera Manager to manage your Cloudera Hadoop cluster, you can use the Microsoft R Server Parcel Generator to create a Cloudera Manager parcel containing additional R packages, and use the resulting parcel to distribute those packages across all the nodes of your cluster.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The Microsoft R Server Parcel Generator is a Python script that takes a library of R packages and creates a Cloudera Manager parcel that <bpt id="p1">**</bpt>excludes any base or recommended packages, or packages included with the standard Microsoft R Server distribution<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Make sure to consider any dependencies your packages might have and be sure to include those in your library.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>You can find the generate_r_parcel.py script at the following link: <ph id="ph1">https://aka.ms/generate_r_parcel.py</ph></source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>You can find the Parcel Generator used to run the script in the <bpt id="p1">*</bpt>MRS-x.y.z/bin<ept id="p1">*</ept> directory.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>You might need to ensure that the script has execute permission using the <ph id="ph1">`chmod`</ph> command, or you can call it as <ph id="ph2">`python generate\_r\_parcel.py`</ph>.)</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>When calling the script, provide a name and a version number for the resulting parcel, together with the path to the library you would like to package.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>When choosing a name for your parcel, be sure to pick a name that is unique in your parcel repository (typically /opt/cloudera/parcel-repo).</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>For example, to package the library /home/RevoUser/R/library, you might call the script as follows:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>By default, the path to the library you package should be the same as the path to the library on the Hadoop cluster.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>You can specify a different destination using the –d flag:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>To distribute and activate your parcel perform the following steps:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Copy or move your .parcel and .sha files to the parcel repository on your Cloudera cluster (typically, /opt/cloudera/parcel-repo)</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Ensure that the .parcel and .sha files are owned by root and have 755 permissions (that is, read, write, and execute permission for root, and read and execute permissions for group and others).</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>In your browser, open Cloudera Manager.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Hosts<ept id="p1">**</ept> in the upper navigation bar to bring up the All Hosts page.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Parcels<ept id="p1">**</ept> to bring up the Parcels page.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Check for New Parcels<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Your new parcel should appear with a <bpt id="p1">**</bpt>Distribute<ept id="p1">**</ept> button.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>After clicking Check for New Parcels you may need to click on “All Clusters” under the “Location” section on the left to see the new parcel.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Click the <bpt id="p1">**</bpt>Distribute<ept id="p1">**</ept> button for your parcel.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The parcel will be distributed to all the nodes of your cluster.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>When the distribution is complete, the <bpt id="p1">**</bpt>Distribute<ept id="p1">**</ept> button is replaced with an <bpt id="p2">**</bpt>Activate<ept id="p2">**</ept> button.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Activate<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Activation prepares your parcel to be used by the cluster.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>After your parcel is distributed and activated your R packages should be present in the libraries on each node and can be loaded into your next R session.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Multinode installation using Cloudera Manager</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The following steps walk you through a multinode installation using Cloudera Manager to create a Cloudera Manager parcel for an R Server installation.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Two parcels are required:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Microsoft R Open<ept id="p1">*</ept> parcel installs open-source R and additional open-source components on the nodes of your Cloudera cluster.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>This distribution of MRO must be downloaded using the link below.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Please do not use MRO from MRAN or the MRO package from another installation of R Server.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Microsoft R Server<ept id="p1">*</ept> parcel installs proprietary components on the nodes of your Cloudera cluster.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Install the Cloudera Manager parcels as follows:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Download the Microsoft R Open for Microsoft R Server Cloudera Manager parcel<ept id="p1">](https://rserverdistribution.azureedge.net/production/MRO/3.3.2/485/1033/f9644b5c602b4479bcdaa88d55cdd977/MRO-3.3.2-Cloudera.tar.gz)</ept>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Note that the parcel consists of two files, the parcel itself and its associated .sha file.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>They may be packaged as a single .tar.gz file for convenience in downloading, but that must be unpacked and the two files copied to the parcel-repo for Cloudera Manager to recognize them as a parcel.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Download and unpack the R Server distribution, which will either be a DVD img file (if you obtained Microsoft R Server via Microsoft Volume Licensing) or a gzipped tar file (if you obtained Microsoft R Server via MSDN or Dev Essentials).</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The distribution file includes the required Cloudera Parcel files.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If you have an img file, you must first mount the file.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The following commands create a mount point and mount the file to that mount point:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If you have a gzipped tar file, you should unpack the file as follows (be sure you have downloaded the file to a writable directory, such as /tmp):</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Copy the parcel files to your local parcel-repo, typically /opt/cloudera/parcel-repo:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>From the mounted img file:      cp /mnt/mrsimage/MRS_Parcel/MRS-9.0.1-* /opt/cloudera/parcel-repo</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>From the unpacked tar file:      cp /tmp/MRS90HADOOP/MRS_Parcel/MRS-9.0.1-* /opt/cloudera/parcel-repo</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>You should have the following files in your parcel repo:</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Be sure all the files are owned by root and have 644 permissions (read, write, permission for root, and read permission for groups and others).</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Parcels should not have a file extension.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If any parcels have a .sha file extension, please rename the file to remove the extension.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>In your browser, open Cloudera Manager.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Hosts<ept id="p1">**</ept> in the upper navigation bar to bring up the All Hosts page.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Parcels<ept id="p1">**</ept> to bring up the Parcels page.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Check for New Parcels<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>MRO and MRS parcels should each appear with a <bpt id="p1">**</bpt>Distribute<ept id="p1">**</ept> button.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>After clicking <bpt id="p1">**</bpt>Check for New Parcels<ept id="p1">**</ept> you may need to click on <bpt id="p2">**</bpt>Location &gt; All Clusters<ept id="p2">**</ept> on the left to see the new parcels.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Click the MRO <bpt id="p1">**</bpt>Distribute<ept id="p1">**</ept> button.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Microsoft R Open will be distributed to all the nodes of your cluster.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>When the distribution is complete, the <bpt id="p1">**</bpt>Distribute<ept id="p1">**</ept> button is replaced with an <bpt id="p2">**</bpt>Activate<ept id="p2">**</ept> button.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Activate<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Activation prepares Microsoft R Open to be used by the cluster.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Click the MRS <bpt id="p1">**</bpt>Distribute<ept id="p1">**</ept> button.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Microsoft R Server will be distributed to all the nodes of your cluster.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>When the distribution is complete, the <bpt id="p1">**</bpt>Distribute<ept id="p1">**</ept> button is replaced with an <bpt id="p2">**</bpt>Activate<ept id="p2">**</ept> button.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Install R on Hadoop overview</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Install R Server 8.0.5 on Hadoop</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Install Microsoft R Server on Linux</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Uninstall Microsoft R Server to upgrade to a newer version</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Troubleshoot R Server installation problems on Hadoop</source>
        </trans-unit></group></body></file></xliff>