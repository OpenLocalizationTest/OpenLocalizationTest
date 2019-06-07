<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxglm.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c3776aa4d058ceefbac702d4539c781afe5fb4dd90b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">76aa4d058ceefbac702d4539c781afe5fb4dd90b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxglm.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxGlm function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Use rxGlm to fit generalized linear regression models for small or large data.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Any valid glm family object can be used.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxGlm, models, regression</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>rxGlm: Generalized Linear Models</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`rxGlm`</ph> to fit generalized linear regression models for small or large data.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Any valid glm family object can be used.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>formula as described in <bpt id="p1">[</bpt>rxFormula<ept id="p1">](rxFormula.md)</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>either a data source object, a character string specifying a .xdf file, or a data frame object.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>either an object of class family or a character string specifying the family.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A family is a description of the error distribution and is associated with a link function to be used in the model.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Any valid family object may be used.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The following family/link combinations are implemented in C++: binomial/logit, gamma/log, poisson/log,  and Tweedie.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Other family/link combinations use a combination of C++ and R code.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>For the Tweedie distribution, use  <ph id="ph1">`family=rxTweedie(var.power, link.power)`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>It is also possible to use <ph id="ph1">`family=tweedie(var.power, link.power)`</ph> from the  R package <bpt id="p1">**</bpt>tweedie<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as probability weights for the observations.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>character string specifying the variable to use as frequency weights for the observations.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>character string specifying a variable to use as an offset for the model (<ph id="ph1">`offset="x"`</ph>).</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>An offset may also be specified as a term in the formula (<ph id="ph1">`offset(x)`</ph>).</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>An offset is a variable to be included as part of the linear predictor that requires no coefficient.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> and the first term of the predictor variables is categorical (a factor or an interaction of factors), the regression is performed by applying the Frisch-Waugh-Lovell Theorem, which uses a partitioned inverse to save on computation time and memory.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>See Details section below.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>a list specifying various parameters that control aspects of stepwise regression.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If it is an empty list (default), no stepwise model selection will be performed.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If not, stepwise regression will be performed and <ph id="ph1">`cube`</ph> must be <ph id="ph2">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxStepControl<ept id="p1">](rxStepControl.md)</ept> for details.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>name of a logical variable in the data set (in quotes) or a logical expression using variables in the data set to specify row selection.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rowSelection = "old"`</ph> will use only observations in which the value of the variable <ph id="ph2">`old`</ph> is <ph id="ph3">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>will use only observations in which the value of the <ph id="ph1">`age`</ph> variable is between 20 and 65 and the value of the <ph id="ph2">`log`</ph> of the <ph id="ph3">`income`</ph> variable is greater than 10.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The row selection is performed after processing any data transformations  (see the arguments <ph id="ph1">`transforms`</ph> or <ph id="ph2">`transformFunc`</ph>).</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`rowSelection`</ph> can be defined outside of the function  call using the expression function.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>an expression of the form <ph id="ph1">`list(name = expression, ...)`</ph> representing the first round of variable transformations.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>As with all expressions, <ph id="ph1">`transforms`</ph> (or <ph id="ph2">`rowSelection`</ph>)  can be defined outside of the function call using the expression function.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>a named list containing objects that can be referenced by <ph id="ph1">`transforms`</ph>, <ph id="ph2">`transformsFunc`</ph>, and <ph id="ph3">`rowSelection`</ph>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>variable transformation function.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>character vector of input data set variables needed for the transformation function.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>See <bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept> for details.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>character vector defining additional R packages (outside of those specified in <ph id="ph1">`rxGetOption("transformPackages")`</ph>) to be made available and  preloaded for use in variable transformation functions, e.g., those explicitly defined in <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> functions via their <ph id="ph2">`transforms`</ph> and <ph id="ph3">`transformFunc`</ph> arguments or those  defined implicitly via their <ph id="ph4">`formula`</ph> or <ph id="ph5">`rowSelection`</ph> arguments.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`transformPackages`</ph> argument may also be <ph id="ph2">`NULL`</ph>,  indicating that no packages outside <ph id="ph3">`rxGetOption("transformPackages")`</ph> will be preloaded.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>user-defined environment to serve as a parent to  all environments developed internally and used for variable data transformation.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`transformEnvir = NULL`</ph>, a new "hash" environment with parent <ph id="ph2">`baseenv()`</ph> is used instead.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, the last level is dropped in  all sets of factor levels in a model.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>If that level has no observations (in any of  the sets), or if the model as formed is otherwise determined to be singular, then  an attempt is made to estimate the model by dropping the first level in all sets  of factor levels.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the starting position is to drop the first level.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Note that for cube regressions, the first set of factors is excluded from these rules  and the intercept is dropped.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>logical value.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, main-effect terms are dropped before their interactions.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph> and if <ph id="ph2">`cube`</ph> is <ph id="ph3">`FALSE`</ph>,  the variance-covariance matrix of the regression coefficients is returned.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">[</bpt>rxCovCoef<ept id="p1">](rxCovRegression.md)</ept> function to obtain these data.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>logical flag.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, the AIC of the fitted model is returned.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The default is <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Starting values for the Iteratively Reweighted Least Squares algorithm  used to estimate the model coefficients.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Supported values for this argument come in three forms:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>- The initial values are based upon the 'mustart' values generated by the family$initialize expression if an R family object is used, or the equivalent for a family coded in C++.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>- A numeric scalar that will be replicated once for each of the coefficients in the model to  form the initial values.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Zeros may be good starting values, depending upon the model.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>- A numeric vector of length <ph id="ph1">`K`</ph>, where <ph id="ph2">`K`</ph> is the number of model coefficients, including the intercept if any and including any that might be dropped from sets of dummies.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>This argument is  most useful when a set of estimated coefficients is available from a similar set of data.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Note that <ph id="ph1">`K`</ph> can be found by running the model on a small number of observations and obtaining  the number of coefficients from the output, say <ph id="ph2">`z`</ph>, via <ph id="ph3">`length(z$coefficients)`</ph>.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>character string specifying the coefficient label style.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The default is "Revo".</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>If "R", R-compatible labels are created.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>number of blocks to read for each chunk of data read from the data source.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>maximum number of iterations.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>convergence tolerance for coefficients.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>If the maximum absolute  change in the coefficients (step), divided by the maximum absolute coefficient value, is less than or equal to this tolerance at the end of an iteration, the estimation is considered to have converged.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>To disable this test, set this value to 0.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>convergence tolerance for the objective function.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>If the absolute  relative change in the deviance (-2.0 times log likelihood) is less than or equal to this tolerance at the end of an iteration, the estimation is considered to have converged.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>To disable this test, set this value to 0.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>integer value with options:</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>: no progress is reported.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>: the number of processed rows is printed and updated.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>: rows processed and timings are reported.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>: rows processed and all timings are reported.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>integer value.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`0`</ph>, no verbose output is printed during calculations.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Integer values from <ph id="ph1">`1`</ph> to <ph id="ph2">`4`</ph> provide increasing amounts of information are provided.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>a valid <bpt id="p1">[</bpt>RxComputeContext<ept id="p1">](RxComputeContext.md)</ept>.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`RxSpark`</ph>  and <ph id="ph2">`RxHadoopMR`</ph> compute  contexts distribute the computation among the nodes specified by the  compute context; for other compute contexts, the  computation is distributed if possible on the local computer.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Revolution Compute Engine.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>The special function <ph id="ph1">`F()`</ph> can be used in <ph id="ph2">`formula`</ph> to force a variable to be interpreted as a factor.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>When <ph id="ph1">`cube`</ph> is <ph id="ph2">`TRUE`</ph>, the Frisch-Waugh-Lovell (FWL) Theorem is applied to the model.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>The FWL approach parameterizes the model to include one coefficient for each category (a single factor level or combination of factor levels) instead of using an intercept in the model with contrasts for each of the factor combinations.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Additionally when <ph id="ph1">`cube`</ph> is <ph id="ph2">`TRUE`</ph>, the output contains a <ph id="ph3">`countDF`</ph> element representing the counts for each category.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>an rxGlm object containing the following elements:</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>named vector of coefficients.</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>variance-covariance matrix for the regression coefficient estimates.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>estimated reciprocal condition number of final weighted cross-product (X'WX) matrix.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>numeric rank of the fitted linear model.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>logical vector specifying whether columns were dropped or not due to collinearity.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>standard errors of the coefficients.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>coefficients divided by their standard errors.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>p-values for coef.t.value; for the poisson and binomial families, the dispersion is taken to be 1, and the normal distribution is used (Pr(&gt;|z|)); for other families the dispersion is estimated,  and the t distribution is used (Pr(&gt;|t|)).</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>the p-value resulting from an F-test on the fitted model.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>degrees of freedom, a 3-vector (p, n-p, p*), the last being the number of non-aliased coefficients.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>(for models including non-intercept terms) a 3-vector with the value of the F-statistic with its numerator and denominator degrees of freedom.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>parameters sent to Microsoft R Services Compute Engine.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>the model formula</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>the matched call.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>number of valid observations.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>number of missing observations.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>minus twice the maximized log-likelihood (up to a constant)</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>for the poisson and binomial families, the dispersion is 1;  for other families the dispersion is estimated, and is the Pearson chi-squared statistic divided by the residual degrees of freedom.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Note</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>The generalized linear models are computed using the Iteratively Reweighted Least Squares (IRLS) algorithm.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>glm, family, <bpt id="p1">[</bpt>rxLinMod<ept id="p1">](rxLinMod.md)</ept>, <bpt id="p2">[</bpt>rxLogit<ept id="p2">](rxLogit.md)</ept>, <bpt id="p3">[</bpt>rxTweedie<ept id="p3">](rxTweedie.md)</ept>, <bpt id="p4">[</bpt>rxTransform<ept id="p4">](rxTransform.md)</ept>.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>