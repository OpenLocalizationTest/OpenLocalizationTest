<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-exec.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3efc6f776f212099afa64b379df4350ea68051d58b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">fc6f776f212099afa64b379df4350ea68051d58b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-exec.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_exec: Executes arbitary R functions in parallel (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Allows the distributed execution of an arbitrary R function in parallel, across nodes (computers) or cores of a “compute context”, such as a cluster.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>For example, you could use the function to execute multiple instances of a model concurrently.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>When used with base R functions, rxexec does not lift the memory constraints of the underlying functions, or make a single-threaded process a multi-threaded one.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>The fundamentals of the function still apply; what changes is the execution framework of those functions.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>parallel execution, multiple executions, remote execution, sql</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>rx_exec</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Allows the distributed execution of an arbitrary R function in parallel, across nodes (computers) or cores of a “compute context”, such as a cluster.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>For example, you could use the function to execute multiple instances of a model concurrently.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>When used with base R functions, rxexec does not lift the memory constraints of the underlying functions, or make a single-threaded process a multi-threaded one.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The fundamentals of the function still apply; what changes is the execution framework of those functions.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>function</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The function to be executed; the nodes or cores on which it is run are determined by the currently-active compute context and by the other arguments of rx_exec.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>args</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Arguments passed to the function ‘function’ each time it is executed.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>for multiple executions with different parameters, args should be a list where each element is a dict.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>each dict element contains the set of named parameters to pass the function on each execution.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>times_to_run</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Specifies the number of times ‘function’ should be executed.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>in case of different parameters for each execution, the length of args must equal times_to_run.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>in case where length of args equals 1 or args is not specified, function will be called times_to_run number of times with the same arguments.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>task_chunk_size</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Specifies the number of tasks to be executed per compute element.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>by submitting tasks in chunks, you can avoid some of the overhead of starting new python processes over and over.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>for example, if you are running thousands of identical simulations on a cluster, it makes sense to specify the task_chunk_size so that each worker can do its allotment of tasks in a single python process.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>A RxComputeContext object.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>local_state</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Dictionary with variables to be passed to a RxInSqlServer compute context not supported in RxSpark compute context.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>callback</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>An optional function to be called with the results from each execution of ‘function’</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>continue_on_failure</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>None or logical value.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If True, the default, then if an individual instance of a job fails due to a hardware or network failure, an attempt will be made to rerun that job.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>(Python errors, however, will cause immediate failure as usual.) Furthermore, should a process instance of a job fail due to a user code failure, the rest of the processes will continue, and the failed process will produce a warning when the output is collected.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Additionally, the position in the returned list where the failure occurred will contain the error as opposed to a result.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>**kwargs</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Contains named arguments to be passed to function.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Alternative to using args param.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>For a function foo that takes two arguments named ‘x’ and ‘y’, kwargs can be used like: rx_exec(function=foo, x=5, y=4) (for a single execution with x=5, y=4) rx_exec(function=foo, x=[1,2,3,4,5], y=6) (for multiple executions with different values of x and y=6) rx_exec(function=foo, x=[1,2,3], y=[4,5,6]) (for multiple executions with different values of x and y) Note: if you want to pass in a list as an argument, you must wrap it in another list.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>For a function foobar that takes an argument named ‘the_list’, kwargs can be used like: rx_exec(function=foobar, the_list=[ [0,1,2,3] ]) (single execution with the_list = [0,1,2,3]) rx_exec(function=foobar, the_list=[ [0,1,2],[3,4,5],[6,7,8] ]) (multiple executions)</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If local compute context or a waiting compute context is active, a list containing the return value of each execution of ‘function’ with specified parameters.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If a non-waiting compute context is active, a jobInfo object, or a list of a jobInfo objects for multiple executions.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>, <bpt id="p1">[</bpt><ph id="ph1">`RxLocalSeq`</ph><ept id="p1">](RxLocalSeq.md)</ept>, <ph id="ph2">`RxLocalParallel`</ph>, <bpt id="p2">[</bpt><ph id="ph3">`RxInSqlServer`</ph><ept id="p2">](RxInSqlServer.md)</ept>, <bpt id="p3">[</bpt><ph id="ph4">`rx_get_compute_context`</ph><ept id="p3">](rx-get-compute-context.md)</ept>, <bpt id="p4">[</bpt><ph id="ph5">`rx_set_compute_context`</ph><ept id="p4">](rx-set-compute-context.md)</ept>.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>