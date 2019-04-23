<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-naive-bayes.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a384bf0623c709c97099001770ecec3ea12d26725.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">384bf0623c709c97099001770ecec3ea12d26725</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-naive-bayes.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Naive Bayes Classifier using RevoScaleR on Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Naive Bayes Classifier in RevoScaleR.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Naïve Bayes Classifier using RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>In this article, we describe one simple and effective family of classification methods known as Naïve Bayes.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>In RevoScaleR, Naïve Bayes classifiers can be implemented using the <bpt id="p1">*</bpt>rxNaiveBayes<ept id="p1">*</ept> function.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Classification, simply put, is the act of dividing observations into classes or categories.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Some examples of this are the classification of product reviews into positive or negative categories or the detection of email spam.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>These classification examples can be achieved manually using a set of rules.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>However, this is not efficient or scalable.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>In Naïve Bayes and other machine learning based classification algorithms, the decision criteria for assigning class are learned from a training data set, which has classes assigned manually to each observation.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The rxNaiveBayes Algorithm</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The Naïves Bayes classification method is simple, effective, and robust.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>This method can be applied to data large or small, it requires minimal training data, and is unlikely to produce a classifier that performs poorly compared to more complex algorithms.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This family of classifiers utilizes Bayes Theorem to determine the probability that an observation belongs to a certain class.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>A training dataset is used to calculate prior probabilities of an observation occurring in a class within the predefined set of classes.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>In RevoScaleR this is done using the <bpt id="p1">*</bpt>rxNaiveBayes<ept id="p1">*</ept> function.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>These probabilities are then used to calculate posterior probabilities that an observation belongs to each class.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The class membership is decided by choosing the class with the largest posterior probability for each observation.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>This is accomplished with the <bpt id="p1">*</bpt>rxPredict<ept id="p1">*</ept> function using the Naïve Bayes object from a call to <bpt id="p2">*</bpt>rxNaiveBayes<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Part of the beauty of Naïve Bayes is its simplicity due to the conditional independent assumption: that the values of each predictor are independent of each other given the class.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>This assumption reduces the number of parameters needed and in turn makes the algorithm extremely efficient.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Naïve Bayes methods differ in their choice of distribution for any continuous independent variables.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Our implementation via the <bpt id="p1">*</bpt>rxNaiveBayes<ept id="p1">*</ept> function assumes the distribution to be Gaussian.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>A Simple Naïve Bayes Classifier</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">[</bpt>Logistic Regression Models<ept id="p1">](how-to-revoscaler-logistic-regression.md)</ept>, we fit a simple logistic regression model to rpart’s kyphosis data and in <bpt id="p2">[</bpt>Decision Trees<ept id="p2">](how-to-revoscaler-decision-tree.md)</ept> and <bpt id="p3">[</bpt>Decision Forests<ept id="p3">](how-to-revoscaler-decision-forest.md)</ept> we used the kyphosis data again to create classification and regression trees.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>We can use the same data with our Naïve Bayes classifier to see which patients are more likely to acquire Kyphosis based on age, number, and start.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>We can train and test our classifier on the kyphosis data for the sake of illustration.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>We use the <bpt id="p1">*</bpt>rxNaiveBayes<ept id="p1">*</ept> function to construct a classifier for the kyphosis data:</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The returned object <bpt id="p1">*</bpt>kyphNaiveBayes<ept id="p1">*</ept> is an object of class <bpt id="p2">*</bpt>rxNaiveBayes<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Objects of this class provide the following useful components: <bpt id="p1">*</bpt>apriori<ept id="p1">*</ept> and <bpt id="p2">*</bpt>tables<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>apriori<ept id="p1">*</ept> component contains the conditional probabilities for the response variable, in this case the Kyphosis variable.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>tables<ept id="p1">*</ept> component contains a list of tables, one for each predictor variable.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>For a categorical variable, the table contains the conditional probabilities of the variable given the target level of the response variable.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>For a numeric variable, the table contains the mean and standard deviation of the variable given the target level of the response variable.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>These components are printed in the output above.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>We can use our Naïve Bayes object with <bpt id="p1">*</bpt>rxPredict<ept id="p1">*</ept> to re-classify the Kyphosis variable for each child in our original dataset:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>When we table the results from the Naïve Bayes classifier with the original Kyphosis variable, it appears that 13 of 81 children are misclassified:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>A Larger Naïve Bayes Classifier</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>As a more complex example, consider the mortgage default example.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>For that example, there are ten input files total and we use nine input data files to create the training data set.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>We then use the model built from those files to make predictions on the final dataset.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>In this section we will use the same strategy to build a Naïve Bayes classifier on the first nine data sets and assign the outcome variable for the tenth data set.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The mortgage default data sets are available for download <bpt id="p1">[</bpt>online<ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698896&amp;clcid=0x409)</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>With the data downloaded we can create the training data set and test data set as follows (remember to modify the first line to match the location of the mortgage default text data files on your own system):</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>In the above code the response variable <bpt id="p1">*</bpt>default<ept id="p1">*</ept> is converted to a factor using the <bpt id="p2">*</bpt>colInfo<ept id="p2">*</ept> argument to <bpt id="p3">*</bpt>rxImport<ept id="p3">*</ept>.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>For the <bpt id="p1">*</bpt>rxNaiveBayes<ept id="p1">*</ept> function, the response variable must be a factor or you will get an error.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Now that we have training and test data sets we can fit a Naïve Bayes classifier with our training data using <bpt id="p1">*</bpt>rxNaiveBayes<ept id="p1">*</ept> and assign values of the <bpt id="p2">*</bpt>default<ept id="p2">*</ept> variable for observations within the test data using <bpt id="p3">*</bpt>rxPredict<ept id="p3">*</ept>:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Notice that we added an additional argument, <bpt id="p1">*</bpt>smoothingFactor<ept id="p1">*</ept>, to our rxNaiveBayes call.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>This is a useful argument when your data are missing levels of a certain variable that you expect to be in your test data.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Based on our training data, the conditional probability for year 2009 will be 0, since it only includes data between the years of 2000 and 2008.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>If we try to use our classifier on the test data without specifying a smoothing factor in our call to <bpt id="p1">*</bpt>rxNaiveBayes<ept id="p1">*</ept> the function <bpt id="p2">*</bpt>rxPredict<ept id="p2">*</ept> produces no results since our test data only has data from 2009.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>In general, smoothing is used to avoid overfitting your model.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>It follows that to achieve the optimal classifier you may want to smooth the conditional probabilities even if every level of each variable is observed.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>We can compare the predicted values of the <bpt id="p1">*</bpt>default<ept id="p1">*</ept> variable from the Naïve Bayes classifier with the actual data in the test dataset:</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>These results demonstrate a 10.2% misclassification rate using our Naïve Bayes classifier.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Naïve Bayes with Missing Data</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>You can control the handling of missing data using the <bpt id="p1">*</bpt>byTerm<ept id="p1">*</ept> argument in the <bpt id="p2">*</bpt>rxNaiveBayes<ept id="p2">*</ept> function.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>By default, <bpt id="p1">*</bpt>byTerm<ept id="p1">*</ept> is set to <bpt id="p2">*</bpt>TRUE<ept id="p2">*</ept>, which means that missings are removed by variable before computing the conditional probabilities.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>If you prefer to remove observations with missings in any variable before computations are done, set the <bpt id="p1">*</bpt>byTerm<ept id="p1">*</ept> argument to <bpt id="p2">*</bpt>FALSE<ept id="p2">*</ept>.</source>
        </trans-unit></group></body></file></xliff>