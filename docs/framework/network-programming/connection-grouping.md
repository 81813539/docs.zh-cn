---
title: "连接分组"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.tgt_pltfrm: 
ms.topic: article
dev_langs:
- VB
- CSharp
- C++
- jsharp
helpviewer_keywords:
- Internet, connections
- connections [.NET Framework], grouping
- WebRequest class, connection grouping
- network resources, connections
- connection pooling
ms.assetid: 2ec502e8-4ba0-4c22-9410-f28eaf4eee63
caps.latest.revision: 7
author: mcleblanc
ms.author: markl
manager: markl
ms.translationtype: HT
ms.sourcegitcommit: 306c608dc7f97594ef6f72ae0f5aaba596c936e1
ms.openlocfilehash: 8f16a539bb7c2bef494c7b5551e1f12bc71de60f
ms.contentlocale: zh-cn
ms.lasthandoff: 08/21/2017

---
# <a name="connection-grouping"></a>连接分组
连接分组将单个应用程序内的特定请求与已定义连接池相联系。 代表用户连接到后端服务器并使用支持委托的身份验证协议（如 Kerberos）的中间层应用程序，或提供其自身凭据的中间层应用程序可要求连接分组，如以下示例所示。 例如，假设用户 Joe 访问显示其工资信息的内部网站。 对 Joe 进行身份验证之后，中间层应用程序服务器使用 Joe 的凭据连接到后端服务器来检索他的工资信息。 接下来 Susan 访问该站点，并请求她的工资信息。 因为中间层应用程序已使用 Joe 的凭据完成了连接，所以后端服务器会使用 Joe 的信息进行响应。 但是，如果应用程序将发送到后端服务器的每个请求分配给由用户名形成的连接组，那么每个用户将属于单独的连接池，并且不会意外地与其他用户分享身份验证信息。  
  
 若要将请求分配到特定的连接组，必须在进行请求之前分为 <xref:System.Net.WebRequest> 的 <xref:System.Net.WebRequest.ConnectionGroupName%2A> 属性分配名称。  
  
## <a name="see-also"></a>另请参阅  
 [管理连接](../../../docs/framework/network-programming/managing-connections.md)   
 [如何：将用户信息分配给组连接](../../../docs/framework/network-programming/how-to-assign-user-information-to-group-connections.md)

