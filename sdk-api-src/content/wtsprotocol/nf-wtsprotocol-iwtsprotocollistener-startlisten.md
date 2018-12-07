---
UID: NF:wtsprotocol.IWTSProtocolListener.StartListen
title: IWTSProtocolListener::StartListen
author: windows-sdk-content
description: IWTSProtocolListener::StartListen is no longer available. Instead, use IWRdsProtocolListener::StartListen.
old-location: termserv\iwtsprotocollistener_startlisten.htm
tech.root: termserv
ms.assetid: d922ea90-a4eb-4495-947c-ef33bd81f40a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWTSProtocolListener interface [Remote Desktop Services],StartListen method, IWTSProtocolListener.StartListen, IWTSProtocolListener::StartListen, StartListen, StartListen method [Remote Desktop Services], StartListen method [Remote Desktop Services],IWTSProtocolListener interface, termserv.iwtsprotocollistener_startlisten, wtsprotocol/IWTSProtocolListener::StartListen
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wtsprotocol.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows Server 2008 R2
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Wtsprotocol.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Wtsprotocol.h
api_name:
 - IWTSProtocolListener.StartListen
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWTSProtocolListener::StartListen


## -description


<p class="CCE_Message">[<b>IWTSProtocolListener::StartListen</b> is no longer available for use as of Windows Server 2012. Instead, use <a href="https://msdn.microsoft.com/d3797411-2ac6-4d3c-8c90-5c566e6d8fa8">IWRdsProtocolListener::StartListen</a>.]

 Notifies the protocol to start listening for client connection requests.


## -parameters




### -param pCallback [in]

A pointer to an <a href="https://msdn.microsoft.com/607fcb85-4602-4651-b246-3e32c8868e47">IWTSProtocolListenerCallback</a> object 
implemented by the Remote Desktop Servicesservice. The protocol uses the 
<b>IWTSProtocolListenerCallback</b> object to notify 
the 

Remote Desktop Services 
service about incoming connection requests. The protocol must add a reference to this object and release it when 
<a href="https://msdn.microsoft.com/5c5b09d3-74d6-4067-b18b-ed2a54af4153">StopListen</a> is called.


## -returns



When you are implementing this method, return <b>S_OK</b> if the function succeeds. If it fails, 
return an <b>HRESULT</b> value that indicates the error. For a list of common error codes, 
see <a href="https://msdn.microsoft.com/ce52efc3-92c7-40e4-ac49-0c54049e169f">Common HRESULT Values</a>.




## -remarks



The <b>StartListen</b> method is called when the Remote Desktop Services service starts.

<ol>
<li>The Remote Desktop Services service calls <a href="https://msdn.microsoft.com/7295a55b-12c7-4ed0-a7a4-9ecee16afdec">CoCreateInstance</a> to create an  <a href="https://msdn.microsoft.com/a54bdb46-b18b-4a6d-90fc-75947f6dd191">IWTSProtocolManager</a> object.</li>
<li>The Remote Desktop Services service calls <a href="https://msdn.microsoft.com/2c947181-5cac-40c1-b993-537b580efafe">CreateListener</a> on the <a href="https://msdn.microsoft.com/a54bdb46-b18b-4a6d-90fc-75947f6dd191">IWTSProtocolManager</a> interface. The protocol creates an <a href="https://msdn.microsoft.com/b11eb19f-ffc3-4a68-85c6-90a2412168f8">IWTSProtocolListener</a> object and passes it back to the Remote Desktop Services service.</li>
<li>The Remote Desktop Services service calls <b>StartListen</b> on the <a href="https://msdn.microsoft.com/b11eb19f-ffc3-4a68-85c6-90a2412168f8">IWTSProtocolListener</a> object.</li>
</ol>



## -see-also




<a href="https://msdn.microsoft.com/b11eb19f-ffc3-4a68-85c6-90a2412168f8">IWTSProtocolListener</a>
 

 

