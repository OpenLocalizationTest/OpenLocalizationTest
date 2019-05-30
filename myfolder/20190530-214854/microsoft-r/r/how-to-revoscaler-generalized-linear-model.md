<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-generalized-linear-model.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e5b9bad6ea3acefa9de372beb279e827e21303851.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5b9bad6ea3acefa9de372beb279e827e21303851</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-generalized-linear-model.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Generalized Linear Models (RevoScaleR) in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Generalized linear models with RevoScaleR.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Generalized Linear Models using RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Generalized linear models (GLM) are a framework for a wide range of analyses.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>They relax the assumptions for a standard linear model in two ways.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>First, a functional form can be specified for the conditional mean of the predictor, referred to as the “link” function.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Second, you can specify a distribution for the response variable.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The rxGlm function in RevoScaleR provides the ability to estimate generalized linear models on large data sets.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The following family/link combinations are implemented in C++ for performance enhancements: binomial/logit, gamma/log, poisson/log, and Tweedie.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Other family/link combinations use a combination of C++ and R code.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Any valid R family object that can be used with glm() can be used with rxGlm(), including user-defined.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The following table shows all of the supported family/link combinations (in addition to user-defined):</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Family</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Default Link Function</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Other Available Link Functions</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>binomial</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>"logit"</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>"probit", "cauchit", "log", "cloglog"</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>gaussian</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>"identity"</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>"log", "inverse"</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Gamma</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>"inverse"</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>"identity", "log"</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>inverse.gaussian</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>"1/mu^2"</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>"inverse", "identity", "log"</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>poisson</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>"log"</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>"identity", "sqrt"</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>quasi</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>"identity" with variance = "constant"</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>"logit", "probit", "cloglog", "inverse", "log", "1/mu^2", "sqrt"</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>quasibinomial</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>"logit"</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Same as binomial, but dispersion parameter not fixed at one</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>quasipoisson</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>"log"</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Same as poisson, but dispersion parameter not fixed at one</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>rxTweedie</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>requires arguments instead of link function</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>A Simple Example Using the Poisson Family</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The Poisson family is used to estimate models of count data.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Examples from the literature include the following types of response variables:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Number of drinks on a Saturday night</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Number of bacterial colonies in a Petri dish</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Number of children born to married women</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Number of credit cards a person has</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>We’ll start with a simple example from Kabacoff’s <bpt id="p1">**</bpt>R in Action<ept id="p1">**</ept> book, using data provided with the <bpt id="p2">***</bpt>robust<ept id="p2">***</ept> R package.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The data are from a placebo-controlled clinical trial of 59 epileptics.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Patients with partial seizures were enrolled in a randomized clinical trial of the anti-epileptic drug, progabide.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Counts of epileptic seizures were recorded during the trial.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The data set also includes a baseline 8-week seizure count and the age of the patient.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>To access this data, first make sure the <bpt id="p1">***</bpt>robust<ept id="p1">***</ept> package is installed, then use the <bpt id="p2">*</bpt>data<ept id="p2">*</ept> command to load the data frame:</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>First, let’s get some basic information on the data set, then draw a histogram of the sumY variable, containing the total count of seizures during the trial.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The data set has 59 observations, and 12 variables.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>The variables of interest are <bpt id="p1">*</bpt>Base<ept id="p1">*</ept>, <bpt id="p2">*</bpt>Age<ept id="p2">*</ept>, <bpt id="p3">*</bpt>Trt<ept id="p3">*</ept>, and <bpt id="p4">*</bpt>sumY<ept id="p4">*</ept>.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>To estimate a model with <bpt id="p1">*</bpt>sumY<ept id="p1">*</ept> as the response variable and the <bpt id="p2">*</bpt>Base<ept id="p2">*</ept> number of seizures, <bpt id="p3">*</bpt>Age<ept id="p3">*</ept>, and the treatment as explanatory variables, we can use <bpt id="p4">*</bpt>rxGlm<ept id="p4">*</ept>.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>A benefit to using <bpt id="p1">*</bpt>rxGlm<ept id="p1">*</ept> is that the code scales for use with a much bigger data set.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Results in:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>To interpret the coefficients, it is sometimes useful to transform them back to the original scale of the dependent variable.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>In this case:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>This suggests that, controlling for the base number of seizures and age, people taking progabide during the trial had 85% of the expected number seizures compared with people who didn’t.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>A common method of checking for overdispersion is to calculate the ratio of the residual deviance with the degrees of freedom.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>This should be about 1 to fit the assumptions of the model.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>We can see that the ratio is well above one.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>The quasi-poisson family can be used to handle over-dispersion.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>In this case, instead of assuming that the variance and mean are one, a relationship is estimated from the data:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Notice that the coefficients are the same as when using the poisson family, but that the standard errors are larger.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>The effect of the treatment is no longer significant.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>An Example Using the Gamma Family</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>The Gamma family is used with data containing positive values with a positive skew.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>A classic example is estimating the value of auto insurance claims.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Using the sample <bpt id="p1">*</bpt>claims.xdf<ept id="p1">*</ept> data set:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>But, these estimates are conditional on the fact that a claim was made.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>An Example Using the Tweedie Family</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The Tweedie family of distributions provides flexible models for estimation.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>The power parameter <bpt id="p1">*</bpt>var.power<ept id="p1">*</ept> determines the shape of the distribution, with familiar models as special cases: if <bpt id="p2">*</bpt>var.power<ept id="p2">*</ept> is set to 0, Tweedie is a normal distribution; when set to 1, it is Poisson; when 2, it is Gamma; when 3, it is inverse Gaussian.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>var.power<ept id="p1">*</ept> is between 1 and 2, it is a compound Poisson distribution and is appropriate for positive data that also contains exact zeros, for example, insurance claims data, rainfall data, or fish-catch data.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">*</bpt>var.power<ept id="p1">*</ept> is greater than 2, it is appropriate for positive data.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>In this example, we use a subsample from the 5% sample of the U.S. 2000 census.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>We consider the annual cost of property insurance for heads of household ages 21 through 89, and its relationship to age, sex, and region.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>A variable “perwt” in the data set represents the probability weight for that observation.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>First, to create the subsample (specify the correct data path for your downloaded data):</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored when run locally using R Client.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>An Xdf data source representing the new data file is returned.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>The new data file has over 5 million observations.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Let’s do one more step in data cleaning.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The variable <bpt id="p1">*</bpt>region<ept id="p1">*</ept> has some long factor level character strings, and it also has a number of levels for which there are no observations.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>We can see this using <bpt id="p1">*</bpt>rxSummary<ept id="p1">*</ept>:</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>We can use the <bpt id="p1">*</bpt>rxFactors<ept id="p1">*</ept> function rename and reduce the number of levels:</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>As a first step to analysis, let’s look at a histogram of the property insurance cost:</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>This data appears to be a good match for the Tweedie family with a variance power parameter between 1 and 2, since it has a “clump” of exact zeros in addition to a distribution of positive values.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>We can estimate the parameters using <bpt id="p1">*</bpt>rxGlm<ept id="p1">*</ept>, setting the <bpt id="p2">*</bpt>var.power<ept id="p2">*</ept> argument to 1.5.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>As explanatory variables we’ll use sex, an “on-the-fly” factor variable with a level for each age, and region:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>A good way to begin examining the results of the estimated model is to look at predicted values for given explanatory characteristics.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>For example, let’s create a prediction data set for the South Atlantic region for all ages and sexes:</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Now we’ll use that as a basis for a similar prediction data set for the Middle Atlantic region:</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Next we combine the two data sets, and compute the predicted values for annual property insurance cost using our estimated <bpt id="p1">*</bpt>rxGlm<ept id="p1">*</ept> model:</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Stepwise Generalized Linear Models</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Stepwise generalized linear models help you determine which variables are most important to include in the model.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>You provide a minimal, or lower, model formula and a maximal, or upper, model formula.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>Using forward selection, backward elimination, or bidirectional search, the algorithm determines the model formula that provides the best fit based on an AIC selection criterion or a significance level criterion.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>As an example, consider again the Gamma family model from earlier in this article:</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>We can recast this model as a stepwise model by specifying a variableSelection argument using the rxStepControl function to provide our stepwise arguments:</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>We see that in the stepwise model fit, age no longer appears in the final model.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Plotting Model Coefficients</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>The ability to save model coefficients using the argument <bpt id="p1">*</bpt>keepStepCoefs = TRUE<ept id="p1">*</ept> within the <bpt id="p2">*</bpt>rxStepControl<ept id="p2">*</ept> call, and to plot them with the function <bpt id="p3">*</bpt>rxStepPlot<ept id="p3">*</ept> was described in great detail for stepwise <bpt id="p4">*</bpt>rxLinMod<ept id="p4">*</ept> in <bpt id="p5">[</bpt>Fitting Linear Models using RevoScaleR<ept id="p5">](how-to-revoscaler-linear-model.md)</ept>.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>This functionality is also available for stepwise <bpt id="p1">*</bpt>rxGLM<ept id="p1">*</ept> objects.</source>
        </trans-unit></group></body></file></xliff>