<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-boosting.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926c13d52521a588c1d9d713953e48b25c7d1bff87e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">c13d52521a588c1d9d713953e48b25c7d1bff87e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-boosting.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Estimate Models using Stochastic Gradient Boosting (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Boosted trees with RevoScaleR in Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Estimate Models Using Stochastic Gradient Boosting</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxBTrees<ept id="p1">*</ept> function in RevoScaleR, like <bpt id="p2">*</bpt>rxDForest<ept id="p2">*</ept>, fits a decision forest to your data, but the forest is generated using a stochastic gradient boosting algorithm.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>This is similar to the decision forest algorithm in that each tree is fitted to a subsample of the training set (sampling without replacement) and predictions are made by aggregating over the predictions of all trees.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Unlike the <bpt id="p1">*</bpt>rxDForest<ept id="p1">*</ept> algorithm, the boosted trees are added one at a time, and at each iteration, a regression tree is fitted to the current pseudo-residuals, that is, the gradient of the loss functional being minimized.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Like the <bpt id="p1">*</bpt>rxDForest<ept id="p1">*</ept> function, <bpt id="p2">*</bpt>rxBTrees<ept id="p2">*</ept> uses the same basic tree-fitting algorithm as <bpt id="p3">*</bpt>rxDTree<ept id="p3">*</ept> (see <bpt id="p4">[</bpt>"The <bpt id="p5">*</bpt>rxDTree<ept id="p5">*</ept> Algorithm"<ept id="p4">](how-to-revoscaler-decision-tree.md#the-rxdtree-algorithm)</ept>).</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>To create the forest, you specify the number of trees using the <bpt id="p1">*</bpt>nTree<ept id="p1">*</ept> argument and the number of variables to consider for splitting at each tree node using the <bpt id="p2">*</bpt>mTry<ept id="p2">*</ept> argument.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>In most cases, you specify the maximum depth to grow the individual trees: shallow trees seem to be sufficient in many applications, but as with <bpt id="p1">*</bpt>rxDTree<ept id="p1">*</ept> and <bpt id="p2">*</bpt>rxDForest<ept id="p2">*</ept>, greater depth typically results in longer fitting times.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Different model types are supported by specifying different loss functions, as follows:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>"gaussian"<ept id="p1">*</ept>, for regression models</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>"bernoulli"<ept id="p1">*</ept>, for binary classification models</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>"multinomial"<ept id="p1">*</ept>, for multi-class classification models</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A Simple Binary Classification Forest</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>Logistic Regression<ept id="p1">](how-to-revoscaler-logistic-regression.md)</ept>, we fit a simple classification tree model to rpart’s kyphosis data.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>That model is easily recast as a classification decision forest using <bpt id="p1">*</bpt>rxBTrees<ept id="p1">*</ept> as follows.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>We set the <bpt id="p1">*</bpt>seed<ept id="p1">*</ept> argument to ensure reproducibility; in most cases you can omit it:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>In this case, we don’t need to explicitly specify the loss function; <bpt id="p1">*</bpt>"bernoulli"<ept id="p1">*</ept> is the default.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>A Simple Regression Forest</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>As a simple example of a regression forest, consider the classic <bpt id="p1">*</bpt>stackloss<ept id="p1">*</ept> data set, containing observations from a chemical plant producing nitric acid by the oxidation of ammonia, and let’s fit the stack loss (<bpt id="p2">*</bpt>stack.loss<ept id="p2">*</ept>) using air flow (<bpt id="p3">*</bpt>Air.Flow<ept id="p3">*</ept>), water temperature (<bpt id="p4">*</bpt>Water.Temp<ept id="p4">*</ept>), and acid concentration (<bpt id="p5">*</bpt>Acid.Conc.<ept id="p5">*</ept>) as predictors:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>A Simple Multinomial Forest Model</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>As a simple multinomial example, we fit an <bpt id="p1">*</bpt>rxBTrees<ept id="p1">*</ept> model to the iris data:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Controlling the Model Fit</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The principal parameter controlling the boosting algorithm itself is the <bpt id="p1">*</bpt>learning rate<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The learning rate (or shrinkage) is used to scale the contribution of each tree when it is added to the ensemble.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The default learning rate is 0.1.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxBTrees<ept id="p1">*</ept> function has a number of other options for controlling the model fit.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Most of these control parameters are identical to the same controls in <bpt id="p1">*</bpt>rxDTree<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>A full listing of these options can be found in the <bpt id="p1">*</bpt>rxBTrees<ept id="p1">*</ept> help file, but the following have been found in our testing to be the most useful at controlling the time required to fit a model with <bpt id="p2">*</bpt>rxBTrees<ept id="p2">*</ept>:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>maxDepth<ept id="p1">*</ept>: sets the maximum depth of any node of the tree.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Computations grow more expensive as the depth increases, so we recommend starting with maxDepth=1, that is, boosted stumps.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>maxNumBins<ept id="p1">*</ept>: controls the maximum number of bins used for each variable.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Managing the number of bins is important in controlling memory usage.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The default is to use the larger of 101 and the square root of the number of observations for small to moderate size data sets (up to about one million observations), but for larger sets to use 1001 bins. For small data sets with continuous predictors, you may find that you need to increase the <bpt id="p1">*</bpt>maxNumBins<ept id="p1">*</ept> to obtain models that resemble rpart.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>minSplit<ept id="p1">*</ept>, <bpt id="p2">*</bpt>minBucket<ept id="p2">*</ept>: determine how many observations must be in a node before a split is attempted (<bpt id="p3">*</bpt>minSplit<ept id="p3">*</ept>) and how many must remain in a terminal node (<bpt id="p4">*</bpt>minBucket<ept id="p4">*</ept>).</source>
        </trans-unit></group></body></file></xliff>