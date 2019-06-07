---
title: remoteExecute function (mrsdeploy) | Microsoft Docs
description: " Base function for executing a block of R code or an R script in the remote R session "
keywords: (mrsdeploy), remoteExecute
author: heidisteen
manager: cgronlun
ms.date: 01/18/2019
ms.topic: reference
ms.prod: microsoft-r
ms.service: ''
ms.assetid: ''
ROBOTS: ''
audience: ''
ms.devlang: ''
ms.reviewer: ''
ms.suite: ''
ms.tgt_pltfrm: ''
ms.technology: r-server
ms.custom: ''
ms.openlocfilehash: f43bc96a3c1d474386ddb5e256cc4b9a4d65badb
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="remoteexecute-remote-execution-of-either-r-code-or-an-r-script"></a>remoteExecute: Remote execution of either R code or an R script. 
 ## <a name="description"></a>Description

Base function for executing a block of R code or an R script in the remote R session


 ## <a name="usage"></a>Usage

```   
  remoteExecute(rcode, script = FALSE, inputs = NULL, outputs = NULL,
    displayPlots = FALSE, writePlots = FALSE, recPlots = FALSE)

```

 ## <a name="arguments"></a>Arguments



 ### `rcode`
 The R code, or an R Script file to be executed 



 ### `script`
 If `TRUE`, treat the `rcode` parameter as a R script file name 



 ### `inputs`
 JSON encoded string of R objects that are loaded into the Remote R session's workspace prior to execution.  Only R objects of type: primitives, vectors and dataframes are supported via this parameter.  Alternatively the [putLocalObject](putLocalObject.md) can be used, prior to a call to this function, to move any R object from the local workspace into the  remote R session. 



 ### `outputs`
 Character vector of the names of the objects to retrieve.  Only primitives, vectors and dataframes can be retrieved using this function  Use [getRemoteObject](getRemoteObject.md)to get any type of R object from the remote session 



 ### `displayPlots`
 If `TRUE`, plots generate during execution are displayed in the local plot window. **NOTE** This capability requires that the '`png`' package is installed on the local machine 



 ### `writePlots`
 If `TRUE`, plots generated during execution are copied to the working directory of the local session 



 ### `recPlots`
 If `TRUE`, plots will be created using the '`recordPlot`' function in R 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)


The console output will be refreshed at a recurring rate. the default is 5000 milliseconds (5 seconds). By setting the option 'mrsdeploy.console_update', you can override this value (i.e. options(mrsdeploy.console_update=7000) Use caution when changing this value to something less than 5000 ms, as it may place a necessary load on the deployr server.  
Values less than 1000 will disable refreshing of the console.


 ## <a name="value"></a>Value

A list containing the results of the execution

 ## <a name="see-also"></a>See Also

[remoteScript](remoteScript.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

#execute a block of R code
resp<-remoteExecute("x<-rnorm(10);y<-rnorm(10);plot(x,y)", writePlots=TRUE)

#execute an R script
resp<-remoteExecute("c:/myScript.R", script=TRUE)

#specify 2 inputs to the script and retrieve 2 outputs.  The supported types for inputs and 
#outputs are: primitives, vectors and dataframes.
data<-'[{"name":"x","value":120}, {"name":"y","value":130}]'
resp<-remoteExecute("c:/myScript.R", script=TRUE, inputs=data, outputs=c("out1", "out2"), writePlots=TRUE)

#alternative using 4 calls
x<-120;y<-130
putLocalObject(c("x","y"))
resp<-remoteExecute("c:/myScript.R", script=TRUE)
getRemoteObject(c("out1", "out2"))
 ## End(Not run) 
```

