---
UID: NN:tsvirtualchannels.IWTSVirtualChannel
title: IWTSVirtualChannel
author: windows-sdk-content
description: Used to control the channel state, and writes on the channel.
old-location: termserv\iwtsvirtualchannel.htm
tech.root: termserv
ms.assetid: 8a5b093f-5756-400f-9442-b95d6010ee46
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IWTSVirtualChannel, IWTSVirtualChannel interface [Remote Desktop Services], IWTSVirtualChannel interface [Remote Desktop Services],described, termserv.iwtsvirtualchannel, tsvirtualchannels/IWTSVirtualChannel
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: tsvirtualchannels.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: TsVirtualChannels.idl
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
 - TsVirtualChannels.h
api_name:
 - IWTSVirtualChannel
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IWTSVirtualChannel interface


## -description


Used to control the channel state, and writes on the channel. This interface is implemented by the framework.

Methods of this interface can be called from any thread.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IWTSVirtualChannel</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IWTSVirtualChannel</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IWTSVirtualChannel</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/b900789d-c7da-4974-8c46-72ea8ffd6892">Close</a>
</td>
<td align="left" width="63%">
Closes the channel.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/fef7067c-6d81-42b7-8534-191bc98906d4">Write</a>
</td>
<td align="left" width="63%">
Starts a write request on the channel.

</td>
</tr>
</table> 

