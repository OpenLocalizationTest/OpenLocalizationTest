<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="fasttrees.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f61c5771a6385ea1b791ea6c0e729f2192ddd9c22.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">61c5771a6385ea1b791ea6c0e729f2192ddd9c22</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">be8355a1-d8a7-4fc6-930e-f4b604fa907f</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\fasttrees.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>fastTrees function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Creates a list containing the function name and arguments to train a  FastTree model with <bpt id="p1">[</bpt>rxEnsemble<ept id="p1">](rxEnsemble.md)</ept>.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), fastTrees</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>fastTrees: fastTrees</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Creates a list containing the function name and arguments to train a FastTree model with <bpt id="p1">[</bpt>rxEnsemble<ept id="p1">](rxEnsemble.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Specifies the total number of decision trees to create in  the ensemble.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>By creating more decision trees, you can potentially get  better coverage, but the training time increases.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The default value is 100.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The maximum number of leaves (terminal nodes) that can be created in any tree.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Higher values potentially increase the size of the tree and get better precision, but risk overfitting and requiring longer training times.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The default value is 20.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Determines the size of the step taken in the direction of the gradient in each step of the learning process.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>This determines how fast or slow the learner converges on the optimal solution.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If the step size is too big, you might overshoot the optimal solution.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>If the step size is too small, training takes longer to converge to the best solution.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Minimum number of training instances required to form a leaf.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>That is, the minimal number of documents allowed in a leaf of a regression tree, out of the sub-sampled data.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>A 'split' means that features in each level of the tree (node) are randomly divided.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The default value is  10.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Only the number of instances is counted even if instances are weighted.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The fraction of randomly chosen instances to use for each tree.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The default value is 0.7.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The fraction of randomly chosen features to use for each tree.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The default value is 1.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The fraction of randomly chosen features to use on each split.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The default value is 1.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Maximum number of distinct values (bins) per feature.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>If the feature has fewer values than the number indicated, each value is placed  in its own bin.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>If there are more values, the algorithm creates  <ph id="ph1">`numBins`</ph> bins.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The feature first use penalty coefficient.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>This is a form of regularization that incurs a penalty for using a new feature when creating the tree.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Increase this value to create trees that don't use many features.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The default value is 0.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Tree fitting gain confidence requirement (should be in the range [0,1)).</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The default value is 0.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, derivatives optimized for unbalanced sets are used.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Only applicable when <ph id="ph1">`type`</ph> equal to <ph id="ph2">`"binary"`</ph>.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The number of threads to use in training.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The default  value is 8.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Specifies the random seed.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Additional arguments.</source>
        </trans-unit></group></body></file></xliff>