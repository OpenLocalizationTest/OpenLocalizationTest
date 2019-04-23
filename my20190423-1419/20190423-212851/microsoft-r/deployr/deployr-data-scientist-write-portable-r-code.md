<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-data-scientist-write-portable-r-code.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338ac44c9e90a85a23e50018e6b404567a487fea0da7.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">c44c9e90a85a23e50018e6b404567a487fea0da7</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-data-scientist-write-portable-r-code.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Writing Portable R Code - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Data scientist's guide to Writing Portable R Code for DeployR</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Writing Portable R Code</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Introduction</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>As a data scientist, you need to aware of several R portability issues that arise when developing R analytics for use in your local R environment and in the DeployR server environment.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>They are:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Package portability</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Input portability</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Portable access to data files</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>These portability issues can be solved when you use the functions in the <ph id="ph1">`deployrUtils`</ph> package.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`deployrPackage()`</ph> to declare your package dependencies in your R code.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`deployrInput()`</ph> to declare the required inputs along with default values in your R code.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Use <ph id="ph1">`deployrExternal()`</ph> to access big data files from your R code.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The steps for using and testing the package functions in your R code locally and then testing them again in the DeployR server environment are described in the <bpt id="p1">[</bpt>Usage<ept id="p1">](#usage)</ept> section at the end of this document.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Package Portability</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Let's begin with some sample R code demonstrating how to declare your package dependencies in a portable manner:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Traditional R package management primarily involves using <ph id="ph1">`install.packages()`</ph> to install R packages from CRAN or a local repository in your local environment and <ph id="ph2">`library()`</ph> to load packages at runtime.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>When preparing portable R code for use both locally and in DeployR server environment, R package management recommendations differ slightly since the R script will be run in a remote server environment whenever executed on the DeployR server.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Unlike your local environment, you do not control that remote environment as a data scientist.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Since that remote environment is entirely independent, it is also potentially different from your local environment, which means that your R code might not be portable if that remote environment doesn't have all the packages your R scripts need.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Solution:<ept id="p1">**</ept> Always declare your package dependencies in your R code using the <ph id="ph1">`deployrPackage()`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>To ensure your R code runs consistently in your local environment and in the DeployR server environment, always use the <ph id="ph1">`deployrPackage`</ph> function from the <ph id="ph2">`deployrUtils`</ph> package in your R code.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>To learn how to get the package, use its functions locally, and test them in DeployR, read the <bpt id="p1">[</bpt>Usage<ept id="p1">](#usage)</ept> section.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>In a nutshell, using the <ph id="ph1">`deployrPackage`</ph> function safeguards your R code by making certain that:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The necessary packages are loaded and available to your R code at runtime.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Your R code is portable across your local environment and the DeployR server environment.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>When you use the <ph id="ph1">`deployrPackage`</ph> function, you can avoid issues such as having tested your R code locally, and then discovering that your R code fails when executed in the DeployR server environment due to one or more missing package dependencies.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Input Portability</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Let's begin with some sample R code demonstrating how to declare your required script inputs in a portable manner:</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The R scripts you develop and deploy to the DeployR server environment are ultimately executed as <bpt id="p1">[</bpt>Analytics Web Services<ept id="p1">](deployr-application-developer-getting-started.md#analytics-web-services)</ept> by client applications.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Most commonly, these R scripts expect input data to be provided by this application upon execution.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>In order for these inputs to be provided, the application developer who is integrating the R scripts must first know which inputs are required.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>As a data scientist creating analytics for use in DeployR, you are responsible for providing the application developers not only with the necessary analytics, but also helping them understand the inputs required by those analytics.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Whenever a required input is missing at runtime, the R script will fail.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Missing inputs present a real problem not only in production, but also when testing R scripts in multiple environments.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Solution:<ept id="p1">**</ept> Always declare the inputs required by your R code and assign them default values using <ph id="ph1">`deployrInput()`</ph>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`deployrInput`</ph> function, provided by the <ph id="ph2">`deployrUtils`</ph> package, enables you to specify the inputs required for your scripts directly in your R code along with the default value for each input.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Using the <ph id="ph1">`deployrInput`</ph> function, you can ensure your code is portable while providing clear guidance to your client application developers as to which script inputs their application will be required to supply.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>To learn how to get the package, use its functions locally, and test them in DeployR, read the <bpt id="p1">[</bpt>Usage<ept id="p1">](#usage)</ept> section.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>In a nutshell, the <ph id="ph1">`deployrInput`</ph> function allows you to:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Declare the required inputs for your script.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Assign default values for those inputs.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>When you declare your required inputs (and default values) using the <ph id="ph1">`deployrInput`</ph> function, your script will be portable and run successfully even when no input values are passed.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>These default values are ideal for developing and testing your scripts both locally and in the DeployR server environment since they guarantee that the script can always execute and return the same results across environments unless, of course, those default values are overwritten programmatically by an application.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Portable Access to Data Files</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Let's begin with some sample R code demonstrating how to reference your data files in a portable manner:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Whenever the data files with which you need to work are too big to be copied from the Web or copied from your local machine to the server, you can ask your administrator to store those files on your behalf in 'big data' external directories on the DeployR main server.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Since you're likely to use a copy or subset of the data in your local environment for development and testing purposes, it becomes interesting to reference those files in a portable manner so that data can be accessed whenever you run the R code locally or on the DeployR server.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Solution:<ept id="p1">**</ept> Always reference your big data files using <ph id="ph1">`deployrExternal()`</ph>.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>In a nutshell, the <ph id="ph1">`deployrExternal`</ph> function provides you with a consistent way of referencing these big data files for reading and writing; thereby, making your R code portable across your local environment and the DeployR server environment.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>All you have to do is:</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Ask your DeployR administrator to physically store a copy of your big data file in the appropriate external directory on the DeployR server on your behalf.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Reference the data file using the <ph id="ph1">`deployrExternal`</ph> function in your R code.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Then, when the R code executes locally, the function looks for a data file by that name in the current working directory of your R session.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>And when the R code executes remotely on the DeployR server, the function looks for a data file by that name in the dedicated external directories without requiring you to know the exact path of the file on the DeployR server.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>When you use the <ph id="ph1">`deployrExternal`</ph> function, you can avoid issues such as having tested your R code locally, and then having to change how you reference the data file when running it up on the DeployR server.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>The following steps describe how to use the functions in the <ph id="ph1">`deployrUtils`</ph> package to ensure the portability of your R code.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>For the complete package help, use <ph id="ph1">`library(help="deployrUtils")`</ph> in your IDE.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Part 1.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>In your local environment:</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Install <ph id="ph1">`deployrUtils`</ph> locally <bpt id="p1">[</bpt>from GitHub<ept id="p1">](https://github.com/Microsoft/deployrUtils/releases)</ept> using your IDE, R console, or terminal window with the following commands:</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Declare package dependencies using <ph id="ph1">`deployrPackage()`</ph> at the top of your script in your preferred IDE.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Consult the package help for more details.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Declare each script input individually and assign default values using <ph id="ph1">`deployrInput()`</ph> in your R code.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Consult the package help for more details.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Reference each big data file using <ph id="ph1">`deployrExternal()`</ph> in your R code.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Consult the package help for more details.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Make sure you ask your DeployR administrator to physically store a copy of your big data file in the appropriate external directory on the DeployR server on your behalf.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Test the script locally with those default values.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Script</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Part 2.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>In the DeployR Repository Manager:</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`deployrUtils`</ph> package is preinstalled in the DeployR server environment.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Log into<ept id="p1">](deployr-repository-manager-about.md#logging-in-and-out)</ept> the Repository Manager.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Login</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Upload<ept id="p1">](deployr-repository-manager-files.md#uploading-files)</ept> your script to the DeployR repository.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Upload</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Verify<ept id="p1">](deployr-data-scientist-getting-started.md#test-analytics)</ept> that the script's behavior remains consistent across environments by running that script using its default values in the <bpt id="p2">[</bpt>Test page<ept id="p2">](deployr-repository-manager-testing-debugging-scripts.md)</ept> before handing it off to the application developer(s).</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>If your script fails on the DeployR server due to one or more missing package dependencies, please contact your DeployR server administrator with details.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>See the <bpt id="p1">[</bpt>Administrator Guidelines<ept id="p1">](../operationalize/configure-manage-r-packages.md)</ept>.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>If your script fails on the DeployR server because the data file could not be found, ask your DeployR administrator to verify that the files you sent him or her were, in fact, deployed to the external directories.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Test Page</source>
        </trans-unit></group></body></file></xliff>