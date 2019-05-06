<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="prune.rxDTree.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc77502b448dad1fc478ee3a73d0d5d33c272625c9a88b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">2b448dad1fc478ee3a73d0d5d33c272625c9a88b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\prune.rxDTree.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>prune.rxDTree function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Prune a decision tree created by rxDTree and return the smaller tree.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), prune.rxDTree, models, tree, classif, regression</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>prune.rxDTree: Pruning an rxDTree Decision Tree</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Prune a decision tree created by <ph id="ph1">`rxDTree`</ph> and return the smaller tree.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>object returned from a call to <ph id="ph1">`rxDTree`</ph>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>a complexity parameter specifying the complexity at which to prune the tree.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Generally, you should examine the <ph id="ph1">`cptable`</ph> component of the <ph id="ph2">`tree`</ph> object to determine a suitable value for <ph id="ph3">`cp`</ph>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed to other methods.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>(There are, in fact, no other methods called by <ph id="ph1">`prune.rxDTree`</ph>.)</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`prune.rxDTree`</ph> function can be used as a <ph id="ph2">`prune`</ph> method for objects of class <ph id="ph3">`rxDTree`</ph>, provided the <bpt id="p1">**</bpt>rpart<ept id="p1">**</ept> package is attached prior to attaching <bpt id="p2">**</bpt>RevoScaleR<ept id="p2">**</ept>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>an object of class <ph id="ph1">`"rxDTree"`</ph> representing the pruned tree.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>It is a list with components similar to those of class <ph id="ph1">`"rpart"`</ph> with the following distinctions:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>-  A vector of integers indicating the node to which each point is allocated.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>This information is always returned if the data source is a data frame.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>If the data source is not a data frame and <ph id="ph1">`outFile`</ph> is specified that is, not <ph id="ph2">`NULL`</ph>, the node indices are written/appended to the specified file with a column name as defined by <ph id="ph3">`outColName`</ph>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>For other components, see rpart.object for details.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Breiman, L., Friedman, J. H., Olshen, R. A.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>and Stone, C. J.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>(1984) <bpt id="p1">*</bpt>Classification and Regression Trees<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Wadsworth.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Therneau, T. M.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>and Atkinson, E. J.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>(2011) <bpt id="p1">*</bpt>An Introduction to Recursive Partitioning Using the RPART Routines<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Yael Ben-Haim and Elad Tom-Tov (2010) A streaming parallel decision tree algorithm.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>Journal of Machine Learning Research<ept id="p1">*</ept> <bpt id="p2">**</bpt>11<ept id="p2">**</ept>, 849--872.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>rpart, rpart.control, rpart.object.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>