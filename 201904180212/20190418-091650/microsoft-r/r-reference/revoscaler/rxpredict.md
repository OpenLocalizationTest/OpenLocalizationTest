<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxpredict.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4bfe5d2dae2fb51eedb6a56a7d2647ae2d783622e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">bfe5d2dae2fb51eedb6a56a7d2647ae2d783622e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxpredict.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxPredict function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Predicted values and residuals for model objects built using RevoScaleR</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxPredict, rxPredict.default, methods, models, regression</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxPredict: Predicted values and residuals for model objects built using RevoScaleR</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Compute predicted values and residuals using the following objects: <bpt id="p1">[</bpt>rxLinMod<ept id="p1">](rxLinMod.md)</ept>, <bpt id="p2">[</bpt>rxGlm<ept id="p2">](rxGlm.md)</ept>, <bpt id="p3">[</bpt>rxLogit<ept id="p3">](rxLogit.md)</ept>, <bpt id="p4">[</bpt>rxDTree<ept id="p4">](rxDTree.md)</ept>, <bpt id="p5">[</bpt>rxBTrees<ept id="p5">](rxBTrees.md)</ept>, and <bpt id="p6">[</bpt>rxDForest<ept id="p6">](rxDForest.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>object returned from a RevoScaleR model fitting function.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Valid values include <ph id="ph1">`rxLinMod`</ph>, <ph id="ph2">`rxLogit`</ph>, <ph id="ph3">`rxGlm`</ph>, <ph id="ph4">`rxDTree`</ph>, <ph id="ph5">`rxBTrees`</ph>, and <ph id="ph6">`rxDForest`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Objects with multiple dependent variables are not supported in rxPredict.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>An <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> data source object to be used for predictions.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>If not using a distributed compute context such as RxHadoopMR, a data frame,  or a character string specifying the input .xdf file can also be used.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>file or existing data frame to store predictions; can be same as the input file or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If not <ph id="ph1">`NULL`</ph>, a character string specifying  the output �.xdf� file, a RxXdfData object, a RxOdbcData data source, or a RxSqlServerData  data source.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`outData`</ph> can also be a delimited <bpt id="p1">[</bpt>RxTextData<ept id="p1">](RxTextData.md)</ept> data source if using a native file system and not appending.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the standard errors  for each dependent variable are calculated.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>character string defining the type of interval calculation to perform.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Supported values are <ph id="ph1">`"none"`</ph>, <ph id="ph2">`"confidence"`</ph>, and <ph id="ph3">`"prediction"`</ph>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>numeric value representing the confidence level on the interval [0, 1].</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, residuals are computed.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Applies to <bpt id="p1">[</bpt>rxGlm<ept id="p1">](rxGLM.md)</ept> and <bpt id="p2">[</bpt>rxLogit<ept id="p2">](rxLogit.md)</ept>, used to set the type of prediction.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Valid values are <ph id="ph1">`"response"`</ph>and <ph id="ph2">`"link"`</ph>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`type = "response"`</ph>, the predictions are on the scale of the response variable.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>For instance, for  the binomial model, the predictions are in the range (0,1).</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`type = "link"`</ph>, the predictions are on the scale of the linear predictors.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Thus for the binomial model, the predictions are of log-odds.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, and the output data set is different from the input data set, variables in the model will be written to the output data set in addition to the predictions (and residuals, standard errors, and confidence bounds, if requested).</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If variables from the input data set are transformed in the model, the transformed variables will also be included.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or character vector of additional variables names from the input data or transforms to include in the <ph id="ph2">`outData`</ph>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`writeModelVars`</ph> is <ph id="ph2">`TRUE`</ph>, model variables will be included as well.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, rows with missing values are removed.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>either <ph id="ph1">`"none"`</ph> to create a new files or <ph id="ph2">`"rows"`</ph> to append rows to an existing file.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outData`</ph> exists and <ph id="ph2">`append`</ph> is <ph id="ph3">`"none"`</ph>, the <ph id="ph4">`overwrite`</ph> argument must be set to <ph id="ph5">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>You can append only to <bpt id="p1">[</bpt>RxTeradata<ept id="p1">](RxTeradata.md)</ept> data source.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, an existing <ph id="ph2">`outData`</ph> will be overwritten.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`overwrite`</ph> is ignored if appending rows.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Ignored for data frames.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, up to 1000 factor levels  for the data will be verified against factor levels in the model.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Setting to <ph id="ph1">`FALSE`</ph> can speed up computations if using lots of factors.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>character vector specifying name(s) to give to the prediction results</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>character vector specifying name(s) to give to the residual results.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or a character vector defining low and high confidence interval variable names, respectively.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the strings <ph id="ph2">`"_Lower"`</ph> and <ph id="ph3">`"_Upper"`</ph> are appended to the dependent variable names to form the  confidence interval variable names.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`NULL`</ph> or a character vector defining variable names corresponding to the standard errors, if calculated.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the string <ph id="ph2">`"_StdErr"`</ph> is appended to the dependent variable names to form the  standard errors variable names.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>character vector specifying name(s) to give to the prediction and residual results; if length is 2, the second name is used for residuals.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>This argument is deprecated and <ph id="ph1">`predVarNames`</ph> and <ph id="ph2">`residVarNames`</ph> should be used instead.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`data`</ph> and <ph id="ph2">`outData`</ph> are the same file, blocksPerRead must be 1.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`0`</ph>: no progress is reported.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`1`</ph>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`2`</ph>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`3`</ph>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no additional output is printed.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`1`</ph>, additional summary information is printed.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>integer in the range of -1 to 9 indicating the compression  level for the output data if written to an <ph id="ph1">`.xdf`</ph> file.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The higher the value, the greater the  amount of compression - resulting in smaller files but a longer time to create them.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>If  <ph id="ph1">`xdfCompressionLevel`</ph> is set to 0, there will be no compression and files will be compatible  with the 6.0 release of Revolution R Enterprise.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>If set to -1, a default level of compression  will be used.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Revolution Compute Engine.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rxPredict`</ph> computes predicted values and/or residuals from an existing model type.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>The most common way to call rxPredict is <ph id="ph1">`rxPredict(modelObject, data, outData)`</ph>.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Typically, all the other arguments are left at their defaults.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>For rxLogit, the residuals are equivalent to those computed for <ph id="ph1">`glm`</ph> with <ph id="ph2">`type`</ph> set to <ph id="ph3">`"response"`</ph>, e.g., <ph id="ph4">`residuals(glmObj, type="response")`</ph>.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`data`</ph> is the same data used to create the <ph id="ph2">`modelObject`</ph>, the predicted values are the fitted values for the original model.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`data`</ph> specified is an .xdf file, the <ph id="ph2">`outData`</ph> must be <ph id="ph3">`NULL`</ph> or an .xdf file.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outData`</ph> is an .xdf file, the computed data will be appended as columns.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outData`</ph> is <ph id="ph2">`NULL`</ph>, the computed columns will be appended to the <ph id="ph3">`data`</ph> .xdf file.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>If the <ph id="ph1">`data`</ph> specified is a data frame, the <ph id="ph2">`outData`</ph> must be <ph id="ph3">`NULL`</ph> or a data frame.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outData`</ph> is a data frame, a copy of the data frame with the new columns appended will be returned.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outData`</ph> is <ph id="ph2">`NULL`</ph>, a vector or list of the computed values will be returned.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>If a transformation function is being used for the model estimation, the information variable <ph id="ph1">`.rxIsPrediction`</ph> can be used to exclude computations for the dependent variable when running <ph id="ph2">`rxPredict`</ph>.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for an example.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>If a data frame is specified as the input <ph id="ph1">`data`</ph>, a data frame is returned.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>If a data frame is specified as the <ph id="ph1">`outData`</ph>, variables containing the results are added to the data frame and it is returned.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outData`</ph> is <ph id="ph2">`NULL`</ph>, a data frame containing the predicted values (and residuals and standard errors, if requested) is returned.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>If an .xdf file is specified as the input <ph id="ph1">`data`</ph>, an <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> data source object is returned that can be used in subsequent RevoScaleR analyses.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outData`</ph> is an .xdf file, the <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> data source represents the <ph id="ph2">`outData`</ph> file.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`outData`</ph> is <ph id="ph2">`NULL`</ph>, the predicted values (and, if requested, residuals) are appended to the original <ph id="ph3">`data`</ph> file.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>The returned <bpt id="p1">[</bpt>RxXdfData<ept id="p1">](RxXdfData.md)</ept> object represents this file.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Computing Standard Errors of Predicted Values</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`computeStdErrors`</ph> to control whether or not prediction standard errors are computed.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`interval`</ph> to control whether confidence or prediction (tolerance) intervals are computed at the specified level (<ph id="ph2">`confLevel`</ph>).</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>These are sometimes referred to as <bpt id="p1">*</bpt>narrow<ept id="p1">*</ept> and <bpt id="p2">*</bpt>wide<ept id="p2">*</ept> intervals, respectively.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`stdErrorsVarNames`</ph> to name the standard errors output variable and <ph id="ph2">`intervalVarNames`</ph> to specify the output variable names of the lower and upper confidence/tolerance intervals.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>In calculating the prediction standard errors, keep the following in mind:</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Prediction standard errors are available for both <bpt id="p1">[</bpt>rxLinMod<ept id="p1">](rxLinMod.md)</ept> and <bpt id="p2">[</bpt>rxLogit<ept id="p2">](rxLogit.md)</ept> models.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Standard errors are computationally intensive for large models, i.e., those involving a large number of model parameters.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxLinMod<ept id="p1">](rxLinMod.md)</ept> and <bpt id="p2">[</bpt>rxLogit<ept id="p2">](rxLogit.md)</ept> must be called with <ph id="ph1">`covCoef = TRUE`</ph> because the variance-covariance matrix of the coefficients must be available.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Cube regressions are not supported (<ph id="ph1">`cube = TRUE`</ph>).</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Multiple dependent variables are currently not supported.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>For <bpt id="p1">[</bpt>rxLogit<ept id="p1">](rxLogit.md)</ept>, <ph id="ph1">`interval = "confidence"`</ph> is supported (unlike predict.glm, which does not support confidence bounds), but <ph id="ph2">`interval = "prediction"`</ph> is not supported.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>If residuals are requested, and if there are missing values in the dependent variable, then all computed values (prediction, standard errors, confidence levels) will be assigned the value missing, and will be removed if <ph id="ph1">`removeMissings = TRUE`</ph>.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>If no residuals are requested, then missings in the dependent variable (which need not exist in the data) have no effect.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxLinMod<ept id="p1">](rxLinMod.md)</ept>, <bpt id="p2">[</bpt>rxLogit<ept id="p2">](rxLogit.md)</ept>, <bpt id="p3">[</bpt>rxGlm<ept id="p3">](rxGLM.md)</ept>, <bpt id="p4">[</bpt>rxPredict.rxDTree<ept id="p4">](rxPredict.rxDTree.md)</ept>, <bpt id="p5">[</bpt>rxPredict.rxDForest<ept id="p5">](rxPredict.rxDForest.md)</ept>, <bpt id="p6">[</bpt>rxPredict.rxNaiveBayes<ept id="p6">](rxPredict.rxNaiveBayes.md)</ept>.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>