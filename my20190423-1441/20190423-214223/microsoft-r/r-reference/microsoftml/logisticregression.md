<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="logisticregression.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86a25609456c367c5f198da022e8488362e3679b3b.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a25609456c367c5f198da022e8488362e3679b3b</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\logisticregression.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>logisticRegression function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Creates a list containing the function name and arguments to train a  logistic regression model with <bpt id="p1">[</bpt>rxEnsemble<ept id="p1">](rxEnsemble.md)</ept>.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), logisticRegression</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>logisticRegression: logisticRegression</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Creates a list containing the function name and arguments to train a logistic regression model with <bpt id="p1">[</bpt>rxEnsemble<ept id="p1">](rxEnsemble.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The L2 regularization weight.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Its value must be greater than  or equal to <ph id="ph1">`0`</ph> and the default value is set to <ph id="ph2">`1`</ph>.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The L1 regularization weight.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Its value must be greater than  or equal to <ph id="ph1">`0`</ph> and the default value is set to <ph id="ph2">`1`</ph>.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Threshold value for optimizer convergence.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>If the improvement between iterations is less than the threshold, the algorithm stops and returns the current model.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Smaller values are slower, but more accurate.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`1e-07`</ph>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Memory size for L-BFGS, specifying the number of past positions and gradients to store for the computation of the next step.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>This optimization parameter limits the amount of memory that is used to compute the magnitude and direction of the next step.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>When you specify less memory,  training is faster but less accurate.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Must be greater than or equal to  <ph id="ph1">`1`</ph> and the default value is <ph id="ph2">`20`</ph>.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Sets the initial weights diameter that specifies  the range from which values are drawn for the initial weights.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>These   weights are initialized randomly from within this range.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>For  example, if the diameter is specified to be <ph id="ph1">`d`</ph>, then the weights  are uniformly distributed between <ph id="ph2">`-d/2`</ph> and <ph id="ph3">`d/2`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`0`</ph>, which specifies that all the weights are  initialized to <ph id="ph2">`0`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Sets the maximum number of iterations.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>After this number  of steps, the algorithm stops even if it has not satisfied convergence criteria.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Specify <ph id="ph1">`TRUE`</ph> to show the statistics of  training data and the trained model; otherwise, <ph id="ph2">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The  default value is <ph id="ph1">`FALSE`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>For additional information about model  statistics, see <bpt id="p1">[</bpt>summary.mlModel<ept id="p1">](mlModel.md)</ept>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Set to a number greater than 0 to use Stochastic Gradient Descent (SGD) to find the initial parameters.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>A non-zero value  set specifies the tolerance SGD uses to determine convergence.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`0`</ph> specifying that SGD is not used.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The number of threads to use in training the model.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>This should be set to the number of cores on the machine.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Note that  L-BFGS multi-threading attempts to load dataset into memory.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>In case of out-of-memory issues, set <ph id="ph1">`trainThreads`</ph> to <ph id="ph2">`1`</ph> to turn off multi-threading.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> the number of threads to use is determined internally.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, forces densification of the internal optimization vectors.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`FALSE`</ph>, enables the logistic regression  optimizer use sparse or dense internal states as it finds appropriate.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Setting <ph id="ph1">`denseOptimizer`</ph> to <ph id="ph2">`TRUE`</ph> requires the internal  optimizer to use a dense internal state, which may help alleviate load  on the garbage collector for some varieties of larger problems.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Additional arguments.</source>
        </trans-unit></group></body></file></xliff>