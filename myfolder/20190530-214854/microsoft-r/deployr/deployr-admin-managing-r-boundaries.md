<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-admin-managing-r-boundaries.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e9ee16fa513813a43b8a863a86374d52233afe623.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9ee16fa513813a43b8a863a86374d52233afe623</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-admin-managing-r-boundaries.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>DeployR Administration Console Help - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Managing R Boundaries in the DeployR Administration Console</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Managing R Boundaries</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>R boundaries are used to constrain runtime resource usage related to:</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Authenticated operations running on projects</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Asynchronous operations running as background jobs</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Anonymous operations running on stateless projects</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>R boundaries help manage the optimal allocation of resources across all operations.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>They also protect the system from poorly written or malicious code that may attempt to consume all system resources in an infinite loop or other threats.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>In this Administration Console, you can access and work with R boundaries by clicking <bpt id="p1">**</bpt>R Boundaries<ept id="p1">**</ept> in the main menu.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Once you create an R boundary, you can assign it to any grid node or user account in the console.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Grid node boundaries take precedence over boundaries associated with individual users.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>You can also designate a particular R boundary as the <bpt id="p1">[</bpt>default system-wide R boundary<ept id="p1">](deployr-admin-managing-server-policies.md#server-policy-properties)</ept> to be used whenever no other boundary is indicated.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If you plan to associate R boundaries with grid nodes, we recommend that you create a custom R boundary for each <bpt id="p1">[</bpt>node operation type<ept id="p1">](deployr-admin-managing-the-grid.md#node-operation-types)</ept> (authenticated, asynchronous, and anonymous operations) supported on the grid.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Figure: Boundary List page</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Creating New Boundaries</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>To create a new boundary:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>R Boundaries<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>From the <bpt id="p1">**</bpt>R Boundary List<ept id="p1">**</ept> page, click the <bpt id="p2">**</bpt>New Boundary<ept id="p2">**</ept> link.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>New R Boundary<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Figure: New R Boundary page</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>New R Boundary<ept id="p1">**</ept> page, define your boundary, including:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Name<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Enter a unique name for the boundary.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>This field is required.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Max CPU (sec)<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Enter the maximum amount of time in seconds that the CPU can be engaged at runtime.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If the time limit is exceeded, then an R error is returned at runtime.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If you enter a value of 0, this constraint will be ignored.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Create<ept id="p1">**</ept> to save the new boundary.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Deleting Boundaries</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>To delete a boundary:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>R Boundaries<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>From the <bpt id="p1">**</bpt>R Boundary List<ept id="p1">**</ept> page, click the name of the boundary you want to delete.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>R Boundary Details<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Delete<ept id="p1">**</ept> and confirm the removal of the boundary.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Viewing and Editing Boundaries</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>To view and edit a boundary:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>R Boundaries.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>From the <bpt id="p1">**</bpt>R Boundary List<ept id="p1">**</ept> page, click the name of the boundary you want to view or edit in the table.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>R Boundary Details<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Figure: R Boundary Details page</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>To edit a boundary, perform the following steps:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Edit<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Make your changes.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Update<ept id="p1">**</ept> to save the changes.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Exporting Boundaries</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>You can export all or selected R boundaries into one <ph id="ph1">`CSV`</ph> file.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Exporting can be used to copy the boundaries to another machine or to preserve them as a backup.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>You can later import the contents of this file to this server or across multiple server deployments.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Figure: Export Boundaries page</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>To export:</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>R Boundaries<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>From the <bpt id="p1">**</bpt>R Boundary List<ept id="p1">**</ept>, click <bpt id="p2">**</bpt>Export Boundaries<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Select the R boundaries you want to export.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>You can choose to export all of them or individually select the boundaries to be exported.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Export to File<ept id="p1">**</ept> and save the file.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Importing Boundaries</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>You can import R boundaries from a <ph id="ph1">`CSV`</ph> file into the server.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>This CSV file can come from a previous export or might be a file you created manually using the proper format.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Figure: Import Boundaries page</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>To import:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>From the main menu, click <bpt id="p1">**</bpt>R Boundaries<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>From the <bpt id="p1">**</bpt>R Boundary List<ept id="p1">**</ept>, click <bpt id="p2">**</bpt>Import Boundaries<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Browse<ept id="p1">**</ept> and select the file to be imported.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>By default, the file has the CSV file extension.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Load<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Choose which R boundaries to import.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>You can choose to import all of them or individually select the boundaries to import.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Import<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>If a boundary by the same name already exists, then a message appears to inform you that the incoming boundary was rejected.</source>
        </trans-unit></group></body></file></xliff>