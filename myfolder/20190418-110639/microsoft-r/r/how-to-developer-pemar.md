<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-developer-pemar.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907fe7edc26eac489bd0762b4ce549351a7893a189a1.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">e7edc26eac489bd0762b4ce549351a7893a189a1</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-developer-pemar.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RevoPemaR functions in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to use the RevoPemaR package in Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to use the RevoPemaR library in Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>RevoPemaR<ept id="p1">**</ept> package provides a framework for writing custom parallel external memory algorithms in R, making use of the R reference classes introduced by John Chambers in R 2.12.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Parallel External Memory Algorithms (PEMA) are algorithms that eliminate in-memory data storage requirements, allowing data to be processed in chunks, in parallel, possibly on different nodes of a cluster.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>The results are then combined and processed at the end (or at the end of each iteration).</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>RevoPemaR<ept id="p1">**</ept> package is used for writing custom PEMA algorithms in R.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The custom PEMA functions created using the <bpt id="p1">**</bpt>RevoPemaR<ept id="p1">**</ept> framework are appropriate for small and large datasets, but are particularly useful in three common situations:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>To analyze data sets that are too large to fit in memory</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>To create scalable data analysis routines that can be developed locally with smaller data sets, then deployed to larger data</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>To perform computations distributed over nodes in a cluster</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Installation</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>RevoPemaR<ept id="p1">**</ept> package is included with Microsoft Machine Learning Server and R Client (which also contains the <bpt id="p2">**</bpt>RevoScaleR<ept id="p2">**</ept> package).</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>RevoPemaR<ept id="p1">**</ept> package can also be installed with a standard download of <bpt id="p2">[</bpt>Microsoft R Open (MRO)<ept id="p2">](https://mran.microsoft.com/open)</ept>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>About R Reference Classes</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The PEMA classes used in <bpt id="p1">**</bpt>RevoPemaR<ept id="p1">**</ept> are based on R Reference Classes.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>We include a brief overview of some tips for using R Reference Classes here, before moving to the specifics of the PEMA classes.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>R Reference Class objects are created using a generator function.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>This function has four important pieces of information:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Name of the class<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Inheritance or <bpt id="p1">*</bpt>superclasses<ept id="p1">*</ept> of the class.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Fields and methods of parent reference classes are inherited.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Fields<ept id="p1">*</ept> or member variables.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>These fields are accessed by reference (as in C++ or Java), so values of the fields for an object of this class can change.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Methods<ept id="p1">*</ept> that can be invoked by objects of this class.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>When working with reference class, keep these tips in mind:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Reference class generators are created using <bpt id="p1">*</bpt>setRefClass<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>For the PEMA classes, we use a wrapper for that function, <bpt id="p1">*</bpt>setPemaClass<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Field values are changed within methods using the non-local assignment operator (<bpt id="p1">*</bpt><ph id="ph1">\&lt;</ph><ph id="ph2">\&lt;</ph><ph id="ph3">-</ph><ept id="p1">*</ept>)</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The reference class object can be accessed in the methods using <bpt id="p1">*</bpt>.self<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The parent method can be accessed using <bpt id="p1">*</bpt>.callSuper<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">*</bpt>usingMethods<ept id="p1">*</ept> call to declare that a method is used by another method.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The code for a method can be displayed using an instantiated reference class object, for example, <bpt id="p1">*</bpt>myRefClassObj$initialize<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Methods are documented internally with an initial line of text, rather than in a .Rd file.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>This information is accessed using the $help method for the generator function.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Tutorial introduction to RevoPemaR</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>This section contains an overview of a simple example of estimating the mean of a variable using the <bpt id="p1">**</bpt>RevoPemaR<ept id="p1">**</ept> framework.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The key step is in creating a <bpt id="p1">*</bpt>PemaMean<ept id="p1">*</ept> reference class generator function that provides the fields and methods for computing the mean using a parallel external memory algorithm.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>This includes creating methods to compute the sum and number of observations for each chunk of data, to update these intermediate results, and at the end to use the intermediate results to compute the mean.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Using setPemaClass to Create a Class Generator</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Start by making sure that the <bpt id="p1">**</bpt>RevoPemaR<ept id="p1">**</ept> package is loaded:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>To create a PEMA class generator function, use the <bpt id="p1">*</bpt>setPemaClass<ept id="p1">*</ept> function.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>It is a wrapper function for <bpt id="p1">*</bpt>setRefClass<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>As with <bpt id="p1">*</bpt>setRefClass<ept id="p1">*</ept>, we specify four basic pieces of information when using <bpt id="p2">*</bpt>setPemaClass<ept id="p2">*</ept>: the class name, the superclasses, the fields, and the methods.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The structure looks something like this:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>Class<ept id="p1">*</ept> is the class name of your choice.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>contains<ept id="p1">*</ept> argument must specify <bpt id="p2">*</bpt>PemaBaseClass<ept id="p2">*</ept> or a child class of <bpt id="p3">*</bpt>PemaBaseClass<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>The specification of fields and methods follows.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Specifying the fields for PemaMean</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The fields or member variables of our class represent all of the variables we need in order to compute and store our intermediate and final results.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Here are the fields we use for our “means” computation:</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>An Overview of the <bpt id="p1">*</bpt>methods<ept id="p1">*</ept> for <bpt id="p2">*</bpt>PemaMean<ept id="p2">*</ept></source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>There are five methods we specify for <bpt id="p1">*</bpt>PemaMean<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>These methods are all in the <bpt id="p1">*</bpt>PemaBaseClass<ept id="p1">*</ept>, and need to be overloaded for any custom analysis.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>initialize<ept id="p1">*</ept>: initializes field values.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>processData<ept id="p1">*</ept>: processes a chunk of data and updates field values</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>updateResults<ept id="p1">*</ept>: updates the field values of a PEMA class object from another</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>processResults<ept id="p1">*</ept>: computes the final results from the final intermediate results</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>getVarsToUse<ept id="p1">*</ept>: the names of the variables in the dataset used for analysis</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>initialize<ept id="p1">*</ept> method</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The primary use of the i<bpt id="p1">*</bpt>nitialize<ept id="p1">*</ept> method is to initialize field values.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The one field that is initialized with user input in this example is the name of the variable to use in the computations, <bpt id="p1">*</bpt>varName<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Use of the ellipses in the function signature allows for initialization values to be passed up to the parent class using .<bpt id="p1">*</bpt>callSuper<ept id="p1">*</ept>, the first action in the <bpt id="p2">*</bpt>initialize<ept id="p2">*</ept> method after the documentation.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Here is the beginning of our methods listing:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>pemaSetClass<ept id="p1">*</ept> function also provides additional functionality used in the <bpt id="p2">*</bpt>initialize<ept id="p2">*</ept> method to ensure that all of the methods of the class and its parent classes are included when an object is serialized.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>This is critical for distributed computing.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>To use this functionality, add the following to the initialize method:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>(If you do not want to use this functionality you can omit this line and set <bpt id="p1">*</bpt>includeMethods<ept id="p1">*</ept> to FALSE in <bpt id="p2">*</bpt>setPemaClass<ept id="p2">*</ept>.)</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Now we finish the field initialization, setting the <bpt id="p1">*</bpt>varName<ept id="p1">*</ept> field to the input value and setting the starting values for our computations to 0, remembering to use the double-arrow non-local assignment operator to set field values:</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>processData<ept id="p1">*</ept> method</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>processData<ept id="p1">*</ept> method is the core of an external memory algorithm.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>It processes a chunk of data and computes intermediate results, updating the field value(s).</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>It takes as an argument a rectangular list of data vectors; typically only the variable(s) of interest is included.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>In our example code we do not compute the mean within this method; that occurs after we have processed all of the data.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Here we compute and update the intermediate results: the sum and number of observations:</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>updateResults<ept id="p1">*</ept> method</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>updateResults<ept id="p1">*</ept> is the key method used when computations are done in parallel.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Consider the following scenario:</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>The master node on a cluster assigns each worker node the task of processing a series of chunks of data.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The workers do so in parallel, each with their own instantiation of a reference class object.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Each worker calls <bpt id="p1">*</bpt>processData<ept id="p1">*</ept> for each chunk of data it needs to process.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>In each call, the values of the fields of its reference class object are updated.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Now the master process must collect the information from each of the nodes, and update all of the information in a single reference class object.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>This is done using the <bpt id="p1">*</bpt>updateResults<ept id="p1">*</ept> method, which takes as an argument another instance of the reference class.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>The reference class object from each of the nodes is processed by the master node, resulting in the final intermediate results in the master node’s reference class object’s fields.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Here is the <bpt id="p1">*</bpt>updateResults<ept id="p1">*</ept> method for our <bpt id="p2">*</bpt>PemaMean<ept id="p2">*</ept>:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>processResults<ept id="p1">*</ept> method</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>processResults<ept id="p1">*</ept> performs any necessary computations to produce the final result from the accumulated intermediate results.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>In this case, it is simple; we divide the sum by the number of valid observations (assuming we have some):</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>getVarsToUse<ept id="p1">*</ept> method</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>getVarsToUse<ept id="p1">*</ept> method specifies the names of the variables in the dataset that are used in the analysis.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Specifying this information can improve performance if reading data from disk.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Creating and Using a PemaMean Reference Class Object</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Instantiating and Exploring a PemaMean Object</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>A version of the code in the previous section is contained within the <bpt id="p1">**</bpt>RevoPemaR<ept id="p1">**</ept> package and exported, so we can directly work with the <bpt id="p2">*</bpt>PemaMean<ept id="p2">*</ept> generator without first running the code.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>We can show the names of all the methods, including those that are explicitly overridden by the <bpt id="p1">*</bpt>PemaMean<ept id="p1">*</ept> class:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Some of the methods (for example, <bpt id="p1">*</bpt>initIteration,<ept id="p1">*</ept> <bpt id="p2">*</bpt>getFieldList<ept id="p2">*</ept>) are inherited from the <bpt id="p3">*</bpt>PemaBaseClass<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Others (for example, <bpt id="p1">*</bpt>callSuper<ept id="p1">*</ept>, <bpt id="p2">*</bpt>methods<ept id="p2">*</ept>) are inherited from the base reference class generator.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>We can use the <bpt id="p1">*</bpt>help<ept id="p1">*</ept> method with the generator function to get help on specific methods:</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Next we generate a default <bpt id="p1">*</bpt>PemaMean<ept id="p1">*</ept> object, and print out the values of its fields (including those inherited):</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>We can also print out the code for a specific method using an instantiated object.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>For example, the initialize method of the <bpt id="p1">*</bpt>PemaMean<ept id="p1">*</ept> object in the <bpt id="p2">**</bpt>RevoPemaR<ept id="p2">**</ept> package is:</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Using a <bpt id="p1">*</bpt>PemaMean<ept id="p1">*</ept> Object with the <bpt id="p2">*</bpt>pemaCompute<ept id="p2">*</ept> Function</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>pemaCompute<ept id="p1">*</ept> function takes two required arguments: an “analysis” object and a data source object.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>The analysis object must be generated by <bpt id="p1">*</bpt>setPemaClass<ept id="p1">*</ept> and inherit (directly or indirectly) from <bpt id="p2">*</bpt>PemaBaseClass<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>The data source object must be either a data frame or a data source object supported by the <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> package if it is available.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>The ellipses take any additional information used in the <bpt id="p1">*</bpt>initialize<ept id="p1">*</ept> method.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Let’s compute a mean of some random numbers:</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>If we again print the values of the fields of our meanPemaObj, we see the updated values:</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>By default the <bpt id="p1">*</bpt>pemaCompute<ept id="p1">*</ept> method reinitializes the <bpt id="p2">*</bpt>pemaObj<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>By setting the <bpt id="p1">*</bpt>initPema<ept id="p1">*</ept> flag to <bpt id="p2">*</bpt>FALSE<ept id="p2">*</ept>, we can add more data to our analysis:</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>The number of total valid observations is now 2000.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Using a <bpt id="p1">*</bpt>RevoScaleR<ept id="p1">*</ept> Data Source with the <bpt id="p2">*</bpt>pemaCompute<ept id="p2">*</ept> Function</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>In the previous section, we analyzed data in memory.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> package provides a data source framework that allows data to be automatically extracted in chunks from data on disk or in a database.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>It also provides the <bpt id="p1">*</bpt>.xdf<ept id="p1">*</ept> file format that can efficiently extract chunks of data.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>We can use a sample .xdf file provided with the package.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>First we create a data source for this file:</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Using the <bpt id="p1">*</bpt>meanPemaObj<ept id="p1">*</ept> created above, we compute the mean of the variable <bpt id="p2">*</bpt>ArrDelay<ept id="p2">*</ept> (the arrival delay in minutes).</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>The data in this file is stored in three blocks, with 200,000 rows in each block.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>pemaCompute<ept id="p1">*</ept> function processes these chunks one at a time:</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>You can control the amount of progress reported to the console using the <bpt id="p1">*</bpt>reportProgress<ept id="p1">*</ept> field of <bpt id="p2">*</bpt>PemaBaseClass<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Using <bpt id="p1">*</bpt>pemaCompute<ept id="p1">*</ept> in a Distributed Compute Context</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> provides a number of distributed compute contexts, such as Hadoop clusters (Cloudera and Hortonworks).</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Use of the same PEMA reference class object on these platforms is experimental.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>It can be tried with data on those platforms by specifying the <bpt id="p1">*</bpt>computeContext<ept id="p1">*</ept> in the <bpt id="p2">*</bpt>pemaCompute<ept id="p2">*</ept> function.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Additional Examples Using RevoPemaR</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>A number of examples are provided in the <bpt id="p1">*</bpt>demoScripts<ept id="p1">*</ept> directory of the <bpt id="p2">*</bpt>RevoPemaR<ept id="p2">*</ept> package.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>You can find the location of this directory by entering:</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Basic Text Mining Examples</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Two PEMA text mining analyses are provided as examples.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>PemaPopularWords<ept id="p1">*</ept> accumulates the words used in a variable containing character data.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>The initialize method provides a variety of arguments to fine-tune the processing.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>The code for the reference class generator is provided in <bpt id="p1">*</bpt>PemaPopularWords.R<ept id="p1">*</ept>, and examples using it in <bpt id="p2">*</bpt>PemaPopularWordsEx.R<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>PemaWordCount<ept id="p1">*</ept> counts instances of specified words in a variable containing character data.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>The code for the reference class generator is provided in <bpt id="p1">*</bpt>PemaWordCount.R<ept id="p1">*</ept>, and examples using it in <bpt id="p2">*</bpt>PemaWordCountEx.R<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>If you are using <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> and are interested in exploring text mining with a large dataset, instructions for downloading and code for importing Amazon reviews of fine foods is contained in the script <bpt id="p2">*</bpt>finefoodsImport.R<ept id="p2">*</ept></source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Performing By-Group Computations</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">*</bpt>PemaByGroup<ept id="p1">*</ept> class is included in <bpt id="p2">*</bpt>RevoPemaR<ept id="p2">*</ept> to facilitate by-group computations.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Examples of using this class are provided in the <bpt id="p1">*</bpt>PemaByGroupEx.R<ept id="p1">*</ept> demo script.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>It is assumed that the relevant variables for each group can fit into memory, and are then processed by arbitrary R functions.</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>It requires that data be pre-sorted by group before processing, so generally cannot be used in distributed compute contexts such as Hadoop.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>An Iterative PEMA Algorithm: Logistic Gradient Descent</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>A simple logistic gradient descent algorithm is provided as an example of an iterative algorithm that inherits from a parent class.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>PemaGradDescent<ept id="p1">*</ept> class generator (in <bpt id="p2">*</bpt>PemaGradDescent.R<ept id="p2">*</ept>) specifies a number of important methods for iterative algorithms, for example:</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>initIteration<ept id="p1">*</ept>: initializes the appropriate field values at the beginning of each iteration</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>fn<ept id="p1">*</ept>: a placeholder for the computation of the objective (loss) function for gradient descent</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>gradientFn<ept id="p1">*</ept>: a placeholder for the computation of the gradient function for gradient descent</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>hasConverged<ept id="p1">*</ept>: checks convergence criteria</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>This class generator cannot be used directly.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>A child class generator must be created that at a minimum specifies the objective function (<bpt id="p1">*</bpt>fn<ept id="p1">*</ept>) and gradient function (<bpt id="p2">*</bpt>gradientFn<ept id="p2">*</ept>).</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>An example is provided in <bpt id="p1">*</bpt>PemaLogitGD.R<ept id="p1">*</ept>, showing a logistic gradient descent.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>A simple example of its use is in <bpt id="p1">*</bpt>PemaLogitGDEx.R<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>Debugging <bpt id="p1">*</bpt>RevoPemaR<ept id="p1">*</ept> Code</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>The R Reference Classes provide standard R debugging tools, and <bpt id="p1">*</bpt>trace<ept id="p1">*</ept> and <bpt id="p2">*</bpt>untrace<ept id="p2">*</ept> methods are provided in the base reference class.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>PemaBaseClass<ept id="p1">*</ept> provides a simple way of printing trace output that is particularly useful in debugging code in a distributed environment.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Calls to the <bpt id="p1">*</bpt>outputTrace<ept id="p1">*</ept> method within other methods print the specified text if the <bpt id="p2">*</bpt>traceLevel<ept id="p2">*</ept> field value exceeds or is equal to the <bpt id="p3">*</bpt>outTraceLevel<ept id="p3">*</ept> argument:</source>
        </trans-unit></group></body></file></xliff>