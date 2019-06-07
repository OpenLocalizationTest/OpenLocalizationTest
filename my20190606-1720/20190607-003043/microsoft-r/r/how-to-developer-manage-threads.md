---
title: 'Manage threads in RevoScaleR (Machine Learning Server) '
description: ''
keywords: How ScaleR establishes and manages thread pools for parallel processing.
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 01/03/2018
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: 30209c83085dc65c525727512e783ba6f33bb5c9
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="managing-threads-in-revoscaler"></a>Managing threads in RevoScaleR

RevoScaleR provides functions for managing the thread pool used for parallel execution.

On Windows, thread pool management is enabled and should not be turned off. 

On Linux, thread pool management is turned off by default to avoid interfering with how Unix systems fork processes. Process forking is only available on Unix-based systems. You can turn the thread pool on if you do not fork your R process. RevoScaleR provides an interface to activate the thread pool:

    rxSetEnableThreadPool(TRUE)

Similarly, the thread pool may be disabled as follows:

    rxSetEnableThreadPool(FALSE)

If you want to ensure that the RevoScaleR thread pool is always enabled on Linux, you can add the preceding command to a *.First* function defined in either your own Rprofile startup file, or the system Rprofile.site file. For example, you can add the following lines after the closing right parenthesis of the existing Rprofile.site file:

    .First <- function()
    {
        .First.sys()
        invisible(rxSetEnableThreadPool(TRUE))
    }

The *.First.sys* function is normally run after all other initialization is complete, including the evaluation of the *.First* function. We need the call to *rxSetEnableThreadPool* to occur after RevoScaleR is loaded. That is done by *.First.sys*, so we call *.First.sys* first.


## <a name="see-also"></a>See Also

+ [Machine Learning Server](../what-is-machine-learning-server.md)
+ [How-to guides in Machine Learning Server](how-to-introduction.md)
+ [RevoScaleR Functions](~/r-reference/revoscaler/revoscaler.md)
