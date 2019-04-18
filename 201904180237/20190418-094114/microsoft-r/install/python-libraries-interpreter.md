<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="python-libraries-interpreter.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea92615f10f2e1408b0e331120e3f329b75878199ea81.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">15f10f2e1408b0e331120e3f329b75878199ea81</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">20cd1eea-d819-421c-a8f6-e0e067dea926</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\python-libraries-interpreter.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Install Python client libraries for remote access to Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Installing python interpreter and packages locally to interact with a remote Machine Learning Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>How to install Python client libraries for remote access to a Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Machine Learning Server includes open-source and Microsoft-specific Python packages for modeling, training, and scoring data for statistical and predictive analytics.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>For classic client-server configurations, where multiple clients connect to and use a remote Machine Learning Server, installing the same Python client libraries on a local workstation enables you to write and run script locally and then push execution to the remote server where data resides.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This is referred to as a <bpt id="p1">[</bpt>remote compute context<ept id="p1">](../r/concept-what-is-compute-context.md)</ept>, operant when you call Python functions from libraries that exist on both client and server environments.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>A remote server can be either of the following server products:</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>SQL Server 2017 Machine Learning Services (In-Database)<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/install/sql-machine-learning-services-windows-install)</ept></source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Machine Learning Server for Hadoop<ept id="p1">](machine-learning-server-hadoop-install.md)</ept></source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Client workstations can be Windows or Linux.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Microsoft Python packages<ept id="p1">](../python-reference/introducing-python-package-reference.md)</ept> common to both client and server systems include the following:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>revoscalepy<ept id="p1">](../python-reference/revoscalepy/revoscalepy-package.md)</ept></source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>microsoftml<ept id="p1">](../python-reference/microsoftml/microsoftml-package.md)</ept></source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>azureml-model-management-sdk<ept id="p1">](../python-reference/azureml-model-management-sdk/azureml-model-management-sdk.md)</ept></source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>pre-trained models<ept id="p1">](microsoftml-install-pretrained-models.md)</ept></source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>This article describes how to install a Python interpreter (Anaconda) and Microsoft's Python packages locally on a client machine.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Once installed, you can use all of the Python modules in Anaconda, Microsoft's packages, and any third-party packages that are Python 3.5 compliant.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>For remote compute context, you can only call the Python functions from packages in the above list.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Check package versions</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>While not required, it's a good idea to cross-check package versions so that you can match versions on the server with those on the client.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>On a server with restricted access, you might need an administrator to get this information for you.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Package information on SQL Server<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/r/determine-which-packages-are-installed-on-sql-server)</ept></source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Package information on Machine Learning Server for Hadoop<ept id="p1">](machine-learning-server-hadoop-install.md#package-list)</ept></source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Install Python libraries on Windows</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Download the installation shell script from <bpt id="p1">[</bpt><ph id="ph1">https://aka.ms/mls93-py</ph><ept id="p1">](https://aka.ms/mls93-py)</ept> (or use <bpt id="p2">[</bpt><ph id="ph2">https://aka.ms/mls-py</ph><ept id="p2">](https://aka.ms/mls-py)</ept> for the 9.2.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>release).</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The script installs Anaconda 4.2.0, which includes Python 3.5.2, along with all packages listed previously.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Open PowerShell window with elevated administrator permissions (right-click <bpt id="p1">**</bpt>Run as administrator<ept id="p1">**</ept>).</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Go to the folder in which you downloaded the installer and run the script.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Add the <ph id="ph1">`-InstallFolder`</ph> command-line argument to specify a folder location for the libraries.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Installation takes some time to complete.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>You can monitor progress in the PowerShell window.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>When setup is finished, you have a complete set of packages.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For example, if you specified <ph id="ph1">`C:\mspythonlibs`</ph> as the folder name, you would find the packages at <ph id="ph2">`C:\mspythonlibs\Lib\site-packages`</ph>.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The installation script does not modify the PATH environment variable on your computer so the new python interpreter and modules you just installed are not automatically available to your tools.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>For help on linking the Python interpreter and libraries to tools, see <bpt id="p1">[</bpt>Link Python tools and IDEs<ept id="p1">](../python/quickstart-python-tools.md)</ept>, replacing the MLS server paths with the path you defined on your workstation For example, for a Python project in Visual Studio, your custom environment would specify <ph id="ph1">`C:\mypythonlibs`</ph>, <ph id="ph2">`C:\mypythonlibs\python.exe`</ph> and <ph id="ph3">`C:\mypythonlibs\pythonw.exe`</ph> for <bpt id="p2">**</bpt>Prefix path<ept id="p2">**</ept>, <bpt id="p3">**</bpt>Interpreter path<ept id="p3">**</ept>, and <bpt id="p4">**</bpt>Windowed interpreter<ept id="p4">**</ept>, respectively.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Offline install</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Download .cab files used for <bpt id="p1">[</bpt>offline installation<ept id="p1">](machine-learning-server-windows-offline.md#file-list-93)</ept> and place them in your %TEMP% directory.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>You can type %TEMP% in a Run command to get the exact location, but it is usually a user directory such as <ph id="ph1">`C:\Users\&lt;your-user-name&gt;\AppData\Local\Temp`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>After copying the files, run the PowerShell script using the same syntax as an online install.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The script knows to look in the temp directory for the files it needs.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Install Python libraries on Linux</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>On each supported OS, the package manager downloads packages from the repository, determines dependencies, retrieves additional packages, and installs the software.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>After installation completes, mlserver-python executable is at '/usr/bin'.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>On Ubuntu 14.04 - 16.04<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>With root or sudo permissions, run the following commands:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Red Hat and CentOS 6/7<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>With root or sudo permissions, run the following commands:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>SUSE Linux Enterprise Server 11<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>With root or sudo permissions, run the following commands:</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Test local package installation</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>As a verification step, call functions from the revoscalepy package and from <bpt id="p1">[</bpt>scikit<ept id="p1">](http://scikit-learn.org/stable/)</ept>, included in Anaconda.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>If you get a "module not found" error for any of the instructions below, verify you are loading the python interpreter from the right location.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>If using Visual Studio, confirm that you selected the custom environment pointing the prefix and interpreter paths to the correct location.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>On Windows, depending on how you run the script, you might see this message: "Express Edition will continue to be enforced".</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Express edition is one of the free SQL Server editions.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>This message is telling you that client libraries are licensed under the Express edition.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Limits on this edition are the same as Standard: in-memory data sets and 2-core processing.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Remote servers typically run higher editions not subjected to the same memory and processing limits.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>When you push the compute context to a remote server, you work under the full capabilities of that system.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Create some data to work with.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>This example loads the iris data set using scikit.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Print out the dataset.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>You should see a 4-column table with measurements for sepal length, sepal width, petal length, and petal width.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Load revoscalepy and calculate a statistical summary for data in one of the columns.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Print the output to view mean, standard deviation, and other measures.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Results<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Now that you have installed local client libraries and verified function calls, try the following walkthroughs to learn how to use the libraries locally and remotely when connected to resident data stores.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Quickstart: Create a linear regression model in a local compute context<ept id="p1">](../python/quickstart-revoscalepy-linear-regression-model.md)</ept></source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to use revoscalepy in a Spark compute context<ept id="p1">](../python/how-to-revoscalepy.md)</ept></source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to use revoscalepy in a SQL Server compute context<ept id="p1">](https://docs.microsoft.com/sql/advanced-analytics/tutorials/use-python-revoscalepy-to-create-model)</ept></source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Remote access to a SQL Server is enabled by an administrator who has configured ports and protocols, enabled remote connections, and assigned user logins.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Check with your administrator to get a valid connection string when using a remote compute context to SQL Server.</source>
        </trans-unit></group></body></file></xliff>