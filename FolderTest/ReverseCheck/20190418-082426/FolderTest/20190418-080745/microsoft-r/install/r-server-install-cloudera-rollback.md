---
title: R Server installation on Cloudera CDH
description: Install Microsoft R Server 9.1.0 on the Cloudera distribution of Apache Hadoop (CDH).
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 03/29/2017
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: 0022d881cc73f585e4d8da054c723dee1267e13f
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="rollback-to-previous-version"></a>Rollback to previous version

**Applies to:** R Server 9.1.0 on the Cloudera distribution of Apache Hadoop (CDH)

If you deployed and activated Microsoft R Server using a parcel and Custom Service Descriptor (CSD), you have the option of rolling back the active deployment in Cloudera Manager. You might do this if there is an older version of R Server in your cluster that you want to use instead.

> [!Note]
> You can have multiple versions of R Server in Cloudera, but only can be active at any given time.

1. In Cloudera Manager, click the Parcel icon to open the parcel list.

2. Find MRS and click **Deactivate**.

The parcel still exists, but R Server is not operational in the cluster.

The above steps only work for 9.1.0 and later. If you have an older version of R Server, see [Install R Server 9.0.1 on CDH](r-server-install-cloudera-901.md) for information about how it was installed.

## <a name="see-also"></a>See Also

[Install R Server 9.1.0 on the Cloudera distribution of Apache Hadoop (CDH)](r-server-install-cloudera.md)
