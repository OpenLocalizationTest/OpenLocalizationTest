<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="RxRemoteJobStatus.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b458d2f8f741fa31ef6a7986f7e903c653f8abfb90.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">58d2f8f741fa31ef6a7986f7e903c653f8abfb90</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\RxRemoteJobStatus.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RxRemoteJobStatus: Execution status of a remote job (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>This enumeration represents the execution status of a remote Python job.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>The enumeration is returned from the rx_get_job_status method and will indicate the current status of the job.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>The enumeration has the following values indicating job status:FINISHED - The job has run to a successful completionFAILED - The job has failedCANCELED - The job was cancelled before it could run to successful completion by using rx_cancel_jobUNDETERMINED - The job’s status could not be determined, typically meaning it has been executed on the server and the job has already been cleaned up by calling rx_get_job_results or rx_cleanup_jobsRUNNING - The distributed computing job is currently executing on the serverQUEUED - The distributed computing job is currently awaiting execution on the server</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>remote, job</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>RxRemoteJobStatus</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This enumeration represents the execution status of a remote Python job.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The enumeration is returned from the rx_get_job_status method and will indicate the current status of the job.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The enumeration has the following values indicating job status:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>FINISHED<ept id="p1">*</ept> - The job has run to a successful completion</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>FAILED<ept id="p1">*</ept> - The job has failed</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>CANCELED<ept id="p1">*</ept> - The job was canceled before it could run to successful completion by using <bpt id="p2">*</bpt>rx_cancel_job<ept id="p2">*</ept></source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>UNDETERMINED<ept id="p1">*</ept> - The job’s status could not be determined, typically meaning it has been executed on the server and the job has already been cleaned up by calling <bpt id="p2">*</bpt>rx_get_job_results<ept id="p2">*</ept> or <bpt id="p3">*</bpt>rx_cleanup_jobs<ept id="p3">*</ept></source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>RUNNING<ept id="p1">*</ept> - The distributed computing job is currently executing on the server</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>QUEUED<ept id="p1">*</ept> - The distributed computing job is currently awaiting execution on the server</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>