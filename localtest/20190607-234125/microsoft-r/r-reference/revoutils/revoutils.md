---
title: 'RevoUtils Functions R Package for Microsoft R '
description: A package providing utility functions useful for script running on the Microsoft R ScaleR engine.
keywords: RevoUtils package reference
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 01/29/2018
ms.topic: reference
ms.prod: mlserver
ms.openlocfilehash: 9fc2a44f21c50303a4530c06aad19e42cc3874ff
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="revoutils-package"></a>RevoUtils package 

The **RevoUtils** package provides utility functions that return information about your installation, such as path and memory usage.

| Package details | |
|--------|-|
| Current version: |  10.0.5 |
| Built on: | R 3.4.3 |
| Package distribution: | [Machine Learning Server](../../what-is-machine-learning-server.md) </br>[R Client (Windows and Linux)](../../r-client/what-is-microsoft-r-client.md) <br/>[R Server 9.1 and earlier](../../what-is-microsoft-r-server.md)   <br/>[SQL Server 2016 and later (Windows only)](https://docs.microsoft.com/sql/advanced-analytics/getting-started-with-machine-learning-services)   <br/> [Azure HDInsight](https://docs.microsoft.com/azure/hdinsight/hdinsight-hadoop-r-server-get-started) <br/>[Azure Data Science Virtual Machines](https://docs.microsoft.com/azure/machine-learning/machine-learning-data-science-provision-vm) |


## <a name="how-to-use-revoutils"></a>How to use RevoUtils

From any R console window, you can call **RevoUtils** functions in an R session. You might want to check on memory usage if your script is crashing or performance is slow. If you get file not found errors, you can use these functions to quickly determine the location of the Home directory or packages installed with Microsoft R.

In an R session, load **RevoUtils** from the command line by typing`library(RevoUtils)`.

## <a name="function-list"></a>Function list

|Class | Description |
|------|-------------|
|[getRevoRepos](getrevorepos.md) | Path to the package repositories. |
|[readNews](readnews.md)  | Read R or package NEWS files.|
|[Revo.home](revo-home.md)  | Path the Home directory. |
|`RevoInfo](revoinfo.md)  | Functions giving information about Microsoft R.|
|[totalSystemMemory](totalsystemmemory.md) |Uses operating system tools to return total system memory. |

## <a name="next-steps"></a>Next steps

Add R packages to your computer by running setup for R Server or R Client: 

+ [R Client](../../r-client/what-is-microsoft-r-client.md) 
+ [R Server](../../what-is-microsoft-r-server.md)

## <a name="see-also"></a>See also

 [Package Reference](../introducing-r-server-r-package-reference.md)    
