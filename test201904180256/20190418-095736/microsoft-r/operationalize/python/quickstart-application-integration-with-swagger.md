<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="quickstart-application-integration-with-swagger.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18cb96a6b5ef0ce8f3487567c3cb12486f6e88bc081.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">b96a6b5ef0ce8f3487567c3cb12486f6e88bc081</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">8ea8c771-7844-49cc-84f5-71599942a18c</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\python\quickstart-application-integration-with-swagger.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Quickstart: Integrate a real-time web service into an application using Swagger - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>In this quickstart you learn how to deploy an python model as a service into an application using Swagger.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>quickstart, Machine Learning Server, deploy python models, real-time web service, Swagger</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Quickstart: Integrate a real-time web service into an application using Swagger</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: Microsoft Learning Server 9.x<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>This quickstart shows how to use a Swagger-generated client to consume a Python model deployed as a real-time web service in Machine Learning Server.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>A web service is a model or code that has been deployed and hosted in a server.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Real-time web services only accept models created with the functions supported by the packages installed with the product.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>revoscalepy<ept id="p1">](./../../python-reference/revoscalepy/revoscalepy-package.md)</ept> package installed on the Machine Learning Server supports the <ph id="ph1">`rx_lin_mod`</ph> function used by the linear model in this quickstart.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>This quickstart shows you how to:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>deploy a Machine Learning Server in Azure</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>create a real-time web service from a Python script</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>use Swagger to integrate the service into a C# application.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This quickstart has been designed for new users and is self-contained.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>You must have an <bpt id="p1">[</bpt>Azure subscription<ept id="p1">](https://azure.microsoft.com/en-us/free/)</ept> and <bpt id="p2">[</bpt>Visual Studio<ept id="p2">](https://www.visualstudio.com/downloads/)</ept>, or some other IDE for developing a C# application, installed to complete it.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>It also assumes some familiarity with Python and C#.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>After you have deployed the Machine Learning Server on Azure, this quickstart takes approximately 10 minutes to complete.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Deploy Machine Learning Server with an ARM template</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>You can configure a Machine Learning Server to act as a deployment server and host analytic web services.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Machine Learning Server web services can be operationalized in two types of configuration:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>One-box configuration<ept id="p1">**</ept>: includes one web node and one compute node that run on a single machine.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This configuration is useful when you want to explore what is needed to operationalize R or Python analytics.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Enterprise configuration<ept id="p1">**</ept>: where multiple nodes are configured on multiple machines along with other enterprise features.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>This configuration can be scaled out or in by adding or removing nodes.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>This quickstart uses the one-box configuration on Windows.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The deployment is automated using an ARM template.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Go to <bpt id="p1">[</bpt>OneBox Configuration for Windows<ept id="p1">](https://github.com/Microsoft/microsoft-r/tree/master/mlserver-arm-templates/one-box-configuration/windows)</ept> and click the <bpt id="p2">**</bpt>Deploy to Azure<ept id="p2">**</ept> button to deploy the ARM Templates.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>arm-template</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>This takes you to the <bpt id="p1">**</bpt>Custom deployment<ept id="p1">**</ept> page in the Azure portal where you need to supply values for basics and settings in the red-started fields.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>custom-deployment</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Agree to the Terms and Conditions and click <bpt id="p1">**</bpt>Purchase<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Find the <bpt id="p1">**</bpt>mlserver<ept id="p1">**</ept> resource in <bpt id="p2">**</bpt>All resources<ept id="p2">**</ept>, click <bpt id="p3">**</bpt>Connect<ept id="p3">**</ept> after the server has been created.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>mlserver-azure-resource</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Open<ept id="p1">**</ept> and then click <bpt id="p2">**</bpt>Connect<ept id="p2">**</ept> again on the <bpt id="p3">**</bpt>Remote Desktop Connection<ept id="p3">**</ept> window.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Use the credentials you specified when creating the server when prompted and then click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept> to log in.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Ignore the RDP warning that the certificate cannot be authenticated.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>For more information on options for configuring a server for operationalization, see <bpt id="p1">[</bpt>Manage and configure Machine Learning Server for operationalization<ept id="p1">](./../../operationalize/configure-start-for-administrators.md)</ept></source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Deploy a Python model as a web service in Machine Learning Server</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>In this step, you build a linear model to predict the ratings from the data in the other columns (complaints, privileges, learning, raises, critical, advance) of the attitude dataset and publish it as a web service.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>This quickstart walks you through the individual steps needed for the two tasks in this section.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>But it also summarizes the commands after the walkthrough in a script that executes all of the commands needed to build and deploy the web service and provides a link to a Jupyter notebook that contains these (and some additional) commands.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>To launch Python command window, open <bpt id="p1">**</bpt>File Explorer<ept id="p1">**</ept>, copy the full path to the executable:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Paste it into <bpt id="p1">**</bpt>Address Bar<ept id="p1">**</ept> of <bpt id="p2">**</bpt>File Explorer<ept id="p2">**</ept> and press <bpt id="p3">**</bpt>Enter<ept id="p3">**</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Read in the attitude dataset</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>From your local machine, read in the data that you use to build the linear model.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>We use the attitude dataset.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>OUTPUT:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Authenticate and initiate the DeployClient</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>This quickstart uses the local 'admin' account for authentication.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The following code imports the <bpt id="p1">[</bpt>DeployClient<ept id="p1">](./../../python-reference/azureml-model-management-sdk/deploy-client.md)</ept> and <bpt id="p2">[</bpt>MLServer<ept id="p2">](./../../python-reference/azureml-model-management-sdk/mlserver.md)</ept> classes from the <bpt id="p3">[</bpt>azureml-model-management-sdk package<ept id="p3">](./../../python-reference/azureml-model-management-sdk/azureml-model-management-sdk.md)</ept> that are used to connect to Machine Learning Server.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Then replace YOUR_ADMIN_PASSWORD with the administrator password that you used to create the server (but do not use the administrator name in place of admin in the <ph id="ph1">`context`</ph> - it must use 'admin') in the following code and run it:</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>There are several ways to authenticate with Machine Learning Server on-premises or in the cloud.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>To learn more about connecting to Machine Learning Server in Python, see <bpt id="p1">[</bpt>Authenticate with Machine Learning Server in Python with azureml-model-management-sdk<ept id="p1">](./../../operationalize/python/how-to-authenticate-in-python.md)</ept>.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Create and run a linear model locally</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Now that you are authenticated, you can use the <bpt id="p1">[</bpt>rx_lin_mod<ept id="p1">](./../../python-reference/revoscalepy/rx-lin-mod.md)</ept> function from the <bpt id="p2">[</bpt>revoscalepy package<ept id="p2">](./../../python-reference/revoscalepy/revoscalepy-package.md)</ept> to build the model.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The following code creates a Generalized Linear Model (GLM) using the imported attitude dataset:</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>OUTPUT:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>This model can now be used to estimate the ratings expected from the attitude dataset.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>The following code shows how to make some predictions locally to test the model:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>OUTPUT:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Publish the model as a real-time web service</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>To publish any model as a real-time service, you must first serialize the model object using the revoscalepy <bpt id="p1">[</bpt>rx_serialize_model<ept id="p1">](./../../python-reference/revoscalepy/rx-serialize-model.md)</ept> function.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Initiate a <bpt id="p1">[</bpt>realtimeDefinition<ept id="p1">](./../../python-reference/azureml-model-management-sdk/realtime-definition.md)</ept> object from the <bpt id="p2">[</bpt>azureml-model-management-sdk package<ept id="p2">](./../../python-reference/azureml-model-management-sdk/azureml-model-management-sdk.md)</ept> to publish the linear model as a real-time Python web service to Machine Learning Server.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Verify that the web service results match the results obtained when the model was run locally.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>To consume the real-time service, call <ph id="ph1">`.consume`</ph> on the real-time <bpt id="p1">[</bpt>service<ept id="p1">](./../../python-reference/azureml-model-management-sdk/service.md)</ept> object.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>You can consume the model using the <bpt id="p1">[</bpt>Service<ept id="p1">](./../../python-reference/azureml-model-management-sdk/service.md)</ept> object returned from <ph id="ph1">`.deploy()`</ph> because you are in the same session as the one you in which you deployed.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>OUTPUT:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>To delete the service, use the following code:</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>OUTPUT:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Summary Python script</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>This script can be run with Python.exe to create the model and deploy it as a web service.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Replace YOUR_ADMIN_PASSWORD in the <ph id="ph1">`context`</ph> with the administrator password that you used to create the server.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Copy the entire script and paste it at the Python command prompt by right-clicking.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Use a Jupyter Notebook</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>There is also a <bpt id="p1">[</bpt>Publish_Realtime_Web_Service_in_Python.ipynb<ept id="p1">](https://github.com/Microsoft/ML-Server-Python-Samples/blob/master/operationalize/Publish_Realtime_Web_Service_in_Python.ipynb)</ept> Jupyter Notebook that can be used on the Machine Learning Server to build  and deploy this model as a web service.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>First you must download the notebook from the Microsoft Machine Learning Python Samples GitHub repo onto your server:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Go to the <bpt id="p1">[</bpt>Microsoft Machine Learning Python Samples<ept id="p1">](https://github.com/Microsoft/ML-Server-Python-Samples)</ept> repo from your Machine Learning Server.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Click on the <bpt id="p1">**</bpt>Clone or download<ept id="p1">**</ept> button and select the <bpt id="p2">**</bpt>Download ZIP<ept id="p2">**</ept> option.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Select <bpt id="p1">**</bpt>Save<ept id="p1">**</ept> and <bpt id="p2">**</bpt>Open folder<ept id="p2">**</ept>, right click on the <bpt id="p3">*</bpt>ML-Server-Python-Samples-master.zip<ept id="p3">*</ept> folder and select <bpt id="p4">**</bpt>Extract All...<ept id="p4">**</ept> and then <bpt id="p5">**</bpt>Extract<ept id="p5">**</ept> to your preferred location.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>The Download directory is used by default.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>To run the Publish_Realtime_Web_Service_in_Python.ipynb Jupyter Notebook:</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Open the File Explorer, navigate to <bpt id="p1">*</bpt>C:\Program Files\Microsoft\ML Server\PYTHON_SERVER\Scripts<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>To open the Notebook Dashboard in your default browser at <ph id="ph1">http://localhost:8888/tree</ph>, right-click and select <bpt id="p1">**</bpt>Run as administrator<ept id="p1">**</ept> on jupyter-notebook.exe.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>To load the Notebook, Click on Upload on the <ph id="ph1">http://localhost:8888/tree</ph> page and navigate to the Publish_Realtime_Web_Service_in_Python.ipynb notebook and click <bpt id="p1">**</bpt>Open<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>The default location is C:\Users\admin-mls\Downloads\ML-Server-Python-Samples-master\ML-Server-Python-Samples-master\operationalize.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>To open the Publish_Realtime_Web_Service_in_Python.ipynb Notebook, click on <bpt id="p1">**</bpt>Upload<ept id="p1">**</ept> opposite it and then double click on the notebook to open it:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>jupyter-notebook</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Build API clients with the Swagger file</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Get the Swagger file</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>To save to Swagger JSON file to a specified location (in the example C:<ph id="ph1">\\</ph>Users<ph id="ph2">\\</ph>\Public<ph id="ph3">\\</ph>Downloads<ph id="ph4">\\</ph>), run the following commands from the Python prompt in the VM:</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Open the linmodservice-swagger.json file and copy the contents.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Go to <bpt id="p1">[</bpt>Swagger<ept id="p1">](https://swagger.io)</ept> homepage on your main machine.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>From the <bpt id="p1">**</bpt>Tools<ept id="p1">**</ept> menu on the homepage, choose <bpt id="p2">**</bpt>Swagger Tools<ept id="p2">**</ept><ph id="ph1"> -&gt; </ph><bpt id="p3">**</bpt>Swagger Editor<ept id="p3">**</ept>.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Choose button for the <bpt id="p1">**</bpt>Online Editor<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Delete the contents in the editor window on the left and past in the contents of the linmodservice-swagger.json file.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Generate the client</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Click the <bpt id="p1">**</bpt>Generate Client<ept id="p1">**</ept> button on the toolbar and choose the language for the client.</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source><ph id="ph1">![</ph>language-choice-in-swagger-editor<ph id="ph2">](./media/quickstart-application-integration-with-swagger/5-language-choice-in-swagger-editor.png)</ph></source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Choose the C# client and save the csharp-client-generated.zip file to your preferred location and extract the zip file.</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Create the C# client to consume the web service</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Open the IO.Swagger.sln from the unzipped ..\csharp-client-generated\csharp-client folder with Visual Studio.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>To add a C# console application to the solution, right-click the <bpt id="p1">**</bpt>Solution 'IO.Swagger'<ept id="p1">**</ept>  in the <bpt id="p2">**</bpt>Solution Explorer<ept id="p2">**</ept><ph id="ph1"> -&gt; </ph><bpt id="p3">**</bpt>Add<ept id="p3">**</ept><ph id="ph2"> -&gt; </ph><bpt id="p4">**</bpt>New Project...<ept id="p4">**</ept><ph id="ph3"> -&gt; </ph><bpt id="p5">**</bpt>Visual C#<ept id="p5">**</ept><ph id="ph4"> -&gt; </ph><bpt id="p6">**</bpt>ConsoleApp (.NET Framework)<ept id="p6">**</ept>.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Accept the default name "ConsoleApp1" and click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>To make it the main application, right-click the <bpt id="p1">**</bpt>ConsoleApp1<ept id="p1">**</ept> project and select <bpt id="p2">**</bpt>Set as StartUp Project<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>To add the IO.Swagger application as a dependency, right-click the <bpt id="p1">**</bpt>ConsoleApp1<ept id="p1">**</ept> project and select <bpt id="p2">**</bpt>Build Dependencies<ept id="p2">**</ept><ph id="ph1"> -&gt;</ph><bpt id="p3">**</bpt>Project Dependencies...<ept id="p3">**</ept>. On the Dependencies tab check the <bpt id="p4">**</bpt>IO.Swagger<ept id="p4">**</ept> box in the <bpt id="p5">**</bpt>Depends on<ept id="p5">**</ept> window and click <bpt id="p6">**</bpt>OK<ept id="p6">**</ept>.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>(The IO.Swagger.Test application can be ignored for our purposes.)</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>Right-click the <bpt id="p1">**</bpt>ConsoleApp1<ept id="p1">**</ept> project and select <bpt id="p2">**</bpt>Add<ept id="p2">**</ept><ph id="ph1"> -&gt; </ph><bpt id="p3">**</bpt>Reference...<ept id="p3">**</ept><ph id="ph2"> -&gt; </ph><bpt id="p4">**</bpt>Projects<ept id="p4">**</ept>.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Check the <bpt id="p1">**</bpt>IO.Swagger<ept id="p1">**</ept> box and click <bpt id="p2">**</bpt>OK<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>To add the RestSharp and NewtonSoft.Json libraries to ConsoleApp1, right-click on the IO.Swagger Solution in the <bpt id="p1">**</bpt>Solution Explorer<ept id="p1">**</ept>, select <bpt id="p2">**</bpt>Manage NuGet Packages for Solution...<ept id="p2">**</ept> and specify and install the versions of the RestSharp and NewtonSoft.Json packages for ConsoleApp1 that match the versions used in IO.Swagger.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>To add the three references needed by the <bpt id="p1">**</bpt>ConsoleApp1<ept id="p1">**</ept> client, right-click on <bpt id="p2">**</bpt>ConsoleApp1<ept id="p2">**</ept> and select <bpt id="p3">**</bpt>Add<ept id="p3">**</ept><ph id="ph1"> -&gt; </ph><bpt id="p4">**</bpt>Reference...<ept id="p4">**</ept>. In the <bpt id="p5">**</bpt>Reference Manager<ept id="p5">**</ept> window, select the <bpt id="p6">**</bpt>Projects<ept id="p6">**</ept> tab on the left and check the box for the <bpt id="p7">**</bpt>IO.Swagger<ept id="p7">**</ept> project.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>Then select the <bpt id="p1">**</bpt>Browse<ept id="p1">**</ept> tab on the left and check the boxes for the versions of the <bpt id="p2">**</bpt>RestSharp<ept id="p2">**</ept> and <bpt id="p3">**</bpt>NewtonSoft.Json<ept id="p3">**</ept> dlls just installed.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>To add references to the installed and click <bpt id="p1">**</bpt>OK<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Replace <bpt id="p1">*</bpt>YOUR_ADMIN_PASSWORD<ept id="p1">*</ept> in the Initialize O16N params section of the following C# code with the password that you used when creating the VM.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Do not change the username, <bpt id="p1">*</bpt>admin<ept id="p1">*</ept>, regardless of the name you used to create the VM.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Paste the resulting code into the Program.cs file of the ConsoleApp1, replacing the code that was there by default.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Then build and run the solution.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>using IO.Swagger.Api; using IO.Swagger.Client; using IO.Swagger.Model; using System; using System.Collections.Generic;</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>OUTPUT:<ept id="p1">**</ept></source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Clean up resources</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>To delete the service created, run this code in the Python command window.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>To stop the VM, return to the Azure portal, locate the server in your resource group and select <bpt id="p1">**</bpt>Stop<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>This option would allow you to restart the VM for use later and not pay for compute resources in the interim.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>If you do not intent to use the VM or its related resource group again, return to the Azure portal, select the resource group for the VM, and click <bpt id="p1">**</bpt>Delete<ept id="p1">**</ept> to remove all of the resource in the group from Azure permanently.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to consume web services in Python synchronously (request/response)<ept id="p1">](how-to-consume-web-services.md)</ept></source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to consume web services in Python asynchronously (batch)<ept id="p1">](how-to-consume-web-services-async.md)</ept></source>
        </trans-unit></group></body></file></xliff>