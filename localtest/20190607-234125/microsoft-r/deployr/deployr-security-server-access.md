---
title: 'Security: Server Access Controls - DeployR 8.x '
description: 'Security in DeployR: Authentication, HTTPS, SSL, and access controls for server, Project file and Repository File, and more.'
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 11/10/2017
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: 3a0767cd8c1f84e0183e6cd42fe28484e368fb8e
ms.sourcegitcommit: 482448f7-1a28-4b2f-b7c2-911be7144b02
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 06/07/2019
---
# <a name="server-access-controls-for-deployr"></a>Server Access Controls for DeployR

Learn about the following server access controls.

<br/>
### <a name="working-with-ip-address-filters"></a>Working with IP Address Filters

While access to DeployR is typically controlled by [authentication mechanisms](../operationalize/configure-authentication.md), DeployR also supports access controls based on IP address filters. Under the [**Server Policies**](deployr-admin-managing-server-policies.md#server-policy-properties) tab in the DeployR Administration Console, you can configure your IP address filter policy. The **Operation Policies** for authenticated, asynchronous, and anonymous operations each support an [IP filter](deployr-admin-managing-server-policies.md#server-policy-properties) property. If you assign an IP filter to this property, then any attempt by a client application to connect from outside of the IP address range on that filter will be automatically rejected.

For example, you can make your DeployR server instance accessible only from IP addresses on the local LAN or VPN, such as `192.168.1.xxx` or `10.xxx.xxx.xxx`. Note that it is possible to achieve these same kinds of access controls with an appropriate configuration on your firewall and/or routers.


<br/>
### <a name="cross-origin-resource-sharing"></a>Cross-Origin Resource Sharing

Cross-Origin Resource Sharing (CORS) enables your client application to freely communicate and make cross-site HTTP requests for resources from a domain other than where the DeployR is hosted.  CORS can be enabled or disabled in the DeployR external configuration file, `$DEPLOYR_HOME\deployr\deployr.groovy`. In DeployR Enterprise, support for CORS is disabled by default.

**To enable CORS support:**

1. Update the relevant properties in ``$DEPLOYR_HOME\deployr\deployr.groovy` by setting `cors.enabled = true`.

   ```
   /*
   * DeployR CORS Policy Configuration
   *
   * cors.headers = [ 'Access-Control-Allow-Origin': 'http://app.example.com']
   */
   cors.enabled = false
   ```

2. Optionally, to restrict cross-site HTTP requests to only those requests coming from a specific domain, specify a value for `Access-Control-Allow-Origin` on the `cors.headers` property.

3. [Stop and restart the DeployR server](deployr-common-administration-tasks.md#startstop).
