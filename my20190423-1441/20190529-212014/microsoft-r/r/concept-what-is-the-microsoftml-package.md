<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="concept-what-is-the-microsoftml-package.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b35ff52691035ca09dd80208fc94f3363e7ae51a0a.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5ff52691035ca09dd80208fc94f3363e7ae51a0a</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\concept-what-is-the-microsoftml-package.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Get started with MicrosoftML - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve">
          <source>What is MicrosoftML?</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>MicrosoftML adds state-of-the-art data transforms, machine learning algorithms, and pre-trained models to R and Python functionality.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>data transforms<ept id="p1">*</ept> provided by MicrosoftML allow you to compose a custom set of transforms in a pipeline that are applied to your data before training or testing.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The primary purpose of these transforms is to allow you to format your data.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>The MicrosoftML functions are provided through the <bpt id="p1">**</bpt>MicrosoftML<ept id="p1">**</ept> package installed with <bpt id="p2">[</bpt>Machine Learning Server<ept id="p2">](../what-is-machine-learning-server.md)</ept>, Microsoft R Client, and <bpt id="p3">[</bpt>SQL Server Machine Learning Services<ept id="p3">](https://docs.microsoft.com/sql/advanced-analytics/getting-started-with-machine-learning-services)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Functions provide fast and scalable <bpt id="p1">*</bpt>machine learning algorithms<ept id="p1">*</ept> that enable you to tackle common machine learning tasks such as classification, regression, and anomaly detection.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>These high-performance algorithms are multi-threaded, some of which execute off disk, so that they can scale up to 100s of GBs on a single-node.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>They are especially suitable for handling a large corpus of text data or high-dimensional categorical data.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>It enables you to run these functions locally on Windows or Linux machines or on Azure HDInsight (Hadoop/Spark) clusters.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Pre-trained models<ept id="p1">](../install/microsoftml-install-pretrained-models.md)</ept> for sentiment analysis and image featurization can also be installed and deployed with MicrosoftML.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>For more information on the pre-trained models and samples, see <bpt id="p1">[</bpt>R samples for MicrosoftML<ept id="p1">](sample-microsoftml.md)</ept> and <bpt id="p2">[</bpt>Python samples for MicrosoftML<ept id="p2">](../python/samples-microsoftml-python.md)</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Match algorithms to machine learning tasks</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Matching data transforms and machine learning algorithms to appropriate data science tasks is key to designing successful intelligent applications.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Machine learning tasks</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>MicrosoftML<ept id="p1">**</ept> package implements algorithms that can perform a variety of machine learning tasks:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>binary classification<ept id="p1">**</ept>: algorithms that learn to predict which of two classes an instance of data belongs to.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>These provide supervised learning in which the input of a classification algorithm is a set of labeled examples.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Each example is represented as a feature vector, and each label is an integer of value of 0 or 1.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The output of a binary classification algorithm is a classifier, which can be used to predict the label of new unlabeled instances.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>multi-class classification<ept id="p1">**</ept>: algorithms that learn to predict the category of an instance of data.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>These provide supervised learning in which the input of a classification algorithm is a set of labeled examples.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Each example is represented as a feature vector, and each label is an integer between 0 and k-1, where k is the number of classes.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The output of a classification algorithm is a classifier, which can be used to predict the label of a new unlabeled instance.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>regression<ept id="p1">**</ept>: algorithms that learn to predict the value of a dependent variable from a set of related independent variables.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Regression algorithms model this relationship to determine how the typical values of dependent variables change as the values of the independent variables are varied.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>These provide supervised learning in which the input of a regression algorithm is a set of examples with dependent variables of known values.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The output of a regression algorithm is a function, which can be used to predict the value of a new data instance whose dependent variables are not known.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>anomaly detection<ept id="p1">**</ept>: algorithms that identify outliers that do not belong to some target class or conform to an expected pattern.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>One-class anomaly detection is a type of unsupervised learning as the input data only contains data that is from the target class and does not contain instances of anomalies to learn from.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Machine learning algorithms</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The following table summarizes the MicrosoftML algorithms, the tasks they support, their scalability, and lists some example applications.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Algorithm (R/Python)</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>ML task supported</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Scalability</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Application Examples</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Fast Linear model</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>(SDCA)</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>binary classification, linear regression</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>#cols: ~1B;</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>#rows: ~1B;</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>CPU: multi-proc</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Mortgage default prediction, Email spam filtering</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>OneClass SVM</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>anomaly detection</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>cols: ~1K;</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>#rows: RAM-bound;</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>CPU: single-proc</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Credit card fraud detection</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Fast Tree</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>binary classification, regression</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>#cols: ~50K;</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>#rows: RAM-bound;</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>CPU: multi-proc</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Bankruptcy prediction</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Fast Forest</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>binary classification, regression</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>#cols: ~50K;</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>#rows: RAM-bound;</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>CPU: multi-proc</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Churn Prediction</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Neural Network</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>binary and multiclass classification, regression</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>#cols: ~10M;</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>#rows: Inf;</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>CPU: multi-proc CUDA GPU</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Check signature recognition, OCR, Click Prediction</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Logistic regression</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>binary and multiclass classification</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>#cols: ~100M;</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>#rows: Inf for single-proc CPU</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>#rows: RAM-bound for multi-proc CPU</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Classifying sentiments from feedback</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Data transforms</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>MicrosoftML<ept id="p1">**</ept> also provides transforms to help tailor your data for machine learning.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>They are used to clean, wrangle, train, and score your data.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>For a description of the transforms, see <bpt id="p1">[</bpt>Machine learning R transforms<ept id="p1">](~/r-reference/microsoftml/microsoftml-package.md#ml-transforms)</ept> and <bpt id="p2">[</bpt>Machine learning Python transforms<ept id="p2">](~/python-reference/microsoftml/microsoftml-package.md#ml-transforms)</ept> reference documentation.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>For reference documentation on the R individual transforms and functions in the product help, see <bpt id="p1">[</bpt>MicrosoftML: machine learning algorithms<ept id="p1">](../r-reference/microsoftml/microsoftml-package.md)</ept>.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>For reference documentation on the Python individual transforms and functions in the product help, see <bpt id="p1">[</bpt>MicrosoftML: machine learning algorithms<ept id="p1">](../python-reference/microsoftml/microsoftml-package.md)</ept>.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>For guidance when choosing the appropriate machine learning algorithm from the MicrosoftML package, see the <bpt id="p1">[</bpt>Cheat Sheet: How to choose a MicrosoftML algorithm<ept id="p1">](how-to-choose-microsoftml-algorithms-cheatsheet.md)</ept>.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Machine Learning Server</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>R samples for MicrosoftML</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Python samples for MicrosoftML</source>
        </trans-unit></group></body></file></xliff>