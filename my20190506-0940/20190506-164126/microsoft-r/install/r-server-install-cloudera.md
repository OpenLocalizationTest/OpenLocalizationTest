<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-cloudera.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc77507b1cfa3d9cfe8c37e963162f04d029ed27231783.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">7b1cfa3d9cfe8c37e963162f04d029ed27231783</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-cloudera.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Server installation on Cloudera CDH</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install Microsoft R Server 9.1 on the Cloudera distribution of Apache Hadoop (CDH).</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Install R Server 9.1 on the Cloudera distribution of Apache Hadoop (CDH)</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Looking for the latest release?</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>Machine Learning Server for Cloudera installation<ept id="p1">](machine-learning-server-cloudera-install.md)</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Cloudera offers a parcel installation methodology for adding services and features to a cluster.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>If you prefer parcel installation over the regular install script used for deploying R Server on other Hadoop distributions, you can use functionality we provide to create the parcel.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>If you've used parcel installation in previous releases of Microsoft R Server, the 9.1.0 release is enhanced in two respects.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>First, instead of using pre-built parcels downloaded from Microsoft, you can generate your own parcel using a new generate_mrs_parcel.sh script.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Secondly, we added support for Custom Service Descriptors (CSDs), which means you can now deploy, configure, and monitor R Server in CDH as a managed service in Cloudera Manager.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The new revised workflow for parcel installation is a two-part exercise:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Part 1: At the console, run script to output parcel and CSD files</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Part 2: In Cloudera Manager, deploy parcels and add MRS as a managed service</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Download and unpacking the distribution remains the same.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Instructions are included in Part 1.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Feature restrictions in a parcel installation</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>R Server includes two packages, <ph id="ph1">`MicrosoftML`</ph> and <ph id="ph2">`mrsdeploy`</ph>, that either cannot be included in the parcel, or included only if the underlying operating system is a specific platform and version.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>is conditionally available.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The package can be included in the parcel if the underlying operating system is CentOS/RHEL 7.x.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If CDH runs on any other operating system, including an earlier version of RHEL, the <ph id="ph1">`MicrosoftML`</ph> package cannot be included.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>is excluded from a parcel installation.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This package has a .NET Core dependency and cannot be added to a parcel.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The workaround is to perform a manual installation of individual packages.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>For instructions, see <bpt id="p1">[</bpt>Manual package installation<ept id="p1">](r-server-install-hadoop-manual-package.md)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>R Server Installation on Hadoop Overview</source>
        </trans-unit></group></body></file></xliff>