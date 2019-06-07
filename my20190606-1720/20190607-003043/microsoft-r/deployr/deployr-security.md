---
title: " Security in DeployR - DeployR 8.x "
description: 'Security in DeployR: Authentication, HTTPS, SSL, and access controls for server, Project file and Repository File, and more.'
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 11/10/2017
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: 37f76ff980ada0e41014d58a0d61bf94886dd58a
ms.sourcegitcommit: 5a1af0c1-a46b-4161-9fcd-2c6c2f004c37
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="overview-of-deployr-security"></a>Overview of DeployR Security

DeployR is a server framework that exposes the R platform as a service to allow the integration of R statistics, analytics, and visualizations inside Web, desktop, and mobile applications. In addition to providing a simple yet powerful Web services API, the framework also supports a highly flexible, enterprise security model.

By default, DeployR supports basic authentication. Users simply provide plain text username and password credentials, which are then matched against user account data stored in the DeployR database. User accounts are created and managed by an administrator using the DeployR Administration Console. Given these credentials are passed from client to server as plain text, we strongly recommend, in your production environments, that you [enable and use HTTPS connections](../operationalize/configure-https.md) every time your application attempts to authenticate with DeployR. 

While basic authentication provides a simple and reliable authentication solution, the ability to deliver a seamless integration with existing enterprise security solutions is often paramount. The DeployR enterprise security model can easily be configured to "plug" into a number of widely adopted enterprise security solutions.

>**Get More DeployR Power:** Basic Authentication is available for all DeployR configurations and editions.  
>Get DeployR Enterprise today to take advantage of great DeployR features like enterprise security and [a scalable grid framework](deployr-admin-managing-the-grid.md). Note that DeployR Enterprise is part of Microsoft R Server.

The DeployR security model is sufficiently flexible that it can work with multiple enterprise security solutions at the same time. As such, DeployR Enterprise ships with a number of security providers that together represent a provider-chain upon which user credentials are evaluated. For more information, see [Authentication and Authorization](../operationalize/configure-authentication.md). Every aspect of the DeployR security model is controlled by the configuration properties found in the DeployR external configuration file. This file can be found at `$DEPLOYR_HOME/deployr/deployr.groovy`.

The following security topics detail how to work with these configuration properties to achieve your preferred security implementation.
+ [Authorization and Authentication](../operationalize/configure-authentication.md)
+ [HTTPS and SSL Support](../operationalize/configure-https.md)
+ [Server Access Policies](deployr-security-server-access.md)
+ [Project and Repository File Access Controls](deployr-security-project-access.md)
+ [Password Policies](deployr-security-passwords.md)
+ [Account Locking Policies](deployr-security-account-locking.md)
+ [RServe Execution Context](deployr-security-rserve-execution-context.md)
