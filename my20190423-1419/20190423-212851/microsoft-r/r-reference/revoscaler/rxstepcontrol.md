<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxstepcontrol.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a5c1ee7def7f3279842e58d9e47e84cb145e6378e.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5c1ee7def7f3279842e58d9e47e84cb145e6378e</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxstepcontrol.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxStepControl function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxStepControl, models, classification, regression</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>rxStepControl: Control for Stepwise Regression</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Various parameters that control aspects of stepwise regression.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>a character string specifying the method of stepwise search:</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>"stepwise": bi-directional search.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>"backward": backward elimination.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>"forward": forward selection.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Default is "stepwise" if the scope argument is not missing, otherwise "backward".</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>either a single formula, or a named list containing components upper and lower, both formulae, defining the range of models to be examined in the stepwise search.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>an integer specifying the maximum number of steps to be considered, typically used to stop the process early and the default is 1000.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>a character string specifying the variable selection criterion:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>"AIC": Akaike's information criterion.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>"SigLevel": significance level, the traditional stepwise approach in SAS.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>This argument is similar to the SELECT option of the GLMSELECT procedure in SAS.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Default is "AIC".</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>a numeric scalar specifying the significance level for adding a variable to the model.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>This argument is used only when stepCriterion = "SigLevel" and  is similar to the SLENTRY option of the GLMSELECT procedure in SAS.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>The defaults are 0.50 for "forward" and 0.15 for "stepwise".</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>a numeric scalar specifying the significance level for dropping a variable from the model.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>This argument is used only when stepCriterion = "SigLevel" and  is similar to the SLSTAY option of the GLMSELECT procedure in SAS.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>The defaults are 0.10 for "backward" and 0.15 for "stepwise".</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>a logical flag specifying whether or not to refit the model at each step.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The default is <ph id="ph1">`NULL`</ph>,  indicating to refit the model at each step for <ph id="ph2">`rxLogit`</ph> and <ph id="ph3">`rxGlm`</ph> but not for <ph id="ph4">`rxLinMod`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>a logical flag specifying whether or not to keep the model coefficients at each step.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`TRUE`</ph>, a data.frame <ph id="ph2">`stepCoefs`</ph> will be returned with the fitted model with rows corresponding to the coefficients and columns corresponding to the iterations.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Additional computation may be required to generate the coefficients at each step.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Those stepwise coefficients can be visualized by plotting the fitted model with <bpt id="p1">[</bpt>rxStepPlot<ept id="p1">](rxStepPlot.md)</ept>.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>optional numeric scalar specifying the scale parameter of the model.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>It is used in computing the AIC statistics for selecting the models.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>The default 0 indicates it should be estimated by maximum likelihood.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>See "scale" in step for details.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>optional numeric scalar specifying the weight of the number of  equivalent degrees of freedom in computing AIC for the penalty.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>See "k" in step for details.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>a character string specifying the test statistic to be included in the results, either "F" or "Chisq".</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Both test statistics are relative to the original model.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>additional arguments to be passed directly to the Microsoft R Services Compute Engine.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Stepwise models must be computed on the same dataset in order to be compared so rows with missing values in any of the variables in the upper model are removed before the model fitting starts.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Consequently, the stepwise models might be different from the corresponding models fitted with only the selected variables if there are missing values in the data set.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>When computing stepwise models with <ph id="ph1">`rxLogit`</ph> or <ph id="ph2">`rxGlm`</ph>, you can sometimes improve the speed and quality of the fitting by setting <ph id="ph3">`returnAlways=TRUE`</ph> in the initial <ph id="ph4">`rxLogit`</ph> or <ph id="ph5">`rxGlm`</ph> call.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>When <ph id="ph1">`returnAlways=TRUE`</ph>, <ph id="ph2">`rxLogit`</ph> and <ph id="ph3">`rxGlm`</ph> always return the solution tried so far that has the minimum deviance.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>A list containing the options.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>References</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Venables, W. N.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>and Ripley, B. D.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>(2002) <bpt id="p1">*</bpt>Modern Applied Statistics with S<ept id="p1">*</ept>. New York: Springer (4th ed).</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Chambers, J. M.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>and Hastie, T. J.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>eds (1992) <bpt id="p1">*</bpt>Statistical Models in S<ept id="p1">*</ept>. Wadsworth &amp; Brooks/Cole.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Goodnight, J. H.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>(1979) A Tutorial on the SWEEP Operator.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>The American Statistician<ept id="p1">*</ept> Vol. <bpt id="p2">**</bpt>33<ept id="p2">**</ept> No.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>3<ept id="p1">**</ept>, 149--158.</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>step, <bpt id="p1">[</bpt>rxStepPlot<ept id="p1">](rxStepPlot.md)</ept>.</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>