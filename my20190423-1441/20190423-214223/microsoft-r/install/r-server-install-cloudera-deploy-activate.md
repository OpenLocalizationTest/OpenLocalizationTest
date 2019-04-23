<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-cloudera-deploy-activate.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86840e93eb016106589f773025fcfc8cfefb5c4af8.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">840e93eb016106589f773025fcfc8cfefb5c4af8</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-cloudera-deploy-activate.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Deploy and activate MRS parcels and CSDs on CDH</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Deploy and activate Microsoft R Server parcels and CSDs on the Cloudera distribution of Apache Hadoop (CDH).</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Deploy and activate the MRS parcel and custom service descriptor (CSD)</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:<ept id="p1">**</ept> R Server 9.1 on the Cloudera distribution of Apache Hadoop (CDH)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>A parcel installation of Microsoft R Server on CDH is a 2-part process.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>In part 1, you <bpt id="p1">[</bpt>generated a parcel and Custom Service Descriptor (CSD) for Microsoft R Server (MRS) 9.1<ept id="p1">](r-server-install-cloudera-generate-parcel.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>This article is part 2.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Because you copied the parcel and CSD to the Cloudera repositories, you can now use Cloudera Manager to deploy the parcel, activate and roll out R Server, and add MRS as a service administered within Cloudera Manager.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Step 1: Distribute the MRS parcel</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>In Cloudera Manager, click the parcel icon on the top right menu bar.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>parcel icon in cloudera manager</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Find <bpt id="p1">**</bpt>MRS<ept id="p1">**</ept> in the parcel list.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If you don't see it, check the parcel-repo folder (by default, /opt/cloudera/parcel-repo) for <ph id="ph1">`MRS-9.1.0-el7.parcel`</ph> and <ph id="ph2">`MRS-9.1.0-el7.parcel.sha`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The machine should be the master node of the cluster.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>parcel list in cloudera manager</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>In the parcel details page, <bpt id="p1">**</bpt>MRS<ept id="p1">**</ept> should have a status of <bpt id="p2">*</bpt>Downloaded<ept id="p2">*</ept> with an option to <bpt id="p3">*</bpt>Distribute<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Distribute<ept id="p1">**</ept> to roll out MRS on available data nodes.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>parcel details in cloudera manager</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Status changes to <bpt id="p1">*</bpt>distributed<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Activate<ept id="p1">**</ept> on the button to make MRS operational in the cluster.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Activate button in parcel detail</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>You are finished with this task when status is "distributed, activated" and the next available action is <bpt id="p1">*</bpt>Deactivate<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Step 2: Add MRS as a service</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>In Cloudera Manager home page, click the down arrow by the cluster name and choose <bpt id="p1">**</bpt>Add Service<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>add service command in cloudera manager</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Find and select <bpt id="p1">**</bpt>Microsoft R Server<ept id="p1">**</ept> and click <bpt id="p2">**</bpt>Continue<ept id="p2">**</ept> to start a wizard for adding services.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>add Microsoft R Server</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>In the next page, add role assignments on all nodes used to run the service, both edge and data nodes.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Continue<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>On the last page, click <bpt id="p1">**</bpt>Finish<ept id="p1">**</ept> to start the service.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>R Server should now be available to use.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Next Steps</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Review the following walkthroughs to move forward with using R Server and the RevoScaleR package in Spark and MapReduce processing models.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Practice data import and exploration on Spark</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Practice data import and exploration on MapReduce</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>R Server installation on Hadoop overview</source>
        </trans-unit></group></body></file></xliff>