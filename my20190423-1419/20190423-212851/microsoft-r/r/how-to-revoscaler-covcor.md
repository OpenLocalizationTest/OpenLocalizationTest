<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-covcor.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-1931010" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a5af81ba56855936d8b1d34f1034b745251c2d225.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">5af81ba56855936d8b1d34f1034b745251c2d225</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">d222ee9a-1b0c-47af-9546-3facf089338a</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">04/23/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-covcor.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Estimate Correlation and Variance/Covariance Matrices in RevoScaleR (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Correlation and variance/covariance matrices in RevoScaleR in Machine Learning Server.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Estimating Correlation and Variance/Covariance Matrices</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxCovCor<ept id="p1">*</ept> function in RevoScaleR calculates the covariance, correlation, or sum of squares/cross-product matrix for a set of variables in a .xdf file or data frame.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>The size of these matrices is determined by the number of variables rather than the number of observations, so typically the results can easily fit into memory in R. A broad category of analyses can be computed from some form of a cross-product matrix, for example, factor analysis and principal components.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>A cross-product matrix is a matrix of the form X'X, where X represents an arbitrary set of raw or standardized variables.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>More generally, this matrix is of the form X'WX, where W is a diagonal weighting matrix.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>Computing Cross-Product Matrices</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>While rxCovCor is the primary tool for computing covariance, correlation, and other cross-product matrices, you will seldom call it directly.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>Instead, it is generally simpler to use one of the following convenience functions:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>rxCov: Use rxCov to return the covariance matrix</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>rxCor: Use rxCor to return the correlation matrix</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>rxSSCP: Use rxSSCP to return the augmented cross-product matrix, that is, we first add a column of 1’s (if no weights are specified) or a column equaling the square root of the weights to the data matrix, and then compute the cross-product.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>Computing a Correlation Matrix for Use in Factor Analysis</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>The 5% sample of the U.S. 2000 census has over 14 million observations.</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>In this example, we compute the correlation matrix for 16 variables derived from variables in the data set for individuals over the age of 20.</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>This correlation matrix is then used as input into the standard R factor analysis function, <bpt id="p1">*</bpt>factanal.<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>First, we specify the name and location of the data set:</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Next, we can take a quick look at some basic demographic and socio-economic variables by calling <bpt id="p1">*</bpt>rxSummary.<ept id="p1">*</ept></source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>(For more information on variables in the census data, see <ph id="ph1">&lt;http://usa.ipums.org/usa-action/variables/group&gt;</ph>.) Throughout the analysis we use the probability weighting variable, <bpt id="p1">*</bpt>perwt<ept id="p1">*</ept>, and restrict the analysis to people over the age of 20.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>This call provides summary information about the variables in this weighted subsample, including cell counts for factor variables:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>Next we call the <bpt id="p1">*</bpt>rxCor<ept id="p1">*</ept> function, a convenience function for <bpt id="p2">*</bpt>rxCovCor<ept id="p2">*</ept> that returns just the Pearson’s correlation matrix for the variables specified.</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>We make heavy use of the <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept> argument to create a series of logical (or dummy) variables from factor variables to be used in the creation of the correlation matrix.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>The resulting correlation matrix is used as input into the factor analysis function provided by the stats package in R. In interpreting the results, the variable <bpt id="p1">*</bpt>poverty<ept id="p1">*</ept> represents family income as a percentage of a poverty threshold, so increases as family income increases.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>First, specify two factors:</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Results in:</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>We can use the same correlation matrix to estimate three factors:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>The degrees of freedom for the model is 102 and the fit was 0.343</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Computing A Covariance Matrix for Principal Components Analysis</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>Principal components analysis, or PCA, is a technique closely related to factor analysis.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>PCA seeks to find a set of orthogonal axes such that the first axis, or <bpt id="p1">*</bpt>first principal component<ept id="p1">*</ept>, accounts for as much variability as possible, and subsequent axes or components are chosen to maximize variance while maintaining orthogonality with previous axes.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>Principal components are typically computed either by a singular value decomposition of the data matrix or an eigenvalue decomposition of a covariance or correlation matrix; the latter permits us to use <bpt id="p1">*</bpt>rxCovCor<ept id="p1">*</ept> and its relatives with the standard R function <bpt id="p2">*</bpt>princomp<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>As an example, we use the rxCov function to calculate a covariance matrix for the log of the classic iris data, and pass the matrix to the princomp function (reproduced from <bpt id="p1">[</bpt>Modern Applied Statistics with S<ept id="p1">](http://www.springer.com/us/book/9780387954578)</ept>):</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Yields the following:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>The default plot method for objects of class princomp is a <bpt id="p1">*</bpt>scree plot<ept id="p1">*</ept>, which is a barplot of the variances of the principal components.</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>We can obtain the plot as usual by calling plot with our principal components object:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>Yields the following plot:</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Another useful bit of output is given by the loadings function, which returns a set of columns showing the linear combinations for each principal component:</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>You may have noticed that we supplied the flag cor=TRUE in the call to princomp; this flag tells princomp to use the correlation matrix rather than the covariance matrix to compute the principal components.</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>We can obtain the same results by omitting the flag but submitting the correlation matrix as returned by rxCor instead:</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>A Large Data Principal Components Analysis</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>Stock market data for open, high, low, close, and adjusted close from 1962 to 2010 is available at <ph id="ph1">&lt;https://github.com/thebigjc/HackReduce/blob/master/datasets/nyse/daily_prices/NYSE_daily_prices_subset.csv&gt;</ph>.</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>The full data set includes 9.2 million observations of daily open-high-low-close data for some 2800 stocks.</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>As you might expect, these data are highly correlated, and principal components analysis can be used for data reduction.</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>We read the original data into a .xdf file, NYSE<ph id="ph1">\_</ph>daily<ph id="ph2">\_</ph>prices.xdf, using the same process we used in the <bpt id="p1">[</bpt>Tutorial: Analyzing loan data with RevoScaleR<ept id="p1">](tutorial-revoscaler-large-data-loan.md)</ept> to read our mortgage data (set <bpt id="p2">*</bpt>revoDataDir<ept id="p2">*</ept> to the full path to the NYSE directory containing the .csv files when you unpack the download):</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Once we have our .xdf file, we proceed as before:</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Yields the following output:</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>The scree plot is shown as follows:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>Between them, the first two principal components explain 99% of the variance; we can therefore replace the five original variables by these two principal components with no appreciable loss of information.</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Ridge Regression</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Another application of correlation matrices is to calculate ridge regression, a type of regression that can help deal with multicollinearity and is part of a broader class of models called Penalized Regression Models.</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Where the ordinary least squares regression minimizes the sum of squared residuals</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>ridge regression minimizes the slightly modified sum</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>The solution to the ridge regression is</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>where <ph id="ph1">![](media/how-to-revoscaler-covcor/math4.png)</ph> is the model matrix.</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>This matrix is similar to the ordinary least squares regression solution with a “ridge” added along the diagonal.</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Since the model matrix is embedded in the correlation matrix, the following function allows us to compute the ridge regression solution:</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>The following example shows how ridge regression dramatically improves the solution in a regression involving heavy multicollinearity:</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>You can supply a vector of lambdas as a quick way to compare various choices:</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>For λ = 0, the ridge regression is identical to ordinary least squares, while as λ → ∞, the coefficients of x and y approach 0.</source>
        </trans-unit></group></body></file></xliff>