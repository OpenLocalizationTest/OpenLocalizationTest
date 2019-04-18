<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxlinmod.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f74c4cf77165add750a60c2954edb66edf710fd08.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">74c4cf77165add750a60c2954edb66edf710fd08</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxlinmod.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxLinMod function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Fit linear models on small or large data.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxLinMod, models, regression</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxLinMod: Linear Models</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Fit linear models on small or large data.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>formula as described in <bpt id="p1">[</bpt>rxFormula<ept id="p1">](rxFormula.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>either a data source object, a character string specifying a .xdf file, or a data frame object.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as frequency weights for the observations.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> and the first term of the predictor variables is categorical (a factor or an interaction of factors), the regression is performed by applying the Frisch-Waugh-Lovell Theorem, which uses a partitioned inverse to save on computation time and memory.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>See Details section below.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> and <ph id="ph2">`cube`</ph> is <ph id="ph3">`TRUE`</ph> the predicted values are computed and included in the <ph id="ph4">`countDF`</ph>component of the returned value.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>This may be memory intensive.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>See Details section below.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>a list specifying various parameters that control aspects of stepwise regression.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If it is an empty list (default), no stepwise model selection will be performed.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>If not, stepwise regression will be performed and <ph id="ph1">`cube`</ph> must be <ph id="ph2">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxStepControl<ept id="p1">](rxStepControl.md)</ept> for details.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>name of a logical variable in the data set (in quotes) or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rowSelection = (age &gt; 20) &amp; (age &lt; 65) &amp; (log(income) &gt; 10)`</ph> will use only observations in which the value of the <ph id="ph2">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph3">`log`</ph> of the <ph id="ph4">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations  (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function  call using the expression function.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>an expression of the form <ph id="ph1">`list(name = expression, ...)`</ph> representing the first round of variable transformations.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>)  can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>a named list containing objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>variable transformation function.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The variables used in the  transformation function must be specified in <ph id="ph1">`transformVars`</ph> if they are not variables used in the model.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>character vector defining additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and  preloaded for use in variable transformation functions, e.g., those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments or those  defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>user-defined environment to serve as a parent to  all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, the last level is dropped in  all sets of factor levels in a model.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>If that level has no observations (in any of  the sets), or if the model as formed is otherwise determined to be singular, then  an attempt is made to estimate the model by dropping the first level in all sets  of factor levels.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the starting position is to drop the first level.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Note that for cube regressions, the first set of factors is excluded from these rules  and the intercept is dropped.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, main-effect terms are dropped before their interactions.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> and if <ph id="ph2">`cube`</ph> is <ph id="ph3">`FALSE`</ph>,  the variance-covariance matrix of the regression coefficients is returned.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">[</bpt>rxCovCoef<ept id="p1">](rxCovRegression.md)</ept> function to obtain these data.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> and if <ph id="ph2">`cube`</ph> is <ph id="ph3">`FALSE`</ph> and if  constant term is included in the formula, then the variance-covariance matrix of the data is returned.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">[</bpt>rxCovData<ept id="p1">](rxCovRegression.md)</ept> function to obtain these data.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>character string specifying the coefficient label style.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>The default is "Revo".</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>If "R", R-compatible labels are created.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
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
          <source>a valid <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The  and <ph id="ph1">`RxHadoopMR`</ph> compute  context distributes the computation among the nodes specified by the  compute context; for other compute contexts, the  computation is distributed if possible on the local computer.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Revolution Compute Engine.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The special function <ph id="ph1">`F()`</ph> can be used in <ph id="ph2">`formula`</ph> to force a variable to be interpreted as a factor.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>When <ph id="ph1">`cube`</ph> is <ph id="ph2">`TRUE`</ph>, the Frisch-Waugh-Lovell (FWL) Theorem is applied to the model.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>The FWL approach parameterizes the model to include one coefficient for each category (a single factor level or combination of factor levels) instead of using an intercept in the model with contrasts for each of the factor combinations.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Additionally when <ph id="ph1">`cube`</ph> is <ph id="ph2">`TRUE`</ph>, the output contains a <ph id="ph3">`countDF`</ph> element representing the counts for each category.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`cubePredictions`</ph> is also <ph id="ph2">`TRUE`</ph>, predicted values using means of conditional independent continuous variables and weighted coefficients of conditional independent categorical variables are also computed and included in <ph id="ph3">`countDF`</ph>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>This may be memory intensive.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>If there are no conditional independent variables (outside of the cube), the predicted values are equivalent to the coefficients and will be included in <ph id="ph1">`countDF`</ph> whenever <ph id="ph2">`cube`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Regardless of the setting for <ph id="ph1">`cube`</ph>, the null model for the F-test of global significance is always the intercept-only model.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`dropFirst`</ph> and <ph id="ph2">`dropMain`</ph> arguments are provided primarily as a convenience to users comparing <ph id="ph3">`rxLinMod`</ph> results to those of <ph id="ph4">`lm`</ph>.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>While <ph id="ph1">`rxLinMod`</ph> will sometimes drop main effects while retaining interactions involving those terms, <ph id="ph2">`lm`</ph> will not.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Setting <ph id="ph1">`dropMain=FALSE`</ph> will give results more akin to those of <ph id="ph2">`lm`</ph>.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Similarly, <ph id="ph1">`lm`</ph> defaults to using treatment contrasts, which essentially drop the first level of each factor from the finished model.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>On the other hand, <ph id="ph1">`rxLinMod`</ph> by default uses a set of contrasts that drop the last level of each factor.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Setting <ph id="ph1">`dropFirst=TRUE`</ph> will give results more akin to those of <ph id="ph2">`lm`</ph>.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Let P be the number of regression coefficients returned for each dependent variable, <ph id="ph1">`Y(n)`</ph> for <ph id="ph2">`n=1,...,N`</ph>, specified in the regression model.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Let <bpt id="p1">**</bpt>X<ept id="p1">**</ept> be the linear regression design matrix.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxLinMod`</ph> function returns an object of class rxLinMod, which is a list containing the following elements:</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>P x N numeric matrix containing the regression coefficients.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>variance-covariance matrix for the regression coefficient estimates.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>variance-covariance matrix for the explanatory variables in the regression model.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>the sum of the squares of the residuals.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>numeric scalar representing the estimated reciprocal condition number of X'X (moment or crossprod) matrix.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>integer scalar denoting the numeric rank of the fitted linear model.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>logical vector specifying whether columns were dropped or not due to collinearity.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>P x N numeric matrix containing the standard errors of the regression coefficients.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>P x N numeric matrix containing the t-statistics for the regression coefficients.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>P x N numeric matrix containing the p-values for the t-stats (Pr(&gt;|t|))</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>N element numeric vector whose nth element is defined by <ph id="ph1">`Y'(n)Y(n)`</ph> for <ph id="ph2">`n=1,...,N`</ph>.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>N element numeric vector whose nth element is defined by <ph id="ph1">`(Y(n) - E{Y(n)})'(Y(n) - E{Y(n)}`</ph>, i.e., the mean deviation of each dependent variable.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>N element numeric vector of standard error of residuals.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>the variance of the residuals.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>N element numeric vector containing r-squared, the fraction of variance explained by the model.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>the p-value resulting from an F-test on the fitted model.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>degrees of freedom, a 3-element vector (p, n-p, p*), the last being the number of non-aliased coefficients.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>N element character vector containing the names of the dependent variables in the specified model.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>when cube is <ph id="ph1">`TRUE`</ph>, partitioned results will also be returned.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>(for models including non-intercept terms) a list containing the named elements: <bpt id="p1">**</bpt>value:<ept id="p1">**</ept> an N element numeric vector of F-statistic values, <bpt id="p2">**</bpt>numdf:<ept id="p2">**</ept> corresponding numerator degrees of freedom and <bpt id="p3">**</bpt>dendf:<ept id="p3">**</ept> corresponding denominator degrees of freedom.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>R-squared statistic 'adjusted', penalizing for higher p.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>parameters sent to Microsoft R Services Compute Engine.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>the model formula.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>For stepwise regression, this is the final model selected.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>the matched call.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>when <ph id="ph1">`cube`</ph> is <ph id="ph2">`TRUE`</ph>, a data frame containing counts information for each cube.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`cubePredictions`</ph> is also <ph id="ph2">`TRUE`</ph>, predicted values for each group in the cube are included.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>number of valid observations.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>number of missing observations.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>minus twice the maximized log-likelihood (up to a constant)</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>for stepwise regression,  a data frame corresponding to the steps taken in the search.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>for stepwise regression,  the base model from which the search is started.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Frisch, Ragnar; Waugh, Frederick V., Partial Time Regressions as Compared with Individual Trends, <bpt id="p1">*</bpt>Econometrica<ept id="p1">*</ept>, <bpt id="p2">**</bpt>1<ept id="p2">**</ept> (4) (Oct., 1933), pp. 387-401.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Lovell, M., 1963, Seasonal adjustment of economic time series, <bpt id="p1">*</bpt>Journal of the American Statistical Association<ept id="p1">*</ept>, <bpt id="p2">**</bpt>58<ept id="p2">**</ept>, pp. 993-1010.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Lovell, M., 2008, A Simple Proof of the FWL (Frisch,Waugh,Lovell) Theorem, <bpt id="p1">*</bpt>Journal of Economic Education<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>lm, <bpt id="p1">[</bpt>rxLogit<ept id="p1">](rxLogit.md)</ept>, <bpt id="p2">[</bpt>rxTransform<ept id="p2">](rxTransform.md)</ept>.</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>