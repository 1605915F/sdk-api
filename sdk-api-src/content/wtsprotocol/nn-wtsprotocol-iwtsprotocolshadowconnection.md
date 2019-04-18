---
UID: NN:wtsprotocol.IWTSProtocolShadowConnection
title: IWTSProtocolShadowConnection (wtsprotocol.h)
author: windows-sdk-content
description: IWTSProtocolShadowConnection is no longer available. Instead, use IWRdsProtocolShadowConnection.
old-location: termserv\iwtsprotocolshadowconnection.htm
tech.root: TermServ
ms.assetid: 83285a6a-903f-4c23-8f62-b04bbeaa52f9
ms.author: windowssdkdev
ms.date: 12/05/2018
ms.keywords: IWTSProtocolShadowConnection, IWTSProtocolShadowConnection interface [Remote Desktop Services], IWTSProtocolShadowConnection interface [Remote Desktop Services],described, termserv.iwtsprotocolshadowconnection, wtsprotocol/IWTSProtocolShadowConnection
ms.topic: interface
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
 - wtsprotocol.h
api_name:
 - IWTSProtocolShadowConnection
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWTSProtocolShadowConnection interface


## -description


<p class="CCE_Message">[<b>IWTSProtocolShadowConnection</b> is no longer available for use as of Windows Server 2012. Instead, use <a href="https://msdn.microsoft.com/d23c4902-4e61-45ff-8a49-62eea1b92d4a">IWRdsProtocolShadowConnection</a>.]

Exposes methods that notify the protocol provider about the status of session shadowing. The <b>IWTSProtocolShadowConnection</b> interface can also be used to exchange information between the shadow client and the shadow target. This interface is implemented by the protocol provider, and its methods are called by the Remote Desktop Services service.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWTSProtocolShadowConnection</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWTSProtocolShadowConnection</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWTSProtocolShadowConnection</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/437983a4-48a4-4b37-99ba-35fe1f03b3ec">DoTarget</a>
</td>
<td align="left" width="63%">
Requests that the protocol start the target side of a shadow connection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/7bfe0c45-551f-47bb-a855-6965fed224dc">Start</a>
</td>
<td align="left" width="63%">
Notifies the protocol that shadowing has started.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/629b82cb-7bf3-4a83-bc96-a1e6a757f974">Stop</a>
</td>
<td align="left" width="63%">
Notifies the protocol that shadowing has stopped.

</td>
</tr>
</table> 

