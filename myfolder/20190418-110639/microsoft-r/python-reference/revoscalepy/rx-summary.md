<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-summary.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907fc962eeebc0480054ef9321ad2e4268392bef4850.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">c962eeebc0480054ef9321ad2e4268392bef4850</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-summary.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_summary: Generate summary statistics (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Produce univariate summaries of objects in revoscalepy.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>summary</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rx_summary</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Produce univariate summaries of objects in revoscalepy.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>formula</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Statistical model using symbolic formulas.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The formula typically does not contain a response variable, i.e. it should be of the form ~ terms.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>either a data source object, a character string specifying a ‘.xdf’ file, or a data frame object to summarize.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If a Spark compute context is being used, this argument may also be an RxHiveData, RxOrcData, RxParquetData or RxSparkDataFrame object or a Spark data frame object from pyspark.sql.DataFrame.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>by_group_out_file</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>None, a character string or vector of character strings specifying .xdf file names(s), or an RxXdfData object or list of RxXdfData objects.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If not None, and the formula includes computations by factor, the by-group summary results will be written out to one or more ‘.xdf’ files.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If more than one .xdf file is created and a single character string is specified, an integer will be appended to the base by_group_out_file name for additional file names.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The resulting RxXdfData objects will be listed in the categorical component of the output object.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>summary_stats</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>A list of strings containing one or more of the following values: “Mean”, “StdDev”, “Min”, “Max”, “ValidObs”, “MissingObs”, “Sum”.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>by_term</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>bool variable.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If True, missings will be removed by term (by variable or by interaction expression) before computing summary statistics.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If False, observations with missings in any term will be removed before computations.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>pweights</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Character string specifying the variable to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>fweights</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Character string specifying the variable to use as frequency weights for the observations.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>row_selection</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>transforms</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>transform_objects</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>transform_function</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Variable transformation function.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>transform_variables</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>List of strings of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>transform_packages</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>transform_environment</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>overwrite</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If True, an existing byGroupOutFile will be overwritten.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>overwrite is ignored byGroupOutFile is None.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>use_sparse_cube</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If True, sparse cube is used.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>remove_zero_counts</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Bool flag.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If True, rows with no observations will be removed from the output for counts of categorical data.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>By default, it has the same value as useSparseCube.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>For large summary computation, this should be set to True, otherwise the Python interpreter may run out of memory even if the internal C++ computation succeeds.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>rows_per_block</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Maximum number of rows to write to each block in the by_group_out_file (if it is not None).</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Integer value with options: 0: No progress is reported.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>1: The number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>2: Rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>3: Rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Integer value.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>If 0, no additional output is printed.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>If 1, additional summary information is printed.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>A valid RxComputeContext object.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>kwargs</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed directly to the Revolution Compute Engine.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>An RxSummary object containing the following elements: nobs.valid: Number of valid observations.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>nobs.missing: Number of missing observations.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>sDataFrame: Data frame containing summaries for continuous variables.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>categorical: List of summaries for categorical variables.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>categorical.type: Types of categorical summaries: can be “counts”, or “cube” (for crosstab counts) or “none” (if there is no categorical summaries).</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>formula: Formula used to obtain the summary.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>