<?xml version="1.0"?><xliff version="1.2" xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:oasis:names:tc:xliff:document:1.2 xliff-core-1.2-transitional.xsd"><file datatype="xml" original="how-to-revoscaler-crosstabs.md" source-language="en-US" target-language="en-US"><header><tool tool-id="mdxliff" tool-name="mdxliff" tool-version="1.0-8ab897d" tool-company="Microsoft" /><xliffext:skl_file_name xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3de93fdc23af305ce68e5983638a7e55917647218.skl</xliffext:skl_file_name><xliffext:version xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">1.2</xliffext:version><xliffext:ms.openlocfilehash xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">de93fdc23af305ce68e5983638a7e55917647218</xliffext:ms.openlocfilehash><xliffext:ms.sourcegitcommit xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">85d1c4fe-cf61-4439-ac27-8f1db11b25b3</xliffext:ms.sourcegitcommit><xliffext:ms.lasthandoff xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">05/29/2019</xliffext:ms.lasthandoff><xliffext:ms.openlocfilepath xmlns:xliffext="urn:microsoft:content:schema:xliffextensions">microsoft-r\r\how-to-revoscaler-crosstabs.md</xliffext:ms.openlocfilepath></header><body><group id="content" extype="content"><trans-unit id="101" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Crosstabs using RevoScaleR (Machine Learning Server)</source>
        </trans-unit><trans-unit id="102" translate="yes" xml:space="preserve" restype="x-metadata">
          <source>Cross-tabulations (contingency tables) with RevoScaleR.</source>
        </trans-unit><trans-unit id="103" translate="yes" xml:space="preserve">
          <source>Crosstabs using RevoScaleR</source>
        </trans-unit><trans-unit id="104" translate="yes" xml:space="preserve">
          <source>Crosstabs, also known as <bpt id="p1">*</bpt>contingency tables<ept id="p1">*</ept> or <bpt id="p2">*</bpt>crosstabulations<ept id="p2">*</ept>, are a convenient way to summarize cross-classified categorical data—that is, data that can be tabulated according to multiple levels of two or more factors.</source>
        </trans-unit><trans-unit id="105" translate="yes" xml:space="preserve">
          <source>If only two factors are involved, the table is sometimes called a <bpt id="p1">*</bpt>two-way table<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="106" translate="yes" xml:space="preserve">
          <source>If three factors are involved, the table is sometimes called a <bpt id="p1">*</bpt>three-way table<ept id="p1">*</ept>.</source>
        </trans-unit><trans-unit id="107" translate="yes" xml:space="preserve">
          <source>For large data sets, cross-tabulations of binned numeric data, that is, data that has been converted to a factor where the levels represent ranges of values, can be a fast way to get insight into the relationships among variables.</source>
        </trans-unit><trans-unit id="108" translate="yes" xml:space="preserve">
          <source>In RevoScaleR, the <bpt id="p1">*</bpt>rxCube<ept id="p1">*</ept> function is the primary tool to create contingency tables.</source>
        </trans-unit><trans-unit id="109" translate="yes" xml:space="preserve">
          <source>For example, the built-in data set <bpt id="p1">*</bpt>UCBAdmissions<ept id="p1">*</ept> includes information on admissions by gender to various departments at the University of California at Berkeley.</source>
        </trans-unit><trans-unit id="110" translate="yes" xml:space="preserve">
          <source>We can look at the contingency table as follows:</source>
        </trans-unit><trans-unit id="111" translate="yes" xml:space="preserve">
          <source>(Because cross-tabulations are explicitly about exploring interactions between variables, multiple predictors must always be specified using the interaction operator ":", and not the terms operator "+".)</source>
        </trans-unit><trans-unit id="112" translate="yes" xml:space="preserve">
          <source>Typing <bpt id="p1">*</bpt>z<ept id="p1">*</ept> yields the following output:</source>
        </trans-unit><trans-unit id="113" translate="yes" xml:space="preserve">
          <source>This data set is widely used in statistics texts because it illustrates Simpson’s paradox, which is that in some cases a comparison that holds true in a number of groups is reversed when those groups are aggregated to form a single group.</source>
        </trans-unit><trans-unit id="114" translate="yes" xml:space="preserve">
          <source>From the preceding table, in which admissions data is aggregated across all departments, it would appear that males are admitted at a higher rate than women.</source>
        </trans-unit><trans-unit id="115" translate="yes" xml:space="preserve">
          <source>However, if we look at the more granular analysis by department, we find that in four of the six departments, women are admitted at a higher rate than men:</source>
        </trans-unit><trans-unit id="116" translate="yes" xml:space="preserve">
          <source>This yields the following output:</source>
        </trans-unit><trans-unit id="117" translate="yes" xml:space="preserve">
          <source>Letting the Data Speak Example 1: Analyzing U.S. 2000 Census Data</source>
        </trans-unit><trans-unit id="118" translate="yes" xml:space="preserve">
          <source>The CensusWorkers.xdf data set contains a subset of the U.S. 2000 5% Census for individuals aged 20 to 65 who worked at least 20 weeks during the year from three states.</source>
        </trans-unit><trans-unit id="119" translate="yes" xml:space="preserve">
          <source>Let’s examine the relationship between wage income (represented in the data set by the variable <bpt id="p1">*</bpt>incwage<ept id="p1">*</ept>) and age.</source>
        </trans-unit><trans-unit id="120" translate="yes" xml:space="preserve">
          <source>A useful way to observe the relationship between numeric variables is to bin the predictor variable (in our case, age), and then plot the mean of the response for each bin.</source>
        </trans-unit><trans-unit id="121" translate="yes" xml:space="preserve">
          <source>The simplest way to bin age is to use the F() wrapper within our initial formula; it creates a separate bin for each distinct value of age.</source>
        </trans-unit><trans-unit id="122" translate="yes" xml:space="preserve">
          <source>(More precisely, it creates a bin of length one from the low value of age to the high value of age—if some ages are missing in the original data set, bins are created for them anyway.)</source>
        </trans-unit><trans-unit id="123" translate="yes" xml:space="preserve">
          <source>We create our original model as follows:</source>
        </trans-unit><trans-unit id="124" translate="yes" xml:space="preserve">
          <source>We first look at the results in tabular form by typing the returned object name, <bpt id="p1">*</bpt>censusWorkersCube<ept id="p1">*</ept>, which yields the following output:</source>
        </trans-unit><trans-unit id="125" translate="yes" xml:space="preserve">
          <source>As we wanted, the table contains average values of <bpt id="p1">*</bpt>incwage<ept id="p1">*</ept> for each level of <bpt id="p2">*</bpt>age<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="126" translate="yes" xml:space="preserve">
          <source>If we want to create a plot of the results, we can use the <bpt id="p1">*</bpt>rxResultsDF<ept id="p1">*</ept> function to conveniently convert the output into a data frame.</source>
        </trans-unit><trans-unit id="127" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>F<ph id="ph1">\_</ph>age<ept id="p1">*</ept> factor variable will automatically be converted back to an integer <bpt id="p2">*</bpt>age<ept id="p2">*</ept> variable.</source>
        </trans-unit><trans-unit id="128" translate="yes" xml:space="preserve">
          <source>Then we can plot the data using <bpt id="p1">*</bpt>rxLinePlot<ept id="p1">*</ept>:</source>
        </trans-unit><trans-unit id="129" translate="yes" xml:space="preserve">
          <source>The resulting plot shows clearly the relationship of income on age:</source>
        </trans-unit><trans-unit id="130" translate="yes" xml:space="preserve">
          <source>Transforming Data</source>
        </trans-unit><trans-unit id="131" translate="yes" xml:space="preserve">
          <source>Because crosstabs require categorical data for the predictors, you have to do some work to crosstabulate continuous data.</source>
        </trans-unit><trans-unit id="132" translate="yes" xml:space="preserve">
          <source>In the previous section, we saw that the F() wrapper can do a transformation within a formula.</source>
        </trans-unit><trans-unit id="133" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>transforms<ept id="p1">*</ept> argument to <bpt id="p2">*</bpt>rxCrossTabs<ept id="p2">*</ept> can be used to give you greater control over such transformations.</source>
        </trans-unit><trans-unit id="134" translate="yes" xml:space="preserve">
          <source>For example, the <bpt id="p1">*</bpt>kyphosis<ept id="p1">*</ept> data from the <bpt id="p2">*</bpt>rpart<ept id="p2">*</ept> package consists of one categorical variable, <bpt id="p3">*</bpt>Kyphosis<ept id="p3">*</ept>, and three continuous variables <bpt id="p4">*</bpt>Age<ept id="p4">*</ept>, <bpt id="p5">*</bpt>Number<ept id="p5">*</ept>, and <bpt id="p6">*</bpt>Start<ept id="p6">*</ept>.</source>
        </trans-unit><trans-unit id="135" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>Start<ept id="p1">*</ept> variable indicates the topmost vertebra involved in a certain type of spinal surgery, and has a range of 1 to 18.</source>
        </trans-unit><trans-unit id="136" translate="yes" xml:space="preserve">
          <source>Since there are 7 cervical vertebrae and 12 thoracic vertebrae, we can specify a transform that classifies the start variable as either cervical or thoracic as follows:</source>
        </trans-unit><trans-unit id="137" translate="yes" xml:space="preserve">
          <source>Similarly, we can create a factorized Age variable as follows (in the original data, age is given in months; with our set of breaks, we cut the data into ranges of years):</source>
        </trans-unit><trans-unit id="138" translate="yes" xml:space="preserve">
          <source>We can now crosstabulate the data using the preceding transforms and it is instructive to start by looking at the three two-way tables formed by tabulating Kyphosis with the three predictor variables:</source>
        </trans-unit><trans-unit id="139" translate="yes" xml:space="preserve">
          <source>From these, we see that the probability of the post-operative complication Kyphosis seems to be greater if the <bpt id="p1">*</bpt>Start<ept id="p1">*</ept> is a cervical vertebra and as more vertebrae are involved in the surgery.</source>
        </trans-unit><trans-unit id="140" translate="yes" xml:space="preserve">
          <source>Similarly, it appears that the dependence on age is non-linear: it first increases with age, peaks in the range 5-9, and then decreases again.</source>
        </trans-unit><trans-unit id="141" translate="yes" xml:space="preserve">
          <source>Cross-Tabulation with rxCrossTabs</source>
        </trans-unit><trans-unit id="142" translate="yes" xml:space="preserve">
          <source>The <bpt id="p1">*</bpt>rxCrossTabs<ept id="p1">*</ept> function is an alternative to the <bpt id="p2">*</bpt>rxCube<ept id="p2">*</ept> function, which performs the same calculations, but displays its results in format similar to the standard R <bpt id="p3">*</bpt>xtabs<ept id="p3">*</ept> function.</source>
        </trans-unit><trans-unit id="143" translate="yes" xml:space="preserve">
          <source>For some purposes, this format can be more informative than the matrix-like display of <bpt id="p1">*</bpt>rxCube<ept id="p1">*</ept>, and in some situations can be more compact as well.</source>
        </trans-unit><trans-unit id="144" translate="yes" xml:space="preserve">
          <source>As an example, consider again the admission data example:</source>
        </trans-unit><trans-unit id="145" translate="yes" xml:space="preserve">
          <source>Freq, Dept = B (sums):         Admit Gender   Admitted Rejected   Male        353      207   Female       17        8</source>
        </trans-unit><trans-unit id="146" translate="yes" xml:space="preserve">
          <source>Freq, Dept = C (sums):         Admit Gender   Admitted Rejected   Male        120      205   Female      202      391</source>
        </trans-unit><trans-unit id="147" translate="yes" xml:space="preserve">
          <source>Freq, Dept = D (sums):         Admit Gender   Admitted Rejected   Male        138      279   Female      131      244</source>
        </trans-unit><trans-unit id="148" translate="yes" xml:space="preserve">
          <source>Freq, Dept = E (sums):         Admit Gender   Admitted Rejected   Male         53      138   Female       94      299</source>
        </trans-unit><trans-unit id="149" translate="yes" xml:space="preserve">
          <source>Freq, Dept = F (sums):         Admit Gender   Admitted Rejected   Male         22      351   Female       24      317</source>
        </trans-unit><trans-unit id="150" translate="yes" xml:space="preserve">
          <source>You can see the row, column, and total percentages by calling the summary function on the rxCrossTabs object:</source>
        </trans-unit><trans-unit id="151" translate="yes" xml:space="preserve">
          <source>summary(z3) Call: rxCrossTabs(formula = Freq ~ Gender:Admit:Dept, data = UCBADF)</source>
        </trans-unit><trans-unit id="152" translate="yes" xml:space="preserve">
          <source>Cross Tabulation Results for: Freq ~ Gender:Admit:Dept Data: UCBADF Dependent variable(s): Freq Number of valid observations: 24 Number of missing observations: 0 Statistic: sums</source>
        </trans-unit><trans-unit id="153" translate="yes" xml:space="preserve">
          <source>Freq, Dept = A (sums): Admitted   Rejected Row Total Male        512.000000 313.000000 825.00000 Row%      62.060606  37.939394</source>
        </trans-unit><trans-unit id="154" translate="yes" xml:space="preserve">
          <source>Col%      85.191348  94.277108</source>
        </trans-unit><trans-unit id="155" translate="yes" xml:space="preserve">
          <source>Tot%      54.876742  33.547696  88.42444 Female       89.000000  19.000000 108.00000 Row%      82.407407  17.592593</source>
        </trans-unit><trans-unit id="156" translate="yes" xml:space="preserve">
          <source>Col%      14.808652   5.722892</source>
        </trans-unit><trans-unit id="157" translate="yes" xml:space="preserve">
          <source>Tot%       9.539121   2.036442  11.57556 Col Total   601.000000 332.000000</source>
        </trans-unit><trans-unit id="158" translate="yes" xml:space="preserve">
          <source>Grand Total 933.000000</source>
        </trans-unit><trans-unit id="159" translate="yes" xml:space="preserve">
          <source>Freq, Dept = B (sums): Admitted   Rejected  Row Total Male        353.000000 207.000000 560.000000 Row%      63.035714  36.964286</source>
        </trans-unit><trans-unit id="160" translate="yes" xml:space="preserve">
          <source>Col%      95.405405  96.279070</source>
        </trans-unit><trans-unit id="161" translate="yes" xml:space="preserve">
          <source>Tot%      60.341880  35.384615  95.726496 Female       17.000000   8.000000  25.000000 Row%      68.000000  32.000000</source>
        </trans-unit><trans-unit id="162" translate="yes" xml:space="preserve">
          <source>Col%       4.594595   3.720930</source>
        </trans-unit><trans-unit id="163" translate="yes" xml:space="preserve">
          <source>Tot%       2.905983   1.367521   4.273504 Col Total   370.000000 215.000000</source>
        </trans-unit><trans-unit id="164" translate="yes" xml:space="preserve">
          <source>Grand Total 585.000000</source>
        </trans-unit><trans-unit id="165" translate="yes" xml:space="preserve">
          <source>Freq, Dept = C (sums): Admitted  Rejected Row Total Male        120.00000 205.00000 325.00000 Row%      36.92308  63.07692</source>
        </trans-unit><trans-unit id="166" translate="yes" xml:space="preserve">
          <source>Col%      37.26708  34.39597</source>
        </trans-unit><trans-unit id="167" translate="yes" xml:space="preserve">
          <source>Tot%      13.07190  22.33115  35.40305 Female      202.00000 391.00000 593.00000 Row%      34.06408  65.93592</source>
        </trans-unit><trans-unit id="168" translate="yes" xml:space="preserve">
          <source>Col%      62.73292  65.60403</source>
        </trans-unit><trans-unit id="169" translate="yes" xml:space="preserve">
          <source>Tot%      22.00436  42.59259  64.59695 Col Total   322.00000 596.00000</source>
        </trans-unit><trans-unit id="170" translate="yes" xml:space="preserve">
          <source>Grand Total 918.00000</source>
        </trans-unit><trans-unit id="171" translate="yes" xml:space="preserve">
          <source>Freq, Dept = D (sums): Admitted  Rejected Row Total Male        138.00000 279.00000 417.00000 Row%      33.09353  66.90647</source>
        </trans-unit><trans-unit id="172" translate="yes" xml:space="preserve">
          <source>Col%      51.30112  53.34608</source>
        </trans-unit><trans-unit id="173" translate="yes" xml:space="preserve">
          <source>Tot%      17.42424  35.22727  52.65152 Female      131.00000 244.00000 375.00000 Row%      34.93333  65.06667</source>
        </trans-unit><trans-unit id="174" translate="yes" xml:space="preserve">
          <source>Col%      48.69888  46.65392</source>
        </trans-unit><trans-unit id="175" translate="yes" xml:space="preserve">
          <source>Tot%      16.54040  30.80808  47.34848 Col Total   269.00000 523.00000</source>
        </trans-unit><trans-unit id="176" translate="yes" xml:space="preserve">
          <source>Grand Total 792.00000</source>
        </trans-unit><trans-unit id="177" translate="yes" xml:space="preserve">
          <source>Freq, Dept = E (sums): Admitted  Rejected Row Total Male         53.000000 138.00000 191.00000 Row%      27.748691  72.25131</source>
        </trans-unit><trans-unit id="178" translate="yes" xml:space="preserve">
          <source>Col%      36.054422  31.57895</source>
        </trans-unit><trans-unit id="179" translate="yes" xml:space="preserve">
          <source>Tot%       9.075342  23.63014  32.70548 Female       94.000000 299.00000 393.00000 Row%      23.918575  76.08142</source>
        </trans-unit><trans-unit id="180" translate="yes" xml:space="preserve">
          <source>Col%      63.945578  68.42105</source>
        </trans-unit><trans-unit id="181" translate="yes" xml:space="preserve">
          <source>Tot%      16.095890  51.19863  67.29452 Col Total   147.000000 437.00000</source>
        </trans-unit><trans-unit id="182" translate="yes" xml:space="preserve">
          <source>Grand Total 584.000000</source>
        </trans-unit><trans-unit id="183" translate="yes" xml:space="preserve">
          <source>Freq, Dept = F (sums): Admitted  Rejected Row Total Male         22.000000 351.00000  373.0000 Row%       5.898123  94.10188</source>
        </trans-unit><trans-unit id="184" translate="yes" xml:space="preserve">
          <source>Col%      47.826087  52.54491</source>
        </trans-unit><trans-unit id="185" translate="yes" xml:space="preserve">
          <source>Tot%       3.081232  49.15966   52.2409 Female       24.000000 317.00000  341.0000 Row%       7.038123  92.96188</source>
        </trans-unit><trans-unit id="186" translate="yes" xml:space="preserve">
          <source>Col%      52.173913  47.45509</source>
        </trans-unit><trans-unit id="187" translate="yes" xml:space="preserve">
          <source>Tot%       3.361345  44.39776   47.7591 Col Total    46.000000 668.00000</source>
        </trans-unit><trans-unit id="188" translate="yes" xml:space="preserve">
          <source>Grand Total 714.000000</source>
        </trans-unit><trans-unit id="189" translate="yes" xml:space="preserve">
          <source>You can see, for example, that in Department A, 62 percent of male applicants are admitted, but 82 percent of female applicants are admitted, and in Department B, 63 percent of male applicants are admitted, while 68 percent of female applicants are admitted.</source>
        </trans-unit><trans-unit id="190" translate="yes" xml:space="preserve">
          <source>A Large Data Example</source>
        </trans-unit><trans-unit id="191" translate="yes" xml:space="preserve">
          <source>The power of <bpt id="p1">*</bpt>rxCrossTabs<ept id="p1">*</ept> is most evident when you need to tabulate a data set that won’t fit into memory.</source>
        </trans-unit><trans-unit id="192" translate="yes" xml:space="preserve">
          <source>For example, in the large airline data set AirOnTime87to12.xdf, you can obtain the mean arrival delay by carrier and day of week as follows (if you have downloaded the data set, modify the first line as follows to reflect your local path):</source>
        </trans-unit><trans-unit id="193" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="194" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="195" translate="yes" xml:space="preserve">
          <source>A Large Data Example</source>
        </trans-unit><trans-unit id="196" translate="yes" xml:space="preserve">
          <source>bigDataDir &lt;- "C:/MRS/Data" bigAirData &lt;- file.path(bigDataDir, "AirOnTime87to12/AirOnTime87to12.xdf") arrDelayXT &lt;- rxCrossTabs(ArrDelay ~ UniqueCarrier:DayOfWeek,     data = bigAirData, blocksPerRead = 30) print(arrDelayXT)</source>
        </trans-unit><trans-unit id="197" translate="yes" xml:space="preserve">
          <source>Gives the following output:</source>
        </trans-unit><trans-unit id="198" translate="yes" xml:space="preserve">
          <source>Call: rxCrossTabs(formula = ArrDelay ~ UniqueCarrier:DayOfWeek, data = bigAirData,     blocksPerRead = 30)</source>
        </trans-unit><trans-unit id="199" translate="yes" xml:space="preserve">
          <source>Cross Tabulation Results for: ArrDelay ~ UniqueCarrier:DayOfWeek File name: C:\MRS\Data\AirOnTime87to12\AirOnTime87to12.xdf Dependent variable(s): ArrDelay Number of valid observations: 145576737 Number of missing observations: 3042918 Statistic: sums</source>
        </trans-unit><trans-unit id="200" translate="yes" xml:space="preserve">
          <source>ArrDelay (sums):              DayOfWeek UniqueCarrier      Mon     Tues      Wed     Thur      Fri      Sat      Sun        AA     15956852 13367087 16498840 20554660 20714146  9359729 14577582        US     11797366 11688903 14065606 17379113 19541862  5865427 10264583        AS      3144578  2677858  3182356  3980209  4415144  2433581  3039129        CO      8464507  7966834  9537366 11901028 11749616  3553719  6562487        DL     18146092 15962559 19474389 24077435 24933864 10483280 16414060        EA       782103   832332   796811  1152825  1405399   638911   670924        HP      3577460  3170343  3700890  4734543  5015896  2864314  3985741        NW      7750970  7818040  9256994 11199718 10294116  3726129  6504924        PA (1)   191137   235924   225260   290844   345238   174284   229677        PI      1164688  1391526  1456173  1515403  1568266   939820   986642        PS        88144   111282   122520   133567   173422    44362    88891        TW      3356944  3459185  4060151  5027427  5267750  1669048  2377671        UA     15941096 14731587 17801128 21060697 20920843  9174567 13688577        WN     12438738  8978339 12215989 21556781 26787623  4972506 15973176        ML (1)    20735    50927    55881    75030    62855    44549    18173        KH        20744   -26425   -24265    30078    98529    33595    43026        MQ      7065052  5152746  5893882  7136735  8087443  2947023  5540099        B6      1886261  1340744  1736450  2373151  2930423  1012698  1969546        DH       795614   527649   708129   801968   986930   227907   504644        EV      5733212  3684210  4005374  5262924  5874647  1753361  4418290        FL      2666677  1694294  1810548  2928247  3068538   819827  2188420        OO      4717107  3106319  3438056  4725854  5481441  2797745  4764041        XE      4870453  3904752  4532069  5349375  5315818  1636826  3531446        TZ       228508   147963   197371   224693   275340    39722   148940        HA       -72468   -92714   -66578     4840   153830    -2082   -22196        OH      2276399  1567510  1830571  2336032  2702519   922531  1659708        F9       551932   484426   566122   858027   729273   337695   526887        YV      1959906  1419073  1463954  1930992  2152270  1270104  1830749        9E       787776   579608   590038   709161   869358   304151   586378        VX        10208    37079    12956    42661    73457     2943    39987</source>
        </trans-unit><trans-unit id="201" translate="yes" xml:space="preserve">
          <source>Using Sparse Cubes</source>
        </trans-unit><trans-unit id="202" translate="yes" xml:space="preserve">
          <source>An additional tool that may be useful when using <bpt id="p1">*</bpt>rxCube<ept id="p1">*</ept> and <bpt id="p2">*</bpt>rxCrossTabs<ept id="p2">*</ept> with large data is the <bpt id="p3">*</bpt>useSparseCube<ept id="p3">*</ept> parameter.</source>
        </trans-unit><trans-unit id="203" translate="yes" xml:space="preserve">
          <source> Compiling cross-tabulations of categorical data can sometimes result in a large number of cells with zero counts, yielding at its core a “sparse matrix”.</source>
        </trans-unit><trans-unit id="204" translate="yes" xml:space="preserve">
          <source> In the usual case, memory is allocated for every cell in the cube, but large cubes may overwhelm memory resources.</source>
        </trans-unit><trans-unit id="205" translate="yes" xml:space="preserve">
          <source>If we instead allocate space only for cells with positive counts, such operations may often proceed successfully.</source>
        </trans-unit><trans-unit id="206" translate="yes" xml:space="preserve">
          <source>As an example, let’s look at the airline data again and construct a case where the cross-tabulation yields many zero entries.</source>
        </trans-unit><trans-unit id="207" translate="yes" xml:space="preserve">
          <source> As the overwhelming number of flights in the data set were not canceled, by appending the <bpt id="p1">*</bpt>Cancelled<ept id="p1">*</ept> predictor in the formula, we would expect a large number of categorical predictor combinations to have zero observations.</source>
        </trans-unit><trans-unit id="208" translate="yes" xml:space="preserve">
          <source> Because the <bpt id="p1">*</bpt>Cancelled<ept id="p1">*</ept> predictor is a logical rather than a factor variable, we need to use the <bpt id="p2">*</bpt>F(.)<ept id="p2">*</ept> function to convert it.</source>
        </trans-unit><trans-unit id="209" translate="yes" xml:space="preserve">
          <source>bigDataDir &lt;- "C:/MRS/Data" bigAirData &lt;- file.path(bigDataDir, "AirOnTime87to12/AirOnTime87to12.xdf")</source>
        </trans-unit><trans-unit id="210" translate="yes" xml:space="preserve">
          <source>arrDelaySparse &lt;- rxCube(ArrDelay ~ UniqueCarrier:DayOfWeek:F(Cancelled),                      data = bigAirData, blocksPerRead = 30, useSparseCube = TRUE) print(arrDelaySparse)</source>
        </trans-unit><trans-unit id="211" translate="yes" xml:space="preserve">
          <source>This gives the following output.</source>
        </trans-unit><trans-unit id="212" translate="yes" xml:space="preserve">
          <source>We get 210 rows with F_Cancelled = 0.</source>
        </trans-unit><trans-unit id="213" translate="yes" xml:space="preserve">
          <source>By default, if useSparseCube=TRUE, rows with zero counts are removed from the result.</source>
        </trans-unit><trans-unit id="214" translate="yes" xml:space="preserve">
          <source>Call: rxCube(formula = ArrDelay ~ UniqueCarrier:DayOfWeek:F(Cancelled),    data = bigAirData, useSparseCube = TRUE, blocksPerRead = 30)</source>
        </trans-unit><trans-unit id="215" translate="yes" xml:space="preserve">
          <source>Cube Results for: ArrDelay ~ UniqueCarrier:DayOfWeek:F(Cancelled) File name: C:/data/AirOnTime87to12/AirOnTime87to12.xdf Dependent variable(s): ArrDelay Number of valid observations: 145576737 Number of missing observations: 3042918 Statistic: ArrDelay means UniqueCarrier DayOfWeek F_Cancelled ArrDelay    Counts 1   AA            Mon       0            6.54609466 2437614 2   US            Mon       0            5.20151371 2268064 3   AS            Mon       0            6.37231471  493475 4   CO            Mon       0            6.49381077 1303473 5   DL            Mon       0            6.63422763 2735223 6   EA            Mon       0            6.13500730  127482 7   HP            Mon       0            6.85447467  521916 8   NW            Mon       0            5.09910096 1520066 9   PA (1)        Mon       0            4.24550765   45021 10  PI            Mon       0            9.32556128  124892 11  PS            Mon       0            7.11355016   12391 12  TW            Mon       0            6.21971889  539726 13  UA            Mon       0            7.51524443 2121168 14  WN            Mon       0            4.11051602 3026077 15  ML (1)        Mon       0            2.05724774   10079 …</source>
        </trans-unit><trans-unit id="216" translate="yes" xml:space="preserve">
          <source>[rows omitted] …</source>
        </trans-unit><trans-unit id="217" translate="yes" xml:space="preserve">
          <source>201 FL            Sun       0            6.91461396  316492 202 OO            Sun       0            6.30954516  755053 203 XE            Sun       0            7.72464706  457166 204 TZ            Sun       0            5.19715263   28658 205 HA            Sun       0           -0.28030915   79184 206 OH            Sun       0            7.12036827  233093 207 F9            Sun       0            5.61844996   93778 208 YV            Sun       0            8.35988986  218992 209 9E            Sun       0            4.18506623  140112 210 VX            Sun       0            5.06036446    7902</source>
        </trans-unit><trans-unit id="218" translate="yes" xml:space="preserve">
          <source>While this particular example will likely run successfully to completion even on a minimally equipped modern computer without setting the <bpt id="p1">*</bpt>useSparseCube<ept id="p1">*</ept> flag to <bpt id="p2">*</bpt>TRUE<ept id="p2">*</ept>, it illustrates how one can quickly start to see the number of zero entries accumulate in an <bpt id="p3">*</bpt>rxCube<ept id="p3">*</ept> computation.</source>
        </trans-unit><trans-unit id="219" translate="yes" xml:space="preserve">
          <source> With larger data sets and a larger number of categorical variable combinations, however, this setting may allow computations of cubes that would not otherwise fit in memory.</source>
        </trans-unit><trans-unit id="220" translate="yes" xml:space="preserve">
          <source>For the <bpt id="p1">*</bpt>rxCrossTabs<ept id="p1">*</ept> function, the <bpt id="p2">*</bpt>useSparseCube<ept id="p2">*</ept> option works exactly the same internally.</source>
        </trans-unit><trans-unit id="221" translate="yes" xml:space="preserve">
          <source>However, because <bpt id="p1">*</bpt>rxCrossTabs<ept id="p1">*</ept> always returns a table, it may require more memory to format its result than <bpt id="p2">*</bpt>rxCube<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="222" translate="yes" xml:space="preserve">
          <source>If you have an extremely large contingency table, we recommend <bpt id="p1">*</bpt>rxCube<ept id="p1">*</ept> with <bpt id="p2">*</bpt>useSparseCube=TRUE<ept id="p2">*</ept> for the greatest chance of completing the computation.</source>
        </trans-unit><trans-unit id="223" translate="yes" xml:space="preserve">
          <source> The <bpt id="p1">*</bpt>useSparseCube<ept id="p1">*</ept> flag may also be used with <bpt id="p2">*</bpt>rxSummary<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="224" translate="yes" xml:space="preserve">
          <source>Tests of Independence on Cross-Tabulated Data</source>
        </trans-unit><trans-unit id="225" translate="yes" xml:space="preserve">
          <source>One common use of contingency tables is to test whether the tabulated variables are independent.</source>
        </trans-unit><trans-unit id="226" translate="yes" xml:space="preserve">
          <source>RevoScaleR includes several tests of independence, all of which expect data in the standard R <bpt id="p1">*</bpt>xtabs<ept id="p1">*</ept> format.</source>
        </trans-unit><trans-unit id="227" translate="yes" xml:space="preserve">
          <source>You can get data in this format from the <bpt id="p1">*</bpt>rxCrossTabs<ept id="p1">*</ept> function by using the argument <bpt id="p2">*</bpt>returnXtabs=TRUE<ept id="p2">*</ept>:</source>
        </trans-unit><trans-unit id="228" translate="yes" xml:space="preserve">
          <source>Tests of Independence on Cross-Tabulated Data</source>
        </trans-unit><trans-unit id="229" translate="yes" xml:space="preserve">
          <source>bigDataDir &lt;- "C:/MRS/Data" bigAirData &lt;- file.path(bigDataDir, "AirOnTime87to12/AirOnTime87to12.xdf") arrDelayXTab &lt;- rxCrossTabs(ArrDel15~ UniqueCarrier:DayOfWeek,     data = bigAirData, blocksPerRead = 30, returnXtabs=TRUE)</source>
        </trans-unit><trans-unit id="230" translate="yes" xml:space="preserve">
          <source>The <ph id="ph1">`blocksPerRead`</ph> argument is ignored if run locally using R Client.</source>
        </trans-unit><trans-unit id="231" translate="yes" xml:space="preserve">
          <source>Learn more...</source>
        </trans-unit><trans-unit id="232" translate="yes" xml:space="preserve">
          <source>You can then use this as input to any of the following functions:</source>
        </trans-unit><trans-unit id="233" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>rxChiSquaredTest<ept id="p1">*</ept>: performs Pearson’s chi-squared test of independence.</source>
        </trans-unit><trans-unit id="234" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>rxFisherTest<ept id="p1">*</ept>: performs Fisher’s exact test of independence.</source>
        </trans-unit><trans-unit id="235" translate="yes" xml:space="preserve">
          <source><bpt id="p1">*</bpt>rxKendallCor<ept id="p1">*</ept>: performs a Kendall tau test of independence.</source>
        </trans-unit><trans-unit id="236" translate="yes" xml:space="preserve">
          <source>There are three flavors of test, a, b, and c; by default, the b flavor, which accounts for ties, is used.</source>
        </trans-unit><trans-unit id="237" translate="yes" xml:space="preserve">
          <source>(In fact, regular <bpt id="p1">*</bpt>rxCrossTabs<ept id="p1">*</ept> or <bpt id="p2">*</bpt>rxCube<ept id="p2">*</ept> output can be used as input to these functions, but they are converted to <bpt id="p3">*</bpt>xtabs<ept id="p3">*</ept> format first, so it is somewhat more efficient to have <bpt id="p4">*</bpt>rxCrossTabs<ept id="p4">*</ept> return the <bpt id="p5">*</bpt>xtabs<ept id="p5">*</ept> format directly.)</source>
        </trans-unit><trans-unit id="238" translate="yes" xml:space="preserve">
          <source>Here we use the <bpt id="p1">*</bpt>arrDelayXTab<ept id="p1">*</ept> data created preceding and perform a Pearson’s chi-squared test of independence on it:</source>
        </trans-unit><trans-unit id="239" translate="yes" xml:space="preserve">
          <source>rxChiSquaredTest(arrDelayXTab)</source>
        </trans-unit><trans-unit id="240" translate="yes" xml:space="preserve">
          <source>Gives the following output:</source>
        </trans-unit><trans-unit id="241" translate="yes" xml:space="preserve">
          <source>Chi-squared test of independence between UniqueCarrier and DayOfWeek  X-squared  df p-value   105645.8 174       0</source>
        </trans-unit><trans-unit id="242" translate="yes" xml:space="preserve">
          <source>For large contingency tables such as this one, the chi-squared test is the tool of choice.</source>
        </trans-unit><trans-unit id="243" translate="yes" xml:space="preserve">
          <source>For smaller tables, particularly those with cells with expected counts fewer than five, Fisher’s exact test is useful.</source>
        </trans-unit><trans-unit id="244" translate="yes" xml:space="preserve">
          <source>On a large table, however, Fisher’s exact test may not be an option.</source>
        </trans-unit><trans-unit id="245" translate="yes" xml:space="preserve">
          <source>For example, if we try it on our airline table, it returns an error:</source>
        </trans-unit><trans-unit id="246" translate="yes" xml:space="preserve">
          <source>rxFisherTest(arrDelayXTab)</source>
        </trans-unit><trans-unit id="247" translate="yes" xml:space="preserve">
          <source>Error in FUN(tbl[, , i], ...) : FEXACT error 40.</source>
        </trans-unit><trans-unit id="248" translate="yes" xml:space="preserve">
          <source>Out of workspace.</source>
        </trans-unit><trans-unit id="249" translate="yes" xml:space="preserve">
          <source>To show the Fisher test, we return to the admissions data from the beginning of the article.</source>
        </trans-unit><trans-unit id="250" translate="yes" xml:space="preserve">
          <source>This time we use <bpt id="p1">*</bpt>rxCrossTabs<ept id="p1">*</ept> to return an <bpt id="p2">*</bpt>xtabs<ept id="p2">*</ept> object:</source>
        </trans-unit><trans-unit id="251" translate="yes" xml:space="preserve">
          <source>UCBADF &lt;- as.data.frame(UCBAdmissions) admissCTabs &lt;- rxCrossTabs(Freq ~ Gender:Admit, data = UCBADF,     returnXtabs=TRUE)</source>
        </trans-unit><trans-unit id="252" translate="yes" xml:space="preserve">
          <source>We then call <bpt id="p1">*</bpt>rxFisherTest<ept id="p1">*</ept> on the resulting table:</source>
        </trans-unit><trans-unit id="253" translate="yes" xml:space="preserve">
          <source>rxFisherTest(admissCTabs) Fisher's Exact Test for Count Data  estimate 1 95% CI Lower 95% CI Upper      p-value    1.840856     1.621356     2.091246 4.835903e-22    HA: two.sided    H0:  odds ratio = 1</source>
        </trans-unit><trans-unit id="254" translate="yes" xml:space="preserve">
          <source>The chi-squared test works equally well on this example:</source>
        </trans-unit><trans-unit id="255" translate="yes" xml:space="preserve">
          <source>rxChiSquaredTest(admissCTabs)</source>
        </trans-unit><trans-unit id="256" translate="yes" xml:space="preserve">
          <source>Chi-squared test of independence between Gender and Admit X-squared df      p-value 91.6096  1 1.055797e-21</source>
        </trans-unit><trans-unit id="257" translate="yes" xml:space="preserve">
          <source>In both cases, we are given indisputable evidence of the independence of our two predictor factors.</source>
        </trans-unit><trans-unit id="258" translate="yes" xml:space="preserve">
          <source>For this example, we could have as easily used the standard R functions <bpt id="p1">*</bpt>chisq.test<ept id="p1">*</ept> and <bpt id="p2">*</bpt>fisher.test<ept id="p2">*</ept>.</source>
        </trans-unit><trans-unit id="259" translate="yes" xml:space="preserve">
          <source>The RevoScaleR enhancements, however, permit <bpt id="p1">*</bpt>rxChisSquaredTest<ept id="p1">*</ept> and <bpt id="p2">*</bpt>rxFisherTest<ept id="p2">*</ept> to work on <bpt id="p3">*</bpt>xtabs<ept id="p3">*</ept> objects with multiple tables.</source>
        </trans-unit><trans-unit id="260" translate="yes" xml:space="preserve">
          <source>For example, if we expand our examination of the admissions data to include the department info, we obtain a multi-way contingency table:</source>
        </trans-unit><trans-unit id="261" translate="yes" xml:space="preserve">
          <source>admissCTabs2 &lt;- rxCrossTabs(Freq ~ Gender:Admit:Dept, data = UCBADF,     returnXtabs=TRUE)</source>
        </trans-unit><trans-unit id="262" translate="yes" xml:space="preserve">
          <source>The chi-squared and Fisher’s exact test results are shown as follows; notice that they provide a test of independence between Gender and Admit for each level of Dept:</source>
        </trans-unit><trans-unit id="263" translate="yes" xml:space="preserve">
          <source>rxChiSquaredTest(admissCTabs2)</source>
        </trans-unit><trans-unit id="264" translate="yes" xml:space="preserve">
          <source>Chi-squared test of independence between Gender and Admit           X-squared df      p-value  Dept==A 16.37177373  1 5.205468e-05  Dept==B  0.08509801  1 7.705041e-01  Dept==C  0.63322380  1 4.261753e-01  Dept==D  0.22159370  1 6.378283e-01  Dept==E  0.80804765  1 3.686981e-01  Dept==F  0.21824336  1 6.403817e-01</source>
        </trans-unit><trans-unit id="265" translate="yes" xml:space="preserve">
          <source>rxFisherTest(admissCTabs2)</source>
        </trans-unit><trans-unit id="266" translate="yes" xml:space="preserve">
          <source>Fisher's Exact Test for Count Data         odds ratio 95% CI Lower 95% CI Upper      p-value  Dept==A  0.3495628    0.1970420    0.5920417 1.669189e-05  Dept==B  0.8028124    0.2944986    2.0040231 6.770899e-01  Dept==C  1.1329004    0.8452173    1.5162918 3.866166e-01  Dept==D  0.9213798    0.6789572    1.2504742 5.994965e-01  Dept==E  1.2211852    0.8064776    1.8385155 3.603964e-01  Dept==F  0.8280944    0.4332888    1.5756278 5.458408e-01    HA: two.sided    H0:  odds ratio = 1</source>
        </trans-unit><trans-unit id="267" translate="yes" xml:space="preserve">
          <source>Like Fisher’s exact test, the Kendall tau correlation test works best on smaller contingency tables.</source>
        </trans-unit><trans-unit id="268" translate="yes" xml:space="preserve">
          <source>Here is an example of what it returns when applied to our admissions data (the results differ from run to run as the underlying algorithm relies on sampling):</source>
        </trans-unit><trans-unit id="269" translate="yes" xml:space="preserve">
          <source>rxKendallCor(admissCTabs2)</source>
        </trans-unit><trans-unit id="270" translate="yes" xml:space="preserve">
          <source>Dept==A -0.13596550   0.000 Dept==B -0.02082575   0.666 Dept==C  0.02865045   0.380 Dept==D -0.01939676   0.585 Dept==E  0.04140240   0.383 Dept==F -0.02319366   0.530    HA: two.sided</source>
        </trans-unit><trans-unit id="271" translate="yes" xml:space="preserve">
          <source>Odds Ratios and Risk Ratios</source>
        </trans-unit><trans-unit id="272" translate="yes" xml:space="preserve">
          <source>Another common task associated with 2 x 2 contingency tables is the calculation of odds ratios and risk ratios (also known as relative risk).</source>
        </trans-unit><trans-unit id="273" translate="yes" xml:space="preserve">
          <source>The two functions <bpt id="p1">*</bpt>rxOddsRatio<ept id="p1">*</ept> and <bpt id="p2">*</bpt>rxRiskRatio<ept id="p2">*</ept> in RevoScaleR can be used to compute these quantities.</source>
        </trans-unit><trans-unit id="274" translate="yes" xml:space="preserve">
          <source>The odds ratio and the risk ratio are closely related: the odds ratio computes the relative odds of an event among two or more groups, while the risk ratio computes the relative probabilities of an event.</source>
        </trans-unit><trans-unit id="275" translate="yes" xml:space="preserve">
          <source>Consider again the contingency table <bpt id="p1">*</bpt>admissCTabs<ept id="p1">*</ept>:</source>
        </trans-unit><trans-unit id="276" translate="yes" xml:space="preserve">
          <source>Odds Ratios and Risk Ratios</source>
        </trans-unit><trans-unit id="277" translate="yes" xml:space="preserve">
          <source>admissCTabs</source>
        </trans-unit><trans-unit id="278" translate="yes" xml:space="preserve">
          <source>Gender   Admitted Rejected   Male       1198     1493   Female      557     1278</source>
        </trans-unit><trans-unit id="279" translate="yes" xml:space="preserve">
          <source>In this example, the odds of being admitted as a male are 1198/1493, or about 4 to 5 against.</source>
        </trans-unit><trans-unit id="280" translate="yes" xml:space="preserve">
          <source>The odds of being admitted as a female are 557/1278, or about 4 to 9 against.</source>
        </trans-unit><trans-unit id="281" translate="yes" xml:space="preserve">
          <source>The odds ratio is (1198/1493)/(557/1278), or 1.8 greater odds that a male will be admitted as opposed to a woman.</source>
        </trans-unit><trans-unit id="282" translate="yes" xml:space="preserve">
          <source>rxOddsRatio(admissCTabs)</source>
        </trans-unit><trans-unit id="283" translate="yes" xml:space="preserve">
          <source>data:</source>
        </trans-unit><trans-unit id="284" translate="yes" xml:space="preserve">
          <source>Z = 0.6104, p-value &lt; 2.2e-16 alternative hypothesis: two.sided 95 percent confidence interval: 1.624377 2.086693 sample estimates: oddsRatio 1.84108</source>
        </trans-unit><trans-unit id="285" translate="yes" xml:space="preserve">
          <source>The risk ratio, by contrast, compares the probabilities of being <bpt id="p1">*</bpt>rejected<ept id="p1">*</ept>, that is, 1493/(1198+1493) for a man versus 1278/(557+1278) for a woman.</source>
        </trans-unit><trans-unit id="286" translate="yes" xml:space="preserve">
          <source>So here the risk ratio is 0.697 (the probability of a woman being rejected) divided by 0.555 (the probability of a man being rejected), or 1.255:</source>
        </trans-unit><trans-unit id="287" translate="yes" xml:space="preserve">
          <source>rxRiskRatio(admissCTabs)</source>
        </trans-unit><trans-unit id="288" translate="yes" xml:space="preserve">
          <source>data:</source>
        </trans-unit><trans-unit id="289" translate="yes" xml:space="preserve">
          <source>Z.Female = 0.2274, p-value &lt; 2.2e-16 alternative hypothesis: two.sided 95 percent confidence interval: 1.199631 1.313560 sample estimates: riskRatio.Female 1.255303</source>
        </trans-unit></group></body></file></xliff>