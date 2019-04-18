<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-cleanup-jobs.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907fbff4c0663bda73a9b4fcc99d441c6c2f617829ba.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">bff4c0663bda73a9b4fcc99d441c6c2f617829ba</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-cleanup-jobs.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_cleanup_jobs:  (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Removes the artifacts for the specified jobs.If job_info_list is a RxRemoteJob object, rx_cleanup_jobs attempts to remove the artifacts.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>However, if the job has successfully completed and force is False, rx_cleanup_jobs issues a warning saying to either set force=True or use rx_get_job_results to get the results and delete the artifacts.If job_info_list is a list of jobs, rx_cleanup_jobs attempts to apply the cleanup rules for a single job to each element in the list.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>cleanup, job</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>rx_cleanup_jobs</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Removes the artifacts for the specified jobs.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>job_info_list<ept id="p1">*</ept> is a <bpt id="p2">*</bpt>RxRemoteJob<ept id="p2">*</ept> object, <bpt id="p3">*</bpt>rx_cleanup_jobs<ept id="p3">*</ept> attempts to remove the artifacts.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>However, if the job has successfully completed and <bpt id="p1">*</bpt>force<ept id="p1">*</ept> is <bpt id="p2">*</bpt>False<ept id="p2">*</ept>, <bpt id="p3">*</bpt>rx_cleanup_jobs<ept id="p3">*</ept> issues a warning saying to either set <bpt id="p4">*</bpt>force=True<ept id="p4">*</ept> or use <bpt id="p5">*</bpt>rx_get_job_results<ept id="p5">*</ept> to get the results and delete the artifacts.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>job_info_list<ept id="p1">*</ept> is a list of jobs, <bpt id="p2">*</bpt>rx_cleanup_jobs<ept id="p2">*</ept> attempts to apply the cleanup rules for a single job to each element in the list.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>job_info_list</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The jobs for which to remove the artifacts, this can be a list of jobs or a single job</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>force</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>True<ept id="p1">*</ept> indicates the cleanup should happen regardless of whether or not the job status can be determined and job results have already been retrieved.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>False<ept id="p1">*</ept> indicates that the should be cleaned up by calling <bpt id="p2">*</bpt>rx_get_job_results<ept id="p2">*</ept> or the job should have completed unsuccessfully (such as by using rx_cancel_job).</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>True<ept id="p1">*</ept>, will print the directories/records being deleted.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>This function does not return a value</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>