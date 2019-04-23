<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-distributed-computing-parallel-jobs.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338ab199d167a0b22af225eb27ce566df43f148682b9.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">b199d167a0b22af225eb27ce566df43f148682b9</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-distributed-computing-parallel-jobs.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Running jobs in parallel using rxExec</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Run jobs in parallele using the rxExec function in the RevoScaleR library.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Running jobs in parallel using rxExec</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>RevoScaleR<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept> functions are engineered to execute in parallel automatically.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>However, if you require a custom implementation, you can use <bpt id="p1">[</bpt>rxExec<ept id="p1">](~/r-reference/revoscaler/rxexec.md)</ept> to manually construct and manage a distributed workload.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>With rxExec, you can take an arbitrary function and run it in parallel on your distributed computing resources in Hadoop.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>This in turn allows you to tackle a wide variety of parallel computing problems.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This article provides comprehensive steps on how to use rxExec, starting with examples showcasing rxExec in a variety of use cases.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Examples using rxExec</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>To demonstrate rxExec usage, this article provides several examples:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Simulate a dice-rolling game</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Determine the probability that any two persons in a given group size share a birthday</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Create a plot of the Mandelbrot set</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Perform naive k-means clustering</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>In general, the only required arguments to rxExec are the function to be run and any required arguments of that function.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Additional optional arguments can be used to control the computation.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Before trying the examples, be sure that your <bpt id="p1">[</bpt>compute context<ept id="p1">](how-to-revoscaler-distributed-computing-compute-context.md)</ept> is set with the option <bpt id="p2">*</bpt>wait=TRUE<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Playing Dice: A Simulation</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>A familiar casino game consists of rolling a pair of dice.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If you roll a 7 or 11 on your initial roll, you win.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If you roll 2, 3, or 12, you lose.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Roll a 4, 5, 6, 8, 9, or 10, NS that number becomes your <bpt id="p1">*</bpt>point<ept id="p1">*</ept> and you continue rolling until you either roll your point again (in which case you win) or roll a 7, in which case you lose.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The game is easily simulated in R using the following function:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Using rxExec, you can invoke thousands of games to help determine the probability of a win.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Using a Hadoop 5-node cluster, we play the game 10000 times, 2000 times on each node:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>We expect approximately 4929 wins in 10000 trials, and our result of 4913 wins is close.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The Birthday Problem</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The birthday problem is an old standby in introductory statistics classes because its result seems counterintuitive.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>In a group of about 25 people, the chances are better than 50-50 that at least two people in the room share a birthday.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Put 50 people in a room and you are practically guaranteed there is a birthday-sharing pair.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Since 50 is so much less than 365, most people are surprised by this result.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>We can use the following function to estimate the probability of at least one birthday-sharing pair in groups of various sizes (the first line of the function is what allows us to obtain results for more than one value at a time; the remaining calculations are for a single n):</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>We can test that it works in a sequential setting, estimating the probability for group sizes 3, 25, and 50 as follows:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>For each group size, 5000 random tests were performed.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For this run, the following results were returned:</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Make sure your compute context is set to a “waiting” context.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Then distribute this computation for groups of 2 to 100 using <ph id="ph1">`rxExec`</ph> as follows, using <bpt id="p1">*</bpt>rxElemArg<ept id="p1">*</ept> to specify a different argument for each call to pbirthday, and then using the <bpt id="p2">*</bpt>taskChunkSize<ept id="p2">*</ept> argument to pass these arguments to the nodes in chunks of 20:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The results are returned in a list, with one element for each node.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>We can use <bpt id="p1">*</bpt>unlist<ept id="p1">*</ept> to convert the results into a single vector:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>We can make a colorful plot of the results by constructing variables for the party sizes and the nodes where each computation was performed:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The resulting plot is shown as follows:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Birthday Problem Plot</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Plotting the Mandelbrot Set</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Computing the Mandelbrot set is a popular parallel computing example because it involves a simple computation performed independently on an array of points in the complex plane.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>For any point <bpt id="p1">*</bpt>z=x+yi<ept id="p1">*</ept> in the complex plane, <bpt id="p2">*</bpt>z<ept id="p2">*</ept> belongs to the Mandelbrot set if and only if <bpt id="p3">*</bpt>z<ept id="p3">*</ept> remains bounded under the iteration <bpt id="p4">*</bpt>z_(n+1)=z_n^2+z_n<ept id="p4">*</ept>.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If we are associating a point (<bpt id="p1">*</bpt>x_0,y_0<ept id="p1">*</ept>) in the plane with a pixel on a computer screen, the following R function returns the number of iterations before the point becomes unbounded, or the maximum number of iterations.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If the maximum number of iterations is returned, the point is assumed to be in the set:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The following function retains the basic computation but returns a vector of results for a given y value:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>We can then distribute this computation by computing several rows at a time on each compute resource.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>In the following, we create an input x vector of length 240, a y vector of length 240, and specify the iteration limit as 100.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>We then call <ph id="ph1">`rxExec`</ph> with our <bpt id="p1">*</bpt>vmandelbrot<ept id="p1">*</ept> function, giving 1/5 of the y vector to each computational node in our five node HPC Server cluster.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>This should be done in a compute context with <bpt id="p1">*</bpt>wait=TRUE<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Finally, we put the results into a 240x240 matrix and create an image plot that shows the familiar Mandelbrot set:</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The resulting plot is shown as follows (not all graphics devices support the useRaster argument; if your plot is empty, try omitting that argument):</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Mandelbrot Plot</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Naïve Parallel k-Means Clustering</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept><ph id="ph1"> </ph>has a built-in analysis function,<ph id="ph2"> `rxKmeans`</ph>, to perform distributed k-means, but in this section we see how the regular R kmeans function can be put to use in a distributed context.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>The kmeans function implements several<bpt id="p1"> *</bpt>iterative relocation<ept id="p1">*</ept><ph id="ph1"> </ph>algorithms for clustering.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source> An iterative relocation algorithm starts from an initial classification and then iteratively moves data points from one cluster to another to reduce sums of squares.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source> One possible starting point is to pick cluster centers at random and then assign points to each cluster so that the sum of squares is minimized.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source> If this procedure is repeated many times for different sets of centers, the set with the smallest error can be chosen.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>We can do this with the ordinary kmeans function, which has a parameter<bpt id="p1"> *</bpt>nstart<ept id="p1">*</ept><ph id="ph1"> </ph>that tells it how many times to pick the starting centers, and also to pick the set of centers that returns a result with smallest error: <ph id="ph2">    </ph>x &lt;- matrix(rnorm(250000), nrow = 5000, ncol = 50) <ph id="ph3">    </ph>system.time(kmeans(x, centers=10, iter.max = 35, nstart = 400))</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>On a Dell XPS laptop with 8 GB of RAM, this takes about a minute and a half.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>To parallelize this computation efficiently, we should do the following:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>- Pass the data to a specified number of computing resources once.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>- Split the work into smaller tasks for passing to each computing resource.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>- Combine the results from all the computing resources so the best result is returned.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>In the case of<bpt id="p1"> *</bpt>kmeans<ept id="p1">*</ept>, we can ask for the computations to be done by<bpt id="p2"> *</bpt>cores<ept id="p2">*</ept>, rather than by<bpt id="p3"> *</bpt>nodes<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source> Because we are distributing the computation, we can do fewer repetitions (<bpt id="p1">*</bpt>nstarts<ept id="p1">*</ept>) on each compute element.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source> We can do all of this with the following function (again, this should be run with a compute context for which<bpt id="p1"> *</bpt>wait=TRUE<ept id="p1">*</ept>):</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>kMeansRSR &lt;- function(x, centers=5, iter.max=10, nstart=1) <ph id="ph1">    </ph>{ <ph id="ph2">        </ph>numTimes &lt;- 20 <ph id="ph3">        </ph>results &lt;- rxExec(FUN = kmeans, x=x, centers=centers, iter.max=iter.max, <ph id="ph4">            </ph>nstart=nstart, timesToRun=numTimes) <ph id="ph5">        </ph>best &lt;- 1 <ph id="ph6">        </ph>bestSS &lt;- sum(results[[1]]$withinss) <ph id="ph7">        </ph>for (j in 1:numTimes) <ph id="ph8">        </ph>{ <ph id="ph9">              </ph>jSS &lt;- sum(results[[j]]$withinss) <ph id="ph10">              </ph>if (bestSS &gt; jSS) <ph id="ph11">              </ph>{ <ph id="ph12">                      </ph>best &lt;- j <ph id="ph13">                     </ph>bestSS &lt;- jSS <ph id="ph14">              </ph>} <ph id="ph15">        </ph>} <ph id="ph16">        </ph>results[[best]] <ph id="ph17">    </ph>}</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Notice that in our<bpt id="p1"> *</bpt>kMeansRSR<ept id="p1">*</ept><ph id="ph1"> </ph>function we are letting the underlying<bpt id="p2"> *</bpt>kmeans<ept id="p2">*</ept><ph id="ph2"> </ph>function find nstart sets of centers per call and the choice of "best" is done in our function after we have called<bpt id="p3"> *</bpt>kmeans numTimes<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source> No parallelization is done to<bpt id="p1"> *</bpt>kmeans<ept id="p1">*</ept><ph id="ph1"> </ph>itself.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>With our<bpt id="p1"> *</bpt>kMeansRSR<ept id="p1">*</ept><ph id="ph1"> </ph>function, we can then repeat the computation from before: <ph id="ph2">    </ph>system.time(kMeansRSR(x, 10, 35, 20))</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>With our 5-node HPC Server cluster, this reduces the time from a minute and a half to about 15 seconds.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Share data across parallel processes</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Data can be shared between rxExec parallel processes by copying it to the environment of each process through the <ph id="ph1">`execObjects`</ph> option to rxExec, or by specifying the data as arguments to each function call.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>For small data, this works well but as the data objects get larger this can create a significant performance penalty due to the time needed to do the copy.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>In such cases, it can be much more efficient to share the data by storing it in a location accessible by each of the parallel processes, such as a local or network file share.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The following example shows how this can be done when parallelizing the computation of statistics on subsets of a larger data table.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>We’ll start by creating some sample data using the <bpt id="p1">**</bpt>data.table<ept id="p1">**</ept> package.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Next we’ll setup for use of the <bpt id="p1">**</bpt>doParallel<ept id="p1">**</ept> backend.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Now we create a function for computing statistics on a selected subset of the data table by passing in both the data table and the tag value to subset by.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>We’ll then run the function using rxExec for each tag value.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>To see the impact of sharing the file via a common storage location rather than passing it to each parallel process we’ll save the data table into an RDS file, which is an efficient way of storing individual R objects, create a new version of the function that reads the data table from the RDS file, and then rerun rxExec using the new function.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Although results may vary, in this case we’ve reduced the elapsed time by 50% by sharing the data table rather than passing it as an in-memory object to each parallel process.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Parallel Random Number Generation</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>When generating random numbers in parallel computation, a frequent problem is the possibility of highly correlated random number streams.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>High-quality parallel random number generators avoid this problem.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>RevoScaleR includes several high-quality parallel random number generators and these can be used with <ph id="ph1">`rxExec `</ph>to improve the quality of your parallel simulations.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>By default, a parallel version of the Mersenne-Twister random number generator is used that supports 6024 separate substreams.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>We can set it to work on our dice example by setting a non-null seed:</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>This makes our simulation repeatable:</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>This random number generator can be asked for explicitly by specifying RNGkind="MT2203":</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>We can build reproducibility into our naïve k-means example as follows:</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>To obtain the default random number generators without setting a seed, specify "auto" as the argument to either RNGseed or RNGkind:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>To verify that we are actually getting uncorrelated streams, we can use runif within rxExec to generate a list of vectors of random vectors, then use the cor function to measure the correlation between vectors:</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Correlations are above 0.3; in repeated runs of the code, the maximum correlation seldom exceeded 0.1.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Because the MT2203 generator offers such a rich array of substreams, we recommend its use.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>You can, however, use several other generators, all from Intel’s Vector Statistical Library, a component of the Intel Math Kernel Library.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>The available generators are as follows: "MCG31", "R250", "MRG32K3A", "MCG59", "MT19937", "MT2203", "SFMT19937" (all of which are pseudo-random number generators that can be used to generate uncorrelated random number streams) plus "SOBOL" and "NIEDERR", which are quasi-random number generators that do not generate uncorrelated random number streams.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Detailed descriptions of the available generators can be found in the <bpt id="p1">[</bpt>Vector Statistical Library Notes<ept id="p1">](http://software.intel.com/sites/products/documentation/doclib/mkl_sa/11/vslnotes/vslnotes.pdf)</ept>.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>About reproducibility</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>For distributed compute contexts, rxExec starts the random number streams on a per-worker basis; if there are more tasks than workers, you may not obtain completely reproducible results because different tasks may be performed by randomly chosen workers.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>If you need completely reproducible results, you can use the taskChunkSize argument to force the number of task <bpt id="p1">*</bpt>chunks<ept id="p1">*</ept> to be less than or equal to the number of workers.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>This will ensure that each chunk of tasks is performed on a single random number stream.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>You can also define a custom function that includes random number generation control within it; this moves the random number control into each task.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>See the help file for rxRngNewStream for details.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>Work with results from non-blocking jobs</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>So far, all of our examples have required a blocking, or waiting, compute context so that we could make immediate use of the results returned by rxExec.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>However some computations are so time consuming that it is not practical to wait on the results.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>In such cases, it is probably best to divide your analysis into two or more pieces, one of which can be structured as a non-blocking job, and then use the pending job (or more usefully, the job results, when available) as input to the remaining pieces.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>For example, let’s return to the birthday example, and see how to restructure our analysis to use a non-blocking job for the distributed computations.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>The pbirthday function itself requires no changes, and our variable specifying the number of ntests can be used as is:</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>However, when we call rxExec, the return object will no longer be the results list, but a jobInfo object:</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>We check the job status:</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>We can then proceed almost as before:</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>The other examples are a bit trickier, in that the result of the calls to rxExec were embedded in functions.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>But again, dividing the computations into distributed and non-distributed components can help—the distributed computations can be non-blocking, and the non-distributed portions can then be applied to the results.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Thus the kmeans example can be rewritten thus:</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>To run this in our non-blocking cluster context, we do the following:</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Once we see that z’s job status is “finished”, we can run findKmeansBest on the results:</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Call RevoScaleR HPA functions with rxExec</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>To this point, none of the functions we have called with rxExec has been a RevoScaleR function, because the intent has been to show how rxExec can be used to address the large class of traditional high-performance computing problems.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>However, there is no inherent reason why rxExec cannot be used with RevoScaleR’s high performance analysis (HPA) functions, and many times it can be useful to do so.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>For example, if you are running a cluster on which every node has two or more cores, you can use rxExec to start an independent analysis on each node, and each of those analyses can take advantage of the multiple cores on its node.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>The following simulation simulates data from a Poisson distribution and then fits a generalized linear model to the simulated data:</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>If we call the above function with rxExec on a five-node cluster compute context, we get five simulations running simultaneously, and can easily produce 1000 simulations as follows:</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>It is important to recognize the distinction between running an HPA function with a distributed compute context, and calling an HPA function using rxExec with a distributed compute context.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>In the former case, we are fitting just one model, using the distributed compute context to farm out portions of the computations, but ultimately returning just one model object.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>In the latter case, we are calculating one model per task, the tasks being farmed out to the various nodes or cores as desired, and a list of models is returned.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Use rxExec in the local compute context</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>By default, if you call <ph id="ph1">`rxExec`</ph> in the local compute context, your computation runS sequentially on your local machine.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>However, you can incorporate parallel computing on your local machine using the special compute context <ph id="ph1">`RxLocalParallel`</ph> as follows:</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>This allows the ParallelR package doParallel to distribute the computation among the available cores of your computer.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>If you are using random numbers in the local parallel context, be aware that <ph id="ph1">`rxExec`</ph> chooses a number of workers based on the number of tasks and the current value of <ph id="ph2">`rxGetOption("numCoresToUse")`</ph>.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>to guarantee each task runS with a separate random number stream, set <ph id="ph1">`rxOptions(numCoresToUse)`</ph> equal to the number of tasks, and explicitly set <bpt id="p1">*</bpt>timesToRun<ept id="p1">*</ept> to the number of tasks.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>For example, if we want a list consisting of five sets of uniform random numbers, we could do the following to obtain reproducible results:</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>numCoresToUse<ept id="p1">**</ept> is a scalar integer specifying the number of cores to use.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>If you set this parameter to either -1 or a value in excess of available cores, ScaleR uses however many cores are available.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Increasing the number of cores also increases the amount of memory required for ScaleR analysis functions.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>HPA functions are not affected by the <ph id="ph1">`RxLocalParallel`</ph> compute context; they run locally and in the usual internally distributed fashion when the <ph id="ph2">`RxLocalParallel`</ph> compute context is in effect.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Use rxExec with foreach back ends</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>If you do not have access to a Hadoop cluster or enterprise database, but do have access to a cluster via PVM, MPI, socket, or NetWorkSpaces connections or a multicore workstation, you can use <ph id="ph1">`rxExec`</ph> with an arbitrary foreach backend (doParallel, doSNOW, doMPI, etc.) Register your parallel backend as usual and then set your RevoScaleR compute context using the special compute context <ph id="ph2">`RxForeachDoPar`</ph>:</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>For example, here is how you might start a SNOW-like cluster connection with the doParallel back end:</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>You then call <ph id="ph1">`rxExec`</ph> as usual.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>The computations are automatically directed to the registered foreach back end.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>HPA functions are not usually affected by the <ph id="ph1">`RxForeachDoPar`</ph> compute context; they run locally and in the usual internally distributed fashion when the RxForeachDoPar compute context is in effect.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>The one exception is when HPA functions are called within <ph id="ph1">`rxExec`</ph>; in this case it is possible that the internal threading of the HPA functions can be affected by the launch mechanism of the parallel backend workers.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>The doMC backend and the multicore-like backend of doParallel both use forking to launch their workers; this is known to be incompatible with the HPA functions.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Control rxExec computations</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>As we have seen in these examples, there are several arguments to <ph id="ph1">`rxExec`</ph> that allow you to fine-tune your <ph id="ph2">`rxExec`</ph> commands.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>Both the birthday example and the Mandelbrot example used the <bpt id="p1">*</bpt>taskChunkSize<ept id="p1">*</ept> argument to specify how many tasks should go to each worker.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>The Mandelbrot example also used the <bpt id="p1">*</bpt>execObjects<ept id="p1">*</ept> argument, which can be used to pass either a character vector or an environment containing objects—the objects specified by the vector or contained in the environment are added to the environment of the function specified in the FUN argument, unless that environment is locked, in which case they are added to the parent frame in which <bpt id="p2">*</bpt>FUN<ept id="p2">*</ept> is evaluated.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>(If you use an environment, it should be one you create with <bpt id="p1">*</bpt>parent=emptyenv();<ept id="p1">*</ept> this allows you to pass only those objects you need to the function’s environment.) These two examples also show the use of <bpt id="p2">*</bpt>rxElemArg<ept id="p2">*</ept> in passing arguments to the workers.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>In the kmeans example, we covered the <bpt id="p1">*</bpt>timesToRun<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>packagesToLoad<ept id="p1">*</ept> argument allows you to specify packages to load on each worker.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>consoleOutput<ept id="p1">*</ept> and <bpt id="p2">*</bpt>autoCleanup<ept id="p2">*</ept> flags serve the same purpose as their counterparts in the compute context constructor functions—that is, they can be used to specify whether console output should be displayed or the associated task files should be cleaned up on job completion for an individual call to 'rxExec'.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Two additional arguments remain to be introduced: <bpt id="p1">*</bpt>oncePerElem<ept id="p1">*</ept> and <bpt id="p2">*</bpt>continueOnFailure<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>oncePerElem<ept id="p1">*</ept> argument restricts the called function to be run once per allotted node; this is frequently used with the <bpt id="p2">*</bpt>timesToRun<ept id="p2">*</ept> argument to ensure that each occurrence is run on a separate node.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>oncePerElem<ept id="p1">*</ept> argument, however, can only be set to <bpt id="p2">*</bpt>TRUE<ept id="p2">*</ept> if <bpt id="p3">*</bpt>elemType="nodes"<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>It must be set to <bpt id="p1">*</bpt>FALSE<ept id="p1">*</ept> if <bpt id="p2">*</bpt>elemType="cores"<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>oncePerElem<ept id="p1">*</ept> is <bpt id="p2">*</bpt>TRUE<ept id="p2">*</ept> and <bpt id="p3">*</bpt>elemType="nodes"<ept id="p3">*</ept>, <bpt id="p4">*</bpt>rxExec<ept id="p4">*</ept>’s results are returned in a list with components named by node.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>If a given node does not have a valid R syntactic name, its name is mangled to become a valid R syntactic name for use in the return list.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>continueOnFailure<ept id="p1">*</ept> argument is used to say that a computation should continue even if one or more of the compute elements fails for some reason; this is useful, for example, if you are running several thousand independent simulations and It doesn’t matter if you get results for all of them.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>Using <bpt id="p1">*</bpt>continueOnFailure=TRUE<ept id="p1">*</ept> (the default), you get results for all compute elements that finish the simulation and error messages for the compute elements that fail.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>The arguments <bpt id="p1">*</bpt>elemType<ept id="p1">*</ept>, <bpt id="p2">*</bpt>consoleOutput<ept id="p2">*</ept>, <bpt id="p3">*</bpt>autoCleanup<ept id="p3">*</ept>, <bpt id="p4">*</bpt>continueOnFailure<ept id="p4">*</ept>, and <bpt id="p5">*</bpt>oncePerElem<ept id="p5">*</ept> are ignored by the special compute contexts 'RxLocalParallel' and 'RxForeachDoPar`.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Conclusion</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>This article provides comprehensive documentation on rxExec for writing custom script that executes jobs in parallel.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Several use cases were used to show how rxExec is used in context, with additional sections providing guidance on relevant tasks associated with custom execution, such as sharing data, structuring jobs, and controlling calculations.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>To learn more, see these related links:</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>Distributed and parallel computing in Machine Learning Server</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>Using foreach and iterators for manual parallel execution</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>Parallel execution using doRSR for script containing RevoScaleR and foreach constructs</source>
        </trans-unit></group></body></file></xliff>