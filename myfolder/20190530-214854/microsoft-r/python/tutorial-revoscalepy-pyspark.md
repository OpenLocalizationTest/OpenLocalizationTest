<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="tutorial-revoscalepy-pyspark.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e6e68265e0db1b64294e58c9034f00eaa7baf4a81.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">6e68265e0db1b64294e58c9034f00eaa7baf4a81</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">eba123f9-b3cc-43c5-aa3c-78bd865c7f3e</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/30/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python\tutorial-revoscalepy-pyspark.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Tutorial: PySpark and revoscalepy interoperabilty in Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn how to use PySpark and revoscalepy Python functions in Spark applications in Hadoop clusters having Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Tutorial: PySpark and revoscalepy interoperability in Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies to: Microsoft Learning Server 9.x</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>PySpark<ept id="p1">](https://spark.apache.org/downloads.html)</ept> is Apache Spark's programmable interface for Python.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../python-reference/revoscalepy/revoscalepy-package.md)</ept> module is Machine Learning Server's Python library for predictive analytics at scale.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>In this tutorial, you learn how to create a logistic regression model using functions from both libraries.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Import packages</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Connect to Spark using <ph id="ph1">`revoscalepy.rx_spark_connect()`</ph>, specifying PySpark interop</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Use PySpark for basic data manipulation</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Use revoscalepy to build a logistic regression model</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../python-reference/revoscalepy/revoscalepy-package.md)</ept> module provides functions for data sources and data manipulation.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>We are using PySpark in this tutorial to illustrate a basic technique for passing data objects between the two programming contexts.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>A Hadoop cluster with Spark 2.0-2.1 with <bpt id="p1">[</bpt>Machine Learning Server for Hadoop<ept id="p1">](../install/machine-learning-server-hadoop-install.md)</ept></source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>A Python IDE, such as Jupyter Notebooks, <bpt id="p1">[</bpt>Visual Studio for Python<ept id="p1">](https://www.visualstudio.com/vs/python/)</ept>, or PyCharm.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Sample data (AirlineSubsetCsv mentioned in the example) downloaded from our <bpt id="p1">[</bpt>sample data web site<ept id="p1">](https://packages.revolutionanalytics.com/datasets/)</ept> to your Spark cluster.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Jupyter Notebook users, update your notebook to include the MMLSPy kernel.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Select this kernel in your Jupyter notebook to use the interoperability feature.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Import the relevant packages</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The following commands import the required libraries into the current session.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Connect to Spark</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Setting <ph id="ph1">`interop = ‘pyspark’`</ph> indicates that you want interoperability.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Data acquisition and manipulation</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The sample data used in this tutorial is airline arrival and departure data, which you can store in a local file path.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Create the model</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>A logistic regression model requires a symbolic formula, specifying the dependent and independent variables, and a data set.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>You can output the results using the print function.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>This tutorial provides an introduction to a basic workflow using PySpark for data preparation and revoscalepy functions for logistic regression.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>For further exploration, review our <bpt id="p1">[</bpt>Python samples<ept id="p1">](python-samples.md)</ept>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>microsoftml function reference</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>revoscalepy function reference</source>
        </trans-unit></group></body></file></xliff>