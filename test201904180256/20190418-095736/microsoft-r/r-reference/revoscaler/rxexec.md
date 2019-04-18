<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxexec.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c02e398b69f3435759fc6bd86a07d4c39451bc51f.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">02e398b69f3435759fc6bd86a07d4c39451bc51f</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxexec.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxExec function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Allows distributed execution of a function in parallel across nodes (computers) or cores  of a compute context such as a cluster.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxExec, IO</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxExec:  Run A Function on Multiple Nodes or Cores</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Allows distributed execution of a function in parallel across nodes (computers) or cores of a "compute context" such as a cluster.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>the function to be executed; the nodes or cores on which it is run are determined by the currently-active compute context and by the other arguments of <bpt id="p1">[</bpt>rxExec<ept id="p1">](rxExec.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>arguments passed to the function <ph id="ph1">`FUN`</ph> each time it is executed.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Separate argument values can be sent for each computation by wrapping a vector or list of argument values in <bpt id="p1">[</bpt>rxElemArg<ept id="p1">](rxElemArg.md)</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>a vector or list specifying arguments to <ph id="ph1">`FUN`</ph>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>This allows a different set of arguments to be passed to <ph id="ph1">`FUN`</ph> each time it is executed.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The length of the vector or list must match the number of times the function will  be executed.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Each of these elements will be passed in turn  to <ph id="ph1">`FUN`</ph>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Using a list of lists allows multiple named or unnamed parameters to be passed.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`elemArgs`</ph> has length 1, that argument is passed to all compute  elements (and thus is an alternative to  ...). The elements of <ph id="ph2">`elemArgs`</ph> may be named; if they are node names those elements will be passed to those nodes.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Alternatively, they can be "rxElem1", "rxElem2" and so on.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>In this case, the list of returned values will have those corresponding names.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>See the Details section for more information.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>This is an alternative to using <bpt id="p1">[</bpt>rxElemArg<ept id="p1">](rxElemArg.md)</ept> one or more times.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>[Deprecated].</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The distributed computing mode to be used.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>This parameter is currently deprecated and is not honored by any of the supported compute contexts.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>It might come back to use in the future.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> and <ph id="ph2">`elemType="nodes"`</ph>, <ph id="ph3">`FUN`</ph> will be run exactly once on each specified node.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>In this case, each element of the return list will be named with the name of the node that computed that element.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, a node may  be used more than once (but never simultaneously).</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`oncePerElem`</ph> must be set to <ph id="ph2">`FALSE`</ph>if <ph id="ph3">`elemType="cores"`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>This parameter is ignored if the active compute context is local.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>integer specifying the total number of instances of the function  <ph id="ph1">`FUN`</ph> to run.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`timesToRun=-1`</ph>, the default, then times is set to the  length of the <ph id="ph2">`elemArgs`</ph> argument, if it exists, else to the number of nodes or cores specified in the compute context object, if that is exact.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>In the latter case, if the <ph id="ph1">`elemType="nodes"`</ph> and a single set of arguments is being passed to each node, each  element of the return list will be named with the name of the node that computed that element.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`timesToRun`</ph> is not -1, it must be consistent with this other information.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>optional character vector specifying additional packages to be  loaded on the nodes for this job.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If provided, these packages are loaded after any <ph id="ph1">`packagesToLoad`</ph> specified in the current distributed compute context.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>optional character vector specifying additional objects to be  exported to the nodes for this job, or an environment containing these objects.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The specified objects are added to <ph id="ph1">`FUN`</ph>'s environment, unless that environment is locked, in which case they are added to the environment in which <ph id="ph2">`FUN`</ph> is evaluated.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>For purposes of efficiency, this argument should not be used for exporting large data  objects.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Passing large data through reference to a shared storage location (e.g., HDFS) is recommended.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>optional integer scalar specifying the number of tasks to be executed per compute element, or worker.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>By submitting tasks in chunks, you can avoid some of the overhead of starting new R processes over and over.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>For example, if you are running thousands of identical simulations on a cluster,  it makes sense to specify the <ph id="ph1">`taskChunkSize`</ph> so that each  worker can do its allotment of tasks in a single R process.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>This argument is incompatible with the <ph id="ph1">`oncePerElem`</ph> argument; if both are supplied, this one is ignored.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>It is also incompatible with lists supplied to <ph id="ph1">`elemArgs`</ph> with compute element names.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, underlying calls to <ph id="ph2">`do.call`</ph> have the corresponding flag set to <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>This is primarily of use to the <bpt id="p1">**</bpt>doRSR<ept id="p1">**</ept> package, but may be of use to other users.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or logical value.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the console output from the  all of the processes is printed to the user console.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Note that the output from different nodes or cores may be interleaved in an unpredictable way.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>,  no console output is displayed.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Output can be retrieved with the function  <bpt id="p1">[</bpt>rxGetJobOutput<ept id="p1">](rxGetJobOutput.md)</ept> for a non-waiting job.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If not <ph id="ph1">`NULL`</ph>,  this flag overrides the  value set in the compute context when the job was submitted.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>,  the setting in the compute context will be used.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>This parameter is ignored  if the active compute context is local.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or logical value.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, artifacts created by the distributed  computing job are deleted when the results are returned or retrieved using <bpt id="p1">[</bpt>rxGetJobResults<ept id="p1">](rxGetJobResults.md)</ept>.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, the artifacts are not deleted,  and the results may be obtained repeatedly using <bpt id="p1">[</bpt>rxGetJobResults<ept id="p1">](rxGetJobResults.md)</ept>,  and the console output via <bpt id="p2">[</bpt>rxGetJobOutput<ept id="p2">](rxGetJobOutput.md)</ept> until  <bpt id="p3">[</bpt>rxCleanupJobs<ept id="p3">](rxCleanup.md)</ept> is used to delete the artifacts.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>If not <ph id="ph1">`NULL`</ph>, this flag overrides  the value set in the compute context when the job was submitted.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>If you routinely  set <ph id="ph1">`autoCleanup=FALSE`</ph>, you may eventually fill your hard disk with  compute artifacts.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>If you set <ph id="ph1">`autoCleanup=TRUE`</ph> and experience performance degradation on a Windows XP client, consider setting <ph id="ph2">`autoCleanup=FALSE`</ph>.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>This  parameter is ignored if the active compute context is local.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or logical value.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the default, then if an individual instance of a job fails due to a hardware or network failure, an attempt will be made to rerun that job.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>(R syntax errors, however, will cause immediate failure as usual.) Furthermore, should a process instance of a job fail due to a user code failure, the rest of the processes will continue,  and the failed process will produce a warning when the output is collected.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Additionally, the position  in the returned list where the failure occured will contain the error as opposed to a result.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>This  parameter is ignored if the active compute context is local or <ph id="ph1">`RxForeachDoPar`</ph>.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph>, the string <ph id="ph2">`"auto"`</ph>, or an integer to be used as the seed for parallel random number generation.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>See the Details section for a description of how the <ph id="ph1">`"auto"`</ph> string is used.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or a character string specifying the type of random number generator to be used.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Allowable strings are the strings accepted by <bpt id="p1">[</bpt>rxRngNewStream<ept id="p1">](rxRng.md)</ept>, <ph id="ph1">`"auto"`</ph>, and, if the active compute context is local parallel, <ph id="ph2">`"L'Ecuyer-CMRG"`</ph> (for compatibility with the parallel package).</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>See the Details section for a description of how the <ph id="ph1">`"auto"`</ph> string is used.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or a list containing options to be passed to the foreach parallel computing backend.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>See foreach for details.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxExec`</ph> has very limited functionality for <ph id="ph2">`RxInSqlServer`</ph> for CTP3; computations are performed sequentially.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>There are two primary sets of use cases:  In the first set, each computing element (node or core) gets the same argument values; in this case, do not use <ph id="ph1">`elemArgs`</ph> or <ph id="ph2">`rxElemArg`</ph>.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>In the second, each element gets a different set of arguments; use <bpt id="p1">[</bpt>rxElemArg<ept id="p1">](rxElemArg.md)</ept> for each argument that has different values, or an <ph id="ph1">`elemArgs`</ph> whose length is equal to the number of times <ph id="ph2">`FUN`</ph> will be executed.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Set 1 (All computing elements get the same arguments):<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>1 <ph id="ph1">`rxExec(FUN, arg1, arg2)`</ph></source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Set 2: Every computing element gets a different set of arguments.<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">[</bpt>rxElemArg<ept id="p1">](rxElemArg.md)</ept> is used, the length of the vector or list for the enclosed argument must equal the number of compute elements.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>For example,</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`elemArgs`</ph> is a nested list, the individual lists are passed to the compute resources according to the following:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>1 The argument lists can be named according to which compute resource each component list should be assigned.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rxExec(FUN, elemArgs=list(compute1=list(arg1,arg2), compute2=list(arg3, arg4)))`</ph>.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>In this case, the list of arguments must be the same length as the list of nodes requested for the current compute context, and have the same names.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`oncePerElem=TRUE`</ph> and <ph id="ph2">`elemType="nodes"`</ph>, then the computation will be performed once on each requested node, and each node is assured of getting the argument with its name.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`oncePerElem=FALSE`</ph>, there is no guarantee that each node will be used in the processing, so arguments intended for a particular node may not be used; they must still be provided, however.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>The component names must be valid R syntactic names.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>If you have nodes on your cluster with names that are not valid R syntactic names, use the function <bpt id="p1">[</bpt>rxMakeRNodeNames<ept id="p1">](rxMakeRNodeNames.md)</ept> on the node name to determine the appropriate name to give the list component.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>When the return value is a list with elements named by compute node, the node names are as returned by the <bpt id="p1">[</bpt>rxMakeRNodeNames<ept id="p1">](rxMakeRNodeNames.md)</ept> function.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>1 The arguments lists, if not named, will be passed to the compute resources allowed by the compute context according to their position in the list.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>This is useful when you don't care which nodes or cores the function is executed on but want different arguments to be executed on each resource.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rxExec(FUN, elemArgs=list(list(arg1,arg2), list(arg3, arg4)))`</ph> or <ph id="ph2">`rxExec(FUN, elemArgs=list(c(arg1, arg2), list(arg3, arg4)))`</ph></source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>The arguments <ph id="ph1">`RNGseed`</ph> and <ph id="ph2">`RNGkind`</ph> can be used to control random number generation in the workers.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>By default, both are <ph id="ph1">`NULL`</ph> and no special random number control is used.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>If either or both <ph id="ph1">`RNGseed`</ph> and <ph id="ph2">`RNGkind`</ph> are set to <ph id="ph3">`"auto"`</ph>, a parallel random number stream is initialized on each worker, using the <ph id="ph4">`"MT2203"`</ph> generator and separate substreams for each worker.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>If other non-null valid values are supplied for these arguments, they are used as is for the <ph id="ph1">`"MT2203"`</ph> generator, which supports multiple substreams, but for other <ph id="ph2">`rxRngNewStream`</ph>-supported generators, the seed will be used as the starting point of a sequence of seeds, one for each worker.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>In the special case of a local parallel compute context, the <ph id="ph1">`"L'Ecuyer-CMRG"`</ph> generator case can be specified, in which case the parallel package's <ph id="ph2">`clusterSetRNGStream`</ph> function is called on the internally generated parallel cluster.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>If a waiting compute context is active, a list with an element for each job, where each element contains the value(s) returned by that job's function call(s).</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>If a non-waiting compute context is active, a jobInfo object.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxGetJobResults<ept id="p1">](rxGetJobResults.md)</ept>.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxElemArg<ept id="p1">](rxElemArg.md)</ept>, <bpt id="p2">[</bpt>rxGetJobResults<ept id="p2">](rxGetJobResults.md)</ept>, <bpt id="p3">[</bpt>rxGetJobStatus<ept id="p3">](rxGetJobResults.md)</ept>, <bpt id="p4">[</bpt>RxComputeContext<ept id="p4">](RxComputeContext.md)</ept>, <bpt id="p5">[</bpt>rxSetComputeContext<ept id="p5">](rxSetComputeContext.md)</ept>, <bpt id="p6">[</bpt>RxSpark<ept id="p6">](RxSpark.md)</ept>, RxHadoopMR, <bpt id="p7">[</bpt>RxForeachDoPar<ept id="p7">](RxForeachDoPar.md)</ept>, <bpt id="p8">[</bpt>RxLocalParallel<ept id="p8">](RxLocalParallel.md)</ept>, <bpt id="p9">[</bpt>RxLocalSeq<ept id="p9">](RxLocalSeq.md)</ept>, <bpt id="p10">[</bpt>rxGetNodeInfo<ept id="p10">](rxGetNodeInfo.md)</ept>, <bpt id="p11">[</bpt>rxMakeRNodeNames<ept id="p11">](rxMakeRNodeNames.md)</ept><ph id="ph1">
</ph><bpt id="p12">[</bpt>rxRngNewStream<ept id="p12">](rxRng.md)</ept></source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>