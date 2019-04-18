<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-decision-forest.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4240641b6fa16d154f6c4fc2b3f32fc5a13454581.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">240641b6fa16d154f6c4fc2b3f32fc5a13454581</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-decision-forest.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>RevoScaleR User's Guide--Estimating Decision Forest Models (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Decision forests with RevoScaleR.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Estimating Decision Forest Models</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxDForest<ept id="p1">*</ept> function in RevoScaleR fits a <bpt id="p2">*</bpt>decision forest<ept id="p2">*</ept>, which is an ensemble of decision trees.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Each tree is fitted to a bootstrap sample of the original data, which leaves about 1/3 of the data unused in the fitting of each tree.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Each data point in the original data is fed through each of the trees for which it was unused; the decision forest prediction for that data point is the statistical <bpt id="p1">*</bpt>mode<ept id="p1">*</ept> of the individual tree predictions, that is, the majority prediction (for classification; for regression problems, the prediction is the mean of the individual predictions).</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Unlike individual decision trees, decision forests are not prone to overfitting, and they are consistently shown to be among the best machine learning algorithms.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>RevoScaleR implements decision forests in the <bpt id="p1">*</bpt>rxDForest<ept id="p1">*</ept> function, which uses the same basic tree-fitting algorithm as <bpt id="p2">*</bpt>rxDTree<ept id="p2">*</ept> (see <bpt id="p3">[</bpt>"The <bpt id="p4">*</bpt>rxDTree<ept id="p4">*</ept> Algorithm"<ept id="p3">](how-to-revoscaler-decision-tree.md#the-rxdtree-algorithm)</ept>).</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>To create the forest, you specify the number of trees using the <bpt id="p1">*</bpt>nTree<ept id="p1">*</ept> argument and the number of variables to consider for splitting in each tree using the <bpt id="p2">*</bpt>mTry<ept id="p2">*</ept> argument.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>In most cases, you specify the maximum depth to grow the individual trees: greater depth typically results in greater accuracy, but as with <bpt id="p1">*</bpt>rxDTree<ept id="p1">*</ept>, also results in longer fitting times.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>A Simple Classification Forest</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>Logistic Regression Models<ept id="p1">](how-to-revoscaler-logistic-regression.md)</ept>, we fit a simple classification tree model to rpart’s kyphosis data.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>That model is easily recast as a classification decision forest using <bpt id="p1">*</bpt>rxDForest<ept id="p1">*</ept> as follows (we set the <bpt id="p2">*</bpt>seed<ept id="p2">*</ept> argument to ensure reproducibility; in most cases you can omit):</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>While decision forests do not produce a unified model, as logistic regression and decision trees do, they do produce reasonable predictions for each data point.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>In this case, we can obtain predictions using <bpt id="p1">*</bpt>rxPredict<ept id="p1">*</ept> as follows:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Compared to the Kyphosis variable in the original kyphosis data, we see that approximately 88 percent of cases are classified correctly:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>A Simple Regression Forest</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>As a simple example of a regression forest, consider the classic <bpt id="p1">*</bpt>stackloss<ept id="p1">*</ept> data set, containing observations from a chemical plant producing nitric acid by the oxidation of ammonia, and let’s fit the stack loss (<bpt id="p2">*</bpt>stack.loss<ept id="p2">*</ept>) using air flow (<bpt id="p3">*</bpt>Air.Flow<ept id="p3">*</ept>), water temperature (<bpt id="p4">*</bpt>Water.Temp<ept id="p4">*</ept>), and acid concentration (<bpt id="p5">*</bpt>Acid.Conc.<ept id="p5">*</ept>) as predictors:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>A Larger Regression Forest Model</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>As a more complex example, we return to the censusWorkers data to which we earlier fit a decision tree.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>We create a regression forest predicting wage income from age, sex, and weeks worked, using the <bpt id="p1">*</bpt>perwt<ept id="p1">*</ept> variable as probability weights (note that we retain the <bpt id="p2">*</bpt>maxDepth<ept id="p2">*</ept> and <bpt id="p3">*</bpt>minBucket<ept id="p3">*</ept> parameters from our earlier decision tree example):</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Large Data Decision Forest Models</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>As with decision trees, scaling decision forests to very large data sets should be done with caution.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The wrong choice of model parameters can easily lead to models that take hours or longer to estimate, even in a distributed computing environment, or that simply cannot be fit at all.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>For non-binary classification problems, as with decision trees, categorical predictors should have a small to moderate number of levels.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>As an example of a large data classification forest, consider the following simple model using the 7% subsample of the full airline data (this uses the variable <bpt id="p1">*</bpt>ArrDel15<ept id="p1">*</ept> indicating flights with an arrival delay of 15 minutes or more):</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn more...<ept id="p1">](tutorial-revoscaler-data-import-transform.md#chunking)</ept></source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Yields the following:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>One problem with this model is that it predicts all flights to be on time.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>As we iterate over this model, we'll remove this limitation.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Looking at the fitted object’s forest component, we see that a number of the fitted trees do not split at all:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>This may well be because our response is extremely unbalanced--that is, the percentage of flights that are late by 15 minutes or more is quite small.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>We can tune the fit by providing a <bpt id="p1">*</bpt>loss matrix<ept id="p1">*</ept>, which allows us to penalize certain predictions in favor of others.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>You specify the loss matrix using the parms argument, which takes a list with named components.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The loss component is specified as either a matrix, or equivalently, a vector that can be coerced to a matrix.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>In the binary classification case, it can be useful to start with a loss matrix with a penalty roughly equivalent to the ratio of the two classes.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>So, in our case we know that the on-time flights outnumber the late flights approximately 4 to 1:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>This model no longer predicts all flights as on time, but now over-predicts late flights.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Adjusting the loss matrix again, this time reducing the penalty, yields the following output:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Controlling the Model Fit</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxDForest<ept id="p1">*</ept> function has a number of options for controlling the model fit.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Most of these control parameters are identical to the same controls in <bpt id="p1">*</bpt>rxDTree<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>A full listing of these options can be found in the <bpt id="p1">*</bpt>rxDForest<ept id="p1">*</ept> help file, but the following have been found in our testing to be the most useful at controlling the time required to fit a model with <bpt id="p2">*</bpt>rxDForest<ept id="p2">*</ept>:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>maxDepth<ept id="p1">*</ept>: sets the maximum depth of any node of the tree.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Computations grow rapidly more expensive as the depth increases, so we recommend a maxDepth of 10 to 15.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>maxNumBins<ept id="p1">*</ept>: controls the maximum number of bins used for each variable.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Managing the number of bins is important in controlling memory usage.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>The default is to use the larger of 101 and the square root of the number of observations for small to moderate size data sets (up to about one million observations), but for larger sets to use 1001 bins. For small data sets with continuous predictors, you may find that you need to increase the <bpt id="p1">*</bpt>maxNumBins<ept id="p1">*</ept> to obtain models that resemble those from rpart.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>minSplit<ept id="p1">*</ept>, <bpt id="p2">*</bpt>minBucket<ept id="p2">*</ept>: determine how many observations must be in a node before a split is attempted (<bpt id="p3">*</bpt>minSplit<ept id="p3">*</ept>) and how many must remain in a terminal node (<bpt id="p4">*</bpt>minBucket<ept id="p4">*</ept>).</source>
        </trans-unit></group></body></file></xliff>