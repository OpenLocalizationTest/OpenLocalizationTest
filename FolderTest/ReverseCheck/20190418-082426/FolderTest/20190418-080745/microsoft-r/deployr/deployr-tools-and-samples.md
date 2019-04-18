---
title: 'DeployR Application Developer Tools and Docs - DeployR 8.x '
description: DeployR Application Developer Tools and Docs
keywords: ''
author: HeidiSteen
ms.author: heidist
manager: cgronlun
ms.date: 11/10/2017
ms.topic: conceptual
ms.prod: mlserver
ms.openlocfilehash: b1eb4eb6df8790c69628985df6aaf92fb279ad29
ms.sourcegitcommit: 9c76acdc-560c-45e5-982b-fef069067335
ms.translationtype: HT
ms.contentlocale: en-US
ms.lasthandoff: 04/18/2019
---
# <a name="developer-tools-api-docs-and-samples"></a>Developer Tools, API Docs, and Samples

**Applies to: DeployR 8.x**   (See [comparison between 8.x and 9.x](../whats-new-in-r-server.md#8vs9))

>Looking to deploy with Machine Learning Server? [Start here](../what-is-operationalization.md).

Get started with DeployR! Use the **RBroker framework** and/or the **client libraries** to communicate with the DeployR server. 

On this page, you can download the framework/library in one of the available languages, follow their tutorials, and consult the comprehensive documentation.

## <a name="rbroker-framework"></a>RBroker Framework

The RBroker Framework is the simplest way to integrate R Analytics into any Java, JavaScript or .NET application. Submit as many R tasks as your application needs. No need to manage client-side request queues or block for results. Let this framework handle all of the complexity while you enjoy effortless scale. Simply define an RTask, submit your task to an instance of RBroker and then retrieve your RTaskResult. It really is that simple.

1. Read the [ **RBroker Framework Tutorial**](deployr-rbroker-framework.md)

2. Get the documentation and download the library for your preferred programming language:
   - **Java**: &nbsp;&nbsp;&nbsp;  &nbsp;&nbsp;&nbsp; &nbsp; &nbsp;&nbsp;&nbsp;[API Doc](http://microsoft.github.io/java-rbroker-framework/) &nbsp;|&nbsp; [Download](https://github.com/microsoft/java-rbroker-framework/releases)  
   - **JavaScript**: &nbsp;&nbsp; [API Doc](http://microsoft.github.io/js-rbroker-framework) &nbsp;|&nbsp; [Download](https://github.com/Microsoft/js-rbroker-framework/releases)  
   - **.NET**: &nbsp;&nbsp;&nbsp;  &nbsp;&nbsp;&nbsp; &nbsp; &nbsp;&nbsp;&nbsp;[API Doc](https://github.com/Microsoft/dotnet-rbroker-framework/releases) &nbsp;|&nbsp; [Download](https://github.com/Microsoft/dotnet-rbroker-framework/releases)<br />  &nbsp; 

3. Explore the RBroker Framework examples for [Java](https://github.com/Microsoft/java-example-rbroker-basics), [JavaScript](https://github.com/Microsoft/js-rbroker-framework), and [.NET](https://github.com/Microsoft/dotnet-rbroker-framework). Find them under the `examples` directory of each GitHub repository. Check out additional sample applications that use the client library or RBroker for [Java](https://github.com/Microsoft/?utf8=%E2%9C%93&query=java-example) and [JavaScript](https://github.com/Microsoft/?utf8=✓&query=js-example).

## <a name="client-libraries"></a>Client Libraries

The DeployR API exposes a wide range of R analytics services to client application developers. If the RBroker Framework doesn't give you exactly what you need then you can get access to the full DeployR API using our client libraries. We currently provide native client library support for Java, JavaScript or .NET developers.

1.  Read the [**Client Library Tutorial**](deployr-client-library.md)

1.  Get the documentation and download the library for your preferred programming language:
    - **Java**: &nbsp;&nbsp;&nbsp;  &nbsp;&nbsp;&nbsp; &nbsp; &nbsp;&nbsp;&nbsp;[API Doc](http://microsoft.github.io/java-client-library/) &nbsp;|&nbsp; [Download](https://github.com/Microsoft/java-client-library/releases)
    - **JavaScript**: &nbsp;&nbsp; [API Doc](https://microsoft.github.io/js-client-library) &nbsp;|&nbsp; [Download](https://github.com/Microsoft/js-client-library/releases)  
    - **.NET**: &nbsp;&nbsp;&nbsp;  &nbsp;&nbsp;&nbsp; &nbsp; &nbsp;&nbsp;&nbsp;[API Doc](https://github.com/Microsoft/dotnet-client-library/releases) &nbsp;|&nbsp; [Download](https://github.com/Microsoft/dotnet-client-library/releases)  <br />  &nbsp;

1.  Explore the client library examples for [Java](https://github.com/Microsoft/java-example-client-basics), [JavaScript](https://github.com/Microsoft/js-client-library/releases), and [.NET](https://github.com/Microsoft/dotnet-client-library). Find them under the `examples` directory of each GitHub repository. Check out additional sample applications that use the client library or RBroker for [Java](https://github.com/Microsoft/?utf8=%E2%9C%93&query=java-example) and [JavaScript](https://github.com/Microsoft/?utf8=✓&query=js-example).

## <a name="api-reference-and-tools"></a>API Reference and Tools

Need to integrate DeployR-powered R Analytics using a different programming language? The [API Reference guide](deployr-api-reference.md) details everything you need to know to get up and running. 

Also described is the [API Explorer tool](deployr-api-explorer-tool.md) used to interactively learn the DeployR API. 