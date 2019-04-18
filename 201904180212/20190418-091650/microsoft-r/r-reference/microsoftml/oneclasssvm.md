<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="oneclasssvm.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-d1654b2" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4c5ad3bbe3cc2fc6f76a2255a514a06b6319d060f.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">c5ad3bbe3cc2fc6f76a2255a514a06b6319d060f</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">31942184-1832-4cbe-8e07-924efec046b4</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/18/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\oneclasssvm.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>oneClassSvm function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Creates a list containing the function name and arguments to train a  OneClassSvm model with <bpt id="p1">[</bpt>rxEnsemble<ept id="p1">](rxEnsemble.md)</ept>.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), oneClassSvm</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>oneClassSvm: oneClassSvm</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Creates a list containing the function name and arguments to train a OneClassSvm model with <bpt id="p1">[</bpt>rxEnsemble<ept id="p1">](rxEnsemble.md)</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The maximal size in MB of the cache that stores the training data.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Increase this for large training sets.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>The default value is 100 MB.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>A character string representing the kernel used for computing inner products.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>For more information, see <bpt id="p1">[</bpt>maKernel<ept id="p1">](kernel.md)</ept>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The following choices are available:</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`rbfKernel()`</ph>: Radial basis function kernel.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Its parameter  represents<ph id="ph1">`gamma`</ph> in the term <ph id="ph2">`exp(-gamma|x-y|^2`</ph>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>If not  specified, it defaults to <ph id="ph1">`1`</ph> divided by the number of features used.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`rbfKernel(gamma = .1)`</ph>.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>This is the default value.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`linearKernel()`</ph>: Linear kernel.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`polynomialKernel()`</ph>: Polynomial kernel with parameter names <ph id="ph2">`a`</ph>,  <ph id="ph3">`bias`</ph>, and <ph id="ph4">`deg`</ph> in the term <ph id="ph5">`(a*&lt;x,y&gt; + bias)^deg`</ph>.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The  <ph id="ph1">`bias`</ph>, defaults to <ph id="ph2">`0`</ph>.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The degree, <ph id="ph1">`deg`</ph>, defaults to  <ph id="ph2">`3`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`a`</ph> is not specified, it is set to <ph id="ph2">`1`</ph> divided by the number of features.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>For example, <ph id="ph1">`maKernelPoynomial(bias = 0, deg = ``  3)`</ph>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`sigmoidKernel()`</ph>: Sigmoid kernel with parameter names  <ph id="ph2">`gamma`</ph> and <ph id="ph3">`coef0`</ph> in the term <ph id="ph4">`tanh(gamma*&lt;x,y&gt; + coef0)`</ph>.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source><ph id="ph1">`gamma`</ph>, defaults to <ph id="ph2">`1`</ph> divided by the number of features.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>The  parameter <ph id="ph1">`coef0`</ph> defaults to <ph id="ph2">`0`</ph>.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>For example,  <ph id="ph1">`sigmoidKernel(gamma = .1, coef0 = 0)`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The threshold for optimizer convergence.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>If the  improvement between iterations is less than the threshold, the algorithm  stops and returns the current model.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>The value must be greater than or equal to <ph id="ph1">`.Machine$double.eps`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The default value is 0.001.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The trade-off between the fraction of outliers and the number of support vectors (represented by the Greek letter nu).</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Must be between 0 and 1, typically between 0.1 and 0.5.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>The default value is 0.1.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Uses the shrinking heuristic if <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>In this case, some samples will be "shrunk" during the training procedure, which may speed up training.</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`TRUE`</ph>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Additional arguments to be passed directly to the Microsoft Compute Engine.</source>
        </trans-unit></group></body></file></xliff>