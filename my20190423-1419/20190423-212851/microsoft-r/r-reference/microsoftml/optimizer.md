<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="optimizer.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338ad0a29fc26ed1559b9bde3264021ade601a86b44d.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d0a29fc26ed1559b9bde3264021ade601a86b44d</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\microsoftml\optimizer.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>maOptimizer function (MicrosoftML)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Specifies Optimization Algorithms for Neural Net.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(MicrosoftML), maOptimizer, adaDeltaSgd, sgd, optimizer</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>maOptimizer: Optimization Algorithms</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Specifies Optimization Algorithms for Neural Net.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>Specifies the decay rate applied to gradients when calculating the step in the ADADELTA adaptive optimization algorithm.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>This rate is used  to ensure that the learning rate continues to make progress by giving smaller weights to remote gradients in the calculation of the step size.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Mathematically, it replaces the mean square of the gradients with an exponentially decaying  average of the squared gradients in the denominator of the update rule.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The  value assigned must be in the range (0,1).</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>Specifies a conditioning constant for the ADADELTA  adaptive optimization algorithm that is used to condition the step size in   regions where the exponentially decaying average of the squared gradients  is small.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The value assigned must be in the range (0,1).</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Specifies the size of the step taken in the direction of the negative gradient for each iteration of the learning process.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>The default value is <ph id="ph1">`= 0.001`</ph>.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Specifies weights for each dimension that control the contribution of the previous step to the size of the next step during  training.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>This modifies the <ph id="ph1">`learningRate`</ph> to speed up training.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The value must be <ph id="ph1">`&gt;= 0`</ph> and <ph id="ph2">`&lt; 1`</ph>.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, Nesterov's Accelerated Gradient Descent is used.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>This method reduces the oracle complexity of gradient descent and is optimal  for smooth convex optimization.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Specifies the scaling weights for the step size.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>After  each weight update, the weights in the network are scaled by <ph id="ph1">`(1 -  ``learningRate * weightDecay)`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>The value must be <ph id="ph1">`&gt;= 0`</ph> and <ph id="ph2">`&lt; 1`</ph>.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Specifies the learning rate reduction ratio: the ratio by which the learning rate is reduced during training.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Reducing the learning rate can avoid local minima.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The value must be <ph id="ph1">`&gt; 0`</ph> and <ph id="ph2">`&lt;= 1`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>A value of <ph id="ph1">`1.0`</ph> means no reduction.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>A value of <ph id="ph1">`0.9`</ph> means the learning rate is reduced to 90  its current value.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The reduction can be triggered either periodically, to occur after a fixed   number of iterations, or when a certain error criteria concerning increases  or decreases in the loss function are satisfied.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>To trigger a periodic rate reduction, specify the frequency  by setting the number of iterations between reductions with the  <ph id="ph1">`lRateRedFreq`</ph> argument.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>To trigger rate reduction based on an error criterion, specify a number   in <ph id="ph1">`lRateRedErrorRatio`</ph>.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>Sets the learning rate reduction frequency by specifying  number of iterations between reductions.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>For example, if <ph id="ph1">`10`</ph> is  specified, the learning rate is reduced once every 10 iterations.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>Specifies the learning rate reduction error criterion.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>If set to <ph id="ph1">`0`</ph>, the learning rate is reduced if the loss increases between iterations.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>If set to a fractional value greater than<ph id="ph1">`0`</ph>, the learning rate is reduced if the loss decreases by less than that fraction of its previous value.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>These functions can be used for the <ph id="ph1">`optimizer`</ph> argument in <bpt id="p1">[</bpt>rxNeuralNet<ept id="p1">](rxNeuralNet.md)</ept>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`sgd`</ph> function specifies Stochastic Gradient Descent.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>maOptimizer</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`adaDeltaSgd`</ph> function specifies the AdaDelta gradient descent, described in the 2012 paper "ADADELTA: An Adaptive Learning Rate Method" by Matthew D.Zeiler.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>A character string that contains the specification for the optimization algorithm.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxNeuralNet<ept id="p1">](rxNeuralNet.md)</ept>,</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>