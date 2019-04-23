<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="deployr-repository-manager-testing-debugging-scripts.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca861d8d39913149ebffe2a96b926fb946651e3803d8.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1d8d39913149ebffe2a96b926fb946651e3803d8</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\deployr\deployr-repository-manager-testing-debugging-scripts.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>DeployR Repository Manager Help - DeployR 8.x</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Testing and Debugging the DeployR Repository Manager</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Testing and Debugging Scripts</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>For tips and guidance on how to develop portable R code using the deployrUtils package, see the <bpt id="p1">[</bpt>Writing Portable R Code<ept id="p1">](../deployr/deployr-data-scientist-write-portable-r-code.md)</ept> guide on the DeployR website.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Use the <bpt id="p1">**</bpt>Test<ept id="p1">**</ept> page to do the following to repository-managed scripts:</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Test and verify the functioning of scripts you own</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Debug and fix the functioning of scripts you own</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Test and verify the functioning of scripts to which you have access rights</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Debug the functioning of scripts to which you have <bpt id="p1">[</bpt>access rights<ept id="p1">](../deployr/deployr-repository-manager-files.md#about-file-properties)</ept></source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Test Page Panes</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Test<ept id="p1">**</ept> page is divided into four panes:</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Source<ept id="p1">**</ept> pane (1):  displays the actual R <bpt id="p2">[</bpt>source code<ept id="p2">](deployr-repository-manager-testing-debugging-scripts.md#inspecting-the-source-code)</ept> contained in the script file</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Debug Console Output<ept id="p1">**</ept> pane (2): displays the R session <bpt id="p2">[</bpt>console output<ept id="p2">](deployr-repository-manager-testing-debugging-scripts.md#reviewing-debug-console-output)</ept> generated during the execution of a script</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Script Execution Parameters<ept id="p1">**</ept> pane (3): allows you to interact with the <bpt id="p2">[</bpt>inputs<ept id="p2">](deployr-repository-manager-testing-debugging-scripts.md#supplying-input-values)</ept> defined in the code and define simple <bpt id="p3">[</bpt>inputs on-the-fly<ept id="p3">](deployr-repository-manager-testing-debugging-scripts.md#quick-on-the-fly-inputs)</ept>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Artifacts<ept id="p1">**</ept> pane (4): allows you to see the <bpt id="p2">[</bpt>files and plots<ept id="p2">](deployr-repository-manager-testing-debugging-scripts.md#reviewing-execution-artifacts)</ept> produced when the code was last executed as well as inspect the API <bpt id="p3">[</bpt>request and response<ept id="p3">](deployr-repository-manager-testing-debugging-scripts.md#reviewing-execution-artifacts)</ept> markup.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Opening the Test Page</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>To access the Test page:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Open a script and click the <bpt id="p1">**</bpt>Test<ept id="p1">**</ept> button on the right of the <bpt id="p2">**</bpt>File Properties<ept id="p2">**</ept> page.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Test<ept id="p1">**</ept> page opens.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Each time you log into the Repository Manager, you are automatically allocated a dedicated R session, which supports all of your R script testing and debugging within the Repository Manager.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>This R session lives for the duration of your HTTP session, until you logout or timeout, at which point it is released.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>You can <bpt id="p1">[</bpt>load data <ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#loading-data-into-the-r-session)</ept>into the R session as well as <bpt id="p2">[</bpt>clear the workspace and working directory<ept id="p2">](deployr-repository-manager-testing-debugging-scripts.md#clearing-the-r-session-working-directory-or-workspace)</ept>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Inspecting the Source Code</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Source<ept id="p1">**</ept> pane presents the script’s R code.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The extent to which you can interact with the source code depends entirely on <bpt id="p1">[</bpt>permissions and policies<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Viewing R Code</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Viewing R Code</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>In this pane, you can view and scroll through the source code of the R script.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Code elements are color-coded for your convenience.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>If you do not own this file and cannot see the code in the <bpt id="p1">**</bpt>Source<ept id="p1">**</ept> pane, then a <bpt id="p2">[</bpt>server policy<ept id="p2">](../what-is-operationalization.md)</ept> was changed by your administrator.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>An onscreen alert will also appear.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Editing R Code</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Only the owners of a file can edit the source code of the <bpt id="p1">[</bpt><bpt id="p2">*</bpt>Latest<ept id="p2">*</ept><ept id="p1">](deployr-repository-manager-files.md#working-with-historical-versions)</ept> version of a script.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>This pane is not meant to be used to write scripts or make major changes to your scripts.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>It is not a substitute for your favorite IDE for R. However, to facilitate the debugging process, the owners of a file can use this pane to make small changes, save those changes to the repository, and test them out.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>To edit the R code:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Find the code you want to change in the <bpt id="p1">**</bpt>Source<ept id="p1">**</ept> pane or position your cursor where you want to write new code.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Type your edits directly into the pane.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Save<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#saving-script-changes)</ept> your script and <bpt id="p2">[</bpt>run it<ept id="p2">](deployr-repository-manager-testing-debugging-scripts.md#running-scripts-in-test-page)</ept> to test the changes.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Only file owners who were assigned the <bpt id="p1">[</bpt><bpt id="p2">**</bpt>POWER_USER<ept id="p2">**</ept><ept id="p1">](../what-is-operationalization.md)</ept> role by the administrator have the permissions to run snippets of code in the <bpt id="p3">**</bpt>Source<ept id="p3">**</ept> pane.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>If you are a file owner assigned the <bpt id="p1">**</bpt>POWER_USER<ept id="p1">**</ept> role, you can select and run snippets from the <bpt id="p2">**</bpt>Source<ept id="p2">**</ept> pane and inspect the workspace in the <bpt id="p3">**</bpt>Debug Console Output<ept id="p3">**</ept> pane to see the R objects within and their values.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Running Scripts in Test Page</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Any DeployR user who can access a script can also test that script by running the script, changing the <bpt id="p1">[</bpt>input values<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#supplying-input-values)</ept>, and then running it again in the <bpt id="p2">**</bpt>Test<ept id="p2">**</ept> page.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>When debugging a script, you may need to <bpt id="p1">[</bpt>interrupt an execution<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#interrupting-code-executions)</ept>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Running Entire Scripts with Default Inputs or No Inputs</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>You can run a script in the <bpt id="p1">**</bpt>Test<ept id="p1">**</ept> page using the script's source code as-is regardless of whether or not any inputs were defined using <bpt id="p2">[</bpt>deployrInput()<ept id="p2">](deployr-repository-manager-testing-debugging-scripts.md)</ept>.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>To run a script with the default values and inputs:</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Open<ept id="p1">](../deployr/deployr-repository-manager-files.md#opening-files)</ept> the script and go to the <bpt id="p2">[</bpt><bpt id="p3">**</bpt>Test<ept id="p3">**</ept> page<ept id="p2">](deployr-repository-manager-testing-debugging-scripts.md)</ept>.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Make no changes in the <bpt id="p1">**</bpt>Script Execution Parameters<ept id="p1">**</ept> pane.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Run<ept id="p1">**</ept> in the toolbar.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>This script is run in its entirety.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Any <bpt id="p1">[</bpt>artifacts<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#reviewing-execution-artifacts)</ept> are then displayed in the Artifacts pane.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Running Entire Scripts with Modified Inputs</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>You can supply new and modified input values for a script, and then pass those input values when executing the script.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Supply new input values in the following ways:</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Defining temporary <bpt id="p1">[</bpt>primitive input values<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#quick-on-the-fly-inputs)</ept> on-the-fly</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Modifying the value of any <bpt id="p1">[</bpt>deployrInput()<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#r-code-inputs-deployrinput)</ept> widgets</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Editing the <bpt id="p1">[</bpt>source code<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#inspecting-the-source-code)</ept> to add, remove, or update any deployrInput() functions (available to script-owners only)</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>For tips and guidance on how to develop portable R code using the deployrInput function from the deployrUtils package, see the <bpt id="p1">[</bpt>Writing Portable R Code<ept id="p1">](../deployr/deployr-data-scientist-write-portable-r-code.md)</ept> guide on the DeployR website.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>To run a script new and modified input values:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Open<ept id="p1">](../deployr/deployr-repository-manager-files.md#opening-files)</ept> the script.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Go to the <bpt id="p1">[</bpt><bpt id="p2">**</bpt>Test<ept id="p2">**</ept> page<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md)</ept>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Supply input values<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#supplying-input-values)</ept>.</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Script Execution Parameters<ept id="p1">**</ept> pane, click <bpt id="p2">**</bpt>Run<ept id="p2">**</ept> in the toolbar.</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>The input values are passed along from this pane, and the script is run in its entirety.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Running Snippets of Code</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>If you own the script and have <bpt id="p1">[</bpt><bpt id="p2">**</bpt>POWER_USER<ept id="p2">**</ept><ept id="p1">](../what-is-operationalization.md)</ept> permissions, you can run a snippet of code directly from the <bpt id="p3">**</bpt>Source<ept id="p3">**</ept> pane.</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>In this way, you can make small changes to your R code and run only the lines you want to test.</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>You can even select a variable name, for example, and run that to see its contents.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Running code from the Source pane will run the selected code as-is without taking into account any modified values or <bpt id="p1">**</bpt>Quick Inputs<ept id="p1">**</ept> defined in the <bpt id="p2">**</bpt>Script Execution Parameters<ept id="p2">**</ept> pane.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>To run code selections:</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Open<ept id="p1">](../deployr/deployr-repository-manager-files.md#opening-files)</ept> the script</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Go to the <bpt id="p1">[</bpt><bpt id="p2">**</bpt>Test<ept id="p2">**</ept> page<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md)</ept>.</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Source<ept id="p1">**</ept> pane, select the code that you want to run.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>If no code is selected, the current line is used.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Press <ph id="ph1">`Ctrl-Enter`</ph> on Windows/Linux or <ph id="ph2">`Command-Enter`</ph> on MAC.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>The code is executed on the server and the response is displayed in the <bpt id="p1">**</bpt>Debug Console Output<ept id="p1">**</ept> and <bpt id="p2">**</bpt>Artifacts<ept id="p2">**</ept> panes.</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Reviewing Debug Console Output</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Debug Console Output<ept id="p1">**</ept> pane, you can see all of the R session console output generated during the execution of the code on the DeployR server.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Each time code is executed in this <bpt id="p1">**</bpt>Test<ept id="p1">**</ept> page, this pane is automatically populated for you.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>While this pane bears some resemblance to R's console, the <bpt id="p1">**</bpt>Debug Console Output<ept id="p1">**</ept> pane in Repository Manager is designed to help you learn more about your script's behavior for the purposes of debugging the script, not to act as your primary development environment.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>This <bpt id="p1">**</bpt>Debug Console Output<ept id="p1">**</ept> pane executes code exclusively on the server and does not have the same capabilities as a full R console.</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>If you are an owner assigned the <bpt id="p1">**</bpt>POWER_USER<ept id="p1">**</ept> role, you can select and run elements from the <bpt id="p2">**</bpt>Source<ept id="p2">**</ept> pane and inspect the workspace here to see the objects and their values.</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Although you cannot type anything into the console, you can still <bpt id="p1">[</bpt>clear the pane, the working directory, or the workspace<ept id="p1">](#manipulating-the-underlying-r-session)</ept>.</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Reviewing Execution Artifacts</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Files &amp; Plots<ept id="p1">**</ept> section of the <bpt id="p2">**</bpt>Artifacts<ept id="p2">**</ept> pane presents the files and plots produced when code was last executed in the <bpt id="p3">**</bpt>Test<ept id="p3">**</ept> page:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Any unnamed or named graphical files generated by the R graphics device, which are visually rendered in the pane</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Non-image files written to the working directory, such as .CSV files, binary files, and so on, which appear as clickable links in the pane</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>These <bpt id="p1">**</bpt>API Request and API Response<ept id="p1">**</ept> sections of the <bpt id="p2">**</bpt>Artifacts<ept id="p2">**</ept> pane present the execution at the API level.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>This information is particularly interesting to DeployR <bpt id="p1">**</bpt>client application developers<ept id="p1">**</ept> since it provides critical details they can use when building their client applications.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>API Request<ept id="p1">**</ept> presents the complete set of parameters sent along to the DeployR server on the script execution API call.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>API Response<ept id="p1">**</ept> presents the complete response markup sent back by the DeployR server on the script execution API call.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Upon each code execution, the <bpt id="p1">**</bpt>Artifacts<ept id="p1">**</ept> pane is cleared and repopulated.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Manipulating the Underlying R Session</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>Each time you log into the Repository Manager, you are automatically allocated a dedicated R session, which supports all of your R script testing and debugging within the Repository Manager.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>This R session lives for the duration of your HTTP session, until you logout or timeout, at which point it is released.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>To help you test and debug your scripts, you can manipulate this underlying R session by:</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Loading<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#loading-data-into-the-r-session)</ept> and moving data into the R session to be used by one or more of the scripts you are debugging</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Clearing<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#clearing-the-r-session-working-directory-or-workspace)</ept> the working directory or workspace of that underlying R session</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Retrieving DeployR-encoded R objects<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#retrieving-r-objects)</ept> from the workspace</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Loading Data into the R Session</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>You can load data into the underlying R session from the <bpt id="p1">**</bpt>Test<ept id="p1">**</ept> page of any open script.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source>Any type of data file can be loaded into the working directory of the underlying R session.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source>For example, you could load a .CSV file that will be read by your script.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>However, only files containing binary R objects, typically with a .rData file extension, can be loaded directly into the workspace from this page.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>You choose to load data files and binary R objects from the repository or from your local machine.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source>You can always load your files; however, your ability to load data files that you do not own from the repository is determined by <bpt id="p1">[</bpt>server policies<ept id="p1">](../what-is-operationalization.md)</ept>.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source>To load data into the underlying R session:</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Test<ept id="p1">**</ept> page of the open script, click the <bpt id="p2">**</bpt>Load<ept id="p2">**</ept> button in the <bpt id="p3">**</bpt>Script Execution Parameters<ept id="p3">**</ept> pane toolbar.</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>To load a file that already exists in the repository, choose <bpt id="p1">**</bpt>Load File from Repository<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>To load a file from your machine, choose <bpt id="p1">**</bpt>Load File from Local Machine<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>In the dialog, select the directory and file containing the data to be loaded.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>Specify whether the data should be loaded into the working directory or workspace:</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>If you are loading a data file, choose <bpt id="p1">**</bpt>Working directory<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>If you are loading a binary R object, choose <bpt id="p1">**</bpt>Workspace<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>If necessary, first save your model or other object outside of DeployR as an .rData file, and then load it here.</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>Click <bpt id="p1">**</bpt>Load<ept id="p1">**</ept> to load the data.</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>If you have loaded data files or R objects into this R session, clearing the workspace and working directory, or even timing out of your user session, will delete the files, data, and R objects you loaded.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source>If that data is still needed, you must reload it.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>Clearing the R Session Working Directory or Workspace</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>You can clear the working directory and/or the workspace on the underlying R session using the menu in the <bpt id="p1">**</bpt>Debug Console Output<ept id="p1">**</ept> pane toolbar.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>When you clear the working directory, all data files in your work directory are deleted, including those files output to the working directory by code executions as well as any files you loaded into the working directory.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source>Likewise, if you clear the workspace, all binary R objects and data models are cleared from the underlying R session workspace including those generated by code executions and those loaded into the workspace.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>If your user session times out, the underlying R session is released.</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>To clear the pane, workspace or working directory:</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>Click the arrow next to the <bpt id="p1">**</bpt>Clear<ept id="p1">**</ept> button in the <bpt id="p2">**</bpt>Debug Console Output<ept id="p2">**</ept> pane toolbar to see the <bpt id="p3">**</bpt>Clear<ept id="p3">**</ept> submenu options.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>Select one of the following options:</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Clear Pane<ept id="p1">**</ept> to clear the output visible on the pane without affecting on the underlying R session.</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Clear Workspace<ept id="p1">**</ept> to clear <bpt id="p2">**</bpt>all<ept id="p2">**</ept> binary R objects or models from the workspace on the underlying R session regardless of whether they were generated during code execution or loaded into the session.</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Clear Working Directory<ept id="p1">**</ept> to clear <bpt id="p2">**</bpt>all<ept id="p2">**</ept> files from the working directory on the underlying R session.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Clear Both<ept id="p1">**</ept> to clear all binary R objects from the workspace and all files from the working directory on the underlying R session.</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>Supplying Input Values</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source>There are two kinds of inputs to your script.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source>They are:</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source>The values for the <bpt id="p1">[</bpt><ph id="ph1">`deployrInput()`</ph><ept id="p1">](../deployr/deployr-data-scientist-write-portable-r-code.md)</ept> widgets</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>Primitive name-value pairs in the <bpt id="p1">**</bpt>Quick Inputs<ept id="p1">**</ept> field</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>Examples of deployrInput() widgets and Quick Inputs</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>To help you test your script, you can supply temporary input values in the <bpt id="p1">**</bpt>Script Execution Parameters<ept id="p1">**</ept> pane in the upper right.</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>You can then pass these values along during the next execution of your R script in this user session.</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>You can:</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Change any values displayed in the <ph id="ph1">`deployrInput()`</ph> widgets</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>Define some primitive values on-the-fly</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>Run<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#running-scripts-in-test-page)</ept> the entire script with the values and quick inputs shown in this pane</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>You can also <bpt id="p1">[</bpt>load data<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#loading-data-into-the-r-session)</ept> into the underlying R session to be used by any script.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>For example, you might create a model, save that in an .rData file, and then load it into the workspace so your script can use the model to score new data.</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>R Code Inputs (deployrInput)</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Any inputs defined in the R code using the deployrInput() function, and their default values, appear at the top in this pane.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>The default values defined in the R code are preselected here for you.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>You can change the value of an input here, run to test your code using the new value, and then evaluate the outcome.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>For tips and guidance on how to develop portable R code using this function from the deployrUtils package, see the <bpt id="p1">[</bpt>Writing Portable R Code<ept id="p1">](../deployr/deployr-data-scientist-write-portable-r-code.md)</ept> guide on the DeployR website.</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>Refer to the deployrUtils package help for more details and examples.</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>If you do not own this file and cannot see the R code in the <bpt id="p1">**</bpt>Source<ept id="p1">**</ept> pane, then the deployrInput() functions <bpt id="p2">[</bpt>cannot be rendered<ept id="p2">](../what-is-operationalization.md)</ept> either.</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>By default, if you can access this file in the Repository Manager, then you are permitted to see any <ph id="ph1">`deployrInput`</ph> widgets in this pane regardless of whether you own the file or not.</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>However, if you do not own this file but know there are <ph id="ph1">`deployrInput`</ph> declarations in the code and cannot see them here, it may be due a change in the server configuration <bpt id="p1">[</bpt>policies<ept id="p1">](../what-is-operationalization.md)</ept> by the DeployR administrator that prohibits the loading and downloading of files that may contain code into an R session.</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>Quick 'on-the-fly' Inputs</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>You can define some temporary basic inputs on-the-fly to help you test your script.</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>Only primitive values (real, integer, string) are accepted.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>To define one, enter each input as a comma-separated name-value pair in the <bpt id="p1">**</bpt>Quick Inputs<ept id="p1">**</ept> field.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>Each input is defined as a comma-separated, name-value pair using the following syntax:</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">**</bpt>Quick Inputs<ept id="p1">**</ept> field is designed to support primitive inputs, but not complex inputs.</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Quick Inputs<ept id="p1">**</ept> cannot be saved.</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>For those, we recommend defining them in your code using the deployrInput()function.</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Quick Inputs<ept id="p1">**</ept> cannot be saved with the script.</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>Retrieving R Objects</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>On the <bpt id="p1">**</bpt>Test<ept id="p1">**</ept> page, you can retrieve and inspect DeployR encoding for R objects in the underlying workspace.</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Since DeployR encodings are used to encode R object data on the DeployR API, the <bpt id="p1">**</bpt>R Objects<ept id="p1">**</ept> feature is of particular interest to client application developers.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>The following kinds of artifacts might be present after you execute code:</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>Unnamed and named <bpt id="p1">[</bpt>plots<ept id="p1">](deployr-repository-manager-testing-debugging-scripts.md#reviewing-execution-artifacts)</ept> from the R graphics device and non-image files that were written to the working directory</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>DeployR encodings of R objects from the workspace</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>You can use the <bpt id="p1">**</bpt>R Objects<ept id="p1">**</ept> field to request that R object(s) in the workspace be returned as a DeployR-encoded object(s) in the <bpt id="p2">[</bpt>response<ept id="p2">](deployr-repository-manager-testing-debugging-scripts.md#reviewing-execution-artifacts)</ept> markup.</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>To learn more about DeployR encoded objects, refer to the <bpt id="p1">[</bpt>DeployR API Reference Guide<ept id="p1">](../deployr/deployr-api-reference.md)</ept>.</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>The following is an example a DeployR encoding of an R vector object returned in the API Response tab of the Artifacts pane for the "workspace" property:</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>The type property indicates how you can decode the encapsulated data for use within his or her client application.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>To retrieve R objects from the workspace:</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>In the <bpt id="p1">**</bpt>Script Execution Parameters<ept id="p1">**</ept> pane, enter the name of an R object that is currently in your workspace or one you expect to be generated from the execution into the <bpt id="p2">**</bpt>R Objects<ept id="p2">**</ept> field.</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>Enter any additional R object names as a comma-separated list, such as</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>Run the script in this <bpt id="p1">**</bpt>Test<ept id="p1">**</ept> page.</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>Once the execution has completed, click <bpt id="p1">**</bpt>API Response<ept id="p1">**</ept> in the toolbar of the <bpt id="p2">**</bpt>Artifacts<ept id="p2">**</ept> pane.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>Search for the "workspace" property to find the DeployR encodings of the named objects in the response markup.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>You cannot save the list of object names you enter in the <bpt id="p1">**</bpt>R Objects<ept id="p1">**</ept> field.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>This is a temporary field used only to retrieve the DeployR encoding of one or more R objects on-the-fly.</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>Interrupting Code Executions</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>Whenever you run code from anywhere in the <bpt id="p1">**</bpt>Test<ept id="p1">**</ept> page, you can interrupt the execution of that code.</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>Since the console output is shown in the <bpt id="p1">**</bpt>Debug Console Output<ept id="p1">**</ept> pane, this is also where you can interrupt an execution in progress.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>To interrupt a code execution:</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>During an execution, find the red icon in the <bpt id="p1">**</bpt>Debug Console Output<ept id="p1">**</ept> pane toolbar.</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>Click the red icon on the toolbar to interrupt and terminate the execution.</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>Saving Script Changes</source>
        </trans-unit><trans-unit id="290" translate="yes" xml:space="preserve">
          <source>The changes you make to the source code of your own scripts in the Repository Manager are not saved automatically.</source>
        </trans-unit><trans-unit id="291" translate="yes" xml:space="preserve">
          <source>If you want to keep any of the changes you make in the <bpt id="p1">**</bpt>Source<ept id="p1">**</ept> pane, you must explicitly save them.</source>
        </trans-unit><trans-unit id="292" translate="yes" xml:space="preserve">
          <source>Changes you make in the <bpt id="p1">**</bpt>Script Execution Parameters<ept id="p1">**</ept> pane to test and debug your script are temporary and cannot be saved.</source>
        </trans-unit><trans-unit id="293" translate="yes" xml:space="preserve">
          <source>To save from the Source pane:</source>
        </trans-unit><trans-unit id="294" translate="yes" xml:space="preserve">
          <source>After you have made changes to the source code in the <bpt id="p1">**</bpt>Test<ept id="p1">**</ept> page, click <bpt id="p2">**</bpt>Save<ept id="p2">**</ept> in the <bpt id="p3">**</bpt>Source<ept id="p3">**</ept> pane toolbar.</source>
        </trans-unit><trans-unit id="295" translate="yes" xml:space="preserve">
          <source>In the submenu, choose one of the following:</source>
        </trans-unit><trans-unit id="296" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Overwrite Latest version<ept id="p1">**</ept> to replace in the current working copy of the script.</source>
        </trans-unit><trans-unit id="297" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Save as new version<ept id="p1">**</ept> to save the changes as the <bpt id="p2">[</bpt><bpt id="p3">*</bpt>Latest<ept id="p3">*</ept> version<ept id="p2">](deployr-repository-manager-files.md#working-with-historical-versions)</ept> with an optional comment, and to preserve what was previously the <bpt id="p4">*</bpt>Latest<ept id="p4">*</ept> version in the file's history.</source>
        </trans-unit><trans-unit id="298" translate="yes" xml:space="preserve">
          <source>on Windows/Linux or <ph id="ph1">`Command-S`</ph> on MAC will save and overwrite the <bpt id="p1">*</bpt>Latest<ept id="p1">*</ept> version.</source>
        </trans-unit></group></body></file></xliff>