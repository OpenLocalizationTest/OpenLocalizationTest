<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="neuralnet.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3638e4fdd3487283232160b460c26098992417eea.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">638e4fdd3487283232160b460c26098992417eea</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\neuralnet.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>neuralNet function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Creates a list containing the function name and arguments to train a  NeuralNet model with <bpt id="p1">[</bpt>rxEnsemble<ept id="p1">](rxEnsemble.md)</ept>.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), neuralNet</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>neuralNet: neuralNet</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Creates a list containing the function name and arguments to train a NeuralNet model with <bpt id="p1">[</bpt>rxEnsemble<ept id="p1">](rxEnsemble.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The default number of hidden nodes in the neural net.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>The default value is 100.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The number of iterations on the full training set.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The default value is 100.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>A list specifying either the <ph id="ph1">`sgd`</ph> or <ph id="ph2">`adaptive`</ph> optimization algorithm.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>This list can be created using <bpt id="p1">[</bpt>sgd<ept id="p1">](optimizer.md)</ept> or <bpt id="p2">[</bpt>adaDeltaSgd<ept id="p2">](optimizer.md)</ept>.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`sgd`</ph>.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The Net# definition of the structure of the neural network.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>For more information about the Net# language, see   <bpt id="p1">[</bpt><ph id="ph1">`Reference Guide`</ph><ept id="p1">](https://azure.microsoft.com/en-us/documentation/articles/machine-learning-azure-ml-netsharp-reference-guide/)</ept></source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>Sets the initial weights diameter that specifies  the range from which values are drawn for the initial learning weights.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The weights are initialized randomly from within this range.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The default value is 0.1.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Specifies an upper bound to constrain the norm of the incoming  weight vector at each hidden unit.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>This can be very important in maxout  neural networks as well as in cases where training produces unbounded weights.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>Specifies the type of hardware acceleration to use.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Possible values are "sse" and "gpu".</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>For GPU acceleration, it is recommended to use a miniBatchSize greater than one.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If you want to use the GPU acceleration, there are additional manual setup steps are required:</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Download and install NVidia CUDA Toolkit 6.5  (<bpt id="p1">[</bpt><ph id="ph1">`CUDA Toolkit`</ph><ept id="p1">](https://developer.nvidia.com/cuda-toolkit-65)</ept> ).</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Download and install NVidia cuDNN v2 Library  (<bpt id="p1">[</bpt><ph id="ph1">`cudnn Library`</ph><ept id="p1">](https://developer.nvidia.com/rdp/cudnn-archive)</ept> ).</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Find the libs directory of the MicrosoftRML package by calling <ph id="ph1">`system.file("mxLibs/x64", package = "MicrosoftML")`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Copy cublas64_65.dll, cudart64_65.dll and cusparse64_65.dll from the CUDA Toolkit 6.5 into the libs directory of the MicrosoftML package.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Copy cudnn64_65.dll from the cuDNN v2 Library into the libs directory of the MicrosoftML package.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Sets the mini-batch size.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Recommended values are between  1 and 256.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>This parameter is only used when the acceleration is GPU.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Setting  this parameter to a higher value improves the speed of training, but it might negatively affect the accuracy.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The default value is 1.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Additional arguments.</source>
        </trans-unit></group></body></file></xliff>