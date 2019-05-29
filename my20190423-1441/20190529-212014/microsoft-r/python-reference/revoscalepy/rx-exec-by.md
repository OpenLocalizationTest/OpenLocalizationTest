<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-exec-by.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b33de81e53420566837229806d8b1224745823cb5f.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">3de81e53420566837229806d8b1224745823cb5f</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-exec-by.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_exec_by: Partition by key and execute functions by partition (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Partition input data source by keys and apply a user-defined function on individual partitions.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>If the input data source is already partitioned, apply a user-defined function directly on the partitions.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Currently supported in local, localpar, RxInSqlServer and RxSpark compute contexts.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>execby, groupby</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>rx_exec_by</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Partition input data source by keys and apply a user-defined function on individual partitions.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>If the input data source is already partitioned, apply a user-defined function directly on the partitions.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Currently supported in local, localpar, RxInSqlServer and RxSpark compute contexts.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>input_data</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A data source object supported in currently active compute context, e.g. ‘RxSqlServerData’ for ‘RxInSqlServer’.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>In ‘RxLocalSeq’ and ‘RxLocalParallel’, a character string specifying a ‘.xdf’ file, or a data frame object can be also used.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If a Spark compute context is being used, this argument may also be an RxHiveData, RxOrcData, RxParquetData or RxSparkDataFrame object or a Spark data frame object from pyspark.sql.DataFrame.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>keys</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>List of strings of variable names to be used for partitioning the input data set.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>function</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The user function to be executed.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The user function takes ‘keys’ and ‘data’ as two required input arguments where ‘keys’ determines the partitioning values and ‘data’ is a data source object of the corresponding partition.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>‘data’ can be a RxXdfData object or a RxODBCData object, which can be transformed to a pandas data frame by using rx_data_step.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>‘keys’ is a dict where keys of the dict are variable names and values are variable values of the partition.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The nodes or cores on which it is running are determined by the currently active compute context.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>function_parameters</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>A dict which defines a list of additional arguments for the user function func.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>filter_function</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>An user function that takes a Panda data frame of keys/values as an input argument, applies filter to the keys/values and returns a data frame containing rows whose keys/values satisfy the filter conditions.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The input data frame has similar format to the results returned by rx_partition which comprises of partitioning variables and an additional variable of partition data source.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>This filter_function allows user to control what data partitions to be applied by the user function ‘function’.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>‘filter_function’ currently is not supported in RxHadoopMR and RxSpark compute contexts.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>A RxComputeContext object.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>kwargs</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Additional arguments.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>A RxExecByResults object inherited from dataframe with each row to be the result of each partition.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The indexes of dataframe are keys, columns are ‘result’ and ‘status’.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>‘result’: the object returned from the user function from each partition.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>‘status’: ‘OK’, if the user function on each partition runs success, otherwise, the exception object.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`rx_partition`</ph><ept id="p1">](rx-partition.md)</ept>.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`RxXdfData`</ph><ept id="p1">](RxXdfData.md)</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>