<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-distributed-computing-background-jobs.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c377b194242e64fc0b1edc9a298fd6b39271a67b88c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">7b194242e64fc0b1edc9a298fd6b39271a67b88c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-distributed-computing-background-jobs.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Running background jobs using RevoScaleR (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Machine Learning Server in-database and cluster computing using the RevoScaleR engine and RevoScaleR package.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Running background jobs using RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server, you can run jobs interactively, waiting for results before continuing on to the next operation, or you can run them asynchronously in the background if a job is long-running.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Non-Waiting jobs</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>By default, all jobs are "waiting jobs" or "blocking jobs" (where control of the R prompt is not returned until the job is complete).</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>As you can imagine, you might want a different interaction model if you are sending time-intensive jobs to your distributed compute context.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Decoupling your current session from in-progress jobs will enable jobs to proceed in the background while you continue to work on your R Console for the duration of the computation.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>This can be useful if you expect the distributed computations to take a significant amount of time, and when such computations are managed by a job scheduler.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Convert a Waiting Job to a Non-Waiting Job</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Suppose you submit a job as a "waiting" job, and then realize that you’d prefer to be able to work in your R session on the local computer while it is running.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>In Windows, simply pressing the Esc will return the cursor to your screen.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Depending on how quickly you press Esc, your job will either be canceled (if it has not yet been accepted by the job scheduler), or will continue to run on the cluster.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Similarly, on Red Hat Enterprise Linux, pressing Ctrl-C will return the cursor to your screen, and either cancel the job or convert it to a non-waiting job.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>For all jobs that run on the cluster, the object <ph id="ph1">`rxgLastPendingJob`</ph> is automatically created.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>You can use the <ph id="ph1">`rxgLastPendingJob`</ph> object to retrieve your results later or to cancel the job.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Create Non-Blocking Jobs</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>To create non-waiting jobs, you simply set wait=FALSE in your compute context object:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>When <bpt id="p1">*</bpt>wait<ept id="p1">*</ept> is set to <bpt id="p2">*</bpt>FALSE<ept id="p2">*</ept>, a job information object rather than a job results object is returned from the submitted job.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>You should always <bpt id="p1">*</bpt>assign<ept id="p1">*</ept> this result so that you can use it to obtain job status while the job is running and obtain the job results when the job completes.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>For example, returning to our initial waiting job example, calling <ph id="ph1">`rxExec`</ph> to get data set information, in the non-blocking case we augment our call to <ph id="ph2">`rxExec`</ph> with an assignment, and then use the assigned object as input to the <ph id="ph3">`rxGetJobStatus`</ph> and <ph id="ph4">`rxGetJobResults`</ph> functions:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If you call <ph id="ph1">`rxGetJobStatus`</ph> quickly, it may show us that the job is "running", but if called after a few seconds (or longer if another job of higher priority is ahead in the queue) it should report "finished", at which point we can ask for the results:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>As in the case of the waiting job, we obtain the following results from our five-node cluster (note that the name of the head node is mangled here to be an R syntactic name):</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Running a linear model on the airline data is more likely to show us the "running" status:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>This shows us the following:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Calling rxGetJobStatus again a few seconds later shows us that the job has completed:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>We can then call <ph id="ph1">`rxGetJobResults`</ph> to obtain the actual computation results:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>As in the blocking case, this gives the following results:</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Capture Job Information</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If you forget to assign the job information object when you first submit your job, don’t panic.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> saves the job information for the last pending job as the object <ph id="ph1">`rxgLastPendingJob`</ph>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>You can assign this value to a more specific name at any time until you submit another non-blocking job.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if script runs locally using R Client.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Also, as in all R sessions, the last value returned can be accessed as <ph id="ph1">`.Last.value;`</ph> if you remember immediately that you forgot to assign the result, you can simply assign <ph id="ph2">`.Last.value`</ph> to your desired job name and be done.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For jobs older than the last pending job, you can use <ph id="ph1">`rxGetJobs`</ph> to obtain all the jobs associated with a given compute context.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>More details on <ph id="ph1">`rxGetJobs`</ph> can be found in the next section.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Cancel a Non-Waiting Job</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Suppose you submit a job and realize you’ve mis-specified the formula.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>In the non-waiting case, it is easy to cancel your job simply by calling <ph id="ph1">`rxCancelJob`</ph> with the job information object you saved when you submitted the job:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Non-Waiting Logistic Regression</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Logistic regression uses an iteratively re-weighted least squares algorithm, and thus in general requires multiple passes through the data for successive iterations.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>This makes it a logical candidate for non-waiting distributed computing.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>For example, we replicated the large airline data set 8 times to create a data set with about one billion observations.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>We also added a variable "Late" to indicate which flights were at least fifteen minutes late.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>To find the probability of a late flight by day of week, we perform the following logistic regression:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>This immediately returns control back to our R Console, and we can do some other things while this 1-billion observation logistic regression completes on our distributed computing resources.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>(Although even with one billion observations, the logistic regression completes in less than a minute.)</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>We verify that the job is finished and retrieve the results as follows:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>We obtain the following results:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Clean up job artifacts using rxGetJobs and rxCleanJobs (distributed computing)</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Normally, whenever a waiting job completes or whenever you call <ph id="ph1">`rxGetJobResults`</ph> to obtain the results of a non-waiting job, any artifacts created during the distributed computation are automatically removed.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>(This is controlled by the <ph id="ph1">`autoCleanup`</ph> flag to the compute context constructor, which defaults to <bpt id="p1">*</bpt>TRUE<ept id="p1">*</ept>.)</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>However, if a waiting job fails to complete for some reason, or you do not collect all the results from your non-waiting jobs, you may begin to accumulate artifacts on your distributed computing resources.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Eventually, this could fill the storage space on these resources, causing system slowdown or malfunction.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>It is therefore a best practice to make sure you clean up your distributed computing resources from time to time.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>One way to do this is to simply use standard operating system tools to delete files from the various shared and working directories you specified in your compute context objects.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>But <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> also supplies a number of tools to help you remove any accumulated artifacts.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The first of these, <ph id="ph1">`rxGetJobs`</ph>, allows you to get a list of all the jobs associated with a given compute context.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>By default, it matches just the head node (if available) and shared directory specified in the compute context; if you re-use these two specifications, ALL the jobs associated with that head node and shared directory are returned:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>To restrict the matching to only those jobs associated with that specific compute context, specify <bpt id="p1">*</bpt>exactMatch=TRUE<ept id="p1">*</ept> when calling <ph id="ph1">`rxGetJobs`</ph>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>To obtain the jobs from a specified range of times, use the <bpt id="p1">*</bpt>startTime<ept id="p1">*</ept> and <bpt id="p2">*</bpt>endTime<ept id="p2">*</ept> arguments.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>For example, to obtain a list of jobs for a particular day, you could use something like the following:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Once you’ve obtained the list of jobs, you can try to clean them up using <ph id="ph1">`rxCleanupJobs`</ph>:</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If any of the jobs is in a "finished" state, <ph id="ph1">`rxCleanupJobs`</ph> will not clean up that job but instead warn you that the job is finished and that you can access the results with <ph id="ph2">`rxGetJobResults`</ph>.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>This helps prevent data loss.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>You can, however, force the cleanup by specifying <bpt id="p1">*</bpt>force=TRUE<ept id="p1">*</ept> in the call to <ph id="ph1">`rxCleanupJobs`</ph>:</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>You can also use <ph id="ph1">`rxCleanupJobs`</ph> to clean up individual jobs:</source>
        </trans-unit></group></body></file></xliff>