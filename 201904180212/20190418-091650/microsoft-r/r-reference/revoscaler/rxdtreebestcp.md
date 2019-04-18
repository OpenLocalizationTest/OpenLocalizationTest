<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxdtreebestcp.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b44650479640720bf484e17d0240b8be6828b9b19e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">4650479640720bf484e17d0240b8be6828b9b19e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxdtreebestcp.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxDTreeBestCp function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Attempts to find the cp for optimal model pruning, where optimal is defined by default in terms of the 1 Standard Error criterion of Breiman, et al.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxDTreeBestCp, models, tree, classif, regression</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxDTreeBestCp:  Find the Best Value of cp for Pruning rxDTree Object</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Attempts to find the cp for optimal model pruning, where optimal is defined by default in terms of the 1 Standard Error criterion of Breiman, et al.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>an object of class <ph id="ph1">`rxDTree`</ph>.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>number of standard errors of cross-validation error to define optimality.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The default, 1, causes <ph id="ph1">`rxDTreeBestCp`</ph> to find the simplest model within one standard error of the minimum cross-validation error.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`rxDTreeBestCp`</ph> function is intended to help automate the <ph id="ph2">`rxDTree`</ph> model fitting function, by applying the 1 Standard Error Criterion of Breiman, et al., to a fitted <ph id="ph3">`rxDTree`</ph> object.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Using the <ph id="ph1">`pruneCp="auto"`</ph> option in <ph id="ph2">`rxDTree`</ph> causes <ph id="ph3">`rxDTreeBestCp`</ph> to be called on the fitted model and the result of that computation supplied as the argument to <ph id="ph4">`prune.rxDTree`</ph>, thus allowing the model to be fitted and pruned in a single call.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>a numeric scalar.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Breiman, L., Friedman, J. H., Olshen, R. A.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>and Stone, C. J.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>(1984) <bpt id="p1">*</bpt>Classification and Regression Trees<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Wadsworth.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxDTree<ept id="p1">](rxDTree.md)</ept>, <bpt id="p2">[</bpt>prune.rxDTree<ept id="p2">](prune.rxDTree.md)</ept>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>