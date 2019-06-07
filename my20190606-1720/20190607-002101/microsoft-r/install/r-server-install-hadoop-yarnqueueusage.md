<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="r-server-install-hadoop-yarnqueueusage.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37fc68f3c9eeb41ac5f1d22e381c4d360286dfec2c.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">fc68f3c9eeb41ac5f1d22e381c4d360286dfec2c</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\install\r-server-install-hadoop-yarnqueueusage.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Enforcing YARN Queue Usage (Microsoft R Server for Hadoop)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Enforce YARN queue usage for a  Microsoft R Server installation on a Hadoop cluster.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Enforcing YARN queue usage</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>R Server tasks running on Spark or MapReduce can be managed through use of YARN job queues.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>To direct a job to a specific queue, the end user must include the queue name in the MapReduce or Spark Compute Context.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>MapReduce</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Use the "hadoopSwitches" option to direct jobs to a specific YARN queue.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Spark</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Use the "extraSparkConfig" option to direct jobs to a specific YARN queue.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Overrides</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Use of a specific queue can be enforced by the Hadoop system administrator by providing an installation override to the <ph id="ph1">`RxSpark()`</ph>, <ph id="ph2">`RxSparkConnect()`</ph>, and <ph id="ph3">`RxHadoopMR()`</ph> compute context functions.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>A benefit is that you no longer have to explicitly specify the queue.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>This procedure involves creating a custom R package that contains the function overrides, installing that package on the nodes in use by end users, and adding the package to the default search path on these nodes.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The following code block provides an example.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If you use this code as a template, remember to change the ‘mrsjobs’ YARN queue name to the queue name that's valid for your system.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Create a new R package, such as “abcMods” if your company abbreviation is ‘abc’, by installing the “devtools” package and running the following command, or use the <ph id="ph1">`package.skeleton()`</ph> function in base R.  To learn more about creating R packages, see <bpt id="p1">[</bpt>Writing R Extensions<ept id="p1">](https://cran.r-project.org/doc/manuals/r-release/R-exts.html)</ept> on the CRAN website, or <bpt id="p2">[</bpt>online version of R Packages<ept id="p2">](http://r-pkgs.had.co.nz/)</ept> from Hadley Wickham.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>This creates the essential package files in the requested directory, in this case ‘/dev/abcMods’.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Edit each of the following to fill in the relevant info.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>DESCRIPTION – text file containing the description of the R package:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>NAMESPACE – text file containing the list of overridden functions to be exported:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>LICENSE – create a text file named ‘LICENSE’ in the package directory with a single line for the license associated with the R package:</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>In the package’s R directory add one or more <ph id="ph1">`*.R`</ph> files with the code for the functions to be overridden.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The following sample code provides for overriding <ph id="ph1">`RxHadoopMR`</ph>, <ph id="ph2">`RxSpark`</ph>, and <ph id="ph3">`RxSparkConnect`</ph> that you might save to a file called "ccOverrides.r" in that directory.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`RxSparkConnect`</ph> function is only available in V9 and later releases.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>After editing the previous components of the package, run the following Linux commands to build the package from the directory containing the <bpt id="p1">**</bpt>abcMods<ept id="p1">**</ept> directory:</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If you need to build the package for users on Windows, then the equivalent commands would be as follows where ‘rpath’ is defined to point to the version of R Server to which you’d like to add the library.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>To test it, start R, load the library, and make a call to <ph id="ph1">`RxHadoopMR()`</ph>:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>You should see the result come back with the queue name set to your override value (for example, <ph id="ph1">`Dmapreduce.job.queuename=mrsjobs)`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>To automate the loading of the package so that users don’t need to specify "library(abcMods)", edit Rprofile.site and modify the line specifying the default packages to include <bpt id="p1">**</bpt>abcMods<ept id="p1">**</ept> as the last item:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Once everything tests out to your satisfaction, install the package on all the edge nodes that your users are logging in to.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>To do this, copy "Rprofile.site" and R’s library/abcMods directory to each of these nodes, or install the package from the abcmods_0.1-0 tar file on each node and manually edit the "Rprofile.site" file on each node.</source>
        </trans-unit></group></body></file></xliff>