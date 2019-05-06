<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-developer-pmml.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc775083a85856b88a6daa29402efe4cbb0f5e31349266.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">83a85856b88a6daa29402efe4cbb0f5e31349266</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">149aa3b7-0352-480d-93b4-88f339cc7750</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/06/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-developer-pmml.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Convert RevoScaleR Model Objects for Use in PMML (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Using PMML with RevoScaleR model objects in Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Converting RevoScaleR Model Objects for Use in PMML</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>The objects returned by RevoScaleR predictive analytics functions have similarities to objects returned by the predictive analytics functions provided by base and recommended packages in R. A key difference between these two types of model objects is that RevoScaleR model objects typically do not contain any components that have the same length as the number of rows in the original data set.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>For example, if you use base R's lm function to estimate a linear model, the result object contains not only all of the data used to estimate the model, but components such as residuals and fitted.values that contain values corresponding to every observation in the data set.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>For estimating models using big data, this is not appropriate.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>However, there is overlap in the model object components that can be very useful when working with other packages.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>For example, the <bpt id="p1">*</bpt>pmml<ept id="p1">*</ept> package generates PMML (Predictive Model Markup Language) code for a number of R model types.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>PMML is an XML-base language that allows users to share models between PMML-compliant applications.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>For more information about PMML, visit <ph id="ph1">&lt;http://www.dmg.org&gt;</ph> .</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>RevoScaleR provides a set of coercion methods to convert a RevoScaleR model object to a standard R model object: <bpt id="p1">*</bpt>as.lm<ept id="p1">*</ept>, <bpt id="p2">*</bpt>as.glm<ept id="p2">*</ept>, <bpt id="p3">*</bpt>as.rpart<ept id="p3">*</ept>, and <bpt id="p4">*</bpt>as.kmeans<ept id="p4">*</ept>.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>As suggested above, these coerced model objects do not have all of the information available in a standard R model object, but do contain information about the fitted model that is similar to standard R.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>For example, let’s create an rxLinMod object by estimating a linear regression on a very large dataset: the airline data with almost 150 million observations.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>Next, the R <bpt id="p1">*</bpt>pmml<ept id="p1">*</ept> package should be downloaded and installed from CRAN.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>After you have done so, generate the RevoScaleR <bpt id="p1">*</bpt>rxLinMod<ept id="p1">*</ept> object, and use the <bpt id="p2">*</bpt>as.lm<ept id="p2">*</ept> method when generating the PMML output:</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The generated output looks as follows:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Similarly, rxLogit and rxGlm functions have as.glm methods:</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>RevoScaleR's <bpt id="p1">*</bpt>rxKmeans<ept id="p1">*</ept> objects can be coerced to <bpt id="p2">*</bpt>kmeans<ept id="p2">*</ept> objects:</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>And RevoScaleR's <bpt id="p1">*</bpt>rxDTree<ept id="p1">*</ept> objects can be coerced to <bpt id="p2">*</bpt>rpart<ept id="p2">*</ept> objects.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>(Note that <bpt id="p1">*</bpt>rpart<ept id="p1">*</ept> is a recommended package that you may need to load.)</source>
        </trans-unit></group></body></file></xliff>