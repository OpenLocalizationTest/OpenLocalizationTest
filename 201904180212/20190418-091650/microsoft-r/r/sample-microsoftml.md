<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="sample-microsoftml.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b496ff63f0531efb9a978d02abddd3a8745c56012f.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">96ff63f0531efb9a978d02abddd3a8745c56012f</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\sample-microsoftml.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R samples for MicrosoftML</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve">
          <source>R samples for MicrosoftML</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>MicrosoftML samples that use the R language are described and linked here to help you get started quickly with Microsoft Machine Learning Server.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>The sentiment analysis and image featurization quickstarts both use pre-trained models.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Pre-trained models are installed through setup as an optional component of the <bpt id="p1">**</bpt>Machine Learning Server<ept id="p1">**</ept> or <bpt id="p2">**</bpt>SQL Server Machine Learning<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>To install them, you must check the <bpt id="p1">**</bpt>ML Models<ept id="p1">**</ept> checkbox on the <bpt id="p2">**</bpt>Configure the installation<ept id="p2">**</ept> page.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>For details, see <bpt id="p1">[</bpt>How to install and deploy pre-trained machine learning models with MicrosoftML<ept id="p1">](../install/microsoftml-install-pretrained-models.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Breast cancer prediction using rxFastLinear</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>This starter <bpt id="p1">[</bpt>breast cancer prediction sample<ept id="p1">](https://github.com/Microsoft/microsoft-r/tree/master/microsoft-ml/Samples/101/BinaryClassification/BreastCancerPrediction)</ept> builds a model to predict breast cancer.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>It uses the well-known Breast Cancer UCI dataset with <bpt id="p1">[</bpt><ph id="ph1">`rxFastLinear`</ph><ept id="p1">](../r-reference/microsoftml/rxfastlinear.md)</ept>algorithm provided by the MicrosoftML package.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The type of machine learning task exhibited in this sample is a binary classification problem.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Specifically, a given set of cell mass characteristics is used to predict whether the mass is benign or malignant.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Sentiment analysis using featurizeText</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>Sentiment analysis<ept id="p1">](https://github.com/Microsoft/microsoft-r/tree/master/microsoft-ml/Samples/101/BinaryClassification/SimpleSentimentAnalysis)</ept> sample is a text analytics sample that shows how to use the <bpt id="p2">[</bpt><ph id="ph1">`featurizeText`</ph><ept id="p2">](../r-reference/microsoftml/featurizetext.md)</ept> transform to featurize text data.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The featurized text data is then used to train a model to predict if a sentence expresses positive or negative sentiments.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The type of machine learning task exhibited in this sample is a supervised binary classification problem.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>More specifically, the example provided shows how to use the <bpt id="p1">[</bpt>featurizeText<ept id="p1">](../r-reference/microsoftml/featurizetext.md)</ept> transform in the MicrosoftML package to produce a bag of counts of n-grams (sequences of consecutive words) from the text for classification.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The sample uses the <bpt id="p1">[</bpt>Sentiment Labelled Sentences<ept id="p1">](https://archive.ics.uci.edu/ml/datasets/Sentiment+Labelled+Sentences)</ept> dataset from the UCI repository, which contains sentences that are labeled as positive or negative sentiment.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Image featurization using featurizeImage</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Image featurization is the process that takes an image as input and produces a numeric vector (aka feature vector) that represents key characteristics (features) of that image.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The features are extracted with an <bpt id="p1">[</bpt><ph id="ph1">`featurizeImage`</ph><ept id="p1">](../r-reference/microsoftml/featurizeimage.md)</ept> transform that runs the image data through one of several available pre-trained Deep Neural Net (DNN) models.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Two samples are provided in the <bpt id="p1">[</bpt>MicrosoftML GitHub repo<ept id="p1">](https://github.com/Microsoft/microsoft-r/tree/master/microsoft-ml/Samples/PreTrainedModels/ImageAnalytics/ImageFeaturizer)</ept> that show how to use these DNN models.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Sample 1: Find similar images<ept id="p1">**</ept>: Here is the scenario this sample addresses: You have a catalog of images in a repository.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>When you get a new image, you want to find the image from your catalog that most closely matches this new image.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Sample 2: Train a model to classify images<ept id="p1">**</ept>: Here is the scenario this sample addresses: train a model to classify or recognize the type of an image using labeled observations from a training set provided.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Specifically, this sample trains a multiclass linear model using the <bpt id="p1">[</bpt><ph id="ph1">`rxLogisticRegression`</ph><ept id="p1">](../r-reference/microsoftml/logisticregression.md)</ept> algorithm to distinguish between fish, helicopter and fighter jet images.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The multiclass training task uses the feature vectors of the images from the training set to learn how to classify these images.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>For some additional discussion on MicrosoftML support of pre-trained deep neural network models for image featurization, see <bpt id="p1">[</bpt>Image featurization with a pre-trained deep neural network model<ept id="p1">](https://blogs.msdn.microsoft.com/rserver/2017/04/12/image-featurization-with-a-pre-trained-deep-neural-network-model/)</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Retail churn tutorial</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>Retail churn tutorial<ept id="p1">](https://github.com/Microsoft/microsoft-r/tree/master/microsoft-ml/Microsoft%20ML%20Tutorial)</ept> guides you through the steps for fitting a model that predicts retail churn.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Customer churn is an expensive problem in retail.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>We focus on predicting which customers are likely to churn, but do not address how to prevent customers from churning.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The tutorial imports data from a retail database, creates a label identifying customers who have churned and features based on customer purchase history, fits a model using multiple learning algorithms, and then compares the performance of these fit models to select the best one.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Machine Learning Server's microsoft on HDInsight/Spark clusters</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>To create an HDInsight (Hadoop) cluster and connect it to R, see <bpt id="p1">[</bpt>Get started using R Server on HDInsight<ept id="p1">](https://docs.microsoft.com/en-us/azure/hdinsight/hdinsight-hadoop-r-server-get-started)</ept></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Microsoft Machine Learning Server 9.2.1 and 9.3 support the <bpt id="p1">[</bpt>sparklyr package from RStudio<ept id="p1">](https://cran.r-project.org/web/packages/sparklyr/index.html)</ept>.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Machine Learning Server and sparklyr can now be used in tandem within a single Spark session.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>For a walkthrough on how to use this package, see <bpt id="p1">[</bpt>Learn how to use Machine Learning Server with sparklyr<ept id="p1">](tutorial-sparklyr-revoscaler.md)</ept>.</source>
        </trans-unit></group></body></file></xliff>