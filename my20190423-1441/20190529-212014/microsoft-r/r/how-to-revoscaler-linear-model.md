<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-linear-model.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3a9637c289160a14b1649e2be0842d4529a5752ee.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a9637c289160a14b1649e2be0842d4529a5752ee</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-linear-model.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Fitting Linear Models (RevoScaleR) in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Linear Models with RevoScaleR.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Fitting Linear Models using RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Linear regression models are fitted in RevoScaleR using the <bpt id="p1">*</bpt>rxLinMod<ept id="p1">*</ept> function.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Like other RevoScaleR functions, <bpt id="p1">*</bpt>rxLinMod<ept id="p1">*</ept> uses an updating algorithm to compute the regression model.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>The R object returned by <bpt id="p1">*</bpt>rxLinMod<ept id="p1">*</ept> includes the estimated model coefficients and the call used to generate the model, together with other information that allows RevoScaleR to recompute the model.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>BSecause <bpt id="p1">*</bpt>rxLinMod<ept id="p1">*</ept> is designed to work with arbitrarily large data sets, quantities such as residuals, and fitted values are not included in the return object, although these can be obtained easily once the model has been fitted.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>As a simple example, let’s use the sample data set AirlineDemoSmall.xdf and fit the arrival delay by day of week:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Because our predictor is categorical, we can use the <bpt id="p1">*</bpt>cube<ept id="p1">*</ept> argument to <bpt id="p2">*</bpt>rxLinMod<ept id="p2">*</ept> to perform the regression using a partitioned inverse, which may be faster and may use less memory than the standard algorithm.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The output object also includes a data frame with the averages or counts for each category:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Typing the name of the object arrDelayLm1 yields the following output:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Obtaining a Summary of the Model</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The print method for the rxLinMod model object shows only the call and the coefficients.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>You can obtain more information about the model by calling the summary method:</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>This produces the following output, which includes substantially more information about the model coefficients, together with the residual standard error, multiple R-squared, and adjusted R-squared:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>DayOfWeek=Sunday     10.3318     0.1330   77.67 2.22e-16 ***</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>93395</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Using Probability Weights</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Probability weights are common in survey data; they represent the probability that a case was selected into the sample from the population, and are calculated as the inverse of the sampling fraction.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The variable <bpt id="p1">*</bpt>perwt<ept id="p1">*</ept> in the census data represents a probability weight.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>You pass probability weights to the RevoScaleR analysis functions using the <bpt id="p1">*</bpt>pweights<ept id="p1">*</ept> argument, as in the following example:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Yields the following output:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Using Frequency Weights</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Frequency weights are useful when your data has a particular form: a set of data in which one or more cases is exactly replicated.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>If you then compact the data to remove duplicated observations and create a variable to store the number of replications of each observation, you can use that new variable as a frequency weights variable in the RevoScaleR analysis functions.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>For example, the sample data set fourthgraders.xdf contains the following 44 rows:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>reps<ept id="p1">*</ept> column shows the number of replications for each observation; the sum of the reps column indicates the total number of observations, in this case 100.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>We can fit a model (admittedly not very useful) of height on eye color with <bpt id="p1">*</bpt>rxLinMod<ept id="p1">*</ept> as follows:</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Typing the name of the object shows the following output:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Using rxLinMod with R Data Frames</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>While RevoScaleR is primarily designed to work with data on disk, it can also be used with in-memory R data frames.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>As an example, consider the R sample data frame “cars”, which contains data recorded in the 1920s on the speed of cars and the distances taken to stop.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>We get the following output (which matches the output given by the R function lm):</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Using the Cube Option for Conditional Predictions</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>If the cube argument is set to TRUE and the first term of the independent variables is categorical, <bpt id="p1">*</bpt>rxLinMod<ept id="p1">*</ept> will compute and return a data frame with category counts.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If there are no other independent variables, or if the <bpt id="p1">*</bpt>cubePredictions<ept id="p1">*</ept> argument is set to TRUE, the data frame will also contain predicted values.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Let’s create a simple data frame to illustrate:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>If we estimate a simple linear regression of y on xfac1, the coefficients are equal to the within- group means:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>In addition to the standard output, the returned object contains a <bpt id="p1">*</bpt>countDF<ept id="p1">*</ept> data frame with information on within-group means and counts in each category.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>In this simple case the within-group means are the same as the coefficients:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Using rxLinMod with the cube option also allows us to compute conditional within-group means.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>If we look at the countDF, we see the within-group means, conditional on the average value of the conditioning variable, xfac2:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>For the variable xfac2, 50% of the observations have the value “One2”, 25% of the observations have the value “Two2”, and 25% have the value “Three2”.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>We can compute the weighted average of the coefficients for xfac2 as:</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>To compute the conditional within-group mean shown in the countDF for xfac1 equal to “One1”, we add this to the coefficient computed for “One1”:</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Conditional within-group means can also be computed using additional continuous independent variables.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Fitted Values, Residuals, and Prediction</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>When you fit a model with lm or any of the other core R model-fitting functions, you get back an object that includes as components both the fitted values for the response variable and the model residuals.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>For models fit with rxLinMod or other RevoScaleR functions, it is usually impractical to include these components, as they can be many megabytes in size.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Instead, they are computed on demand using the rxPredict function.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>This function takes an rxLinMod object as its first argument, an input data set as its second argument, and an output data set as its third argument.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>If the input data set is the same as the data set used to fit the rxLinMod object, the resulting predictions are the fitted values for the model.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>If the input data set is a different data set (but one containing the same variable names used in fitting the rxLinMod object), the resulting predictions are true predictions of the response for the new data from the original model.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>In either case, residuals for the predicted values can be obtained by setting the flag computeResiduals to TRUE.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>For example, we can draw from the 7% sample of the large airline data set (available <bpt id="p1">[</bpt>online<ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698896&amp;clcid=0x409)</ept>) training and prediction data sets as follows (remember to customize the first line below for your own system):</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>We can then fit a linear model with the training data and compute predicted values on the prediction data set as follows:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>To see the first few rows of the result, use rxGetInfo as follows:</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Prediction Standard Errors, Confidence Intervals, and Prediction Intervals</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>You can also use rxPredict to obtain prediction standard errors, provided you have included the variance-covariance matrix in the original rxLinMod fit.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>If you choose to compute the prediction standard errors, you can also obtain either of two kinds of intervals: <bpt id="p1">*</bpt>confidence intervals<ept id="p1">*</ept> that for a given confidence level tells us how confident we are that the expected value is within the given interval, and <bpt id="p2">*</bpt>prediction intervals<ept id="p2">*</ept> that specify, for a given confidence level, how likely future observations are to fall within the interval given what has already been observed.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Standard error computations are computationally intensive, and they may become prohibitive on large data sets with a large number of predictors.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>To illustrate the computation, we start with a small data set, using the example on page 132 of <bpt id="p1">*</bpt>Introduction to the Practice of Statistics,<ept id="p1">*</ept> (5<bpt id="p2">&lt;sup&gt;</bpt>th<ept id="p2">&lt;/sup&gt;</ept> Edition).</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>The predictor, neaInc, is the increase in “non-exercise activity” in response to an increase in caloric intake.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The response, fatGain, is the associated increase in fat.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>We first read in the data and create a data frame to use in our analysis:</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Next we fit the linear model with rxLinMod, setting covCoef=TRUE to ensure we have the variance-covariance matrix in our model object:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Now we use rxPredict to obtain the fitted values, prediction standard errors, and confidence intervals.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>By setting writeModelVars to TRUE, the variables used in the model will also be included in the output data set.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>In this first example, we obtain confidence intervals:</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>The standard errors are by default put into a variable named by concatenating the name of the response variable with an underscore and the string “StdErr”:</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>We can view the original data, the fitted prediction line, and the confidence intervals as follows:</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>The resulting plot is shown below:</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>The prediction intervals can be obtained and plotted as follows:</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>The resulting plot is shown below:</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>We can fit the prediction standard errors on our large airline regression model if we first refit it with covCoef=TRUE:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>We can then obtain the prediction standard errors and a confidence interval as before:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>We can then look at the first few lines of targetInfile to see the first few predictions and standard errors:</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Stepwise Variable Selection</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Stepwise linear regression is an algorithm that helps you determine which variables are most important to a regression model.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>You provide a minimal, or lower, model formula and a maximal, or upper, model formula, and using forward selection, backward elimination, or bidirectional search, the algorithm determines the model formula that provides the best fit based on an AIC selection criterion.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>In SAS, stepwise linear regression is implemented through PROC REG.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>In open-source R, it is implemented through the function <bpt id="p1">*</bpt>step<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>The problem with using the function <bpt id="p1">*</bpt>step<ept id="p1">*</ept> in R is that the size of the data set that can be analyzed is severely limited by the requirement that all computations must be done in memory.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>RevoScaleR provides an implementation of stepwise linear regression that is not constrained by the use of "in-memory" algorithms.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Stepwise linear regression in RevoScaleR is implemented by the functions <bpt id="p1">*</bpt>rxLinMod<ept id="p1">*</ept> and <bpt id="p2">*</bpt>rxStepControl<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Stepwise linear regression begins with an initial model of some sort.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Consider, for example,  the airline training data set AirlineData06to07.xdf featured in <bpt id="p1">[</bpt>Fitting Linear Models using RevoScaleR<ept id="p1">](how-to-revoscaler-linear-model.md)</ept>:</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>We are interested in fitting a model that will predict arrival delay (<bpt id="p1">*</bpt>ArrDelay<ept id="p1">*</ept>) as a function of some of the other variables.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>To keep things simple, we’ll start with our by now familiar model of arrival delay as a function of <bpt id="p1">*</bpt>DayOfWeek<ept id="p1">*</ept> and <bpt id="p2">*</bpt>CRSDepTime<ept id="p2">*</ept>:</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>The question is, can we improve this model by adding more predictors?</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>If so, which ones?</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>To use stepwise selection in RevoScaleR, you add the <bpt id="p1">*</bpt>variableSelection<ept id="p1">*</ept> argument to your call to <bpt id="p2">*</bpt>rxLinMod<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>variableSelection<ept id="p1">*</ept> argument is a list, most conveniently created by using the <bpt id="p2">*</bpt>rxStepControl<ept id="p2">*</ept> function.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Using <bpt id="p1">*</bpt>rxStepControl<ept id="p1">*</ept>, you specify the method (the default, "stepwise", specifies a bidirectional search), the scope (lower and upper formulas for the search), and various control parameters.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>With our model, we first want to try some more numeric predictors, so we specify our model as follows:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Methods of Variable Selection</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Three methods of variable selection are supported by rxLinMod:</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>"forward"<ept id="p1">*</ept>: starting from the minimal model, variables are added one at a time until no additional variable satisfies the selection criterion, or until the maximal model is reached.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>"backward"<ept id="p1">*</ept>: starting from the maximal model, variables are removed one at a time until the removal of another variable won’t satisfy the selection criterion, or until the minimal model is reached.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>"stepwise"<ept id="p1">*</ept> (the default): a combination of forward and backward selection, in which variables are added to the minimal model, but at each step, the model is reanalyzed to see if any variables that have been added are candidates for deletion from the current model.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>You specify the desired method by supplying a named component <bpt id="p1">*</bpt>"method"<ept id="p1">*</ept> in the list supplied for the <bpt id="p2">*</bpt>variableSelection<ept id="p2">*</ept> argument, or by specifying the <bpt id="p3">*</bpt>method<ept id="p3">*</ept> argument in a call to <bpt id="p4">*</bpt>rxStepControl<ept id="p4">*</ept> that is then passed as the <bpt id="p5">*</bpt>variableSelection<ept id="p5">*</ept> argument.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Variable Selection with Wide Data</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>We’ve found that generalized linear models do not converge if the number of predictors is greater than the number of observations.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>If your data has more variables, it won’t be possible to include all of them in the maximal model for stepwise selection.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>We recommend you use domain experience and insights from initial data explorations to choose a subset of the variables to serve as the maximal model before performing stepwise selection.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>There are a few things you can do to reduce the number of predictors.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>If there are many variables that measure the same quantitative or qualitative entity, try to select one variable that represents the entity best.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>For example, include a variable that identifies a person’s political party affiliation instead of including many variables representing how the person feels about individual issues.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>If your goal with linear modeling is the interpretation of individual predictors, you want to ensure that correlation between variables in the model is minimal to avoid multicollinearity.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>This means checking for these correlations before modeling.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Sometimes it is useful to combine correlated variables into a composite variable.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Height and weight are often correlated, but can be transformed into BMI.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Combining variables allows you to reduce the number of variables without losing any information.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Ultimately, the variables you select will depend on how you plan to use the results of your linear model.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Specifying Model Scope</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>You use the <bpt id="p1">*</bpt>scope<ept id="p1">*</ept> argument in <bpt id="p2">*</bpt>rxStepControl<ept id="p2">*</ept> (or a named component <bpt id="p3">*</bpt>"scope"<ept id="p3">*</ept> in the list supplied for the <bpt id="p4">*</bpt>variableSelection<ept id="p4">*</ept> argument) to specify which variables should be considered for inclusion in the final model selection and which should be ignored.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>Whether you specify a separate value for scope also determines which models the algorithm tries next.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>You can specify the scope as a simple formula (which will be treated as the upper bound, or maximal model), or as a named list with components <bpt id="p1">*</bpt>"lower"<ept id="p1">*</ept> and <bpt id="p2">*</bpt>"upper"<ept id="p2">*</ept> (either of which may be missing).</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>For example, to analyze the iris data with a minimal model involving the single predictor <bpt id="p1">*</bpt>Sepal.Width<ept id="p1">*</ept> and a maximal model involving <bpt id="p2">*</bpt>Sepal.Width<ept id="p2">*</ept>, <bpt id="p3">*</bpt>Petal.Length<ept id="p3">*</ept>, and the interaction between <bpt id="p4">*</bpt>Petal.Width<ept id="p4">*</ept> and <bpt id="p5">*</bpt>Species<ept id="p5">*</ept>, we can specify our variable selection model as follows:</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>In general, the models considered are determined from the <bpt id="p1">*</bpt>scope<ept id="p1">*</ept> argument as follows:</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>"lower"<ept id="p1">*</ept> scope only: All models considered will include this lower model up to the base model specified in the <bpt id="p2">*</bpt>formula<ept id="p2">*</ept> argument to <bpt id="p3">*</bpt>rxLinMod<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>"upper"<ept id="p1">*</ept> scope only: All models considered will include the terms in the base model (specified by the <bpt id="p2">*</bpt>formula<ept id="p2">*</ept> argument to <bpt id="p3">*</bpt>rxLinMod<ept id="p3">*</ept>), plus additional terms as specified in the upper scope.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Both <bpt id="p1">*</bpt>"lower"<ept id="p1">*</ept> and <bpt id="p2">*</bpt>"upper"<ept id="p2">*</ept> scope supplied: All models considered will include at least the terms in the lower scope and additional terms are added using terms from the upper scope until the stopping criterion is reached or the full upper scope model is selected.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>No scope supplied: The minimal model includes just the intercept term and the maximal model include at most the terms specified in the base model.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>(This convention is identical to that used by R’s <bpt id="p1">*</bpt>step<ept id="p1">*</ept> function.)</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Specifying the Selection Criterion</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>By default, variable selection is determined using the Akaike Information Criterion, or AIC; this is the R standard.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>If you want a stepwise selection that is more SAS-like, you can specify <bpt id="p1">*</bpt>stepCriterion="SigLevel".<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>If this is set, rxLinMod uses either an F-test (default) or Chi-square test to determine whether to add or drop terms from the model.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>You can specify which test to perform using the <bpt id="p1">*</bpt>test<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>For example, we can refit our airline model using the SigLevel step criterion with an F-test as follows:</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>In this case (and with many other well-behaved models), the results of using the SigLevel step criterion are identical to those using AIC.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>You can control the significance levels for adding and dropping models using the <bpt id="p1">*</bpt>maxSigLevelToAdd<ept id="p1">*</ept> and <bpt id="p2">*</bpt>minSigLevelToDrop<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>maxSigLevelToAdd<ept id="p1">*</ept> specifies a significance level below which a variable can be considered for inclusion in the model; the <bpt id="p2">*</bpt>minSigLevelToDrop<ept id="p2">*</ept> specifies a significance level above which a variable currently included can be considered for dropping.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>By default, for <bpt id="p1">*</bpt>method="stepwise",<ept id="p1">*</ept> both the levels are set to 0.15.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>We can tighten the selection criterion to the 0.10 level as follows:</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Plotting Model Coefficients</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>By default, the values of the parameters at each step of the stepwise selection are not preserved.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Using an additional argument, <bpt id="p1">*</bpt>keepStepCoefs<ept id="p1">*</ept>, in your <bpt id="p2">*</bpt>rxStepControl<ept id="p2">*</ept> statement saves the values of the coefficients from each step of the regression.</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>This coefficient data can then be plotted using another function, <bpt id="p1">*</bpt>rxStepPlot.<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Consider the stepwise linear regression on the iris data from <bpt id="p1">[</bpt>Fitting Linear Models using RevoScaleR<ept id="p1">](how-to-revoscaler-linear-model.md)</ept>:</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Notice the addition of the argument <bpt id="p1">*</bpt>keepStepCoefs = TRUE<ept id="p1">*</ept> to the <bpt id="p2">*</bpt>rxStepContol<ept id="p2">*</ept> call.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>This produces an extra piece of output in the <bpt id="p1">*</bpt>rxLinMod<ept id="p1">*</ept> object, a dataframe containing the values of the coefficients at each step of the regression.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>This dataframe, <bpt id="p1">*</bpt>stepCoefs<ept id="p1">*</ept>, can be accessed as follows:</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>Trying to glean patterns and information from a table can be difficult.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>So we’ve added another function, <bpt id="p1">*</bpt>rxStepPlot<ept id="p1">*</ept>, which allows the user to plot the parameter values at each step.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Using the iris model object, we plot the coefficients:</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>rxStepPlot(rxlm.step)</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>From this plot, we can tell when a variable enters the model by noting the step when it becomes non-zero.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Lines are labeled with the numbers on the right axis to indicate the parameter.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>The numbers correspond to the order they appear in the data frame <bpt id="p1">*</bpt>stepCoef<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>You’ll notice that the 7<bpt id="p1">&lt;sup&gt;</bpt>th<ept id="p1">&lt;/sup&gt;</ept> and 10<bpt id="p2">&lt;sup&gt;</bpt>th<ept id="p2">&lt;/sup&gt;</ept> parameters don’t show up in this plot because the <bpt id="p3">*</bpt>species3<ept id="p3">*</ept> parameter is the reference category for species.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>The function <bpt id="p1">*</bpt>rxStepPlot<ept id="p1">*</ept> is easily customized by using additional graphical parameters from the <bpt id="p2">*</bpt>matplot<ept id="p2">*</ept> function from base R. In the following example, we update our original call to <bpt id="p3">*</bpt>rxStepPlot<ept id="p3">*</ept> to demonstrate how to specify the colors used for each line, adjust the line width, and add a proper title to the plot:</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>By default, the <bpt id="p1">*</bpt>rxStepPlot<ept id="p1">*</ept> function uses seven line colors.</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>If the number of parameters exceeds the number of colors, they are reused in the same order.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>However, the line types are set to vary from 1 to 5, so lines that have the same color may differ in line type.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>The line types can also be specified using the <bpt id="p1">*</bpt>lty<ept id="p1">*</ept> argument in the <bpt id="p2">*</bpt>rxStepPlot<ept id="p2">*</ept> call.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Fixed-Effects Models</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>Fixed-effects models are commonly associated with studies in which multiple observations are recorded for each test subject, for example, yearly observations of median housing price by city, or measurements of tensile strength from samples of steel rods by batch.</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>To fit such a model with rxLinMod, include a factor variable specifying the subject (the cities, or the batch identifier) as the first predictor, and specify <bpt id="p1">*</bpt>cube=TRUE<ept id="p1">*</ept> to use a partitioned inverse and omit the intercept term.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>For example, the MASS library contains the data set <bpt id="p1">*</bpt>petrol<ept id="p1">*</ept>, which consists of measurements of the yield of a certain refining process with possible predictors including specific gravity, vapor pressure, ASTM 10% point, and volatility measured as the ASTM endpoint for 10 samples of crude oil.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>The following example (reproduced from <bpt id="p1">[</bpt>Modern Applied Statistics with S<ept id="p1">](http://www.springer.com/us/book/9780387954578)</ept>), first scales the numeric predictors, then fits the fixed-effects model:</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Least Squares Dummy Variable (LSDV) Models</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>RevoScaleR is capable of estimating huge models where fixed effects are estimated by dummy variables, that is, binary variables set to 1 or TRUE if the observation is in a particular category.</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>Creation of these dummy variables is often accomplished by interacting two or more factor variables using “:” in the formula.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>If the first term in an rxLinMod (or rxLogit) model is purely categorical and the “cube” argument is set to TRUE, the estimation uses a partitioned inverse to save on computation time and memory.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>A Quick Review of Interacting Factors</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>First, let’s do a quick, cautionary review of interacting factor variables by experimenting with a small made-up data set.</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>The data set has 20 observations with three variables: a numeric variable income and two factor variables representing region and sex.</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>There are three easy ways to compute the within group means of every combination of age and region using RevoScaleR.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>First, we can use <bpt id="p1">*</bpt>rxSummary<ept id="p1">*</ept>:</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>which includes in its output:</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>Second, we could use rxCube:</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>which includes in its output:</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>Or, we can use <bpt id="p1">*</bpt>rxLinMod<ept id="p1">*</ept> with <bpt id="p2">*</bpt>cube=TRUE<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>The intercept is automatically omitted, and four dummy variables are created from the two factors: one for each combination of region and sex.</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>The coefficients are simply the within group means:</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>which includes in its output:</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>The same model could be estimated using: <bpt id="p1">*</bpt>lm(income~region:sex + 0, data=myData<ept id="p1">*</ept>).</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>Below we refer to these within group means as <bpt id="p1">*</bpt>MeanIncRuralFemale, MeanIncUrbanFemale, MeanIncRuralMale,<ept id="p1">*</ept> and <bpt id="p2">*</bpt>MeanIncUrbanMale.<ept id="p2">*</ept></source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>If we add an intercept, we encounter perfect multicollinearity and one of the coefficients will be dropped.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>The intercept is then the mean of a reference group and the other coefficients represent the differences or contrasts between the within group means and the reference group.</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>For example,</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>produces:</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>We can see that the dummy variable for urban males was dropped; urban males are the reference group and the Intercept is equal to <bpt id="p1">*</bpt>MeanIncUrbanMale.<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>The other coefficients represent contrasts from the reference group, so for example, <bpt id="p1">*</bpt>regionRural:sexFemale<ept id="p1">*</ept> is equal to <bpt id="p2">*</bpt>MeanIncRuralFemale – MeanIncUrbanMale.<ept id="p2">*</ept></source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>Another variation is to use “<ph id="ph1">\*</ph>”in the formula for factor crossing.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>Using <bpt id="p1">*</bpt>a<ph id="ph1">\*</ph>b<ept id="p1">*</ept> is equivalent to using <bpt id="p2">*</bpt>a + b + a:b<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>which results in:</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>The dropping of coefficients in rxLinMod can be controlled to obtain the same results:</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>Coefficients using this model can be more difficult to interpret, and in fact are highly dependent on the order of the factor levels.</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>In this case, we see the following relationship between the estimated coefficients and the within group means</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>(Intercept)</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source>MeanIncRuralFemale</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source>regionUrban</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>MeanIncUrbanFemale – MeanIncRuralFemale</source>
        </trans-unit><trans-unit id="299" translate="yes" xml:space="preserve">
          <source>sexMale</source>
        </trans-unit><trans-unit id="300" translate="yes" xml:space="preserve">
          <source>MeanIncRuralMale – MeanIncRuralFemale</source>
        </trans-unit><trans-unit id="301" translate="yes" xml:space="preserve">
          <source>regionUrban:sexMale</source>
        </trans-unit><trans-unit id="302" translate="yes" xml:space="preserve">
          <source>MeanIncUrbanMale – MeanIncUrbanFemale - MeanIncRuralMale + MeanIncRuralFemale</source>
        </trans-unit><trans-unit id="303" translate="yes" xml:space="preserve">
          <source>If we set up our data slightly differently, we get different results.</source>
        </trans-unit><trans-unit id="304" translate="yes" xml:space="preserve">
          <source>Let’s use the same income data but a different naming convention for the factors:</source>
        </trans-unit><trans-unit id="305" translate="yes" xml:space="preserve">
          <source>Using the same model, <bpt id="p1">*</bpt>lm(income~region<ph id="ph1">\*</ph>sex, data=myData1)<ept id="p1">*</ept>, results in:</source>
        </trans-unit><trans-unit id="306" translate="yes" xml:space="preserve">
          <source>With this superficial modification to the data, the coefficient for the dummy variable for regionUrban has jumped from $1531 to $2464.</source>
        </trans-unit><trans-unit id="307" translate="yes" xml:space="preserve">
          <source>This is due to the change in reference group; in this model the Urban coefficient represents the difference between mean urban and rural male income, while in the previous model it was the difference between mean urban and rural female income.</source>
        </trans-unit><trans-unit id="308" translate="yes" xml:space="preserve">
          <source>That is, the relationship between the within group means and the new coefficients are:</source>
        </trans-unit><trans-unit id="309" translate="yes" xml:space="preserve">
          <source>(Intercept)</source>
        </trans-unit><trans-unit id="310" translate="yes" xml:space="preserve">
          <source>MeanIncRuralMale</source>
        </trans-unit><trans-unit id="311" translate="yes" xml:space="preserve">
          <source>regionUrban</source>
        </trans-unit><trans-unit id="312" translate="yes" xml:space="preserve">
          <source>MeanIncUrbanMale – MeanIncRuralMale</source>
        </trans-unit><trans-unit id="313" translate="yes" xml:space="preserve">
          <source>sexWoman</source>
        </trans-unit><trans-unit id="314" translate="yes" xml:space="preserve">
          <source>MeanIncRuralFemale – MeanIncRuralMale</source>
        </trans-unit><trans-unit id="315" translate="yes" xml:space="preserve">
          <source>regionUrban:sexMale</source>
        </trans-unit><trans-unit id="316" translate="yes" xml:space="preserve">
          <source>MeanIncUrbanFemale – MeanIncUrbanMale - MeanIncRuralFemale + MeanIncRuralMale</source>
        </trans-unit><trans-unit id="317" translate="yes" xml:space="preserve">
          <source>Omitting the intercept provides yet another combination of results.</source>
        </trans-unit><trans-unit id="318" translate="yes" xml:space="preserve">
          <source>For example, using rxLinMod with the original factor labeling:</source>
        </trans-unit><trans-unit id="319" translate="yes" xml:space="preserve">
          <source>results in:</source>
        </trans-unit><trans-unit id="320" translate="yes" xml:space="preserve">
          <source>region=Rural</source>
        </trans-unit><trans-unit id="321" translate="yes" xml:space="preserve">
          <source>MeanIncRuralMale</source>
        </trans-unit><trans-unit id="322" translate="yes" xml:space="preserve">
          <source>region=Urban</source>
        </trans-unit><trans-unit id="323" translate="yes" xml:space="preserve">
          <source>MeanIncUrbanMale</source>
        </trans-unit><trans-unit id="324" translate="yes" xml:space="preserve">
          <source>Sex=Female</source>
        </trans-unit><trans-unit id="325" translate="yes" xml:space="preserve">
          <source>MeanIncUrbanFemale – MeanIncUrbanMale</source>
        </trans-unit><trans-unit id="326" translate="yes" xml:space="preserve">
          <source>region=Rural, sex=Female</source>
        </trans-unit><trans-unit id="327" translate="yes" xml:space="preserve">
          <source>(MeanIncRuralFemale – MeanIncRuralMale) - (MeanIncUrbanFemale – MeanIncUrbanMale)</source>
        </trans-unit><trans-unit id="328" translate="yes" xml:space="preserve">
          <source>With large data sets it is common to estimate many interaction terms, and if some categories have zero counts, it may not even be obvious what the reference group is.</source>
        </trans-unit><trans-unit id="329" translate="yes" xml:space="preserve">
          <source>Also note that setting <bpt id="p1">*</bpt>cube=TRUE<ept id="p1">*</ept> in the preceding model is of limited use: only the first term from the expanded expression (in this case <bpt id="p2">*</bpt>region<ept id="p2">*</ept>) is estimated using a partitioned inverse.</source>
        </trans-unit><trans-unit id="330" translate="yes" xml:space="preserve">
          <source>Using Dummy Variables in rxLinMod: Letting the Data Speak Example 2</source>
        </trans-unit><trans-unit id="331" translate="yes" xml:space="preserve">
          <source>In previous articles, we looked at the CensusWorkers.xdf data set and examined the relationship between wage income and age.</source>
        </trans-unit><trans-unit id="332" translate="yes" xml:space="preserve">
          <source>Now let’s add another variable, and examine the relationship between wage income and sex and age.</source>
        </trans-unit><trans-unit id="333" translate="yes" xml:space="preserve">
          <source>We can start with a simple dummy variable model, computing the mean wage income by sex:</source>
        </trans-unit><trans-unit id="334" translate="yes" xml:space="preserve">
          <source>which computes:</source>
        </trans-unit><trans-unit id="335" translate="yes" xml:space="preserve">
          <source>Similarly, we could look at a simple linear relationship between wage income and age:</source>
        </trans-unit><trans-unit id="336" translate="yes" xml:space="preserve">
          <source>resulting in:</source>
        </trans-unit><trans-unit id="337" translate="yes" xml:space="preserve">
          <source>Computing the two end points on the regression line, we can plot it:</source>
        </trans-unit><trans-unit id="338" translate="yes" xml:space="preserve">
          <source>The next typical step is to combine the two approaches by estimating separate intercepts for males and females:</source>
        </trans-unit><trans-unit id="339" translate="yes" xml:space="preserve">
          <source>which results in:</source>
        </trans-unit><trans-unit id="340" translate="yes" xml:space="preserve">
          <source>age          573.232      5.816   98.56 2.22e-16 ***</source>
        </trans-unit><trans-unit id="341" translate="yes" xml:space="preserve">
          <source>We create a small sample data set with the same variables we use in censusWorkers, but with only four observations representing the high and low value of age for both sexes.</source>
        </trans-unit><trans-unit id="342" translate="yes" xml:space="preserve">
          <source>Using the <ph id="ph1">`rxPredict`</ph> function, the predicted values for each one of these sample observations is computed, which we then plot:</source>
        </trans-unit><trans-unit id="343" translate="yes" xml:space="preserve">
          <source>These types of models are often relaxed further by allowing both the slope and intercept to vary by group:</source>
        </trans-unit><trans-unit id="344" translate="yes" xml:space="preserve">
          <source>age for sex=Female   288.876      8.556   33.76 2.22e-16 ***</source>
        </trans-unit><trans-unit id="345" translate="yes" xml:space="preserve">
          <source>Again getting predictions and plotting:</source>
        </trans-unit><trans-unit id="346" translate="yes" xml:space="preserve">
          <source>We could continue the process, experimenting with functional forms for age.</source>
        </trans-unit><trans-unit id="347" translate="yes" xml:space="preserve">
          <source>But, since we have many observations (and therefore many degrees of freedom), we can take advantage of the F() function available in revoScaleR to let the data speak for itself.</source>
        </trans-unit><trans-unit id="348" translate="yes" xml:space="preserve">
          <source>The F() function creates a factor variable from a numeric variable “on-the-fly”, creating a level for every integer value.</source>
        </trans-unit><trans-unit id="349" translate="yes" xml:space="preserve">
          <source>This allows us to compute and observe the shape of the functional form using a purely dummy variable model:</source>
        </trans-unit><trans-unit id="350" translate="yes" xml:space="preserve">
          <source>This model estimated a total of 92 coefficients, all for dummy variables representing every age in the range of 20 to 65 for each sex.</source>
        </trans-unit><trans-unit id="351" translate="yes" xml:space="preserve">
          <source>To visually examine the coefficients we could add observations to our plotData data frame and use rxPredict to compute predicted values for each of the 92 groups represented, but since the model contains only dummy variables in an initial cube term, we can instead use the “counts” data frame returned with the rxLinMod object:</source>
        </trans-unit><trans-unit id="352" translate="yes" xml:space="preserve">
          <source>Intercept-Only Models</source>
        </trans-unit><trans-unit id="353" translate="yes" xml:space="preserve">
          <source>You may have seen intercept-only models fitted with R’s <bpt id="p1">*</bpt>lm<ept id="p1">*</ept> function, where the model formula is of the form response ~ 1.</source>
        </trans-unit><trans-unit id="354" translate="yes" xml:space="preserve">
          <source>In RevoScaleR these models should be fitted using <bpt id="p1">*</bpt>rxSummary<ept id="p1">*</ept>, because the intercept-only model simply returns the mean of the response.</source>
        </trans-unit><trans-unit id="355" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit></group></body></file></xliff>