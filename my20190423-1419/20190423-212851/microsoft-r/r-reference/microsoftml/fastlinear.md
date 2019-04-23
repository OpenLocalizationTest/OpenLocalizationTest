<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="fastlinear.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338aa48d4947a69bc98cbb73a7c7a202b51673c7792d.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a48d4947a69bc98cbb73a7c7a202b51673c7792d</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\fastlinear.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>fastLinear function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Creates a list containing the function name and arguments to train a  Fast Linear model with <bpt id="p1">[</bpt>rxEnsemble<ept id="p1">](rxEnsemble.md)</ept>.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), fastLinear</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>fastLinear: fastLinear</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Creates a list containing the function name and arguments to train a Fast Linear model with <bpt id="p1">[</bpt>rxEnsemble<ept id="p1">](rxEnsemble.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Specifies the empirical loss function to optimize.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>For binary classification, the following choices are available:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>logLoss<ept id="p1">](loss.md)</ept>: The log-loss.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>This is the default.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>hingeLoss<ept id="p1">](loss.md)</ept>: The SVM hinge loss.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Its parameter represents the margin size.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>smoothHingeLoss<ept id="p1">](loss.md)</ept>: The smoothed hinge loss.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Its parameter represents the smoothing constant.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>For linear regression, squared loss <bpt id="p1">[</bpt>squaredLoss<ept id="p1">](loss.md)</ept> is currently supported.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>When this parameter is set to <ph id="ph1">`NULL`</ph>, its default value depends on the type of learning:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>logLoss<ept id="p1">](loss.md)</ept> for binary classification.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>squaredLoss<ept id="p1">](loss.md)</ept> for linear regression.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Specifies the L2 regularization weight.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The value must be either non-negative or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> is specified, the  actual value is automatically computed based on data set.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>is the default value.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Specifies the L1 regularization weight.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The value must be either non-negative or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> is specified, the  actual value is automatically computed based on data set.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>is the default value.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Specifies how many concurrent threads can be used to run the algorithm.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>When this parameter is set to <ph id="ph1">`NULL`</ph>, the number of threads used is determined based on the number of logical processors available to the process as well as the sparsity of data.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Set it to <ph id="ph1">`1`</ph> to run the algorithm in a single thread.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Specifies the tolerance threshold used as a  convergence criterion.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>It must be between 0 and 1.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`0.1`</ph>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The algorithm is considered to have converged if the relative  duality gap, which is the ratio between the duality gap and the primal loss,  falls below the specified convergence tolerance.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Specifies an upper bound on the number of training iterations.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>This parameter must be positive or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph> is specified, the actual value is automatically computed based on data set.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Each iteration requires a complete pass over the training data.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Training  terminates after the total number of iterations reaches the specified   upper bound or when the loss function converges, whichever happens earlier.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Specifies whether to shuffle the training data.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Set <ph id="ph1">`TRUE`</ph> to shuffle the data; <ph id="ph2">`FALSE`</ph> not to shuffle.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>SDCA is a stochastic optimization algorithm.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>If shuffling is turned on, the training data is shuffled on each iteration.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>The number of iterations after which the loss function is computed and checked to determine whether it has converged.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>The value  specified must be a positive integer or <ph id="ph1">`NULL`</ph>.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`NULL`</ph>, the actual value is automatically computed based on data set.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Otherwise,  for example, if <ph id="ph1">`checkFrequency = 5`</ph> is specified, then the loss function is computed and convergence is checked every 5 iterations.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The computation of the loss function requires a separate complete pass over the training data.</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Additional arguments.</source>
        </trans-unit></group></body></file></xliff>