<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-get-job-output.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926cd75767ab8daacdd8d39465fcac255e14a29b36f.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">cd75767ab8daacdd8d39465fcac255e14a29b36f</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-get-job-output.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_get_job_output: Gets the console output from the various nodes in a non-waiting distributed computing job.</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoscalepy)</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>During a job run, the state of the output is non-deterministic (that is, it may or may not be on disk, and what is on disk at any given point in time may not reflect the actual completion state of a job).If auto_cleanup has been set to True on the distributed computing job’s compute context, the console output will not persist after the job completes.Unlike rx_get_job_results, this function does not remove any job information upon retrieval.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>job, output</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>rx_get_job_output</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>During a job run, the state of the output is non-deterministic (that is, it may or may not be on disk, and what is on disk at any given point in time may not reflect the actual completion state of a job).</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>auto_cleanup<ept id="p1">*</ept> has been set to <bpt id="p2">*</bpt>True<ept id="p2">*</ept> on the distributed computing job’s compute context, the console output will not persist after the job completes.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Unlike <bpt id="p1">*</bpt>rx_get_job_results<ept id="p1">*</ept>, this function does not remove any job information upon retrieval.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>job_info</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The distributed computing job for which to retrieve the job output</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>str<ept id="p1">*</ept> that contains the console output for the nodes participating in the distributed computing job</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>