<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="rxcovregression.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86c57b8673cccc2dc90841fb9d5fe5e6bbe9c6794a.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">c57b8673cccc2dc90841fb9d5fe5e6bbe9c6794a</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">a507aa1d-ad98-40e9-8c2d-f550e7c4ca86</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r-reference\revoscaler\rxcovregression.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>rxCovCoef function (revoAnalytics) | Microsoft Docs</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Obtain covariance and correlation matrices for the coefficient estimates within rxLinMod,  rxLogit, and rxGlm objects and explanatory variables within rxLinMod and rxLogit objects.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>(revoAnalytics), rxCovCoef, rxCovCoef.rxLinMod, rxCovCoef.rxLogit, rxCovCoef.rxGlm, rxCorCoef, rxCorCoef.rxLinMod, rxCorCoef.rxLogit, rxCorCoef.rxGlm, rxCovData, rxCovData.rxLinMod, rxCovData.rxLogit, rxCorData, rxCorData.rxLinMod, rxCorData.rxLogit, models, regression</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>rxCovCoef: Covariance and Correlation Matrices for Linear Model Coefficients and Explanatory Variables</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Description</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>Obtain covariance and correlation matrices for the coefficient estimates within <ph id="ph1">`rxLinMod`</ph>, <ph id="ph2">`rxLogit`</ph>, and <ph id="ph3">`rxGlm`</ph> objects and explanatory variables within <ph id="ph4">`rxLinMod`</ph> and <ph id="ph5">`rxLogit`</ph> objects.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>Usage</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Arguments</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>object of class <ph id="ph1">`rxLinMod`</ph>, <ph id="ph2">`rxLogit`</ph>, or <ph id="ph3">`rxGlm`</ph> that  satisfies conditions in the Details section.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Details</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxCovCoef`</ph> and <ph id="ph2">`rxCorCoef`</ph>, the rxLinMod, rxLogit, or rxGlm object must have been fit with <ph id="ph3">`covCoef = TRUE`</ph> and <ph id="ph4">`cube = FALSE`</ph>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>The degrees of freedom must be greater than 0.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxCovData`</ph> and <ph id="ph2">`rxCorData`</ph>, the rxLinMod or rxLogit object must have been fit with an intercept term as well as with <ph id="ph3">`covData = TRUE`</ph> and <ph id="ph4">`cube = FALSE`</ph>.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Value</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>If <ph id="ph1">`p`</ph> is the number of columns in the model matrix, then</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxCovCoef`</ph> a <ph id="ph2">`p x p`</ph> numeric matrix containing the covariances of the model coefficients.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxCorCoef`</ph> a <ph id="ph2">`p x p`</ph> numeric matrix containing the correlations amongst the model coefficients.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxCovData`</ph> a <ph id="ph2">`(p - 1) x (p - 1)`</ph> numeric matrix containing the covariances of the non-intercept terms in the model matrix.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>For <ph id="ph1">`rxCorData`</ph> a <ph id="ph2">`(p - 1) x (p - 1)`</ph> numeric matrix containing the correlations amongst the non-intercept terms in the model matrix.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Author(s)</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Microsoft Corporation <bpt id="p1">[</bpt><ph id="ph1">`Microsoft Technical Support`</ph><ept id="p1">](https://go.microsoft.com/fwlink/?LinkID=698556&amp;clcid=0x409)</ept></source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>See Also</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source><bpt id="p1">[</bpt>rxLinMod<ept id="p1">](rxLinMod.md)</ept>, <bpt id="p2">[</bpt>rxLogit<ept id="p2">](rxLogit.md)</ept>, <bpt id="p3">[</bpt>rxCovCor<ept id="p3">](rxCovCor.md)</ept>.</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Examples</source>
        </trans-unit></group></body></file></xliff>