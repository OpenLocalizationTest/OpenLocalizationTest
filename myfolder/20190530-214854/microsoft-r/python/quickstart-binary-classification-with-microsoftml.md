<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="quickstart-binary-classification-with-microsoftml.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e03bb07a8dd3669b8cecb9217e3b1f5e677b0bdbb.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">03bb07a8dd3669b8cecb9217e3b1f5e677b0bdbb</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python\quickstart-binary-classification-with-microsoftml.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Quickstart: Binary classification with microsoftml - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to deploy an R model as a service</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>quickstart, Machine Learning Server, deploy python models</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Quickstart: An example of binary classification with the microsoftml Python package</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Applies to: Machine Learning Server 9.x</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Learn how to use binary classification using the functions in the <bpt id="p1">[</bpt>microsoftml package<ept id="p1">](../python-reference/microsoftml/microsoftml-package.md)</ept> that ships with Machine Learning Server.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Data scientists work <bpt id="p1">[</bpt>locally in their preferred Python IDE<ept id="p1">](../install/python-libraries-interpreter.md)</ept> and favorite version control tools to build scripts and models.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This example uses the well known breast cancer dataset.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The dataset contains characteristics of cell nuclei and has a target label to indicate whether the tumor was benign (0) or malignant (1).</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The example builds a linear model with the <bpt id="p1">[</bpt>rx_fast_linear<ept id="p1">](../python-reference/microsoftml/rx-fast-linear.md)</ept> function from the <bpt id="p2">[</bpt>microsoftml package<ept id="p2">](../python-reference/microsoftml/microsoftml-package.md)</ept>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Time estimate</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>After you have completed the prerequisites, this task takes approximately <bpt id="p1">*</bpt>10<ept id="p1">*</ept> minutes to complete.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Before you begin this QuickStart, have the following ready:</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>An instance of <bpt id="p1">[</bpt>Machine Learning Server <ept id="p1">](../what-is-machine-learning-server.md)</ept> installed with the Python option.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Familiarity with Python.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Here's a video tutorial<ept id="p1">](https://mva.microsoft.com/en-us/training-courses/introduction-to-programming-with-python-8360?l=lqhuMxFz_8904984382)</ept>.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Familiarity with Jupyter notebooks.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Learn <bpt id="p1">[</bpt>how to load sample Python notebooks<ept id="p1">](how-to-revoscalepy-jupyter-nb-config.md)</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Example code</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The example for this quickstart is stored in a Jupyter notebook.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This notebook format allows you to not only see the code alongside detailed explanations, but also allows you to try out the code.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>This quickstart notebook walks you through how to:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Load the example data</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Import the microsoftml package</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Add transforms for featurization</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Train and evaluate the model</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Predict using the model on new data</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>You can try it yourself with the notebook.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>&amp;#9658; <bpt id="p1">[</bpt><bpt id="p2">**</bpt>Download the Jupyter notebook to try it out<ept id="p2">**</ept><ept id="p1">](https://github.com/Microsoft/ML-Server-Python-Samples/blob/master/microsoftml/quickstarts/binary-classification/Binary%2BClassification%2BQuickstart.ipynb)</ept>.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Now that you've tried this example, you can start developing your own solutions using the MicrosoftML packages and APIs for R and Python:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>MicrosoftML R package functions</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>microsoftml Python package functions</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>For more about Machine Learning Server in general, see <bpt id="p1">[</bpt>Overview of Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>For more machine learning samples using the microsoftml Python package, see <bpt id="p1">[</bpt>Python samples for MicrosoftML<ept id="p1">](samples-microsoftml-python.md)</ept>.</source>
        </trans-unit></group></body></file></xliff>