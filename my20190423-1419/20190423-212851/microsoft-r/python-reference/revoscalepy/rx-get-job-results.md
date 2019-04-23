<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-get-job-results.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338af3fde5e352f64e9e72f21051dcb531585ef15588.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">f3fde5e352f64e9e72f21051dcb531585ef15588</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-get-job-results.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_get_job_results: Obtain Distributed Computing Job Status and Results (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Obtain distributed computing results and processing status.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>rx_get_job_results</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Obtain distributed computing results and processing status.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>job_info</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A job object as returned by rx_exec or a revoscalepy analysis function, if available.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>console_output</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>None or bool value.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>If True, the console output from all of the processes is printed to the user console.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If False, no console output is displayed.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Output can be retrieved with the function rxGetJobOutput for a non-waiting job.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If not None, this flag overrides the value set in the compute context when the job was submitted.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If None, the setting in the compute context will be used.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>auto_cleanup</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>None or bool value.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>If True, the default behavior is to clean up any artifacts created by the distributed computing job.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If False, then the artifacts are not deleted, and the results may be acquired using rxGetJobResults, and the console output via rxGetJobOutput until the rxCleanupJobs is used to delete the artifacts.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If not None, this flag overwrites the value set in the compute context when the job was submitted.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If you routinely set auto_cleanup=False, you will eventually fill your hard disk with compute artifacts.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If you set auto_cleanup=True and experience performance degradation on a Windows XP client, consider setting auto_cleanup=False.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Either the results of the run (prepended with console output if the console_output argument is set to True) or a message saying that the results are not available because the job has not finished, has failed, or was deleted.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>