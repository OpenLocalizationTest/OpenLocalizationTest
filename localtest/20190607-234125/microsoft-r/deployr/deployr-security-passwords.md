---
title: " Security - DeployR 8.x "
description: 'Security in DeployR: Authentication, HTTPS, SSL, and access controls for server, Project file and Repository File, and more.'
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 11/10/2017
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: 1d23edd3340303d21bb01cacdd31f33b1a4ec3d0
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="password-policies"></a>Password Policies

>[!Important]
>This topic applies to DeployR 8.0.0 and earlier. It does not apply to DeployR for Microsoft R Server 8.0.5 

To customize password constraints on user account passwords adjust the password policy configuration properties.

The `deployr.security.password.min.characters` property enforces a minimum length for any basic authentication password. The `deployr.security.password.upper.case` property, when enabled, enforces the requirement for user passwords to contain at least a single uppercase character. The `deployr.security.password.alphanumeric`property, when enabled, enforces the requirement for user passwords to contain both alphabetic and numeric characters.

```
/*
* DeployR Password Policy Configuration
*
* Note: enable password.upper.case if basic-auth users
* are required to have at least one upper case character
* in their password.
*/
deployr.security.password.min.characters = 8
deployr.security.password.upper.case = true
deployr.security.password.alphanumeric = true
```
    
These policies affect basic authentication only and have no impact on CA Single Sign On, LDAP/AD or PAM authentication where passwords are maintained and managed outside of the DeployR database.