<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="quickstart-publish-r-web-service.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a503d4f514b1212985c648c1de287c5c69150e613.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">503d4f514b1212985c648c1de287c5c69150e613</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\quickstart-publish-r-web-service.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Quickstart: Deploy R models as web services with mrsdeploy - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>How to deploy an R model as a service</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>quickstart, Machine Learning Server, Microsoft R Server, deploy r models</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Quickstart: Deploy an R Model as a web service with mrsdeploy</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Applies to: R Client 3.x, R Server 9.x, Machine Learning Server 9.x</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Learn how to publish an R model as a web service with Machine Learning Server, formerly known as Microsoft R Server.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Data scientists work locally with <bpt id="p1">[</bpt>Microsoft R Client<ept id="p1">](../r-client-get-started.md)</ept> in their preferred R IDE and favorite version control tools to build scripts and models.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Using the mrsdeploy package that ships with Microsoft R Client and Machine Learning Server, you can develop, test, and ultimately deploy these R analytics as web services in your production environment.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>A Machine Learning Server R web service is an R code execution on the <bpt id="p1">[</bpt>operationalization compute node<ept id="p1">](configure-start-for-administrators.md#configure-server-for-operationalization)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Each web service is uniquely defined by a <ph id="ph1">`name`</ph> and <ph id="ph2">`version`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>You can use the functions in <bpt id="p1">[</bpt>the mrsdeploy package<ept id="p1">](../r-reference/mrsdeploy/mrsdeploy-package.md)</ept> to gain access a service's lifecycle from an R script.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>A set of <bpt id="p1">[</bpt>RESTful APIs<ept id="p1">](https://microsoft.github.io/deployr-api-docs/#services-management-apis)</ept> is also available to provide direct programmatic access to a service's lifecycle directly.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Time estimate</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If you have completed the prerequisites, this task takes approximately <bpt id="p1">*</bpt>10<ept id="p1">*</ept> minutes to complete.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Prerequisites</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Before you begin this QuickStart, have the following ready:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>An instance of <bpt id="p1">[</bpt>Microsoft R Client installed<ept id="p1">](../r-client-get-started.md)</ept> on your local machine.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>You can optionally configure an R IDE of your choice, such as R Tools for Visual Studio, to run Microsoft R Client.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>An instance of <bpt id="p1">[</bpt>Machine Learning Server installed<ept id="p1">](../what-is-machine-learning-server.md)</ept> that has been <bpt id="p2">[</bpt>configured to operationalize analytics<ept id="p2">](configure-start-for-administrators.md#configure-server-for-operationalization)</ept>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>For your convenience, <bpt id="p1">[</bpt>Azure Resource Management (ARM) templates<ept id="p1">](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-overview#template-deployment)</ept> are available to quickly deploy and configure the server for operationalization in Azure.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The connection details to that instance of Machine Learning Server.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Contact your administrator for any missing connection details.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>After <bpt id="p1">[</bpt>connecting to Machine Learning Server<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept> in R, deploy your analytics as web services so others can consume them.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Example code</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>This article walks through the deployment of a simple R model as a web service hosted in Machine Learning Server.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Here is the entire R code for the example that we walk through in the sections that follow.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Be sure to replace the remoteLogin() function with the correct login details for your configuration.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Connecting to Machine Learning Server using the mrsdeploy package is covered <bpt id="p1">[</bpt>in this article<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>A.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Model locally</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Now let's dive into this example down.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Let's start by creating the model locally, then publish it, and then share it with other authenticated users.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Launch your R IDE or Rgui so you can start entering R code.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>If you have R Server 9.0.1, load the mrsdeploy package.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>In later releases, this package is preloaded for you.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Create a GLM model called <ph id="ph1">`carsModel`</ph> using the dataset <ph id="ph2">`mtcars`</ph>, which is a built-in data frame in R. Using horsepower (hp) and weight (wt), this model estimates the probability that a vehicle has been fitted with a manual transmission.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Examine the results of the locally executed code.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>You can compare these results to the results of the web service later.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>B.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Publish model as a web service</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>From your local R IDE, log in to Machine Learning Server <bpt id="p1">**</bpt>with your credentials<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Use the appropriate authentication function from <bpt id="p1">[</bpt>the mrsdeploy package<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept> (<ph id="ph1">`remoteLogin`</ph> or <ph id="ph2">`remoteLoginAAD`</ph>) for your authentication method.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>For simplicity, the following code uses the basic local 'admin' account for authentication with the <ph id="ph1">`remoteLogin`</ph> function and <ph id="ph2">`session = false`</ph> so that no remote R session is started.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Learn more about authenticating with Active Directory LDAP or Azure Active Directory in the article "<bpt id="p1">[</bpt>Connecting to Machine Learning Server from mrsdeploy<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept>."</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Be sure to replace the remoteLogin() function with the <bpt id="p1">[</bpt>correct login details for your configuration<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept>.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Now, you are successfully connected to the remote Machine Learning Server.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Publish the model as a web service to Machine Learning Server using <bpt id="p1">[</bpt>the publishService() function<ept id="p1">](how-to-deploy-web-service-publish-manage-in-r.md)</ept> from the mrsdeploy package.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>In this example, you publish a web service called <ph id="ph1">`"mtService"`</ph> using the model <ph id="ph2">`carsModel`</ph> and the function <ph id="ph3">`manualTransmission`</ph>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>As an input, the service takes a list of vehicle horsepower and vehicle weight represented as an R numerical.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>As an output, a percentage as an R numeric for the probability each vehicle has of being fitted with a manual transmission.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>When publishing a service, specify its name and version, the R code, the inputs, and the outputs needed for application integration as well as other parameters.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>To publish a web service while in a remote R session, carefully <bpt id="p1">[</bpt>review these guidelines<ept id="p1">](../r/how-to-execute-code-remotely.md#publish-remote-session)</ept>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>C.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Consume the service in R to test</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Consume the service in R directly after publishing it to verify that the results are as expected.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The results should match the results obtained when the model was run locally earlier.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>As long as the package versions are the same on Machine Learning Server as they are locally, you should get the same results.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>You can check for differences using <bpt id="p1">[</bpt>a remote session "diff report."<ept id="p1">](../r/how-to-execute-code-remotely.md#diff)</ept></source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>If you get an alphanumeric error code, such as <ph id="ph1">`Message: b55088c4-e563-459a-8c41-dd2c625e891d`</ph>, when consuming a service, search for that code in the <bpt id="p1">[</bpt>compute node's log file<ept id="p1">](configure-run-diagnostics.md#logs)</ept> to reveal the full error message.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>D.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Get the Swagger-based JSON file</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Anyone can test and consume the service using its auto-generated Swagger-based JSON file.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>This Swagger-based JSON file is specific to a given version of a service.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>You can easily get this file during the same authenticated session in which you published the service.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>It can be downloaded to the local file system.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>You can get this Swagger file as long as the web service exists as described in the article "<bpt id="p1">[</bpt>How to interact with and consume web services in R<ept id="p1">](how-to-consume-web-service-interact-in-r.md)</ept>."</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>In this example, we executed these commands to download the Swagger-based JSON file:</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Learn how to get and share<ept id="p1">](how-to-consume-web-service-interact-in-r.md#data-scientists-share)</ept> this Swagger-based JSON file after the session ends.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Next steps</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>After it has been deployed, the web service can be:</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Consumed directly in R by another data scientist<ept id="p1">](how-to-consume-web-service-interact-in-r.md#data-scientists-share)</ept>, for testing purposes for example</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Integrated into an application by an application developer<ept id="p1">](how-to-build-api-clients-from-swagger-for-app-integration.md)</ept>  using the  Swagger-based .JSON file produced when the web service was published.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>How to execute R code remotely</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>You can use Microsoft R Client to run your R code locally and from R Client you can connect remotely to Machine Learning Server to run your code there.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>You can easily switch between the local context and the remote context using pause() and resume() functions.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Learn more in this article, <bpt id="p1">[</bpt>Remote Execution in Microsoft Machine Learning Server<ept id="p1">](../r/how-to-execute-code-remotely.md)</ept>.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Requirements for remote execution include:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Configure an R Integrated Development Environment (IDE) to work with <bpt id="p1">[</bpt>Microsoft R Client<ept id="p1">](../r-client-get-started.md)</ept>.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Obtain <bpt id="p1">[</bpt>authenticated access<ept id="p1">](configure-authentication.md)</ept> to an instance of Machine Learning Server with its <bpt id="p2">[</bpt>operationalization feature configured<ept id="p2">](configure-start-for-administrators.md#configure-server-for-operationalization)</ept>.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>More resources</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>This section provides a quick summary of useful links for data scientists operationalizing R analytics with Machine Learning Server.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>About Operationalization</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Functions in mrsdeploy package</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Connecting to Machine Learning Server from mrsdeploy</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Working with web services in R</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Asynchronous batch execution of web services in R</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Execute on a remote Machine Learning Server</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>How to integrate web services and authentication into your application</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>Get started for administrators</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>User Forum</source>
        </trans-unit></group></body></file></xliff>