---
title: 'Solution templates for Machine Learning Server and R Server | Machine Learning Server '
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 2/16/2018
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: 657f39263e1efbd6c7767be7b77de896f32ed1e8
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="solution-templates-for-machine-learning-server-and-microsoft-r-server-9192"></a>Solution templates for Machine Learning Server and Microsoft R Server 9.1/9.2

Several solution templates exist to help you accelerate time to value when using Machine Learning Server or Microsoft R Server 9.1/9.2. We offer solutions tailored to specific industries and problem sets: [marketing](#marketing), [healthcare](#healthcare), [financial and retail](#financial).


<a name="marketing"></a> 

## <a name="9658-marketing-solutions"></a>&#9658; Marketing solutions 

### <a name="campaign-optimization"></a>Campaign optimization 

When a business launches a marketing campaign to interest customers in new or existing product(s), they often use a set of business rules to select leads for their campaign to target. Machine learning can be used to help increase the response rate from these leads. 
  
This solution demonstrates how to use a model to predict actions that are expected to maximize the purchase rate of leads targeted by the campaign. These predictions serve as the basis for recommendations to be used by a renewed campaign on how to contact (for example, e-mail, SMS, or cold call) and when to contact (day of week and time of day) the targeted leads.

||||
|---|----|--|
||**Learn more:**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>- [Home](https://microsoft.github.io/r-server-campaign-optimization) <br>- [Code](https://github.com/Microsoft/r-server-campaign-optimization)|**Deploy on:**<br>- [SQL Server](https://aka.ms/campaignoptimization)<br>- [HDInsight Spark Cluster](https://aka.ms/campaign-hdi)|

<a name="healthcare"></a> 

## <a name="9658-healthcare-solutions"></a>&#9658; Healthcare solutions

### <a name="predicting-hospital-length-of-stay"></a>Predicting hospital length of stay

This solution enables a predictive model for Length of Stay for in-hospital admissions. Length of Stay (LOS) is defined in number of days from the initial admit date to the date that the patient is discharged from any given hospital facility. There can be significant variation of LOS across various facilities and across disease conditions and specialties even within the same healthcare system. Advanced LOS prediction at the time of admission can greatly enhance the quality of care as well as operational workload efficiency and help with accurate planning for discharges resulting in lowering of various other quality measures such as readmissions.

||||
|---|----|--|
||**Learn more:**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>- [Home](https://microsoft.github.io/r-server-hospital-length-of-stay) <br>- [Code](https://github.com/Microsoft/r-server-hospital-length-of-stay)|**Deploy on:**<br>- [SQL Server](https://aka.ms/hospital-los)<br>&nbsp; |

<a name="financial"></a> 

## <a name="9658-financial-and-retail-solutions"></a>&#9658; Financial and retail solutions

### <a name="loan-credit-risk"></a>Loan credit risk

If we had a crystal ball, we would only loan money to someone if we knew they would pay us back. A lending institution can make use of predictive analytics to reduce the number of loans it offers to those borrowers most likely to default, increasing the profitability of its loan portfolio. This solution is based on simulated data for a small personal loan financial institution, containing the borrower’s financial history as well as information about the requested loan. It uses predictive analytics to help decide whether or not to grant a loan for each borrower.

||||
|---|----|--|
||**Learn more:**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>- [Home](https://microsoft.github.io/r-server-loan-credit-risk/) <br>- [Code](https://github.com/Microsoft/r-server-loan-credit-risk)|**Deploy on:**<br>- [SQL Server](https://aka.ms/loan-credit-risk)<br>- [HDInsight Spark Cluster](https://aka.ms/loan-credit-risk-hdi)|

### <a name="loan-charge-off"></a>Loan charge-off

A charged off loan is a loan that is declared by a creditor (usually a lending institution) that an amount of debt is unlikely to be collected, usually when the loan repayment is severely delinquent by the debtor. Given that high chargeoff has negative impact on lending institutions’ year end financials, lending institutions often monitor loan chargeoff risk closely to prevent loans from getting charged-off. Using Azure HDInsight R Server, a lending institution can leverage machine learning predictive analytics to predict the likelihood of loans getting charged off and run a report on the analytics result stored in HDFS and hive tables.

||||
|---|----|--|
||**Learn more:**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>- [Home](https://microsoft.github.io/r-server-loan-chargeoff) <br>- [Code](https://github.com/Microsoft/r-server-loan-chargeoff/)|**Deploy on:**<br>- [SQL Server](https://aka.ms/loanchargeoffsql)<br>- [HDInsight Spark Cluster](https://aka.ms/loanchargeoffhdi)|

### <a name="fraud-detection"></a>Fraud detection

Fraud detection is one of the earliest industrial applications of data mining and machine learning. This solution shows how to build and deploy a machine learning model for online retailers to detect fraudulent purchase transactions.

||||
|---|----|--|
||**Learn more:**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>- [Home](https://microsoft.github.io/r-server-fraud-detection/) <br>- [Code](https://github.com/Microsoft/r-server-fraud-detection)|**Deploy on:**<br>- [SQL Server](https://aka.ms/fraud-detection)<br>- [HDInsight Spark Cluster](https://aka.ms/fraud-detectinon-hdi)|
