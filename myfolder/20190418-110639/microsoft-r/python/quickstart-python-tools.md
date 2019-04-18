<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="quickstart-python-tools.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f8c8ac078f8563ec0f12c2e5613b9073e9ca94283.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8c8ac078f8563ec0f12c2e5613b9073e9ca94283</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\python\quickstart-python-tools.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Link to Machine Learning Server from Python tools</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Link Python tools like PyCharm, Jupyter notebooks, and Visual Studio to Machine Learning Server Python executable and libraries</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Machine Learning Server, python tools</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Link Python tools and IDEs to the Python interpreter installed with Machine Learning Server</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: Machine Learning Server 9.x<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Machine Learning Server installs a local, folder-only install of Anaconda to avoid interfering with other Python distributions on your system.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>As such, packages providing the Python modules in Machine Learning Server (revoscalepy, microsoftml, azureml-model-management-sdk) are not available system-wide.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>In this article, learn how to load the Python interpreter installed with Machine Learning Server in your Python IDE of choice.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Before you begin, have the following ready:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>An instance of <bpt id="p1">[</bpt>Machine Learning Server <ept id="p1">](../what-is-machine-learning-server.md)</ept> installed with the Python option.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>A Python IDE, such as <bpt id="p1">[</bpt>Visual Studio 2017 Community Edition<ept id="p1">](https://www.visualstudio.com/downloads/)</ept> with Python.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Need help learning Python?</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Here's a video tutorial<ept id="p1">](https://mva.microsoft.com/en-us/training-courses/introduction-to-programming-with-python-8360?l=lqhuMxFz_8904984382)</ept>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Python.exe (built-in)</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>To use the Python modules interactively, start the Python executable from the installation path.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>On Windows, go to \Program Files\Microsoft\ML Server\PYTHON_SERVER and run Python.exe to open an interactive command-line window.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>As a validation step, load the revoscalepy module and run the example code for <bpt id="p1">[</bpt>rx_summary<ept id="p1">](../python-reference/revoscalepy/rx-summary.md#example)</ept> to print out summary statistics using an embedded sample data set:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Visual Studio 2017 with Python</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The setup program for Machine Learning Server 9.3 adds Python distribution information to the registry, which makes loading Python modules more straightforward than in previous releases.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>However, when using an earlier release or to confirm settings, follow these steps to add Machine Learning Server's Python distribution information to an environment.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Python environments (Visual Studio docs)<ept id="p1">](https://docs.microsoft.com/visualstudio/python/managing-python-environments-in-visual-studio)</ept>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">**</bpt>Tools<ept id="p1">**</ept><ph id="ph1"> &gt; </ph><bpt id="p2">**</bpt>Python<ept id="p2">**</ept><ph id="ph2"> &gt; </ph><bpt id="p3">**</bpt>Python environments<ept id="p3">**</ept>, click <bpt id="p4">**</bpt>+ Custom<ept id="p4">**</ept> to create a new environment.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">**</bpt>Description<ept id="p1">**</ept>, give the environment name, and then fill in the following fields.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">**</bpt>Prefix path<ept id="p1">**</ept>, enter <ph id="ph1">`C:\Program Files\Microsoft\ML Server\PYTHON_SERVER`</ph>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Auto Detect<ept id="p1">**</ept> in the top right to auto-fill the remaining fields:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Interpreter path<ept id="p1">**</ept> should be <ph id="ph1">`C:\Program Files\Microsoft\ML Server\PYTHON_SERVER\python.exe`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Windowed interpreter<ept id="p1">**</ept> should be <ph id="ph1">`C:\Program Files\Microsoft\ML Server\PYTHON_SERVER\pythonw.exe`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Language version<ept id="p1">**</ept> should be <ph id="ph1">`3.5`</ph> for Python 3.5.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Path<ept id="p1">**</ept> should be read-only.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Apply<ept id="p1">**</ept> in the top right to save the environment.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>You can use the environment you just created by selecting it in an interactive window.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>As a verification step, run the example from the <bpt id="p1">[</bpt>rx_summary function<ept id="p1">](../python-reference/revoscalepy/rx-summary.md#example)</ept> in revoscalepy.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Visual Studio interactive Python window</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For new projects, you can also add an environment to your project in <bpt id="p1">**</bpt>Solution Explorer<ept id="p1">**</ept><ph id="ph1"> &gt; </ph><bpt id="p2">**</bpt>Python Environments<ept id="p2">**</ept><ph id="ph2"> &gt; </ph><bpt id="p3">**</bpt>Add/Remove Environments<ept id="p3">**</ept>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Visual Studio Solution Explorer</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Jupyter Notebooks (local)</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Jupyter Notebooks is distributed with Anaconda, which is the Python distribution used by Machine Learning Server.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>A local executable is installed with Machine Learning Server.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>On Windows, go to <bpt id="p1">**</bpt>\Program Files\Microsoft\ML Server\PYTHON_SERVER\Scripts<ph id="ph1">\\</ph><ept id="p1">**</ept> and double-click <bpt id="p2">**</bpt>jupyter-notebook.exe<ept id="p2">**</ept> to start a Jupyter Notebook session in the default browser window.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>On Linux, go to <bpt id="p1">**</bpt>/opt/microsoft/mlserver/9.3.0/runtime/python/bin/<ept id="p1">**</ept> and type <ph id="ph1">`./jupyter notebook`</ph>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>You should get a series of messages that includes the server endpoint and a URL that you can copy into a browser, assuming one is available on your computer.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>For additional instructions on configuring a multi-user server, see <bpt id="p1">[</bpt>How to add Machine Learning Server modules to single and multi-user Jupyter Notebook instances<ept id="p1">](how-to-revoscalepy-jupyter-nb-config.md)</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Jupyter Notebooks are a presentation concept, integrating script and text on the same page.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Script is interactive on the page, often Python or R, but could be any one of the 40 languages supported by Jupyter.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The text is user-provided content that describes the script.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Notebooks are executed on a server, accessed over http, and rendered as HTML in a browser to the person requesting the notebook.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>Jupyter documentation<ept id="p1">](https://jupyter.readthedocs.io/en/latest/content-quickstart.html)</ept>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>How to load Python samples on Windows</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Download just the .ipynb files from the GitHub repo <bpt id="p1">[</bpt><ph id="ph1">https://github.com/Microsoft/ML-Server-Python-Samples</ph><ept id="p1">](https://github.com/Microsoft/ML-Server-Python-Samples)</ept>:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Go to the source page: <bpt id="p1">[</bpt>ML-Server-Python-Samples/microsoftml/quickstarts/binary-classification/Binary+Classification+Quickstart.ipynb<ept id="p1">](https://github.com/Microsoft/ML-Server-Python-Samples/blob/master/microsoftml/quickstarts/binary-classification/Binary%2BClassification%2BQuickstart.ipynb)</ept></source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>In the GitHub page for this notebook, click <bpt id="p1">**</bpt>Raw<ept id="p1">**</ept> to show the Python script.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Use the browser save-as command to save a local copy of the file.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Apply an <bpt id="p1">**</bpt>.ipynb<ept id="p1">**</ept> file extension.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Some browsers append a .txt file extension automatically.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Remove the extraneous .txt extension if you see it in the file name.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Upload the .ipynb to your local server:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Navigate to the Jupyter-notebook executable on your computer: <ph id="ph1">`C:\Program Files\Microsoft\ML Server\PYTHON_SERVER\Scripts`</ph></source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Right-click <bpt id="p1">**</bpt>Run as administrator<ept id="p1">**</ept> on <ph id="ph1">`jupyter-notebook.exe`</ph></source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The Notebook Dashboard opens in your default browser at <ph id="ph1">`http://localhost:8888/tree`</ph>.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Upload<ept id="p1">**</ept> on the top right corner.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Navigate to the folder where you saved the .ipynb file.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Most likely, it's in the Downloads folder: <ph id="ph1">`\Downloads\ML-Server-Python-Samples-master\microsoftml\quickstarts\binary-classification\Binary+Classification+Quickstart.ipynb`</ph></source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Select the file and click <bpt id="p1">**</bpt>Open<ept id="p1">**</ept> to add the notebook to your server.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Click the notebook to load it, then click <bpt id="p1">**</bpt>Run<ept id="p1">**</ept> to step through the content and script.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>For this particular notebook, no additional configuration is required.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>For the web service notebook, read the readme for configuration requirements.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>PyCharm</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>In PyCharm, set the interpreter to the Python executable installed by Machine Learning Server.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>In a new project, in Settings, click <bpt id="p1">**</bpt>Add Local<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Enter <ph id="ph1">`C:\Program Files\Microsoft\ML Server\PYTHON_SERVER`</ph>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>You can now import revoscalepy, microsoftml, or azureml-model-management-sdk modules.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>You can also choose <bpt id="p1">**</bpt>Tools<ept id="p1">**</ept><ph id="ph1"> &gt; </ph><bpt id="p2">**</bpt>Python Console<ept id="p2">**</ept> to open an interactive window.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Now that you know how to load the Python libraries, you might want to explore them in-depth:</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>revoscalepy Python package functions<ept id="p1">](../python-reference/revoscalepy/revoscalepy-package.md)</ept></source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml Python package functions<ept id="p1">](../python-reference/microsoftml/microsoftml-package.md)</ept></source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>azureml-model-management-sdk<ept id="p1">](../python-reference/azureml-model-management-sdk/azureml-model-management-sdk.md)</ept></source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>For more about Machine Learning Server in general, see <bpt id="p1">[</bpt>Overview of Machine Learning Server<ept id="p1">](../what-is-machine-learning-server.md)</ept></source>
        </trans-unit></group></body></file></xliff>