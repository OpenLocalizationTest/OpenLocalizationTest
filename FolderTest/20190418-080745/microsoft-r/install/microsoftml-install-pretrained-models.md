<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="microsoftml-install-pretrained-models.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335eaf2333ae46998f6a275e732ad684fe4e476149d.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eaf2333ae46998f6a275e732ad684fe4e476149d</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">9c76acdc-560c-45e5-982b-fef069067335</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\microsoftml-install-pretrained-models.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Pre-trained machine learning models for sentiment analysis and image detection - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve">
          <source>Pre-trained machine learning models for sentiment analysis and image detection</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>For sentiment analysis of text and image classification, Machine Learning Server offers two approaches for training the models: you can train the models yourself using your data, or install pre-trained models that come with training data obtained and developed by Microsoft.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>The advantage of pre-trained models is that you can score and classify new content right away.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Sentiment analysis scores raw unstructured text in positive-negative terms, returning a score between 0 (negative) and 1 (positive), indicating relative sentiment.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Image detection identifies features of the image.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>There are several use cases for this model: image recognition, image classification.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>For image recognition, the model returns n-grams that possibly describe the image.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>For image classification, the model evaluates images and returns a classification based on possible classes you provided (for example, is the image a fish or a dog).</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Pre-trained models are available for both R and Python development, through the <bpt id="p1">[</bpt>MicrosoftML R package<ept id="p1">](../r-reference/microsoftml/microsoftml-package.md)</ept> and the <bpt id="p2">[</bpt>microsoftml Python package<ept id="p2">](../python-reference/microsoftml/microsoftml-package.md)</ept>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Benefits of using pre-trained models</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Pre-trained models have been made available to support customers who need to perform tasks such as sentiment analysis or image featurization, but do not have the resources to obtain the large datasets or train a complex model.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Using pre-trained models lets you get started on text and image processing most efficiently.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Currently the models that are available are deep neural network (DNN) models for sentiment analysis and image classification.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>All four pre-trained models were trained on CNTK.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The configuration of each network was based on the following reference implementations:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Resnet-18</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Resnet-50</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>ResNet-101</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>AlexNet</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>For more information about deep residual networks and their implementation using CNTK, go the <bpt id="p1">[</bpt>Microsoft Research<ept id="p1">](https://www.microsoft.com/research/)</ept> web site and search for these articles:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Microsoft Researchers’ Algorithm Sets ImageNet Challenge Milestone</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Microsoft Computational Network Toolkit offers most efficient distributed deep learning computational performance</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>How to install the models</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Pre-trained models are installed through setup as an optional component of Machine Learning Server or <bpt id="p1">[</bpt>SQL Server Machine Learning<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/r/install-pretrained-models-sql-server)</ept>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>You can also get the R version of the models through <bpt id="p1">[</bpt>Microsoft R Client<ept id="p1">](../r-client/what-is-microsoft-r-client.md)</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Run a Machine Learning Server setup program for your target platform: <bpt id="p1">[</bpt>Install Machine Learning Server<ept id="p1">](r-server-install.md)</ept>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>When specifying components to install, add at least one language (R Server or Python) and the pre-trained models.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Language support is required.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The models cannot be installed as a standalone component.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>After setup completes, verify the models are on your computer.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Pre-trained models are local, added to the MicrosoftML and microsftml library, respectively, when you run setup.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The files are \mxlibs<ph id="ph1">\&lt;</ph>modelname&gt;_updated.model for Python and \mxlibs\x64<ph id="ph2">\&lt;</ph>modelname&gt;_updated.model for R.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>For samples demonstrating use of the pre-trained models, see <bpt id="p1">[</bpt>R Samples for MicrosoftML<ept id="p1">](../r/sample-microsoftml.md)</ept> and <bpt id="p2">[</bpt>Python Samples for MicrosoftML<ept id="p2">](../python/samples-microsoftml-python.md)</ept>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Install the models by running the setup program or installation script for the target platform or product:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Machine Learning Server<ept id="p1">](r-server-install.md)</ept></source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install R Client on Windows<ept id="p1">](../r-client/install-on-windows.md)</ept></source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install R Client on Linux<ept id="p1">](../r-client/install-on-linux.md)</ept></source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Install Python client libraries<ept id="p1">](python-libraries-interpreter.md)</ept></source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Review the associated function reference help:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>featurize_image (microsoftml Python)<ept id="p1">](../python-reference/microsoftml/featurize-image.md)</ept></source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>featurize_text (microsoftml Python)<ept id="p1">](../python-reference/microsoftml/featurize-text.md)</ept></source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>featurizeImage (MicrosoftML R)<ept id="p1">](../r-reference/microsoftml/featurizeimage.md)</ept></source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>featurizeText (MicrosoftML R)<ept id="p1">](../r-reference/microsoftml/featurizetext.md)</ept></source>
        </trans-unit></group></body></file></xliff>