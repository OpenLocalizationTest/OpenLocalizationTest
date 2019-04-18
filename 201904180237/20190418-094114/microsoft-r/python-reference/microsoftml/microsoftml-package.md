<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="microsoftml-package.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926226b7a879b7d4479e87acc678e8b37850ead71d5.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">226b7a879b7d4479e87acc678e8b37850ead71d5</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python-reference\microsoftml\microsoftml-package.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>microsoftml package for Python (Microsoft Machine Learning Server and SQL Server Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Function help reference for the microsoftml python package of SQL Server Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>microsoftml API, API</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>microsoftml package</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>microsoftml<ept id="p1">**</ept> module is a collection of Python functions used in machine learning solutions.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>It includes functions for training and transformations, scoring, text and image analysis, and feature extraction for deriving values from existing data.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Package details</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Current version:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>9.3</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Built on:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Anaconda 4.2<ept id="p1">](https://www.continuum.io/why-anaconda)</ept> distribution of <bpt id="p2">[</bpt>Python 3.5<ept id="p2">](https://www.python.org/doc)</ept></source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Package distribution:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server 9.x<ept id="p1">](../../what-is-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SQL Server 2017 Machine Learning Services<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/python/sql-server-python-services)</ept></source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SQL Server 2017 Machine Learning Server (Standalone)<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/r/r-server-standalone)</ept></source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>How to use microsoftml</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>microsoftml<ept id="p1">**</ept> module is installed as part of Microsoft Machine Learning Server or SQL Server Machine Learning when you add Python to your installation.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>You get the full collection of proprietary packages plus a Python distribution with its modules and interpreters.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>You can use any Python IDE to write Python script calling functions in <bpt id="p1">**</bpt>microsoftml<ept id="p1">**</ept>, but the script must run on a computer having either Microsoft Machine Learning Server or SQL Server Machine Learning Server with Python.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Microsoftml<ept id="p1">**</ept> and <bpt id="p2">**</bpt>revoscalepy<ept id="p2">**</ept> are tightly coupled; data sources used in <bpt id="p3">**</bpt>microsoftml<ept id="p3">**</ept> are defined as <bpt id="p4">[</bpt><bpt id="p5">**</bpt>revoscalepy<ept id="p5">**</ept><ept id="p4">](../revoscalepy/revoscalepy-package.md)</ept> objects.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Compute context limitations in <bpt id="p1">**</bpt>revoscalepy<ept id="p1">**</ept> transfer to <bpt id="p2">**</bpt>microsoftml<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Namely, all functionality is available for local operations, but switching to a remote compute context requires <bpt id="p1">[</bpt>RxSpark<ept id="p1">](../revoscalepy/RxSpark.md)</ept> or <bpt id="p2">[</bpt>RxInSQLServer<ept id="p2">](../revoscalepy/RxInSQLServer.md)</ept>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Functions by category</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>This section lists the functions by category to give you an idea of how each one is used.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>You can also use the table of contents to find functions in alphabetical order.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>1-Training functions</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.rx_ensemble<ept id="p1">](rx-ensemble.md)</ept></source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Train an ensemble of models</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.rx_fast_forest<ept id="p1">](rx-fast-forest.md)</ept></source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Random Forest</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.rx_fast_linear<ept id="p1">](rx-fast-linear.md)</ept></source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Linear Model with Stochastic Dual Coordinate Ascent</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.rx_fast_trees<ept id="p1">](rx-fast-trees.md)</ept></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Boosted Trees</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.rx_logistic_regression<ept id="p1">](rx-logistic-regression.md)</ept></source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Logistic Regression</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.rx_neural_network<ept id="p1">](rx-neural-network.md)</ept></source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Neural Network</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.rx_oneclass_svm<ept id="p1">](rx-oneclass-svm.md)</ept></source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Anomaly Detection</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>2-Transform functions</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Categorical variable handling</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.categorical<ept id="p1">](categorical.md)</ept></source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Converts a text column into categories</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.categorical_hash<ept id="p1">](categorical-hash.md)</ept></source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Hashes and converts a text column into categories</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Schema manipulation</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.concat<ept id="p1">](concat.md)</ept></source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Concatenates multiple columns into a single vector</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.drop_columns<ept id="p1">](drop-columns.md)</ept></source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Drops columns from a dataset</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.select_columns<ept id="p1">](select-columns.md)</ept></source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Retains columns of a dataset</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Variable selection</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.count_select<ept id="p1">](count-select.md)</ept></source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Feature selection based on counts</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.mutualinformation_select<ept id="p1">](mutualinformation-select.md)</ept></source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Feature selection based on mutual information</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Text analytics</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.featurize_text<ept id="p1">](featurize-text.md)</ept></source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Converts text columns into numerical features</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.get_sentiment<ept id="p1">](get-sentiment.md)</ept></source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Sentiment analysis</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Image analytics</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.load_image<ept id="p1">](load-image.md)</ept></source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Loads an image</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.resize_image<ept id="p1">](resize-image.md)</ept></source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Resizes an Image</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.extract_pixels<ept id="p1">](extract-pixels.md)</ept></source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Extracts pixels from an image</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.featurize_image<ept id="p1">](featurize-image.md)</ept></source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Converts an image into features</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Scoring functions</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.rx_predict<ept id="p1">](rx-predict.md)</ept></source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Scores using a Microsoft machine learning model</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>Featurization functions</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Function</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml.rx_featurize<ept id="p1">](rx-featurize.md)</ept></source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Data transformation for data sources</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>For SQL Server, add both Python modules to your computer by running setup:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Set up Python Machine Learning Services<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/python/setup-python-machine-learning-services)</ept>.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Follow this SQL Server tutorial for hands-on experience:</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Using the MicrosoftML Package with SQL Server<ept id="p1">](https://docs.microsoft.com/en-us/sql/advanced-analytics/using-the-microsoftml-package)</ept></source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server<ept id="p1">](../../what-is-machine-learning-server.md)</ept></source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SQL Server Machine Learning Services with Python<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/python/sql-server-python-services)</ept></source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SQL Server Machine Learning Server (Standalone)<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/r/r-server-standalone)</ept></source>
        </trans-unit></group></body></file></xliff>