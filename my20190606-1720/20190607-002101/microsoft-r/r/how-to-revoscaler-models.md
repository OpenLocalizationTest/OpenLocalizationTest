<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-models.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-4e81c41" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37b0ecd8b2b40fb6eb39464f4ecf5a535c1a33fd43.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">b0ecd8b2b40fb6eb39464f4ecf5a535c1a33fd43</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5a1af0c1-a46b-4161-9fcd-2c6c2f004c37</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">06/07/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-models.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Models in RevoScaleR on Machine Learning Server</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Models in RevoScaleR on Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Models in RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Specifying a model with RevoScaleR is similar to specifying a model with the standard R statistical modeling functions, but there are some significant differences.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>Understanding these differences can help you make better use of RevoScaleR.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>The purpose of this article is to explain these differences at a high level so that when we begin fitting models in script, the terminology does not seem too foreign.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>External Memory Algorithms</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>The first thing to know about RevoScaleR’s statistical algorithms is that they are <bpt id="p1">*</bpt>external memory<ept id="p1">*</ept> algorithms that work on one chunk of data at time.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>All of RevoScaleR’s algorithms share a basic underlying structure:</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>An <bpt id="p1">*</bpt>initialization<ept id="p1">*</ept> step, in which data structures are created and given initial values, a data source is identified and opened for reading, and any other initial conditions are satisfied.</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">*</bpt>process data<ept id="p1">*</ept> step, in which a chunk of data is read, some calculations are performed, and the result is passed back to the master process.</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>An <bpt id="p1">*</bpt>update results<ept id="p1">*</ept> step, in which the results of the process data step are merged with previous results.</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>A <bpt id="p1">*</bpt>finalize results<ept id="p1">*</ept> step, in which any final processing is performed and a result is returned.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>An important consideration in using external memory algorithms is deciding how big a <bpt id="p1">*</bpt>chunk<ept id="p1">*</ept> of data is.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>You want to use a chunk size that’s as large as possible while still allowing the process data step to complete without swapping.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>All of the RevoScaleR modeling functions allow you to specify a <bpt id="p1">*</bpt>blocksPerRead<ept id="p1">*</ept> argument.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>To make effective use of this, you need to know how many blocks your data file contains and how large the data file is.</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The number of blocks can be obtained using the <bpt id="p1">*</bpt>rxGetInfo<ept id="p1">*</ept> function.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>Formulas in RevoScaleR</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>RevoScaleR uses a variant of the Wilkinson-Rogers formula notation that is similar to, but not exactly the same as, that used in the standard R modeling functions.</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>The response, or dependent, variables are separated from the predictor, or independent, variables by a tilde (~).</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>In most of the modeling functions, multiple response variables are permitted, specified using the <bpt id="p1">*</bpt>cbind<ept id="p1">*</ept> function to combine them.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>Independent variables (<bpt id="p1">*</bpt>predictors<ept id="p1">*</ept>) are separated by plus signs (+).</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>Interaction terms can be created by joining two or more variables with a colon (:).</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>Interactions between two categorical variables add one coefficient to the model for every combination of levels of the two variables.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>For example, if we have the categorical variables sex with two levels and education with four levels, the interaction of sex and education will add eight coefficients to the fitted model.</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>Interactions between a continuous variable and a categorical variable add one coefficient to the model representing the continuous variable for each level of the categorical variable.</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>(However, in RevoScaleR, such interactions cannot be used with the <bpt id="p1">*</bpt>rxCube<ept id="p1">*</ept> or <bpt id="p2">*</bpt>rxCrossTabs<ept id="p2">*</ept> functions.) The interaction of two continuous variables is the same as multiplying the two variables.</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>An asterisk (<ph id="ph1">\*</ph>) between two variables adds all subsets of interactions to the model.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Thus, sex<ph id="ph1">\*</ph>education is equivalent to sex + education + sex:education.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The special function syntax <bpt id="p1">*</bpt>F(x)<ept id="p1">*</ept> can be used to have RevoScaleR treat a numeric variable <bpt id="p2">*</bpt>x<ept id="p2">*</ept> as a categorical variable (factor) for the purposes of the analysis.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>You can include additional arguments <bpt id="p1">*</bpt>low<ept id="p1">*</ept> and <bpt id="p2">*</bpt>high<ept id="p2">*</ept> to specify the minimum and maximum values to be included in the factor variable; RevoScaleR creates a bin for each integer value from the low to high values.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>You can use the logical flag <bpt id="p1">*</bpt>exclude<ept id="p1">*</ept> to specify whether values outside that range are omitted from the model (<bpt id="p2">*</bpt>exclude=TRUE<ept id="p2">*</ept>) or included as a separate level (<bpt id="p3">*</bpt>exclude=FALSE<ept id="p3">*</ept>).</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Similarly, the special function syntax <bpt id="p1">*</bpt>N(x)<ept id="p1">*</ept> can be used to have RevoScaleR treat <bpt id="p2">*</bpt>x<ept id="p2">*</ept> as a continuous numeric variable.</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>(This syntax is provided for completeness, but is not recommended.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>In general, if you want to recover numeric data from a factor, you will want to do so from the <bpt id="p1">*</bpt>levels<ept id="p1">*</ept> of the factor.)</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>In RevoScaleR, formulas in which the first independent variable is categorical may be handled specially, as <bpt id="p1">*</bpt>cubes<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>See the following section for more details.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Letting the Data Speak For Itself</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>Classical statistics is largely concerned with fitting predictive models to limited observations.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>Data analysts and statisticians use exploratory techniques to visualize the data and then make informed guesses as to the appropriate form for a predictive model.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Large data analysis, on the other hand, provides the opportunity to let the data speak for itself.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>With millions of observations in hand, we don’t have to guess about the form of relationships between variables: they become clear.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>A general approach to finding the relationship between two numeric variables x and y might be as follows.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>First, bin the x values.</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Then, for each bin, plot the mean of the y values contained in that bin.</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>As the bins become narrower and narrower, the resulting plot becomes a plot of E(y|x) for each value of x.</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>Cubes and Cube Regression</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>In RevoScaleR, a <bpt id="p1">*</bpt>cube<ept id="p1">*</ept> is a type of multi-dimensional array.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>It may have any number of dimensions, thus making it a hypercube, and each dimension consists of categorical data.</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>The most common operation on a cube is simple cross-tabulation, computing the cell counts for every combination of levels within the cube; this is done using the <bpt id="p1">*</bpt>rxCube<ept id="p1">*</ept> function.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>But cubes can also be passed as the first independent variable in a linear or logistic regression, in which case the regression can be computed in a special way.</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Because the cube consists of categorical data, one part of the moment matrix is diagonal.</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>This makes it possible to compute the regression using a partitioned inverse method, which may be faster and may use less memory than the usual regression method.</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>When a linear or logistic regression is fitted with the argument <bpt id="p1">*</bpt>cube=TRUE<ept id="p1">*</ept> (and a categorical variable as the first predictor), the partitioned inverse method is used and the model is fitted without an intercept term.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Because the first term in the regression is categorical, it is equivalent to a complete set of dummy variables and thus is collinear with a constant term.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>By dropping the intercept term, the collinearity is resolved and a coefficient can be computed for each level of the categorical predictor.</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The R-squared, however, is computed as if an intercept were included.</source>
        </trans-unit></group></body></file></xliff>