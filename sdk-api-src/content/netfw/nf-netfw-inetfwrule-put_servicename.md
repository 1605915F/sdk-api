---
UID: NF:netfw.INetFwRule.put_ServiceName
title: INetFwRule::put_ServiceName
author: windows-sdk-content
description: Specifies the service name property of the application.
old-location: ics\inetfwrule_servicename.htm
tech.root: ics
ms.assetid: 52bcc317-b900-44b6-8ab4-637ffbd74729
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: INetFwRule interface [ICS/ICF],ServiceName property, INetFwRule.ServiceName, INetFwRule.put_ServiceName, INetFwRule::ServiceName, INetFwRule::get_ServiceName, INetFwRule::put_ServiceName, ServiceName property [ICS/ICF], ServiceName property [ICS/ICF],INetFwRule interface, ics.inetfwrule_servicename, netfw/INetFwRule::ServiceName, netfw/INetFwRule::get_ServiceName, netfw/INetFwRule::put_ServiceName, put_ServiceName
ms.topic: method
req.header: netfw.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: FirewallAPI.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - FirewallAPI.dll
api_name:
 - INetFwRule.ServiceName
 - INetFwRule.get_ServiceName
 - INetFwRule.put_ServiceName
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# INetFwRule::put_ServiceName


## -description


Specifies the service name property of the application.

This property is read/write.


## -parameters


## -remarks



This property is optional. A serviceName value of "*" indicates that a service, not an application,  must be sending or receiving traffic.

Also see the restrictions on changing properties described in the Remarks section of the <a href="https://msdn.microsoft.com/59e2a140-bf55-4f0e-bf4b-1a39d3dc0457">INetFwRule</a> interface page.




## -see-also




<a href="https://msdn.microsoft.com/59e2a140-bf55-4f0e-bf4b-1a39d3dc0457">INetFwRule</a>
 

 

