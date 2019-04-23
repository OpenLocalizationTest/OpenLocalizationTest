<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="quickstart-deploy-python-web-service.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a283f78fb962eea4b0af616c5b59569efa7c5bae3.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">283f78fb962eea4b0af616c5b59569efa7c5bae3</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\python\quickstart-deploy-python-web-service.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to deploy Python models as web services - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to deploy an python model as a service</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>quickstart, Machine Learning Server, deploy python models</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Quickstart: Deploy a Python model as a web service with azureml-model-management-sdk</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Applies to: Machine Learning Server 9.x</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Learn how to deploy a Python model as a <bpt id="p1">[</bpt>web service with Machine Learning Server<ept id="p1">](../concept-what-are-web-services.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Data scientists work locally in their preferred Python IDE and favorite version control tools to build scripts and models.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Using the <bpt id="p1">[</bpt>azureml-model-management-sdk Python package<ept id="p1">](../../python-reference/azureml-model-management-sdk/azureml-model-management-sdk.md)</ept> that ships with Machine Learning Server, you can develop, test, and ultimately deploy these Python analytics as web services in your production environment.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server, a web service is a model and/or code that has been deployed and hosted in the server.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Each web service is uniquely defined by a <ph id="ph1">`name`</ph> and <ph id="ph2">`version`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>When consumed, the service consists of the code execution on a <bpt id="p1">[</bpt>compute node<ept id="p1">](../configure-start-for-administrators.md#configure-server-for-operationalization)</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Learn more <bpt id="p1">[</bpt>about web services<ept id="p1">](../concept-what-are-web-services.md)</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>You can use the functions in <bpt id="p1">[</bpt>the azureml-model-management-sdk Python library <ept id="p1">](../../python-reference/azureml-model-management-sdk/azureml-model-management-sdk.md)</ept> to manage the web service's lifecycle from a Python script.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A set of <bpt id="p1">[</bpt>RESTful APIs<ept id="p1">](https://microsoft.github.io/deployr-api-docs/#services-management-apis)</ept> is also available to provide direct programmatic access to a service's lifecycle.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Time estimate</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>After you have completed the prerequisites, this task takes approximately <bpt id="p1">*</bpt>10<ept id="p1">*</ept> minutes to complete.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Before you begin this QuickStart, have the following ready:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Machine Learning Server with Python that's <bpt id="p1">**</bpt><bpt id="p2">[</bpt>configured to operationalize models<ept id="p2">](../../operationalize/configure-machine-learning-server-one-box.md)</ept><ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Try an <bpt id="p1">[</bpt>Azure Resource Management template<ept id="p1">](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-overview#template-deployment)</ept> to quickly configure a server for operationalization.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>connection details (host, username, password)<ept id="p1">](../../operationalize/python/how-to-authenticate-in-python.md)</ept>  to that server instance from your administrator.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>Python client libraries for remote access to Machine Learning Server<ept id="p1">](https://docs.microsoft.com/machine-learning-server/install/python-libraries-interpreter)</ept> installed on your machine.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Familiarity with Python.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Here's a video tutorial<ept id="p1">](https://mva.microsoft.com/en-us/training-courses/introduction-to-programming-with-python-8360?l=lqhuMxFz_8904984382)</ept>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Familiarity with Jupyter notebooks.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Learn <bpt id="p1">[</bpt>how to load sample Python notebooks<ept id="p1">](../../python/how-to-revoscalepy-jupyter-nb-config.md)</ept>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Example code</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The example for this quickstart is stored in a Jupyter notebook.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>This notebook format allows you to not only see the code alongside detailed explanations, but also allows you to try out the code.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>This example walks through the deployment of a Python model as a web service hosted in Machine Learning Server.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>We will build a simple linear model using the <bpt id="p1">[</bpt>rx_lin_mod<ept id="p1">](../../python-reference/revoscalepy/rx-lin-mod.md)</ept> function from the <bpt id="p2">[</bpt>revoscalepy package<ept id="p2">](../../python-reference/revoscalepy/revoscalepy-package.md)</ept> installed with Machine Learning Server or <bpt id="p3">[</bpt>locally on Windows machine<ept id="p3">](../../install/python-libraries-interpreter.md)</ept>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>This package requires a connection to Machine Learning Server.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The notebook example walks you through how to:</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Create and run a linear model locally</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Authenticate with Machine Learning Server<ept id="p1">](how-to-authenticate-in-python.md)</ept> from your Python script</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Publish the model as a Python web service to Machine Learning Server</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Examine, test, and consume the service in the same session</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Delete the service</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>You can try it yourself with the notebook.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>&amp;#9658; <bpt id="p1">[</bpt><bpt id="p2">**</bpt>Download the Jupyter notebook to try it out<ept id="p2">**</ept><ept id="p1">](https://github.com/Microsoft/ML-Server-Python-Samples/blob/master/operationalize/Quickstart_Publish_Python_Web_Service.ipynb)</ept>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>After it has been deployed, the web service can be:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Consumed directly in Python by someone else<ept id="p1">](how-to-consume-web-services.md)</ept> for testing purposes See an example in <bpt id="p2">[</bpt>this Jupyter notebook<ept id="p2">](https://github.com/Microsoft/ML-Server-Python-Samples/blob/master/operationalize/Explore_Consume_Python_Web_Services.ipynb)</ept>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Integrated into an application by an application developer<ept id="p1">](../how-to-build-api-clients-from-swagger-for-app-integration.md)</ept>  using the  Swagger-based .JSON file produced when the web service was published.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>This section provides a quick summary of useful links for data scientists looking to operationalize their analytics with Machine Learning Server.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>About Operationalization</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>What are web services</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Functions in azureml-model-management-sdk package</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Connecting to Machine Learning Server in Python</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Working with web services in Python</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Example of deploying real-time web service</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>How to consume web services in Python synchronously (request/response)</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>How to consume web services in Python asynchronously (batch)</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>How to integrate web services and authentication into your application</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Get started for administrators</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>User Forum</source>
        </trans-unit></group></body></file></xliff>