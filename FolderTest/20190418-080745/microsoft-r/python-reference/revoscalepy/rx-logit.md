<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rx-logit.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335d9a4c59aceb92e3ef2d7bd215a5fd5a4942d8772.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d9a4c59aceb92e3ef2d7bd215a5fd5a4942d8772</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\revoscalepy\rx-logit.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rx_logit: Fit a logistic regression model (revoscalepy)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Use rx_logit to fit logistic regression models for small or large data sets.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>logic</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rx_logit</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Use rx_logit to fit logistic regression models for small or large data sets.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>formula</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Statistical model using symbolic formulas.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Dependent variable must be binary.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>It can be a bool variable, a factor with only two categories, or a numeric variable with values in the range (0,1).</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>In the latter case it will be converted to a bool.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>data</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Either a data source object, a character string specifying a ‘.xdf’ file, or a data frame object.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>If a Spark compute context is being used, this argument may also be an RxHiveData, RxOrcData, RxParquetData or RxSparkDataFrame object or a Spark data frame object from pyspark.sql.DataFrame.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>pweights</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Character string specifying the variable to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>fweights</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Character string specifying the variable to use as frequency weights for the observations.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>cube</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Bool flag.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If True and the first term of the predictor variables is categorical (a factor or an interaction of factors), the regression is performed by applying the Frisch-Waugh-Lovell Theorem, which uses a partitioned inverse to save on computation time and memory.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>cube_predictions</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Bool flag.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If True and cube is True the estimated model is evaluated (predicted) for each cell in the cube, fixing the non-cube variables in the model at their mean values, and these predictions are included in the countDF component of the returned value.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>This may be time and memory intensive for large models.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>variable_selection</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>A list specifying various parameters that control aspects of stepwise regression.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If it is an empty list (default), no stepwise model selection will be performed.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>If not, stepwise regression will be performed and cube must be False.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>row_selection</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>transforms</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>transform_objects</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>A dictionary of variables besides the data that are used in the transform function.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>See rx_data_step for examples.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>transform_function</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Name of the function that will be used to modify the data before the model is built.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The variables used in the transform function must be specified in transform_objects.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>See rx_data_step for examples.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>transform_variables</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>List of strings of the column names needed for the transform function.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>transform_packages</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>None.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Not currently supported, reserved for future use.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>drop_first</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Bool flag.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If False, the last level is dropped in all sets of factor levels in a model.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If that level has no observations (in any of the sets), or if the model as formed is otherwise determined to be singular, then an attempt is made to estimate the model by dropping the first level in all sets of factor levels.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>If True, the starting position is to drop the first level.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Note that for cube regressions, the first set of factors is excluded from these rules and the intercept is dropped.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>drop_main</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Bool value.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>If True, main-effect terms are dropped before their interactions.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>cov_coef</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Bool flag.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>If True and if cube is False, the variance-covariance matrix of the regression coefficients is returned.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>cov_data</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Bool flag.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If True and if cube is False and if constant term is included in the formula, then the variance-covariance matrix of the data is returned.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>initial_values</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Starting values for the Iteratively Reweighted Least Squares algorithm used to estimate the model coefficients.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>coef_label_style</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Character string specifying the coefficient label style.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The default is “Revo”.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>blocks_per_read</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>max_iterations</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Maximum number of iterations.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>coefficent_tolerance</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Convergence tolerance for coefficients.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>If the maximum absolute change in the coefficients (step), divided by the maximum absolute coefficient value, is less than or equal to this tolerance at the end of an iteration, the estimation is considered to have converged.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>To disable this test, set this value to 0.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>gradient_tolerance</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>This argument is deprecated.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>objective_function_tolerance</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Convergence tolerance for the objective function.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>report_progress</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Integer value with options: 0: No progress is reported.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>1: The number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>2: Rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>3: Rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>verbose</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Integer value.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>compute_context</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>A RxComputeContext object for prediction.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>kwargs</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Additional parameters</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Returns</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>A RxLogitResults object of linear model.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt><ph id="ph1">`rx_lin_mod`</ph><ept id="p1">](rx-lin-mod.md)</ept>.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Example</source>
        </trans-unit></group></body></file></xliff>