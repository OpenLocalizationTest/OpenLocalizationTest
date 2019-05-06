<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-distributed-computing-foreach.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750120ee56f9367962b216cd72dda4e438d517b92a9.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">120ee56f9367962b216cd72dda4e438d517b92a9</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-distributed-computing-foreach.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Using foreach and iterators (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>High level guide to using foreach and iterators packages.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Using foreach and iterators for manual parallel execution</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Although RevoScaleR performs parallel execution automatically, you can manage parallel execution yourself using the open-source <bpt id="p1">[</bpt>foreach package<ept id="p1">](https://CRAN.R-project.org/package=foreach)</ept>.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>This package provides a looping structure for R script.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>When you need to loop through repeated operations, and you have multiple processors or nodes to work with, you can use <bpt id="p1">**</bpt>foreach<ept id="p1">**</ept> in your script to execute a for loop in parallel.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Developed by Microsoft, foreach is an open-source package that is bundled with Machine Learning Server but is also available on the Comprehensive R Archive Network, CRAN.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>One common approach to parallelization is to see if the iterations within a loop can be performed independently, and if so, you can try to run the iterations concurrently rather than sequentially.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>About the foreach package</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The foreach package is a set of tools that allow you to run virtually anything that can be expressed as a for-loop as a set of parallel tasks.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>One scenario is to run multiple simulations in parallel.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>As a simple example, consider the case of simulating 10000 coin flips, which can be done by sampling with replacement from the vector <ph id="ph1">`c(H, T)`</ph>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>To run this simulation 10 times sequentially, use foreach with the <ph id="ph1">`%do%`</ph> operator:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Comparing the foreach output with that of a similar <ph id="ph1">`for`</ph> loop shows one obvious difference: foreach returns a list containing the value returned by each computation.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>A <ph id="ph1">`for`</ph> loop, by contrast, returns only the value of its last computation, and relies on user-defined side effects to do its work.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>We can parallelize the operation immediately by replacing <ph id="ph1">`%do%`</ph> with <ph id="ph2">`%dopar%`</ph>:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>However, if we run this example, we see the following warning:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>To actually run in parallel, we need to have a “parallel backend” for foreach.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Parallel backends are discussed in the next section.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Parallel Backends</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>In order for loops coded with foreach to run in parallel, you must register a parallel backend to manage the execution of the loop.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Any type of mechanism for running code in parallel could potentially have a parallel backend written for it.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Currently, Machine Learning Server includes the <bpt id="p1">**</bpt>doParallel<ept id="p1">**</ept> backend; this uses the <bpt id="p2">**</bpt>parallel<ept id="p2">**</ept> package of R 2.14.0 or later to run jobs in parallel, using either of the component parallelization methods incorporated into the parallel package: SNOW-like functionality using socket connections, or multicore-like functionality using forking (on Linux only).</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The doParallel package is a parallel backend for foreach that is intended for parallel processing on a single computer with multiple cores or processors.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Additional parallel backends are available from CRAN:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>doMPI<ept id="p1">**</ept> for use with the Rmpi package</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>doRedis<ept id="p1">**</ept> for use with the rredis package</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>doMC<ept id="p1">**</ept> provides access to the multicore functionality of the parallel package</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>doSNOW<ept id="p1">**</ept> for use with the now superseded SNOW package.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>To use a parallel backend, you must first register it.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Once a parallel backend is registered, calls to <ph id="ph1">`%dopar%`</ph> run in parallel using the mechanisms provided by the parallel backend.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>However, the details of registering the parallel backends differ, so we consider them separately.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Using the doParallel parallel backend</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The parallel package of R 2.14.0 and later combines elements of snow and multicore; doParallel similarly combines elements of both doSNOW and doMC.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>You can register doParallel with a cluster, as with doSNOW, or with a number of cores, as with doMC.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>For example, here we create a cluster and register it:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Once you’ve registered the parallel backend, you’re ready to run foreac` code in parallel.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>For example, to see how long it takes to run 10,000 bootstrap iterations in parallel on all available cores, you can run the following code:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Getting information about the parallel backend</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>To find out how many workers foreach is going to use, you can use the getDoParWorkers function:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>This is a useful sanity check that you’re actually running in parallel.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>If you haven’t registered a parallel backend, or if your machine only has one core, <ph id="ph1">`getDoParWorkers`</ph> will return 1.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>In either case, don’t expect a speed improvement.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`getDoParWorkers`</ph> function is also useful when you want the number of tasks to be equal to the number of workers.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>You may want to pass this value to an iterator constructor, for example.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>You can also get the name and version of the currently registered backend:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Nesting Calls to foreach</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>An important feature of foreach is nesting operator <ph id="ph1">`%:%`</ph>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Like the <ph id="ph1">`%do%`</ph> and <ph id="ph2">`%dopar%`</ph> operators, it is a binary operator, but it operates on two foreach objects.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>It also returns a foreach object, which is essentially a special merger of its operands.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Let’s say that we want to perform a Monte Carlo simulation using a function called <ph id="ph1">`sim`</ph>.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`sim`</ph> function takes two arguments, and we want to call it with all combinations of the values that are stored in the vectors <ph id="ph2">`avec`</ph> and <ph id="ph3">`bvec`</ph>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The following doubly-nested <ph id="ph1">`for`</ph> loop does that.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>For testing purposes, the <ph id="ph1">`sim`</ph> function is defined to return $10 a + b$ (although an operation this trivial is not worth executing in parallel):</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>In this case, it makes sense to store the results in a matrix, so we create one of the proper size called <ph id="ph1">`x`</ph>, and assign the return value of <ph id="ph2">`sim`</ph> to the appropriate element of <ph id="ph3">`x`</ph> each time through the inner loop.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>When using foreach, we don’t create a matrix and assign values into it.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Instead, the inner loop returns the columns of the result matrix as vectors, which are combined in the outer loop into a matrix.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Here’s how to do that using the <ph id="ph1">`%:%`</ph> operator:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>This is structured very much like the nested <ph id="ph1">`for`</ph> loop.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The outer foreach is iterating over the values in “bvec”, passing them to the inner foreach, which iterates over the values in “avec” for each value of “bvec”.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Thus, the “sim” function is called in the same way in both cases.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The code is slightly cleaner in this version, and has the advantage of being easily parallelized.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>When parallelizing nested <ph id="ph1">`for`</ph> loops, there is always a question of which loop to parallelize.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>The standard advice is to parallelize the outer loop.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>This results in larger individual tasks, and larger tasks can often be performed more efficiently than smaller tasks.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>However, if the outer loop doesn’t have many iterations and the tasks are already large, parallelizing the outer loop results in a small number of huge tasks, which may not allow you to use all of your processors, and can also result in load-balancing problems.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>You could parallelize an inner loop instead, but that could be inefficient because you’re repeatedly waiting for all the results to be returned every time through the outer loop.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>And if the tasks and number of iterations vary in size, then it’s really hard to know which loop to parallelize.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>But in our Monte Carlo example, all of the tasks are completely independent of each other, and so they can all be executed in parallel.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>You really want to think of the loops as specifying a single stream of tasks.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>You just need to be careful to process all of the results correctly, depending on which iteration of the inner loop they came from.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>That is exactly what the <ph id="ph1">`%:%`</ph> operator does: it turns multiple <bpt id="p1">**</bpt>foreach<ept id="p1">**</ept> loops into a single loop.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>That is why there is only one <ph id="ph1">`%do%`</ph> operator in the example above.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>And when we parallelize that nested <bpt id="p1">**</bpt>foreach<ept id="p1">**</ept> loop by changing the <ph id="ph1">`%do%`</ph> into a <ph id="ph2">`%dopar%`</ph>, we are creating a single stream of tasks that can all be executed in parallel:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Of course, we’ll actually only run as many tasks in parallel as we have processors, but the parallel backend takes care of all that.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The point is that the <ph id="ph1">`%:%`</ph> operator makes it easy to specify the stream of tasks to be executed, and the <ph id="ph2">`.combine`</ph> argument to <bpt id="p1">**</bpt>foreach<ept id="p1">**</ept> allows us to specify how the results should be processed.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The backend handles executing the tasks in parallel.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>For more on nested <bpt id="p1">**</bpt>foreach<ept id="p1">**</ept> calls, see the vignette “Nesting <bpt id="p2">**</bpt>foreach<ept id="p2">**</ept> Loops” in the <bpt id="p3">**</bpt>foreach<ept id="p3">**</ept> package.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Using Iterators</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>An <bpt id="p1">&lt;span&gt;</bpt><bpt id="p2">*</bpt>iterator<ept id="p2">*</ept><ept id="p1">&lt;/span&gt;</ept> is a special type of object that generalizes the notion of a looping variable.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>When passed as an argument to a function that knows what to do with it, the iterator supplies a sequence of values.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>The iterator also maintains information about its state, in particular its current index.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`iterators`</ph> package includes a number of functions for creating iterators, the simplest of which is <ph id="ph2">`iter`</ph>, which takes virtually any R object and turns it into an iterator object.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>The simplest function that operates on iterators is the <ph id="ph1">`nextElem`</ph> function, which when given an iterator, returns the next value of the iterator.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>For example, here we create an iterator object from the sequence 1 to 10, and then use <ph id="ph1">`nextElem`</ph> to iterate through the values:</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>You can create iterators from matrices and data frames, using the <ph id="ph1">`by`</ph> argument to specify whether to iterate by row or column:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Iterators can also be created from functions, in which case the iterator can be an endless source of values:</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>For practical applications, iterators can be paired with <bpt id="p1">**</bpt>foreach<ept id="p1">**</ept> to obtain parallel results quite easily:</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Some Special Iterators</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The notion of an iterator is new to R, but should be familiar to users of languages such as Python.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`iterators`</ph> package includes a number of special functions that generate iterators for some common scenarios.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>For example, the <ph id="ph1">`irnorm`</ph> function creates an iterator for which each value is drawn from a specified random normal distribution:</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Similarly, the <ph id="ph1">`irunif`</ph>, <ph id="ph2">`irbinom`</ph>, and <ph id="ph3">`irpois`</ph> functions create iterators which draw their values from uniform, binomial, and Poisson distributions, respectively.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>(These functions use the standard R distribution functions to generate random numbers, and these are not necessarily useful in a distributed or parallel environment.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>When using random numbers with <bpt id="p1">**</bpt>foreach<ept id="p1">**</ept>, we recommend using the doRNG package to ensure independent random number streams on each worker.)</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>We can then use these functions just as we used <ph id="ph1">`irnorm`</ph>:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`icount`</ph> function returns an iterator that counts starting from one:</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Writing Iterators</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>There will be times when you need an iterator that isn’t provided by the <ph id="ph1">`iterators`</ph> package.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>That is when you need to write your own custom iterator.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Basically, an iterator is an S3 object whose base class is <ph id="ph1">`iter`</ph>, and has <ph id="ph2">`iter`</ph> and <ph id="ph3">`nextElem`</ph> methods.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>The purpose of the <ph id="ph1">`iter`</ph> method is to return an iterator for the specified object.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>For iterators, that usually just means returning itself, which seems odd at first.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>But the <ph id="ph1">`iter`</ph> method can be defined for other objects that don’t define a <ph id="ph2">`nextElem`</ph> method.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>We call those objects <bpt id="p1">&lt;span&gt;</bpt><bpt id="p2">*</bpt>iterables<ept id="p2">*</ept><ept id="p1">&lt;/span&gt;</ept>, meaning that you can iterate over them.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`iterators`</ph> package defines <ph id="ph2">`iter`</ph> methods for vectors, lists, matrices, and data frames, making those objects iterables.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>By defining an <ph id="ph1">`iter`</ph> method for iterators, they can be used in the same context as an iterable, which can be convenient.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>For example, the <bpt id="p1">**</bpt>foreach<ept id="p1">**</ept> function takes iterables as arguments.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>It calls the <ph id="ph1">`iter`</ph> method on those arguments in order to create iterators for them.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>By defining the <ph id="ph1">`iter`</ph> method for all iterators, we can pass iterators to <bpt id="p1">**</bpt>foreach<ept id="p1">**</ept> that we created using any method we choose.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Thus, we can pass vectors, lists, or iterators to <bpt id="p1">**</bpt>foreach<ept id="p1">**</ept>, and they are all processed by <bpt id="p2">**</bpt>foreach<ept id="p2">**</ept> in exactly the same way.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`iterators`</ph> package comes with an <ph id="ph2">`iter`</ph> method defined for the <ph id="ph3">`iter`</ph> class that simply returns itself.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>That is usually all that is needed for an iterator.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>However, if you want to create an iterator for some existing class, you can do that by writing an <ph id="ph1">`iter`</ph> method that returns an appropriate iterator.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>That will allow you to pass an instance of your class to <bpt id="p1">**</bpt>foreach<ept id="p1">**</ept>, which will automatically convert it into an iterator.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>The alternative is to write your own function that takes arbitrary arguments, and returns an iterator.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>You can choose whichever method is most natural.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>The most important method required for iterators is <ph id="ph1">`nextElem`</ph>.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>This simply returns the next value, or throws an error.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Calling the <ph id="ph1">`stop`</ph> function with the string <ph id="ph2">`StopIteration`</ph> indicates that there are no more values available in the iterator.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>In most cases, you don’t actually need to write the <ph id="ph1">`iter`</ph> and <ph id="ph2">`nextElem`</ph> methods; you can inherit them.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>By inheriting from the class <ph id="ph1">`abstractiter`</ph>, you can use the following methods as the basis of your own iterators:</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>The following function creates a simple iterator that uses these two methods:</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Note that we called the internal function <ph id="ph1">`nextEl`</ph> rather than <ph id="ph2">`nextElem`</ph> to avoid masking the standard <ph id="ph3">`nextElem`</ph> generic function.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>That causes problems when you want your iterator to call the <ph id="ph1">`nextElem`</ph> method of another iterator, which can be quite useful.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>We create an instance of this iterator by calling the <ph id="ph1">`iforever`</ph> function, and then use it by calling the <ph id="ph2">`nextElem`</ph> method on the resulting object:</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Notice that it doesn’t make sense to implement this iterator by defining a new <ph id="ph1">`iter`</ph> method, since there is no natural iterable on which to dispatch.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>The only argument that we need is the object for the iterator to return, which can be of any type.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>Instead, we implement this iterator by defining a normal function that returns the iterator.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>This iterator is quite simple to implement, and possibly even useful, but exercise caution if you use it.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Passing it to <bpt id="p1">**</bpt>foreach<ept id="p1">**</ept> will result in an infinite loop unless you pair it with a finite iterator.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Similarly, never pass this iterator to <ph id="ph1">`as.list`</ph> without the <ph id="ph2">`n`</ph> argument.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>The iterator returned by <ph id="ph1">`iforever`</ph> is a list that has a single element named <ph id="ph2">`nextElem`</ph>, whose value is a function that returns the value of <ph id="ph3">`x`</ph>.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Because we are subclassing <ph id="ph1">`abstractiter`</ph>, we inherit a <ph id="ph2">`nextElem`</ph> method that will call this function, and because we are subclassing <ph id="ph3">`iter`</ph>, we inherit an <ph id="ph4">`iter`</ph> method that will return itself.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Of course, the reason this iterator is so simple is because it doesn’t contain any state.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Most iterators need to contain some state, or it will be difficult to make it return different values and eventually stop.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Managing the state is usually the real trick to writing iterators.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>As an example of writing a stateful iterator, let’s modify the previous iterator to put a limit on the number of values that it returns.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>We’ll call the new function <ph id="ph1">`irep`</ph>, and give it another argument called <ph id="ph2">`times`</ph>:</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Now let’s try it out:</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>The real difference between <ph id="ph1">`iforever`</ph> and <ph id="ph2">`irep`</ph> is in the function that gets called by the <ph id="ph3">`nextElem`</ph> method.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>This function not only accesses the values of the variables <ph id="ph1">`x`</ph> and <ph id="ph2">`times`</ph>, but it also modifies the value of <ph id="ph3">`times`</ph>.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>This is accomplished by means of the <ph id="ph1">`&lt;&lt;-`</ph> operator, and the magic of lexical scoping.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Technically, this kind of function is called a <bpt id="p1">&lt;span&gt;</bpt><bpt id="p2">*</bpt>closure<ept id="p2">*</ept><ept id="p1">&lt;/span&gt;</ept>, and is a somewhat advanced feature of <ph id="ph1">`R`</ph>.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>The important thing to remember is that <ph id="ph1">`nextEl`</ph> is able to get the value of variables that were passed as arguments to <ph id="ph2">`irep`</ph>, and it can modify those values using the <ph id="ph3">`&lt;&lt;-`</ph> operator.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>These are <bpt id="p1">&lt;span&gt;</bpt><bpt id="p2">*</bpt>not<ept id="p2">*</ept><ept id="p1">&lt;/span&gt;</ept> global variables: they are defined in the enclosing environment of the <ph id="ph1">`nextEl`</ph> function.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>You can create as many iterators as you want using the <ph id="ph1">`irep`</ph> function, and they will all work as expected without conflicts.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Note that this iterator only uses the arguments to <ph id="ph1">`irep`</ph> to store its state.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>If any other state variables are needed, they can be defined anywhere inside the <ph id="ph1">`irep`</ph> function.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>More examples of writing iterators can be found in the vignette “Writing Custom Iterators” in the <ph id="ph1">`iterators`</ph> package.</source>
        </trans-unit></group></body></file></xliff>