<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-get-jobs.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37c7dd663c37fda3881c09f398cfb2c9af8df52a11.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">c7dd663c37fda3881c09f398cfb2c9af8df52a11</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-get-jobs.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_get_jobs: Get Distributed Computing Jobs (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Returns a list of job objects associated with the given compute context and matching the specified parameters.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>get, job</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rx_get_jobs</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Returns a list of job objects associated with the given compute context and matching the specified parameters.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>A compute context object.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>exact_match</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Determines if jobs are matched using the full compute context, or a simpler subset.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If True, only jobs which use the same context object are returned.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If False, all jobs which have the same headNode (if available) and ShareDir are returned.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>start_time</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>A time, specified as a POSIXct object.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If specified, only jobs created at or after start_time are returned.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>end_time</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>A time, specified as a POSIXct object.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If specified, only jobs created at or before end_time are returned.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>states</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If specified (as a list of strings of states that can include “none”, “finished”, “failed”, “canceled”, “undetermined” “queued”or “running”), only jobs in those states are returned.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Otherwise, no filtering is performed on job state.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If True (the default), a brief summary of each job is printed as it is found.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>This includes the current job status as returned by rx_get_job_status, the modification time of the job, and the current job ID (this is used as the component name in the returned list of job information objects).</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If no job status is returned, the job status shows none.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Returns a list of job information objects based on the compute context.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>