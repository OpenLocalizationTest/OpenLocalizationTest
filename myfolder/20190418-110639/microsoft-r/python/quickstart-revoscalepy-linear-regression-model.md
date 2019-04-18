<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="quickstart-revoscalepy-linear-regression-model.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907fc02f79a2afc6a241e0e543788e990911ce2221af.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">c02f79a2afc6a241e0e543788e990911ce2221af</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python\quickstart-revoscalepy-linear-regression-model.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Python tutorial: Linear regression model using revoscalepy on Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Learn how to build and deploy a model using revoscalepy Python functions.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Predict outcomes.</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Summarize  data.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Quickstart: Create a linear regression model using revoscalepy in Python</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: Machine Learning Server 9.x<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>This Python quickstart demonstrates a linear regression model on a local Machine Learning Server, using functions from the <bpt id="p1">[</bpt>revoscalepy library<ept id="p1">](../python-reference/revoscalepy/revoscalepy-package.md)</ept> and built-in sample data.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Steps are executed on a Python command line using Machine Learning Server in the default local compute context.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>In this context, all operations run locally: data is fetched from the data source, and the model-fitting runs in your current Python environment.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The revoscalepy library for Python contains objects, transformations, and algorithms similar to what's included in the <bpt id="p1">[</bpt>RevoScaleR package<ept id="p1">](../r-reference/revoscaler/revoscaler.md)</ept> for the R language.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>With revoscalepy, you can write a Python script that creates a compute context, moves data between compute contexts, transforms data, and trains predictive models using popular algorithms such as logistic and linear regression, decision trees, and more.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>For the SQL Server version of this tutorial, see <bpt id="p1">[</bpt>Use Python with revoscalepy to create a model (SQL Server)<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/tutorials/use-python-revoscalepy-to-create-model)</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Start Python</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>On Windows, go to C:\Program Files\Microsoft\ML Server\PYTHON_SERVER, and double-click <bpt id="p1">**</bpt>Python.exe<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>On Linux, enter <bpt id="p1">**</bpt>mlserver-python<ept id="p1">**</ept> at the command line.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Import libraries and functions</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Paste in the following statements to import libraries and functions.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Create a data source object</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The data is retrieved locally from a sample .xdf file included in your installation.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>In this step, set the file path and then create a data source object to load the data.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The sample data provides airline delays over a given time period, for multiple airlines.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Create a linear regression model</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>In a linear regression, you model the relationship between dependent and independent variables.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>In this step, the duration of a delay is captured for each day of the week.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Predict delays</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Using a prediction function, you can predict the likelihood of a delay for each day.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Summarize data</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>In this last step, extract summary statistics from the computed prediction to understand the range and shape of prediction.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Print the output to the console.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The rx_summary function returns mean, standard deviation, and min-max values.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Results<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The ability to switch compute context to a different machine or platform is a powerful capability.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>To see how this works, continue with the SQL Server version of this tutorial: <bpt id="p1">[</bpt>Use Python with revoscalepy to create a model (SQL Server)<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/tutorials/use-python-revoscalepy-to-create-model)</ept>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>You can also review <bpt id="p1">[</bpt>linear modeling for RevoScaleR<ept id="p1">](../r/how-to-revoscaler-linear-model.md)</ept>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>For linear models, the Python implementation in revoscalepy is similar to the R implementation in RevoScaleR.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to use revoscalepy in local and remote compute contexts<ept id="p1">](how-to-revoscalepy.md)</ept></source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Python Function Reference<ept id="p1">](../python-reference/introducing-python-package-reference.md)</ept></source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml function reference<ept id="p1">](../python-reference/microsoftml/microsoftml-package.md)</ept></source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>revoscalepy function reference<ept id="p1">](../python-reference/revoscalepy/revoscalepy-package.md)</ept></source>
        </trans-unit></group></body></file></xliff>