<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-data-scientist-getting-started.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a79095619b5c62031318f711d47d9326bdb7fe222.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">79095619b5c62031318f711d47d9326bdb7fe222</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-data-scientist-getting-started.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Getting Started with DeployR for Data Scientists - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Getting started for Data Scientists: high level introduction to DeployR for Data Scientists</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Data Scientists, r programmer, DeployR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Getting Started - Data Scientists</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to: DeployR 8.x<ept id="p1">**</ept>   (See <bpt id="p2">[</bpt>comparison between 8.x and 9.x<ept id="p2">](../whats-new-in-r-server.md#8vs9)</ept>)</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Looking to deploy with Machine Learning Server?</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Start here<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>This guide for data scientists offers a high-level introduction to DeployR.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>It helps you understand, as a data scientist, how best to work with the product tools to deliver compelling R analytics solutions in collaboration with <bpt id="p1">[</bpt>application developers<ept id="p1">](deployr-application-developer-getting-started.md)</ept>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>In a nutshell, DeployR makes your R analytics (R scripts, models, and data files) easily consumable by any application.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The sections that follow explain the steps you'll take to prepare those analytics and make them available to those who need them.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>They are:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Develop<ept id="p1">](#develop-analytics)</ept> your R scripts and other analytics with portability in mind</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Test<ept id="p1">](#test-analytics)</ept> those analytics inside and outside of DeployR</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Collaborate<ept id="p1">](#collaborate)</ept> with application developers to deliver powerful R analytic solutions</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>For a general introduction to DeployR, read the <bpt id="p1">[</bpt>About DeployR<ept id="p1">](deployr-about.md)</ept> document.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Develop Analytics</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>With DeployR, you can remain focused on creating the R code, models, and data files necessary to drive your analytics solutions without having to concern yourself with how these outputs are eventually <bpt id="p1">[</bpt>used by application developers<ept id="p1">](deployr-application-developer-getting-started.md)</ept> in their software solutions.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>That also means that, with minimal change in your current workflow, you can continue developing your analytics with your preferred R integrated development environment (IDE).</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>All it takes to prepare your R code for use in DeployR is a few simple portability enhancements, which you can make with your existing tool chain.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Use the following functions from the <ph id="ph1">`deployrUtils`</ph> R package to <bpt id="p1">[</bpt>make your R code portable<ept id="p1">](deployr-data-scientist-write-portable-r-code.md)</ept>:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>The <ph id="ph1">`deployrPackage`</ph> function<ept id="p1">](deployr-data-scientist-write-portable-r-code.md#package-portability)</ept> guarantees package portability from your local environment to the DeployR server environment when you use it to declare all of the package dependencies in your R script.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Packages declared using this function are automatically loaded at runtime, either in your local environment or on the DeployR server.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If the packages declared are not yet installed, then they're automatically installed before being loaded.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>The <ph id="ph1">`deployrInput`</ph> function<ept id="p1">](deployr-data-scientist-write-portable-r-code.md#input-portability)</ept> guarantees script input portability when you use it to define the inputs required by your scripts along with their default values.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>The <ph id="ph1">`deployrExternal`</ph> function<ept id="p1">](deployr-data-scientist-write-portable-r-code.md#portable-access-to-data-files)</ept> guarantees portability from your local environment to the DeployR server environment when you use it to reference the big data files from within your R scripts.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>You can install <ph id="ph1">`deployrUtils`</ph> locally <bpt id="p1">[</bpt>from GitHub<ept id="p1">](https://github.com/Microsoft/deployrUtils/releases)</ept> using your IDE, R console, or terminal window with the following commands:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Learn more on how to <bpt id="p1">[</bpt>write portable R code using these functions<ept id="p1">](deployr-data-scientist-write-portable-r-code.md)</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Script in IDE</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Once your R code, models, and data files are ready, you can <bpt id="p1">[</bpt>verify<ept id="p1">](#Test-Analytics)</ept> their behavior in a DeployR server environment.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Reproducibility Tip:<ept id="p1">**</ept> Use <bpt id="p2">[</bpt>the <ph id="ph1">`checkpoint`</ph> package<ept id="p2">](https://mran.microsoft.com/package/checkpoint/)</ept> to make sure your script always has the same package dependency versions from a specific date across environments and users by pointing to the same fixed CRAN repository snapshot.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>When the exact same package dependencies are used, you get reproducible results.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>This package is installed with Microsoft R Open (and Revolution R Open).</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Test Analytics</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Perhaps not surprisingly, the next step after developing your analytics is to test them.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The first step is to test your analytics in your local environment.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Then, when you are ready, upload those analytics to the DeployR server environment so you can test your R scripts in a live debugging environment.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Testing Locally</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Testing locally involves running your R code within your local R integrated development environment as you always have.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If you encounter issues during your tests, simply refine your analytics and retest them.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>When satisfied with your results, the next step is to verify that you obtain the same results when testing remotely.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Login</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Testing Remotely</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Testing remotely involves executing your R scripts in the DeployR server environment.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Doing so is easy when you use the web-based <bpt id="p1">[</bpt>Repository Manager<ept id="p1">](deployr-repository-manager-about.md)</ept> that ships with DeployR.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>In just a few clicks, you can upload and test your R scripts, models, and data files via the Repository Manager.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Here's how:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Log into<ept id="p1">](deployr-repository-manager-about.md#logging-in-and-out)</ept> the web-based DeployR landing page.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Login</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Open the Repository Manager tool.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Create a directory<ept id="p1">](deployr-repository-manager-directories.md#creating-directories)</ept> that you can use to store your development copies of your R analytics.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>In our example, we'll call this directory you'll use for development and testing in DeployR, <ph id="ph1">`fraud-score-dev`</ph>.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>These copies of your R analytics won't be shared with the application developers.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>We'll do that in a later step in the <bpt id="p1">[</bpt>Collaboration<ept id="p1">](#collaborate)</ept> section.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>New Directory</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Upload<ept id="p1">](deployr-repository-manager-files.md#uploading-files)</ept> your R scripts, models, and data files into that development directory.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Those files are now <bpt id="p1">[</bpt>Analytics Web Services<ept id="p1">](deployr-application-developer-getting-started.md#analytics-web-services)</ept> that, with the proper permissions, can be consumed by any application.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Upload</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Open the R script<ept id="p1">](deployr-repository-manager-files.md#opening-files)</ept> you want to test.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Open File</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Click <bpt id="p2">**</bpt>Test<ept id="p2">**</ept><ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md)</ept> on the right of the <bpt id="p3">**</bpt>File Properties<ept id="p3">**</ept> page to open the <bpt id="p4">**</bpt>Test<ept id="p4">**</ept> page.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Test<ept id="p1">**</ept> page acts as a live debugging environment.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Click <bpt id="p2">**</bpt>Run<ept id="p2">**</ept><ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#running-scripts-in-test-page)</ept> in the upper-right hand pane to execute the R script.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>As the script executes, you'll see the <bpt id="p1">[</bpt>console output<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#reviewing-debug-console-output)</ept> in the bottom left pane.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>After execution, you can review the <bpt id="p1">[</bpt>response markup<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#reviewing-execution-artifacts)</ept> in the bottom right pane.</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Test Page</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Verify that you experience the same R script behavior in the DeployR server environment as you did when you tested your R scripts locally.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>If you encounter issues or want to make further changes to your analytics, then you can refine and test your analytics locally before returning to the Repository Manager to upload and retest remotely again.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>If you are ready to start <bpt id="p1">[</bpt>collaborating with your application developers<ept id="p1">](#collaborate)</ept>, you can make your R scripts and other analytics available to them.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Collaborate</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Collaboration with the application developers on your team makes it possible to deliver sophisticated software solutions powered by R analytics.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Whenever you develop new analytics or improve existing ones, you must inform the application developers on your team and hand off those analytics as described in this section.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>How you share and collaborate on these R analytics depends on whether you plan to do so <bpt id="p1">[</bpt>on-server<ept id="p1">](#On-Server-Collaboration)</ept>, which requires access to a common DeployR server instance, or <bpt id="p2">[</bpt>off-server<ept id="p2">](#Off-Server-Collaboration)</ept>.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Collaborate</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>This document focuses on the roles and responsibilities of the data scientist.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>To learn more about the role of the application developer, read the <bpt id="p1">[</bpt>Getting Started<ept id="p1">](deployr-application-developer-getting-started.md)</ept> guide for application developers.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Guidance</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>We strongly recommend the following approach to collaboration:</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Share only stable, tested snapshots of your R analytic files with application developers.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Provide the application developers with all necessary details regarding your R analytic files.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Share Stable, Tested Snapshots</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>We recommend sharing your R analytic files with application developers prior to their final iteration.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>By releasing early versions or prototypes of your work, you make it possible for the application developers to begin their integration work.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>You can then continue refining, adding, and testing your R analytics in tandem.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>However, you don't want to share every iteration of your files either.</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>As you develop and update your R analytics, certain modifications might result in code-breaking changes in an R script’s runtime behavior.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>For this reason, we strongly recommend sharing file snapshots only if they have been <bpt id="p1">**</bpt>fully tested by you<ept id="p1">**</ept> to minimize the chances of introducing errors when the application developers try them out.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>In practice, each snapshot of your R analytics should include completed functionality and/or changes that affects the application interface for which the application developers will need to accommodate.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>We also recommend, when working in DeployR, that you keep the development copies of your R analytics in a private and distinct directory from the directory where you'll share your stable snapshots with application developers.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>Provide Complete Details to Application Developers</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Once you share a snapshot with application developers, you must let them know that this the snapshot is available and also provide them with <bpt id="p1">**</bpt>any information that will help them integrate your R analytics<ept id="p1">**</ept> into their application code.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Rather than leave the developer guessing as to why their code no longer works, we strongly recommend that you not only to tell them which files are available, but perhaps more importantly, what has changed.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Be sure to include:</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>The list of new/updated filenames and their respective directories</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>Any new/updated inputs required by your R script</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Any new/updated outputs generated by your R scripts</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Communicate</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>On-Server Collaboration</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>When the application developers have access to the same DeployR server instance as you, you can share stable, tested R analytics snapshots there.</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Log into<ept id="p1">](deployr-repository-manager-about.md#logging-in-and-out)</ept> the web-based <bpt id="p2">[</bpt>Repository Manager<ept id="p2">](deployr-repository-manager-about.md)</ept>.</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>Login</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Open the Repository Manager tool.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Create a snapshot directory<ept id="p1">](deployr-repository-manager-directories.md#creating-directories)</ept> for collaboration in which you'll share the snapshots of your R analytics with application developers.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>Keep in mind that each snapshot should be a stable and tested version of your R analytics.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>We recommend that you follow a convention when naming your project directories that enables those directories to be easily associated.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>In our example, the directory we used to upload and test these R analytics in DeployR before sharing them is called <ph id="ph1">`fraud-score-dev`</ph>.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>And here, we'll name the snapshot directory <ph id="ph1">`fraud-score`</ph>.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>New Directory</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>Create a copy of each file from your development directory to the newly created project directory:</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Open each file<ept id="p1">](deployr-repository-manager-files.md#opening-files)</ept>.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>File Properties<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Open File</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>File Properties<ept id="p1">**</ept> page, choose <bpt id="p2">**</bpt>Copy<ept id="p2">**</ept> from the <bpt id="p3">**</bpt>Manage<ept id="p3">**</ept> menu.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Copy File<ept id="p1">**</ept> dialog opens.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>Copy File</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Enter a name for the file in the <bpt id="p1">**</bpt>Name<ept id="p1">**</ept> field.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>We recommend you use the same name as you have in your development directory.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>If a file by that name already exists, this will become the new Latest version of that file.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>The version history is available to file owners.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>Select the new directory you've just created from the <bpt id="p1">**</bpt>Directory<ept id="p1">**</ept> drop down list.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Copy<ept id="p1">**</ept> to make the copy.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>The dialog closes and the <bpt id="p1">**</bpt>Files<ept id="p1">**</ept> tab appears on the screen.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Repeat steps a - e for each file you are ready to share.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>Add any application developers who will work with these files as owners of those files in the new directory so they can access, test, and download them:</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>From the <bpt id="p1">**</bpt>Files<ept id="p1">**</ept> tab, click the name of the new directory under the <bpt id="p2">**</bpt>My Files<ept id="p2">**</ept> tree on the left side of the page.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Contents of New Directory</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Open each file<ept id="p1">](deployr-repository-manager-files.md#opening-files)</ept> in the new directory.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>File Properties<ept id="p1">**</ept> page appears.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>Optionally, add notes to the application developers in the <bpt id="p1">**</bpt>Description<ept id="p1">**</ept> field.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>For example, you could let them know which values should be retrieved.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Add/Remove<ept id="p1">**</ept> to <bpt id="p2">[</bpt>add application developers as owners<ept id="p2">](deployr-repository-manager-files.md#adding-and-removing-owners)</ept> of the file.</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>Add Owners</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>Repeat steps a - d for each file you've just copied to the new directory.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>Inform your application developers that new or updated analytics are available for integration.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Be sure to provide them with any details that can help them integrate those analytics.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Now the application developer(s) can review the files in the Repository Manager.</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>They can also test the R scripts in the Test page and explore the artifacts.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>Application developers can use the files in this instance of DeployR as they are, make copies of the files, set permissions on those files, or even download the files to use in a separate instance of DeployR.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Off-Server Collaboration</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>If <bpt id="p1">[</bpt>application developers<ept id="p1">](deployr-application-developer-getting-started.md)</ept> on your project do not have access to the same instance of DeployR as you, then you can share stable snapshots of your R analytics by:</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Sending the files directly to application developers via email, or</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>Putting them on a secure shared resource such as shared NFS drive, OneDrive, or Dropbox.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>Keep in mind that:</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>It is critical that you provide the application developers with any details that can help them integrate those analytics.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>The files you share should be stable and tested snapshots of your R analytics.</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Once you've shared those files, the application developers can upload the files into their DeployR server any way they want including through the <bpt id="p1">[</bpt>Repository Manager<ept id="p1">](deployr-repository-manager-about.md)</ept>, using client libraries, or via the <bpt id="p2">[</bpt>raw API<ept id="p2">](deployr-api-reference.md)</ept>.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>More Resources</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>Use the table of contents to find all of the guides and documentation needed by the data scientist, administrator, or application developer.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>Key Documents</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>About DeployR</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>How to Write Portable R Code with deployrUtils<ept id="p1">](deployr-data-scientist-write-portable-r-code.md)</ept><ph id="ph1"> ~ </ph><ph id="ph2">`deployrUtils`</ph> package documentation</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Repository Manager Help<ept id="p1">](deployr-repository-manager-about.md)</ept> ~ Online help for the DeployR Repository Manager.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>About Throughput<ept id="p1">](deployr-admin-scale-and-throughput.md#about-throughput)</ept> ~ Learn how to optimize your throughput</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Getting Started For Application Developers</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>Getting Started For Administrators</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Support Channel</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>Microsoft R Server (and DeployR) Forum</source>
        </trans-unit></group></body></file></xliff>