---
title: remoteCommandLine function (mrsdeploy) | Microsoft Docs
description: " Displays the 'REMOTE>' command prompt and provides a remote execution context.  All R commands entered at the R console will be executed in the remote R session. "
keywords: (mrsdeploy), remoteCommandLine
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
ms.openlocfilehash: ec4fe70c0d0f2e7b70fbd8fb263474d4d7ec460b
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
 # <a name="remotecommandline-display-the-remote-command-prompt"></a>remoteCommandLine: Display the 'REMOTE>' command prompt. 
 ## <a name="description"></a>Description

Displays the 'REMOTE>' command prompt and provides a remote execution context.  All R commands entered at the R console will be executed in the remote R session.


 ## <a name="usage"></a>Usage

```   
  remoteCommandLine(prompt = "REMOTE> ", displayPlots = TRUE,
    writePlots = FALSE, recPlots = TRUE)

```

 ## <a name="arguments"></a>Arguments



 ### `prompt`
 The command prompt to be shown when in 'REMOTE' mode. 



 ### `displayPlots`
 If `TRUE`, plots generated during execution are displayed in the local plot window. **NOTE** This capability requires that the '`png`' package is installed on the local machine. 



 ### `writePlots`
 If `TRUE`, plots generated during execution are copied to the working directory of the local session. 



 ### `recPlots`
 If `TRUE`, plots will be created using the '`recordPlot`' function in R. 



 ## <a name="details"></a>Details

Complete documentation: [`https://go.microsoft.com/fwlink/?linkid=836352`](https://go.microsoft.com/fwlink/?linkid=836352)


Once the 'REMOTE>' command prompt is shown, these commands become available: `pause()` #when entered, switches back to the local R session command prompt and local execution context.  
`exit` #exit and logout from the remote session.


 ## <a name="see-also"></a>See Also

[resume](resume.md)

 ## <a name="examples"></a>Examples

 ```

  ## Not run:

remoteCommandLine()

#switch from REMOTE command prompt back to the local command prompt.
REMOTE>pause()

#switch from local command prompt back to the REMOTE command prompt.
>resume()

#exit and logout from the remote session.
REMOTE>exit
 ## End(Not run) 
```

