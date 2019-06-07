<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxexecby.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c376af348ab7ae553e4a9dfccaebc2d5efee5c809fb.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">6af348ab7ae553e4a9dfccaebc2d5efee5c809fb</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxexecby.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxExecBy function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Partition input data source by keys and apply user defined function on individual partitions.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>If input data source is already partitioned, apply user defined function on partitions directly.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Currently supported in local, localpar, <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> and <bpt id="p2">[</bpt>RxSpark<ept id="p2">](RxSpark.md)</ept> compute contexts.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxExecBy, ExecBy</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>rxExecBy: Partition Data by Key Values and Execute User Function on Each Partition</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Partition input data source by keys and apply user defined function on individual partitions.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>If input data source is already partitioned, apply user defined function on partitions directly.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Currently supported in <ph id="ph1">`local`</ph>, <ph id="ph2">`localpar`</ph>, <bpt id="p1">[</bpt>RxInSqlServer<ept id="p1">](RxInSqlServer.md)</ept> and <bpt id="p2">[</bpt>RxSpark<ept id="p2">](RxSpark.md)</ept> compute contexts.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>a data source object suppported in currently active compute context, e.g., <bpt id="p1">[</bpt>RxSqlServerData<ept id="p1">](RxSqlServerData.md)</ept> for <bpt id="p2">[</bpt>RxInSqlServer<ept id="p2">](RxInSqlServer.md)</ept> and <bpt id="p3">[</bpt>RxHiveData<ept id="p3">](RxSparkData.md)</ept> for <bpt id="p4">[</bpt>RxSpark<ept id="p4">](RxSpark.md)</ept>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>In <ph id="ph1">`local`</ph> and <ph id="ph2">`localpar`</ph> compute contexts, a character string specifying a .xdf file or a data frame object can be also used.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>character vector of variable names to specify the values in those variables are used for partitioning.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>the user function to be executed.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The user function takes <ph id="ph1">`keys`</ph> and <ph id="ph2">`data`</ph> as two required input arguments where <ph id="ph3">`keys`</ph> determines the partitioning values and <ph id="ph4">`data`</ph> is a data source object of the corresponding partition.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>can be a <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object or a RxODBCData object, which can be transformed to a standard R data frame by using <bpt id="p2">[</bpt>rxDataStep<ept id="p2">](rxDataStep.md)</ept> method.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The nodes or cores on which it is running are determined by the currently active compute context.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>list of additional arguments for the user function <ph id="ph1">`func`</ph>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>the user function that takes a data frame of keys values as an input argument, applies filter to the keys values and returns a data frame containing rows whose keys values satisfy the filter conditions.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The input data frame has similar format to the results returned by <bpt id="p1">[</bpt>rxPartition<ept id="p1">](rxPartition.md)</ept> which comprises of partitioning variables and an additional variable of partition data source.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>This <ph id="ph1">`filterFunc`</ph> allows user to control what data partitions to be applied by the user function <ph id="ph2">`func`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>currently is not supported in RxHadoopMR and <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute contexts.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>a RxComputeContext object.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Compute Engine.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>A list which is the same length as the number of partitions in the <ph id="ph1">`inData`</ph> argument.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Each element in the top level list contains a three element list described below.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>a list which contains key values for the partition.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>the object returned from the invocation of the user function with <ph id="ph1">`keys`</ph> values.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>When an error occurs during the invocation of the user function the value will be <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>a string which takes the value of either <ph id="ph1">`"OK"`</ph> or <ph id="ph2">`"Error"`</ph>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>RxSpark<ept id="p1">](RxSpark.md)</ept> compute context, it may include additional warning and error messages.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The user function can call any function defined in R packages which are loaded by default and pass parameters which are defined in base R, the default loaded packages, or user defined S3 classes.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The user function won't work with global variables or functions in non-default loaded packages unless they are redefined or reloaded within the scope of the user function.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxExecByPartition<ept id="p1">](rxExecByPartition.md)</ept>, <bpt id="p2">[</bpt>rxImport<ept id="p2">](rxImport.md)</ept>, <bpt id="p3">[</bpt>rxDataStep<ept id="p3">](rxDataStep.md)</ept>, <bpt id="p4">[</bpt>RxTextData<ept id="p4">](RxTextData.md)</ept>, <bpt id="p5">[</bpt>RxXdfData<ept id="p5">](RxXdfData.md)</ept>, <bpt id="p6">[</bpt>RxHiveData<ept id="p6">](RxSparkData.md)</ept>, <bpt id="p7">[</bpt>RxSqlServerData<ept id="p7">](RxSqlServerData.md)</ept></source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>