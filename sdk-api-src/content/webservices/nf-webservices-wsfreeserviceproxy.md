---
UID: NF:webservices.WsFreeServiceProxy
title: WsFreeServiceProxy function (webservices.h)
author: windows-sdk-content
description: Releases the memory associated with a Service Proxy resource.
old-location: wsw\wsfreeserviceproxy.htm
tech.root: wsw
ms.assetid: fb200cf8-c1d4-4a97-afef-f7c4ed5efb10
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: WsFreeServiceProxy, WsFreeServiceProxy function [Web Services for Windows], webservices/WsFreeServiceProxy, wsw.wsfreeserviceproxy
ms.topic: function
req.header: webservices.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: WebServices.lib
req.dll: WebServices.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - WebServices.dll
api_name:
 - WsFreeServiceProxy
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# WsFreeServiceProxy function


## -description


Releases the memory associated with  a Service Proxy resource.
            


## -parameters




### -param serviceProxy [in]

A pointer to the <b>Service Proxy</b> to release.  The pointer must reference a valid <a href="https://msdn.microsoft.com/623766ae-fe82-40f9-93c8-e78fe48bc6d1">WS_SERVICE_PROXY</a> object
                    returned by <a href="https://msdn.microsoft.com/9215684b-979e-48ad-b4ee-2ae1db1e3034">WsCreateServiceProxy</a>. The referenced value may not be <b>NULL</b>.
                


## -returns



This function does not return a value.




## -remarks



For details of when it is allowed to call this function, see <a href="https://msdn.microsoft.com/e1a5bf5e-dbc1-43e3-981b-7db4caa08bdc">Service Proxy</a> .
            



