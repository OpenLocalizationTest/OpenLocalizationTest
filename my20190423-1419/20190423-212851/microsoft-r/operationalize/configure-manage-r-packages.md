<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="configure-manage-r-packages.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338acae2420f743281fb6c20bb03c25b2a9e77f9a2b8.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">cae2420f743281fb6c20bb03c25b2a9e77f9a2b8</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\operationalize\configure-manage-r-packages.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Package Management when operationalizing - Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>R Package Management with Machine Learning Server</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>R package management when operationalizing analytics with Machine Learning Server</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Applies to:  Machine Learning Server, Microsoft R Server 9.x</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>One of the strengths of the R language is the thousands of third-party packages that have been made publicly available via CRAN, the Comprehensive R Archive Network.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>R includes various functions that make it easy to download and install these packages.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Whenever you deploy an R script, the packages (and their dependencies) needed by that R code must be available at runtime, or else the execution fails.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>By adopting the R package management approaches discussed herein, data scientists can avoid issues such as a locally tested script tested failing due to missing package dependencies in the remote environment.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>As the Machine Learning Server administrator, you must ensure that the R code running on any compute nodes has access to the R package dependencies declared within that code.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The right set of R package versions must be installed for the organization and accessible to all users.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>However, in many enterprise environments, access to the Internet is limited or non-existent.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>In such environments, it is useful to create a local package repository that users can access from within the corporate firewall using <bpt id="p1">[</bpt>Option 1<ept id="p1">](#offline)</ept>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>You can also manually install the packages using a master script using <bpt id="p1">[</bpt>Option 2<ept id="p1">](#master)</ept>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Data scientists can also test out packages without risk to the production environment using <bpt id="p1">[</bpt>the mrsdeploy package option (3)<ept id="p1">](#mrsdeploy)</ept>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Option 1: Local Package Repository (Offline Solution)</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Audience:<ept id="p1">**</ept> System administrator</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:<ept id="p1">**</ept> Development -or- Production Environments</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>You can create a local R package repository of the R packages you need using the R package <ph id="ph1">`miniCRAN`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>You can then copy this repository to all compute nodes and then install directly from this repository.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>This production-safe approach provides an excellent way to:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Keep a standard, sanctioned library of R packages for production use</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Allow packages to be installed in an offline environment</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>To use the miniCRAN method:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>On the machine with Internet access:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Launch your preferred R IDE or an R tool such as Rgui.exe.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>At the R prompt, install the <ph id="ph1">`miniCRAN`</ph> package on a computer that has Internet access.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>To point to a different snapshot, set the <ph id="ph1">`CRAN_mirror`</ph> value.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>By default, the CRAN mirror specified by your version of Microsoft R Open is used.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>For example, for Machine Learning Server 9.2.1 that date is 2017-09-01.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Create a miniCRAN repository in which the packages are downloaded and installed.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>This repository creates the folder structure that you need to copy the packages to each compute node later.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Download and install the packages you need to this computer.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>If you aren't sure which packages to list, consider using a list of the top “n” (e.g. 500) packages by download/popularity as a starting point.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Then, extend with additional packages as needed over time.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>For Mac and Windows binaries, it is possible to look at the particular bin/contrib repo you’re interested in, for example: <ph id="ph1">https://cran.microsoft.com/snapshot/2018-01-16/bin/windows/contrib/3.4/PACKAGES</ph></source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>It is also possible to <bpt id="p1">[</bpt>create your own mirror<ept id="p1">](https://cran.r-project.org/mirror-howto.html)</ept> to get ALL packages instead of using miniCRAN; however, this would be very large and grow stale quickly requiring regular updates.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>On each compute node:</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Copy the miniCRAN repository from the machine with Internet connectivity to the R_SERVICES library on the SQL Server instance.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Launch your preferred R IDE or an R tool such as Rgui.exe.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>At the R prompt, run the R command install.packages().</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>At the prompt, specify a repository and specify the directory containing the files you copied.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>That is, the local miniCRAN repository.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Run the following R command and reviewing the list of installed packages:</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Option 2: R Script with List of Approved Packages</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Audience:<ept id="p1">**</ept> System administrator</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:<ept id="p1">**</ept> Development -or- Production Environments</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>As we mentioned before, it is imperative that the right set of R package versions are installed and accessible to all users.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Option 2 makes use of a master R script containing the list of specific package versions to install across the configuration on behalf of your users.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Using a master script ensures that the same packages (along with all its required package dependency) are installed each time.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>To produce the list of packages, consider which R packages (and versions) are needed and sanctioned for production.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Also consider requests from users to add new R packages or update package versions.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>This production-safe approach provides an excellent way to</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Keep a standard (and sanctioned) library of R packages for production use.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Manage R package dependencies and package versions.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Schedule timely updates to R packages.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>This option does require the  machines hosting the compute node have access to the Internet to install the packages.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>To use a master script to install packages:</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Create the master list of packages (and versions) in an R script format.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>For example:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Manually run this R script on each compute node.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Update and manually rerun this script on each compute node each time a new package or version is needed in the server environment.</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Option 3: Remote Session Testing</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Audience:<ept id="p1">**</ept> Data Scientist or the system administrator</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Applies to:<ept id="p1">**</ept> Development Environments</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>To avoid issues where a locally tested script fails in the Machine Learning Server environment due to missing package dependencies, install the R packages into the workspace of a remote R session yourself.</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>This remote execution and snapshot approach provides an excellent way to:</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Try out new package or package versions without posing any risks to a stable production environment</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Install packages without requiring any intervention from the administrator</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>The packages you install using this method do not 'contaminate' the production environment for other users since they are only available in the context of the given R session.</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Those packages remain installed for the lifecycle of the R session.</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>You can prolong this lifecycle by saving the session workspace and working directory into a <bpt id="p1">**</bpt>snapshot<ept id="p1">**</ept>.</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Then, whenever you want to access the workspace, the installed R packages, and the working directory files as they were, you can recall the snapshot using its ID.</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Learn more about snapshots and remote execution...</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>For optimal performance, consider the size of the snapshot carefully especially when publishing a service.</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Before creating a snapshot, ensure that keep only those workspace objects you need and purge the rest.</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>Note:<ept id="p1">**</ept> After you've sufficiently tested the packages as described in this section, you can request that the administrator install a package across the configuration for all users.</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>To install packages within an R session:</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Develop and test your code locally.</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Load the mrsdeploy package.</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Authenticate to create the remote session.</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Learn more about the authentication functions and their arguments in the article: "<bpt id="p1">[</bpt>Connecting to Machine Learning Server from mrsdeploy<ept id="p1">](how-to-connect-log-in-with-mrsdeploy.md)</ept>.</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>"</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>For example, for Azure Active Directory:</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>For example, for Active Directory/LDAP:</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>A new remote session is started.</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Run R code in the remote environment:</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Install new R packages and upload any needed R objects and files into the remote R session.</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Pause the remote session and execute your R scripts to test the code and newly installed packages in the remote environment.</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>To allow the workspace and working directory to be reused later, create a session snapshot.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>A snapshot is a prepared environment image of an R session saved to Machine Learning Server, which includes the session's R packages, R objects and data files.</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>This snapshot can be loaded into any subsequent remote R session for the user who created it.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>Learn more about snapshots.</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>Take note of the <ph id="ph1">`snapshotId`</ph> to call this snapshot later.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>To reuse those installed packages, objects and files:</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>You can reload the snapshot (installed packages, objects, files) within the context of a remote session.</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>You can ask your administrator to install a package across the configuration for all users once you've sufficiently tested the package as described in this section.</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>R Server 9.0 users!</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>When loading a library for the REMOTE session, set lib.loc=getwd() as such:</source>
        </trans-unit></group></body></file></xliff>