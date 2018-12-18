---
UID: NN:mixerocx.IMixerOCXNotify
title: IMixerOCXNotify
author: windows-sdk-content
description: The IMixerOCXNotify interface is implemented by clients and called by the Overlay Mixer to send notifications of events affecting the video display rectangle.
old-location: dshow\imixerocxnotify.htm
tech.root: DirectShow
ms.assetid: b73416c0-2312-4164-8a6d-f8776dc1447f
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: IMixerOCXNotify, IMixerOCXNotify interface [DirectShow], IMixerOCXNotify interface [DirectShow],described, IMixerOCXNotifyInterface, dshow.imixerocxnotify, mixerocx/IMixerOCXNotify
ms.topic: interface
req.header: mixerocx.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Strmiids.lib
 - Strmiids.dll
api_name:
 - IMixerOCXNotify
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# IMixerOCXNotify interface


## -description



The <code>IMixerOCXNotify</code> interface is implemented by clients and called by the Overlay Mixer to send notifications of events affecting the video display rectangle.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMixerOCXNotify</b> interface inherits from the <a href="https://msdn.microsoft.com/33f1d79a-33fc-4ce5-a372-e08bda378332">IUnknown</a> interface. <b>IMixerOCXNotify</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IMixerOCXNotify</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd407086(v=VS.85).aspx">OnDataChange</a>
</td>
<td align="left" width="63%">
Notifies the client when the video rectangle's aspect ratio or size, or the display palette, has changed.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd407087(v=VS.85).aspx">OnInvalidateRect</a>
</td>
<td align="left" width="63%">
Notifies the client that the video rectangle has been invalidated.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/en-us/library/Dd407088(v=VS.85).aspx">OnStatusChange</a>
</td>
<td align="left" width="63%">
Notifies the client that a status change has occurred.

</td>
</tr>
</table> 


## -see-also




<a href="https://msdn.microsoft.com/en-us/library/Dd407084(v=VS.85).aspx">IMixerOCX Interface</a>
 

 

