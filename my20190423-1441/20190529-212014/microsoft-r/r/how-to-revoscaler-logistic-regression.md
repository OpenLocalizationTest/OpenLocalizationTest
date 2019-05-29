<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-logistic-regression.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3d45e8e593133dbd4ccefaef7ea000b3206604f3b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d45e8e593133dbd4ccefaef7ea000b3206604f3b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-logistic-regression.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Fitting Logistic Regression Models (RevoScaleR) in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Logistic regression with RevoScaleR.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Fitting Logistic Regression Models using Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Logistic regression is a standard tool for modeling data with a binary response variable.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>In R, you fit a logistic regression using the <bpt id="p1">*</bpt>glm<ept id="p1">*</ept> function, specifying a binomial family and the logit link function.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>In RevoScaleR, you can use <bpt id="p1">*</bpt>rxGlm<ept id="p1">*</ept> in the same way (see <bpt id="p2">[</bpt>Fitting Generalized Linear Models<ept id="p2">](how-to-revoscaler-generalized-linear-model.md)</ept>) or you can fit a logistic regression using the optimized <bpt id="p3">*</bpt>rxLogit<ept id="p3">*</ept> function; because this function is specific to logistic regression, you need not specify a family or link function.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>A Simple Logistic Regression Example</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>As an example, consider the <bpt id="p1">*</bpt>kyphosis<ept id="p1">*</ept> data set in the <bpt id="p2">*</bpt>rpart<ept id="p2">*</ept> package.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>This data set consists of 81 observations of four variables (Age, Number, Kyphosis, Start) in children following corrective spinal surgery; it is used as the initial example of <bpt id="p1">*</bpt>glm<ept id="p1">*</ept> in the White Book (see <bpt id="p2">[</bpt>Additional Resources<ept id="p2">](../resources-more.md)</ept> for more information.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The variable Kyphosis reports the absence or presence of this deformity.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>We can use <bpt id="p1">*</bpt>rxLogit<ept id="p1">*</ept> to model the probability that kyphosis is present as follows:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The following output is returned:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The same model can be fit with <ph id="ph1">`glm`</ph> (or <ph id="ph2">`rxGlm`</ph>) as follows:</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Stepwise Logistic Regression</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Stepwise logistic regression is an algorithm that helps you determine which variables are most important to a logistic model.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>You provide a minimal, or lower, model formula and a maximal, or upper, model formula, and using forward selection, backward elimination, or bidirectional search, the algorithm determines the model formula that provides the best fit based on an AIC or significance level selection criterion.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>RevoScaleR provides an implementation of stepwise logistic regression that is not constrained by the use of "in-memory" algorithms.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Stepwise linear regression in RevoScaleR is implemented by the functions <bpt id="p1">*</bpt>rxLogit<ept id="p1">*</ept> and <bpt id="p2">*</bpt>rxStepControl<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Stepwise logistic regression begins with an initial model of some sort.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>We can look at the kyphosis data again and start with a simpler model: Kyphosis ~ Age:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>We can specify a stepwise model using rxLogit and rxStepControl as follows:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The methods for variable selection (forward, backward, and stepwise), the definition of model scope, and the available selection criteria are all the same as for stepwise linear regression; see <bpt id="p1">[</bpt>"Stepwise Variable Selection"<ept id="p1">](how-to-revoscaler-linear-model.md#stepwise-variable-selection)</ept> and the rxStepControl help file for more details.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Plotting Model Coefficients</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The ability to save model coefficients using the argument <bpt id="p1">*</bpt>keepStepCoefs = TRUE<ept id="p1">*</ept> within the <bpt id="p2">*</bpt>rxStepControl<ept id="p2">*</ept> call and to plot them with the function <bpt id="p3">*</bpt>rxStepPlot<ept id="p3">*</ept> was described in great detail for stepwise <bpt id="p4">*</bpt>rxLinMod<ept id="p4">*</ept> in <bpt id="p5">[</bpt>Fitting Linear Models using RevoScaleR<ept id="p5">](how-to-revoscaler-linear-model.md)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>This functionality is also available for stepwise <bpt id="p1">*</bpt>rxLogit<ept id="p1">*</ept> objects.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Prediction</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>As described above for linear models, the objects returned by the RevoScaleR model-fitting functions do not include fitted values or residuals.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>We can obtain them, however, by calling <bpt id="p1">*</bpt>rxPredict<ept id="p1">*</ept> on our fitted model object, supplying the original data used to fit the model as the data to be used for prediction.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>For example, consider the mortgage default example in <bpt id="p1">[</bpt>Tutorial: Analyzing loan data with RevoScaleR<ept id="p1">](tutorial-revoscaler-large-data-loan.md)</ept>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>In that example, we used ten input data files to create the data set used to fit the model.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>But suppose instead we use nine input data files to create the training data set and use the remaining data set for prediction.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>We can do that as follows (again, remember to modify the first line for your own system):</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>We can then fit a logistic regression model to the training data and predict with the prediction data set as follows:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>To view the first 30 rows of the output data file, use rxGetInfo as follows:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Prediction Standard Errors and Confidence Intervals</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>You can use rxPredict to obtain prediction standard errors and confidence intervals for models fit with rxLogit in the same way as for those fit with rxLinMod.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The original model must be fit with covCoef=TRUE:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>You then specify <ph id="ph1">`computeStdErr=TRUE`</ph> to obtain prediction standard errors; if this is TRUE, you can also specify <ph id="ph2">`interval="confidence"`</ph> to obtain a confidence interval:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The first ten lines of the file with predictions can be viewed as follows:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Using ROC Curves to Evaluate Estimated Binary Response Models</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">*</bpt>receiver operating characteristic<ept id="p1">*</ept> (ROC) curve can be used to visually assess binary response models.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>It plots the <bpt id="p1">*</bpt>True Positive Rate<ept id="p1">*</ept> (the number of correctly predicted TRUE responses divided by the actual number of TRUE responses) against the <bpt id="p2">*</bpt>False Positive Rate<ept id="p2">*</ept> (the number of incorrectly predicted TRUE responses divided by the actual number of FALSE responses), calculated at various thresholds.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>True Positive Rate<ept id="p1">*</ept> is the same as the <bpt id="p2">*</bpt>sensitivity<ept id="p2">*</ept>, and the <bpt id="p3">*</bpt>False Positive Rate<ept id="p3">*</ept> is equal to one minus the <bpt id="p4">*</bpt>specificity<ept id="p4">*</ept>.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Let’s start with a simple example.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Suppose we have a data set with 10 observations.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The variable <bpt id="p1">*</bpt>actual<ept id="p1">*</ept> contains the actual responses, or the ‘truth’.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>The variable <bpt id="p1">*</bpt>badPred<ept id="p1">*</ept> are the predicted responses from a very poor model.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The variable <bpt id="p1">*</bpt>goodPred<ept id="p1">*</ept> contains the predicted responses from a great model.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>We can now call the <bpt id="p1">*</bpt>rxRocCurve<ept id="p1">*</ept> function to compute the sensitivity and specificity for the ‘bad’ predictions, and draw the ROC curve.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The numBreaks argument indicates the number of breaks to use in determining the thresholds for computing the true and false positive rates.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Since all of our predictions are wrong at every threshold, the ROC curve is a flat line at 0.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>Area Under the Curve<ept id="p1">*</ept> (AUC) summary statistic is 0.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>At the other extreme, let’s draw an ROC curve for our great model:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>With perfect predictions, we see the True Positive Rate is 1 for all thresholds, and the AUC is 1.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>We’d expect a random guess ROC curve to lie along with white diagonal line.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Now let’s use actual model predictions in an ROC curve.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>We’ll use the small mortgage default sample data to estimate a logistic model and them compute predicted values:</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Now, let’s estimate a different model (with 1 less independent variable), and add the predictions from that model to our output data set:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Now we can compute the sensitivity and specificity for both models, using rxRoc:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>With the <bpt id="p1">*</bpt>removeDups<ept id="p1">*</ept> argument set to its default of <bpt id="p2">*</bpt>TRUE<ept id="p2">*</ept>, rows containing duplicate entries for sensitivity and specificity were removed from the returned data frame.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>In this case, it results in many fewer rows for Model2 than Model1.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>We can use the <bpt id="p1">*</bpt>rxRoc<ept id="p1">*</ept> <bpt id="p2">*</bpt>plot<ept id="p2">*</ept> method to render our ROC curve using the computed results.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The resulting plot shows that the second model is much closer to the “random” diagonal line than the first model.</source>
        </trans-unit></group></body></file></xliff>