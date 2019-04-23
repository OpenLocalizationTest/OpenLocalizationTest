<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="concept-what-are-web-services.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a908bdc9f2603766db6cffff0c67f33f67163e031.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">908bdc9f2603766db6cffff0c67f33f67163e031</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\concept-what-are-web-services.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>What is a web service - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>In Machine Learning Server, a web service is an R or Python code execution on the operationalization compute node</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>What are web services in Machine Learning Server?</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies to: Machine Learning Server</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>In Machine Learning Server, a web service is an R or Python code execution on the <bpt id="p1">[</bpt>operationalization compute node<ept id="p1">](configure-start-for-administrators.md#configure-server-for-operationalization)</ept>.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Data scientists can deploy R and Python code and models as web services into Machine Learning Server to give other users a chance to use their code and predictive models.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Once hosted there, these web services are exposed and available for consumption.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Web services can be consumed directly in R or Python, programmatically using <bpt id="p1">[</bpt>REST APIs<ept id="p1">](https://microsoft.github.io/deployr-api-docs/#services-management-apis)</ept>, or via <bpt id="p2">[</bpt>Swagger-generated client libraries<ept id="p2">](how-to-build-api-clients-from-swagger-for-app-integration.md)</ept>.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>They can be consumed synchronously, in real-time, or in batch mode.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>They can also be deployed from one platform and consumed on another.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Web services facilitate the consumption and integration of the operationalized models and code they contain.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Once you've built a predictive model, in many cases the next step is to operationalize the model.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>That is to generate predictions from the pre-trained model on demand.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>In this scenario, where new data often become available one row at a time, latency becomes the critical metric.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>It is important to respond with the single prediction (or score) as quickly as possible.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Each web service is uniquely defined by its name and version.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>You can use the functions in the <bpt id="p1">[</bpt>mrsdeploy R package<ept id="p1">](../r-reference/mrsdeploy/mrsdeploy-package.md)</ept> or the <bpt id="p2">[</bpt>azureml-model-management-sdk Python package<ept id="p2">](../python-reference/azureml-model-management-sdk/azureml-model-management-sdk.md)</ept> to gain access a service's lifecycle from an R or Python script.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Requirement!</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Before you can deploy and work with web services, you must have access to a Machine Learning Server instance <bpt id="p1">[</bpt>configured to host web services<ept id="p1">](../operationalize/configure-start-for-administrators.md#configure-server-for-operationalization)</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>There are two types of web services: standard and real-time.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Standard web services</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>These web services offer fast execution and scoring of arbitrary Python or R code and models.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>They can contain code, models, and model assets.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>They can also take specific inputs and provide specific outputs for those users who are integrating the services inside their applications.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Standard web services, like all web services, are identified by their name and version.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Additionally, they can also be defined by any Python or R code, models, and any necessary model assets.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>When deploying a standard web service, you should also define the required inputs and any output the application developers use to integrate the service in their applications.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>See a standard web service deployment example: <bpt id="p1">[</bpt>R<ept id="p1">](../operationalize/quickstart-publish-r-web-service.md)</ept><ph id="ph1">  |  </ph><bpt id="p2">[</bpt>Python<ept id="p2">](../operationalize/python/quickstart-deploy-python-web-service.md)</ept></source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Real-time web services</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Real-time web services do not support arbitrary code and only accept models created with the supported functions from packages installed with the product.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>See the following sections for the list of supported functions by language and package.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Real-time web services offer even lower latency to produce results faster and score more models in parallel.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The improved performance boost comes from the fact that these web services do not depend on an interpreter at consumption time even though the services use the objects created by the model.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Therefore, fewer additional resources and less time is spent spinning up a session for each call.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Additionally, the model is only loaded once in the compute node and can be scored multiple times.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>For real-time services, you do <bpt id="p1">**</bpt>not<ept id="p1">**</ept> need to specify:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>inputs and outputs (dataframes are assumed)</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>code (only serialized models are supported)</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>See real-time web service deployment examples: <bpt id="p1">[</bpt>R<ept id="p1">](how-to-deploy-web-service-publish-manage-in-r.md#realtime-example)</ept><ph id="ph1">  |  </ph><bpt id="p2">[</bpt>Python<ept id="p2">](python/how-to-deploy-manage-web-services.md#realtime-example)</ept></source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Supported R functions for real time</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>A model object created with these supported functions:</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>R package</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Supported functions</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>RevoScaleR</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>rxBTrees, rxDTree, rxDForest, rxLogit, rxLinMod</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>MicrosoftML</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Machine learning and transform tasks:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>rxFastTrees, rxFastForest, rxLogisticRegression, rxOneClassSvm, rxNeuralNet, rxFastLinear, featurizeText, concat, categorical, categoricalHash, selectFeatures, featurizeImage, getSentiment, loadimage, resizeImage, extractPixels, selectColumns, and dropColumns</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>While mlTransform featurization is supported in real-time scoring, R transforms are not supported.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Instead, use sp_execute_external_script.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source><bpt id="p1">&lt;a name="inputdf"&gt;</bpt><ept id="p1">&lt;/a&gt;</ept> There are additional restrictions on the input dataframe format for microsoftml models:</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>The dataframe must have the same number of columns as the formula specified for the model.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The dataframe must be in the exact same order as the formula specified for the model.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>The columns must be of the same data type as the training data.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Type casting is not possible.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Supported Python functions for real time</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Python package</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Supported functions</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>revoscalepy</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>rx_btrees, rx_dforest, rx_dtree, rx_logit, rx_lin_mod</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>microsoftml</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Machine learning and transform tasks:</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>categorical, categorical_hash, concat, extract_pixels, featurize_text, featurize_image, get_sentiment, rx_fast_trees, rx_fast_forest, rx_fast_linear, rx_logistic_regression, rx_neural_network, rx_oneclass_svm, load_image, resize_image, select_columns, and drop_columns.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>See the preceding <bpt id="p1">[</bpt>input dataframe format restrictions<ept id="p1">](#inputdf)</ept>.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Versioning</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Every time a web service is published, a version is assigned to the web service.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Versioning enables users to better manage the release of their web services and helps the people consuming your service to find it easily.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>At publish time, specify an alphanumeric string that is meaningful to those users who consume the service.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>For example, you could use '2.0', 'v1.0.0', 'v1.0.0-alpha', or 'test-1'.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Meaningful versions are helpful when you intend to share services with others.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>We highly recommend a <bpt id="p1">**</bpt>consistent and meaningful versioning convention<ept id="p1">**</ept> across your organization or team such as semantic versioning.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Learn more about semantic versioning here: <ph id="ph1">http://semver.org/</ph>.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>If you do not specify a version, a globally unique identifier (GUID) is automatically assigned.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>These GUID numbers are long making them harder to remember and use.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Who consumes web services</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>After a web service has been published, authenticated users can consume that web service on various platforms and in various languages.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>You can consume directly in R or Python, using APIs, or in your preferred language via Swagger.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>You can make it easy for others to find your web services by providing them with the name and version of the web service.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Data scientists<ept id="p1">**</ept> who want to explore and consume the services directly <bpt id="p2">[</bpt>in R<ept id="p2">](../operationalize/how-to-consume-web-service-interact-in-r.md#consume-service)</ept> and <bpt id="p3">[</bpt>in Python<ept id="p3">](../operationalize/python/how-to-consume-web-services.md#consume-service)</ept>.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Quality engineers<ept id="p1">**</ept> who want to bring the models in these web services into validation and monitoring cycles.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Application developers<ept id="p1">**</ept> who want to call and integrate a web service into their applications.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Developers can generate client libraries for integration using the Swagger-based JSON file generated during service deployment.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Read "<bpt id="p1">[</bpt>How to integrate web services and authentication into your application<ept id="p1">](how-to-build-api-clients-from-swagger-for-app-integration.md)</ept>" for more details.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Services can also be consumed using the <bpt id="p1">[</bpt>RESTful APIs<ept id="p1">](concept-api.md)</ept> that provide direct programmatic access to a service's lifecycle.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>How are web services consumed</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Web services can be consumed using one of these approaches:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Approach</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Request Response</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>The service is consumed directly using a single synchronous consumption call.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Learn how <bpt id="p1">[</bpt>in R<ept id="p1">](../operationalize/how-to-consume-web-service-interact-in-r.md)</ept> <ph id="ph1">\|</ph> <bpt id="p2">[</bpt>in<ph id="ph2">&amp;nbsp;</ph>Python<ept id="p2">](../operationalize/python/how-to-consume-web-services.md)</ept></source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Asynchronous Batch</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Users send a single asynchronous request to the server who in turn makes multiple service calls on their behalf.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Learn how <bpt id="p1">[</bpt>in R<ept id="p1">](../operationalize/how-to-consume-web-service-asynchronously-batch.md)</ept></source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Permissions</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>By default, any authenticated Machine Learning Server user can:</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Publish a new service</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Update and delete web services they have published</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Retrieve any web service object for consumption</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>Retrieve a list of any or all web services</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Destructive tasks, such as deleting a web service, are available only to the user who initially created the service.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>However, your administrator can also <bpt id="p1">[</bpt>assign role-based authorization<ept id="p1">](configure-roles.md)</ept> to further control the permissions around web services.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>When you list services, you can see your role for each one of them.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>See also</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>In R:</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>Deploy and manage web services in R</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>List, get, and consume web services in R</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>Asynchronous web service consumption via batch</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>In Python:</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Deploy and manage web services in Python</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>List, get, and consume web services in Python</source>
        </trans-unit></group></body></file></xliff>