<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxformula.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc775098bffc4e4d395b8c1929bdc82f4fcc4cdced1dbc.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">98bffc4e4d395b8c1929bdc82f4fcc4cdced1dbc</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxformula.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxFormula function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Highlights of the similarities and differences in formulas between <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> and standard R functions.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxFormula, models</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxFormula: Formula Syntax for RevoScaleR Analysis Functions</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Highlights of the similarities and differences in formulas between <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> and standard R functions.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The formula syntax used by the <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> analysis functions is similar, but not identical, to regular R formula syntax.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>The most important differences are:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>With the exception of <bpt id="p1">[</bpt>rxSummary<ept id="p1">](rxSummary.md)</ept>, dot (<ph id="ph1">`.`</ph>) explanatory variable expansion is not supported.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>Multiple column producing in-line variable transformations, e.g. poly and bs, are not supported.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The original order of the explanatory variables are maintained, i.e. the main effects are not forced to precede the interaction terms.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>(See <ph id="ph1">`keep.order = TRUE`</ph> setting in terms.formula for more information.)</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>A formula typically consists of a <bpt id="p1">*</bpt>response<ept id="p1">*</ept>, which in most <bpt id="p2">**</bpt>RevoScaleR<ept id="p2">**</ept> functions can be a single variable or multiple variables combined using cbind, the <ph id="ph1">`"~"`</ph> operator, and one or more <bpt id="p3">*</bpt>predictors<ept id="p3">*</ept>,typically separated by the <ph id="ph2">`"+"`</ph> operator.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">[</bpt>rxSummary<ept id="p1">](rxSummary.md)</ept> function typically requires a formula with no response.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Interactions are indicated using the <ph id="ph1">`":"`</ph> operator.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>The interaction of two categorical variables results in a categorical variable containing the full set of combinations of the two categories and adds a coefficient to the model for each category.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The interaction of two continuous variables is the same as the multiplication of the two variables.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The interaction of a continuous and a categorical variable adds a coefficient for the continuous variable for each level of the categorical variable.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>The asterisk operator <ph id="ph1">`"*"`</ph> between categorical variables adds all subsets of interactions of the variables to the model.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>In <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept>, predictors must be single-column variables.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source><bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> formulas support two formula functions for managing categorical variables:</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>creates a categorical variable out of continuous variable <ph id="ph1">`x`</ph>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Additional arguments <ph id="ph1">`low`</ph>, <ph id="ph2">`high`</ph>, and <ph id="ph3">`exclude`</ph> can be included to specify the value of the lowest category, the highest category, and how to handle values outside the specified range.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>For each integer in the range from <ph id="ph1">`low`</ph> to <ph id="ph2">`high`</ph> inclusive, <bpt id="p1">**</bpt>RevoScaleR<ept id="p1">**</ept> creates a level and assigns values greater than or equal to an integer n, but less than n+1, to n's level.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`x`</ph> is already a factor, <ph id="ph2">`F(x, low, high, exclude)`</ph> can be used to limit the range of levels used; in this case <ph id="ph3">`low`</ph> and <ph id="ph4">`high`</ph> represent the indexes of the factor levels, and must be integers  in the range from 1 to the number of levels.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>creates a continuous variable from categorical variable <ph id="ph1">`x`</ph>.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Note, however, that the value of this  function is equivalent to the factor codes, and has no relation to any  numeric values within the levels of the function.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>For this, use the construction <ph id="ph1">`as.numeric(levels(x))[x]`</ph>.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxTransform<ept id="p1">](rxTransform.md)</ept>, <bpt id="p2">[</bpt>rxCrossTabs<ept id="p2">](rxCrossTabs.md)</ept>, <bpt id="p3">[</bpt>rxCube<ept id="p3">](rxCube.md)</ept>, <bpt id="p4">[</bpt>rxLinMod<ept id="p4">](rxLinMod.md)</ept>, <bpt id="p5">[</bpt>rxLogit<ept id="p5">](rxLogit.md)</ept>, <bpt id="p6">[</bpt>rxSummary<ept id="p6">](rxSummary.md)</ept>.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>